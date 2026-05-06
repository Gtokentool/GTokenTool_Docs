---
description: 在Uniswap V3添加/移除流动性
---

# 🟥 Uniswap V3添加/移除流动性教程？

Uniswap v3 通过「集中流动性」功能，允许 LP（流动性提供者） 为特定的价格区间提供流动性，并将不同用户对同一交易对提供的流动性汇总到一个池子里（形成一条综合曲线）供用户交易，从而提高资金利用率。

## Uniswap V3添加流动性

### 1. 添加代币设置手续费

点击「资金池」-「+ New Position」，选择要添加的代币并设置手续费费率。0.05% 适合稳定币交易对，0.3% 适合常规资产交易对，1% 适合小众资产交易对。

<figure><img src="../.gitbook/assets/1 (44).png" alt=""><figcaption></figcaption></figure>

### 2. 设置价格区间

Min Price 是最低价，Max Price 是最高价，Current Price 是当前该资金池中的成交价（即当前汇率）。根据自己想要提供流动性的价格区间设置对应的 Min Price 和 Max Price 即可。

<figure><img src="../.gitbook/assets/2 (38).png" alt=""><figcaption></figcaption></figure>

### 3. 设置要投入的代币数量

如果你是第一次提供某币种的流动性，则需要先对该币种进行授权。图中以 USDT 为例，点击「Approve USDT」进行授权，授权成功后再点击「Add」进入下一步。

<figure><img src="../.gitbook/assets/3 (34).png" alt=""><figcaption></figcaption></figure>

### 4. 添加流动性

再次点击「Add」确认提供流动性，当交易发出后需要等待处理。成功后，即可在 Uniswap 的资金池页面看到添加的流动性。

<figure><img src="../.gitbook/assets/4 (29).png" alt=""><figcaption></figcaption></figure>

### 5. 查看添加流动性信息

点击「In range」即可查看在 Uniswap v3 存入流动性获取的 NFT（即流动性凭证），该 NFT 是一张动态的图片，展示了交易对、手续费率、ID 和价格区间等信息。

<figure><img src="../.gitbook/assets/5 (27).png" alt=""><figcaption></figcaption></figure>

## Uniswap V3移除流动性

### 1. 找到上面添加的流动性

在 DApp 浏览页面找到并打开 Uniswap，切换至资金池页面。接着点击「Remove Liquidity」，输入要退出流动性的资金数额，如果要全部退出，点击「Max」即可，然后点击「Remove」。

<figure><img src="../.gitbook/assets/6 (26).png" alt=""><figcaption></figcaption></figure>

### 2. 移除流动性

在弹出的流动性移除详情页中再次点击「Remove」-「确认」，交易发出后需要等待处理。成功后，即可在 Uniswap 的资金池页面看到提示。回到 imToken 资产页面也会看到同步更新的资产数额。

<figure><img src="../.gitbook/assets/7 (19).png" alt=""><figcaption></figcaption></figure>

流动性移除后，LP 仍能在 Uniswap 和 imToken 看到代表仓位的 NFT，但此时该仓位会在 Uniswap 上显示为 Inactive（非活跃）的状态。

## Uniswap V3资金池的特点：

**1、V3池子不支持分红合约**\
和V2相比，V3不支持LP分红、持币分红等复杂的分红合约，只能支持标准合约。如果您在 GTokenTool 创建的是分红合约，必须在V2添加流动性，以确保功能的稳定运行，不能在V3加池。

**2、V3锁池麻烦**\
很多人习惯通过 Pinksales 等平台锁池，一次锁个三年、五年的。但是V3的池子是无法这样锁的，至少在粉红平台并不支持，需要注意。

**3、Arb链不支持Uniswap V2**\
目前，Uniswap只在Arb链上部署V3合约。如果要想在Arb链上实现代币的复杂功能，需要通过SushiSwap V2做资金池。

**4、V3支持单边流动性**\
在一个成熟的资金池里，用户可以通过V3增加单边流动性，即只增加同一个代币，无需以交易对的形式添加流动性。

### 🤝 连接 GTokenTool <a href="#lian-jie-gtokentool" id="lian-jie-gtokentool"></a>

* **💬 Telegram社群**：[点击加入官方群组](https://t.me/gtokentool)
* **🐦 Twitter (X)**：[关注我们获取最新动态](https://x.com/gtokentool)
* **📚 官方文档**：[查看 Gitbook 文档](https://docs.gtokentool.com/)
* **💻 开源代码**：[访问 GitHub 仓库](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)
* **📺 视频教程**：[订阅 YouTube 频道](https://www.youtube.com/@GTokenTool)

> ⚠️ 风险提示与免责声明
>
> GTokenTool 保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。
>
> 以上信息内容仅供参考，GTokenTool 对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。**请谨慎投资。**
