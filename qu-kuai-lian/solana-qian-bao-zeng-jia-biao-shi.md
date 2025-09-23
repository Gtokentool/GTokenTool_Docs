---
description: >-
  在Solana钱包中增加标识（如自定义图标、标签或名称）可以帮助您更方便地识别和管理钱包地址或代币。以下是如何在不同类型的Solana钱包中实现这一功能的说明：
---

# Solana钱包增加标识

## Phantom Wallet

自定义代币图标或标签：

1.打开 Phantom 钱包扩展或移动应用。

2.点击界面上的代币，然后选择右上角的设置图标。

3.如果支持，您可以添加自定义名称或查看详细信息。

4.如果代币的图标未显示，可以通过手动添加代币地址的方式重新加载其元数据。

添加备注： Phantom 当前不支持对钱包地址或交易添加备注功能，但您可以使用外部工具（例如 Excel）来记录备注。

## Solflare Wallet

添加地址备注：

1.登录 Solflare 钱包。&#x20;

2.导航到“地址簿”或类似的联系人功能。&#x20;

3.对存储的地址添加备注或标签。

代币标识：

1.如果代币图标未正确加载，确保钱包已连接到有效的 RPC 节点。

2.手动输入代币合约地址并刷新代币列表。

## 自托管钱包（例如 CLI 或脚本方式）

自定义标识：

1.如果您使用的是命令行钱包（如 Solana CLI），可以将地址和备注存储在本地文件（如 JSON 文件）中。

2.例如：

{ "wallet1": { "address": "your\_wallet\_address", "note": "Main wallet" }, "wallet2": { "address": "another\_wallet\_address", "note": "For staking" } }

## 自定义开发（例如 DApp 集成）

如果您正在开发与 Solana 区块链交互的应用程序，可以为钱包地址和代币实现自定义标识功能。

在前端界面上：

1.使用标识（如图标和描述）关联钱包地址。

2.将这些标识存储在去中心化存储（如 IPFS）或中心化存储中（如 Firebase）。

## 提示

Token Metadata：确保代币的元数据已经正确发布到 Solana 的代币元数据服务（例如 Metaplex Metadata Standard）。

确保安全：在标识中不要暴露敏感信息，例如私钥或助记词。

如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
