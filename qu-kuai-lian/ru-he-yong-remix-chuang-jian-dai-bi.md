# 如何用remix创建代币

## 步骤 1: 打开 Remix IDE <a href="#id-3bac" id="id-3bac"></a>

1. 打开你的浏览器，访问 Remix IDE。

## 步骤2: 创建一个新的 Solidity 文件 <a href="#id-39c1" id="id-39c1"></a>

1. 在 Remix 左侧文件浏览器中，点&#x51FB;**“文件资源管理器”**。
2. 点&#x51FB;**“contracts”**&#x6587;件夹。
3. 点&#x51FB;**“Create New File”**&#x6309;钮，命名文件为`MyToken.sol`。

## 步骤3:编写代币方案代码 <a href="#id-991c" id="id-991c"></a>

在`MyToken.sol`文件中，编写以下 Solidity 代码，这是一个基于 ERC-20 标准的简单代币合约：

```
// SPDX-License-Identifier: MIT
 pragma solidity ^ 0.8 .0 ;

导入 “@openzeppelin/contracts/token/ERC20/ERC20.sol” ;
导入 “@openzeppelin/contracts/access/Ownable.sol” ;

合约MyToken是ERC20，Ownable {
    构造函数（uint256 initialSupply）ERC20（“MyToken”，“MTK”）{ 
        _mint（msg.sender ， initialSupply）; 
    } 
}
```

## 步骤4：编译程序 <a href="#id-5a52" id="id-5a52"></a>

1. 在 Remix 左侧面板中，点&#x51FB;**“Solidity Compiler”**&#x56FE;标。
2. 选择适当的 Solidity 版本（与合约中的`pragma`语句匹配）。
3. 点&#x51FB;**“Compile MyToken.sol”**&#x6309;钮。如果合约编译成功，你就会看到绿色的复选标记。

## 步骤5：部署合约 <a href="#id-7abd" id="id-7abd"></a>

1. 在 Remix 左侧面板中，点&#x51FB;**“部署并运行交易”**&#x56FE;标。
2. 确&#x4FDD;**“Environment”**&#x8BBE;置&#x4E3A;**“Injected Web3”**&#x6216;&#x8005;**“JavaScript VM”**。
3. &#x5728;**“契约”**&#x4E0B;拉菜单中，选择`MyToken`。
4. &#x5728;**“Deploy”**&#x90E8;分，输入初始供应量（例如：`1000000`），这是初始铸造的代币数量。
5. 点&#x51FB;**“部署”**&#x6309;钮。

> 自此，你的代币就部署完成了，不过需要部署合约还需要自己编写代码，这里推荐GTokenTool一键部署平台：[https://www.gtokentool.com/](https://www.gtokentool.com/)

交流群：[https://t.me/gtokentool](https://t.me/gtokentool)
