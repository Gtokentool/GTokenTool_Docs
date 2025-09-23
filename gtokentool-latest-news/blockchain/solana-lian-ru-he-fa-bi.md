# solana链如何发币

## 1. 安装Solana CLI和Spl Token CLI <a href="#id-3e0a" id="id-3e0a"></a>

首先，你需要安装Solana CLI和Spl Token CLI。这些工具可以帮助你与Solana区块链进行交互，并创建代币。

### 安装Solana CLI <a href="#id-4e5a" id="id-4e5a"></a>

按照Solana官方文档中的步骤安装Solana CLI。

`sh -c "$(curl -sSfL https://release.solana.com/v1.10.33/install)"`

### 安装Spl Token CLI <a href="#id-2325" id="id-2325"></a>

Spl Token CLI是一个与Solana SPL（Solana Program Library）代币标准交互的工具。

`cargo install spl-token-cli`

## 2. 配置Solana CLI <a href="#id-87a5" id="id-87a5"></a>

配置Solana CLI以连接到测试网或主网。

solana 配置集 - url [https://api.testnet.solana.com](https://api.testnet.solana.com/)

或

solana 配置集 — url [https://api.mainnet-beta.solana.com](https://api.mainnet-beta.solana.com/)

创建一个Solana钱包（或使用现有的钱包）。

solana-keygen new — 输出文件 \~/.config/solana/id.json

solana 空投 1

## 3.创建项目 <a href="#id-45de" id="id-45de"></a>

使用Spl Token CLI创建新的代币。

spl-token 创建令牌

我们将返回一个纪念地址，例如：

创建令牌 A1b2C3d4E5F6G7H8I9J0K1L2M3N4O5P6Q7R8S9T0

## 4.创建帐户 <a href="#f7e0" id="f7e0"></a>

为你的钱包掏钱以该钱。

spl-token 创建账户 A1b2C3d4E5F6G7H8I9J0K1L2M3N4O5P6Q7R8S9T0

希望返回一个新的纪念账户地址，例如：

创建帐户 B1c2D3e4F5G6H7I8J9K0L1M2N3O4P5Q6R7S8T9U0

向你的代币价值中铸造新的代币。

spl代币铸造A1b2C3d4E5F6G7H8I9J0K1L2M3N4O5P6Q7R8S9T0 1000 B1c2D3e4F5G6H7I8J9K0L1M2N3O4P5Q6R7S8T9U0

我会铸造1000个代币到你的账户。

## 6.验证余额 <a href="#d83a" id="d83a"></a>

验证你的代币账户中的余额。

spl-token 账户

您应该会看到类似以下的结果，显示您的目标余额：

```
代币余额
--------------------------------------------------------------
 A1b2C3d4E5F6G7H8I9J0K1L2M3N4O5P6Q7R8S9T0 1000
```

## 7. 发送邮件 <a href="#c227" id="c227"></a>

请将代币授予其他Solana地址。

spl-token 转移 — 资金接收者 A1b2C3d4E5F6G7H8I9J0K1L2M3N4O5P6Q7R8S9T0 100 RecipientTokenAddress

如有其他问题，加入社区：[https://t.me/gtokentool](http://twitter.com/gtokentool)

[\
](https://medium.com/@ylmskj11?source=post_page-----d146bfb82ef0--------------------------------)
