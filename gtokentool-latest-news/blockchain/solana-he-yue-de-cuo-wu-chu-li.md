---
description: >-
  文章主要介绍了 Solana 合约开发中的错误处理，包括使用 Rust 语言开发的相关机制，列举了多种错误类型如 ProgramError
  及其子类型，如自定义错误、参数无效等，还阐述了错误处理的好处，如明确性、可维护性和优化用户体验等。
---

# Solana合约的错误处理

### 错误处理

Solana合约开发中错误处理是一个重要的部分，它帮助开发者和用户理解合约执行过程中发生的问题。Solana使用Rust编程语言开发智能合约（称为程序），并提供了一套丰富的错误处理机制，其中包括定义和使用错误类型。

在合约开发中，我们需要返回ProgramResult类型，其定义为：

```
 use {
     std::{
         result::Result as ResultGeneric,
     },
 };
 
 pub type ProgramResult = ResultGeneric<(), ProgramError>;
```

其实就是一个使用了ProgramError作为Err部分的Result类型枚举。

### 错误类型

上面提到的ProgramError的定义为：

```
/// Reasons the program may fail
 #[derive(Clone, Debug, Deserialize, Eq, Error, PartialEq, Serialize)]
 pub enum ProgramError {
    /// Allows on-chain programs to implement program-specific error types and see them returned
    /// by the Solana runtime. A program-specific error may be any type that is represented as
    /// or serialized to a u32 integer.
    #[error("Custom program error: {0:#x}")]
    Custom(u32),
    #[error("The arguments provided to a program instruction were invalid")]
    InvalidArgument,
    #[error("An instruction's data contents was invalid")]
    InvalidInstructionData,
    #[error("An account's data contents was invalid")]
    InvalidAccountData,
    #[error("An account's data was too small")]
    AccountDataTooSmall,
    #[error("An account's balance was too small to complete the instruction")]
    InsufficientFunds,
    #[error("The account did not have the expected program id")]
    IncorrectProgramId,
    #[error("A signature was required but not found")]
    MissingRequiredSignature,
    #[error("An initialize instruction was sent to an account that has already been initialized")]
    AccountAlreadyInitialized,
    #[error("An attempt to operate on an account that hasn't been initialized")]
    UninitializedAccount,
    #[error("The instruction expected additional account keys")]
    NotEnoughAccountKeys,
    #[error("Failed to borrow a reference to account data, already borrowed")]
    AccountBorrowFailed,
    #[error("Length of the seed is too long for address generation")]
    MaxSeedLengthExceeded,
    #[error("Provided seeds do not result in a valid address")]
    InvalidSeeds,
    #[error("IO Error: {0}")]
    BorshIoError(String),
    #[error("An account does not have enough lamports to be rent-exempt")]
    AccountNotRentExempt,
    #[error("Unsupported sysvar")]
    UnsupportedSysvar,
    #[error("Provided owner is not allowed")]
    IllegalOwner,
    #[error("Accounts data allocations exceeded the maximum allowed per transaction")]
    MaxAccountsDataAllocationsExceeded,
    #[error("Account data reallocation was invalid")]
    InvalidRealloc,
    #[error("Instruction trace length exceeded the maximum allowed per transaction")]
    MaxInstructionTraceLengthExceeded,
    #[error("Builtin programs must consume compute units")]
    BuiltinProgramsMustConsumeComputeUnits,
}
```

#### **`Custom(u32)`** ：

自定义错误。允许合约开发者定义具体的错误码。当运行时返回错误时，这些自定义的错误码可以帮助确定错误发生的具体位置或原因。 既然是用u32类区别合约错误，自然我们想到了Rust里面的enum来定义错误：

```
#[derive(Clone, Debug, Eq, Error, FromPrimitive, PartialEq)]
 pub enum HelloWorldError {
     #[error("Not owned by HelloWolrd Program")]
     NotOwnedByHelloWrold,
 }

```

但是这是我们自定义的枚举，要如何让他变成上面的Custom(u32) 呢？因此需要定义转换函数：

```
impl From<HelloWorldError> for ProgramError {
     fn from(e: HelloWorldError) -> Self {
         ProgramError::Custom(e as u32)
     }
 }
```

直接将枚举的值，转换成了Custom里面的错误码。

错误码有了，但是错误码对应的意义是什么呢？



```
impl PrintProgramError for HelloWorldError {
    fn print<E>(&self)
    where
        E: 'static + std::error::Error + DecodeError<E> + PrintProgramError + FromPrimitive,
    {
        match self {
            HelloWorldError::NotOwnedByHelloWrold => msg!("Error: Greeted account does not have the correct program id!"),
        }
    }
 }
```

这里通过PrintProgramError trate的实现，来定义其错误消息。

这样在出错的时候，返回相应错误。

```
if greeting_account.owner != program_id {
         msg!("Greeted account does not have the correct program id");
         return Err(HelloWorldError::NotOwnedByHelloWrold.into());
     }
```

通过into直接转换。

### **`InvalidArgument`**：

参数无效。当传递给合约指令的参数不符合预期时，会返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
) -> ProgramResult {
    msg!("Hello World Rust program entrypoint");
    //碰到参数无效错误，返回错误
     Err(ProgramError::InvalidArgument)  
} 
```

### **`InvalidInstructionData`**：

指令数据无效。如果指令的数据字段包含了非法或不可解析的数据，将返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 指令数据无效，返回错误
      Err(ProgramError::InvalidInstructionData)  
 } 
```

### **`InvalidAccountData`**：

账户数据无效。账户的数据内容不符合合约要求时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
) -> ProgramResult {
  msg!("Hello World Rust program entrypoint");
  //碰到账户数据无效错误，返回错误
   Err(ProgramError::InvalidAccountData)  
} 
```

1. **`AccountDataTooSmall`**：

账户数据过小。账户提供的存储空间不足以存储所需的数据时，将返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 账户数据过小，返回错误
      Err(ProgramError::AccountDataTooSmall)  
 } 
```

1. **`InsufficientFunds`**：

资金不足。账户的余额不足以完成交易时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到账户的余额不足，返回错误
      Err(ProgramError::InsufficientFunds)  
 } 
```

### **`IncorrectProgramId`**：

程序ID不正确。执行交易时，如果账户的程序ID与预期的不一致，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 程序ID不正确，返回错误
      Err(ProgramError::IncorrectProgramId)  
 } 
```

### **`MissingRequiredSignature`**：

缺少必要的签名。如果交易需要的签名没有被提供，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到缺少必要的签名，返回错误
      Err(ProgramError::MissingRequiredSignature)  
 } 
```

### **`AccountAlreadyInitialized`**：

账户已经初始化。向已初始化的账户发送初始化指令时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到向已初始化的账户发送初始化指令，返回错误
      Err(ProgramError::AccountAlreadyInitialized)  
 } 
```

### **`UninitializedAccount`**：

未初始化的账户。尝试操作一个未被初始化的账户时，将返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 未初始化的账户，返回错误
      Err(ProgramError::UninitializedAccount)  
 } 
```

### **`NotEnoughAccountKeys`**：

账户密钥不足。指令需要更多的账户密钥，但没有提供足够的时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到账户密钥不足，返回错误
      Err(ProgramError::NotEnoughAccountKeys)  
 } 
```

### **`AccountBorrowFailed`**：

账户借用失败。无法借用对账户数据的引用时（可能是由于它已经被借用），返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到账户借用失败，返回错误
      Err(ProgramError::AccountBorrowFailed)  
 } 
```

### **`MaxSeedLengthExceeded`**：

种子长度超出最大限制。在地址生成时提供的种子长度过长，将返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到种子长度超出最大限制，返回错误
      Err(ProgramError::MaxSeedLengthExceeded)  
 } 
```

### **`InvalidSeeds`**：

种子无效。提供的种子未能生成有效地址时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 种子无效错误，返回错误
      Err(ProgramError::InvalidSeeds)  
 } 
```

### **`BorshIoError(String)`** ：

Borsh序列化/反序列化错误。在进行Borsh数据编码或解码时发生错误，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到Borsh序列化/反序列化错，返回错误
      Err(ProgramError::`BorshIoError("string".to_string()))  
 } 
```

### **`AccountNotRentExempt`**：

账户不免租金。账户的余额不足以维持其在区块链上存储的状态，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到账户不免租金，返回错误
      Err(ProgramError::AccountNotRentExempt)  
 } 
```

### **`UnsupportedSysvar`**：

不支持的系统变量。尝试使用不支持的系统变量时，将返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到不支持的系统变量错误，返回错误
      Err(ProgramError::UnsupportedSysvar)  
 } 
```

### **`IllegalOwner`**：

非法的所有者。尝试将账户的所有权设置为非法的程序ID时，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到非法的所有，返回错误
      Err(ProgramError::IllegalOwner)  
 } 
```

### **`MaxAccountsDataAllocationsExceeded`**：

账户数据分配超过每笔交易的最大允许量，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到 账户数据分配超过每笔交易的最大允许量，返回错误
      Err(ProgramError::MaxAccountsDataAllocationsExceeded)  
 } 
```

### **`InvalidRealloc`**：

无效的重新分配。在尝试对账户数据空间进行重新分配时发生错误，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到无效的重新分配，返回错误
      Err(ProgramError::InvalidRealloc)  
 } 
```

### **`MaxInstructionTraceLengthExceeded`**：

指令追踪长度超出每笔交易允许的最大值，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到指令追踪长度超出每笔交易允许的最大值，返回错误
      Err(ProgramError::MaxInstructionTraceLengthExceeded)  
 } 
```

### **`BuiltinProgramsMustConsumeComputeUnits`**：

内置程序必须消耗计算单位。如果内置程序未消耗计算单位，返回此错误。

```
pub fn process_instruction(  _program_id: &Pubkey, _accounts: &[AccountInfo],_instruction_data: &[u8],  
 ) -> ProgramResult {
     msg!("Hello World Rust program entrypoint");
     //碰到内置程序必须消耗计算单位，返回错误
      Err(ProgramError::BuiltinProgramsMustConsumeComputeUnits)  
 } 
```

### 错误处理的好处



1. **明确性**：自定义错误使错误条件更加明确，便于开发者理解代码失败的原因。
2. **可维护性**：集中管理错误类型有助于代码的维护和更新。
3. **用户体验**：为终端用户提供更具体的错误信息，有助于他们理解发生了什么，尤其是在需要调试或解决问题时。

上面的错误基本涵盖了所有写合约时可能出现的错误类型，即使有漏网之鱼不匹配的情况，也可以通过字段定义错误创建适合自己合约的错误。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
