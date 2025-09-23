# 5️⃣ STON.fi生成流动性代币教程

作为TON生态系统中最重要的去中心化交易所之一，STON.fi凭借其AMM模型和与TON钱包的无缝集成，已成为TON生态流动性提供者的首选平台。本教程将深入讲解如何在STON.fi上生成流动性代币(LP Token)的完整流程和高级技巧。

## 什么是STON.fi

STON.fi 是基于 TON 区块链的去中心化自动做市商平台，交易费用几乎为零、滑点低，平台与 TON 钱包无缝集成、用户体验感好。STON.FI 专为 Telegram 用户设计，支持每秒数百万笔交易，具备高吞吐量和良好的扩展性。用户无需桥接或转换即可跨链交换本地代币，平台采用报价请求（RFQ）系统和哈希时间锁定合约（HTLC）技术，既消除了交易风险，也摆脱了第三方依赖，保障了交易的安全性与流畅度。

## STON.Fi 背景 <a href="#h2-ston-fi" id="h2-ston-fi"></a>

STON.fi 由 Viacheslav Baranov（CEO）与 Stanislav Bazylevich（COO）、Mike Fedorov（CBO）、Andrey Fedorov（CMO）共同创立于 2022 年。公司总部位于阿联酋迪拜，专注于去中心化金融（DeFi）领域。作为一家私营公司，STON.FI 拥有 47 名员工，致力于为区块链生态系统提供创新解决方案。公司已从 Anton Bukov、CoinFund 和 Delphi Ventures 等投资方融资 449 万美元。STON.fi 将通过将原生代币 STON 融入其核心机制，利用其在市场中的地位，推动基于区块链的去中心化、社区驱动的金融服务。

## STON.fi V2的推出

STON.fi正在进行一系列称为STON.fi V2的更新。这一系列的关键组成部分是向交易所添加新类型的流动性池。

在9月25日，AMM DEX STON.fi在其Telegram频道上宣布推出STON.fi V2。

STON.fi V2是一系列旨在增强安全性、稳定性、性能、界面并添加新功能的更新。

STON.fi V2已经为交易所引入了几个重要的更新：

更新的智能合约。STON.fi已经更新了其智能合约。根据交易所的说法：「新的STON.fi V2智能合约满足现代交易的所有要求。」

安全创建流动性池。现在，您可以在一次操作中创建流动性池并为其提供流动性！这确保了您的代币完全受到针对新池的“狙击机器人”攻击的保护，这些攻击旨在操纵价格。

SDK中的推荐系统。您现在可以在集成STON.fi SDK时灵活配置推荐佣金。

## 为什么选择 STON.fi <a href="#why-ston.fi" id="why-ston.fi"></a>

STON.fi 成立于 2022 年。它的目标是建立一个用户友好的加密货币交易所，通过接触 `Telegram` 受众来实现大规模采用。 STON.fi 高度重视社区，代表着一个人性化的 `DEX`，为用户提供快速支持并考虑他们的意见。

具有分片功能的 TON 区块链架构允许 STON.fi DEX 用户每秒进行数百万笔交易。

如果你想在TON区块链上发行代币并使其可以交易，STON.fi是一个很棒的选择。GTokenTool小编，教大家在STON.fi创建代币流动性，也就是俗称的加池子，和撤池子。

## 准备工作

### 1.1 钱包配置

**推荐钱包**：

* Tonkeeper (移动端最佳体验)
* OpenMask (浏览器扩展)
* MyTonWallet (桌面端)

**安全提示**：

* 确保使用官方渠道下载钱包
* 小额测试交易后再进行大额操作
* 记录并安全保管助记词

### 1.2 资金准备

* 主网TON用于支付Gas费(建议至少准备5-10 TON)
* 计划提供流动性的代币对(等值配对)

## STON.fi生成流动性代币教程

### 1、连接钱包

打开STON.fi的官网：[https://app.ston.fi/pools](https://app.ston.fi/pools) ，点击右上角Connect Wallet，连接钱包。

<figure><img src="../.gitbook/assets/1 (37).png" alt=""><figcaption></figcaption></figure>

弹出一列钱包让你选择，选择这个Tonkeeper钱包，然后会弹出钱包插件，点击连接钱包。

<figure><img src="../.gitbook/assets/2 (32).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/3 (28).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/4 (24).png" alt=""><figcaption></figcaption></figure>

### 2、生成流动性

点击页面的Add liquidity，并选择你要加池的代币。

<figure><img src="../.gitbook/assets/5 (22).png" alt=""><figcaption></figcaption></figure>

输入代币合约地址，并且确定要添加的代币数量。

<figure><img src="../.gitbook/assets/6 (21).png" alt=""><figcaption></figcaption></figure>

确认无误后，点击Confirm，会弹出钱包，钱包确认就可以了。

## STON.fi生成流动性代币注意事项

### **1、STON上面没有代币头像怎么办？**

答：需要在STON完成申请，且池子内有超过1万U的流动性，才能进入到STON的默认列表里，从而获得头像。申请链接：[https://docs.google.com/forms/d/e/1FAIpQLScGTZjf5DVRutqykFKF477MHoFS9-qzPhkdbOKmo\_hZn66FVA/viewform](https://docs.google.com/forms/d/e/1FAIpQLScGTZjf5DVRutqykFKF477MHoFS9-qzPhkdbOKmo_hZn66FVA/viewform)

### **2、创建流动性的时候提示余额不够？**

答：在STON创建池子，连同gas，需要额外支出1.7个TON，他会要求钱包里至少2.7TON才能发起交易。

### **3、在STON上面交易需要支付费用吗？**

答：每笔交易需要支出0.3%的费用，其中0.2% 的费用将作为增加资金池规模而支付给流动性提供者的费用，0.1% 的费用支付给STON.fi协议。

### **4、为什么我的LP Token价值在变化？**

答：这是AMM池的正常现象，价值随池中资产比例变化而变化，包含无常损失因素。

### **5、添加流动性后为什么看不到收益？**

答：收益通过LP Token本身价值增长体现，STON.fi不单独显示手续费收益。

### **6、最小流动性添加量是多少？**

答：理论上无最低限制，但Gas费占比过高时不经济，建议至少价值10TON以上。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
