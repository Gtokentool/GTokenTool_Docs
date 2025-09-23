---
description: 在Orca创建流动性资金池
icon: files
---

# Orca创建/撤除流动性(加池子)教程

Orca是Sol链上较为知名的去中心化交易所之一，和Raydium相比，在Orca上创建流动性所需要的费用极低（通常少于0.5sol），而且大家习惯在Orca上创建USDC的池子，因为USDC池子比SOL池子的无偿损失会更低，不用担心SOL价格波动带来的风险。

## Orca创建流动性资金池流程：

### 1. 填写相应的代币信息

打开网页：[https://www.orca.so/create-pool](https://www.orca.so/create-pool)，填写相应的代币信息：

<figure><img src="../../.gitbook/assets/image.avif" alt=""><figcaption></figcaption></figure>

* **Token A**：就是你发行的代币，输入合约地址找到你的币。
* **Token B**：底池代币，例如USDT、SOL、USDC等。
* **Fee tier**：就是费率/滑点，我的建议是填0.2%，填对的太小不利于交易。
* **Initial price**：初始价格，假设你是做代币+SOL的池子，那么这个价格就是一个币值多少SOL的意思。
* **Liquidity range**：流动性范围，指的是你代币价格的范围，目前有FULL和CUSTOM两个选择。如果你不懂什么意思，直接选择FULL这个就行，即：全范围，和薄饼V2是一样的。如果选择CUSTOM，就是V3的概念了，这里不建议使用。

### 2. 输入相应的代币数量

所有的信息填写完成之后，下一步就是输入相应的代币数量。最终填写完成的如下：

<figure><img src="../../.gitbook/assets/image (1).jpg" alt=""><figcaption></figcaption></figure>

### 3. 点击“Create Pool”

确定价格无误之后，点击“`Create Pool`（创建池子）”，然后会跳出钱包，点击确认，即可完成资金池的创建。

## **池子做好之后，应该如何查看？**

我们打开页面：[https://v1.orca.so/liquidity](https://v1.orca.so/liquidity) ，重新连接钱包（如果已经连接，则不需要）。

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>

然后点击`Portfolio`，等待几秒钟，就能看到自己的池子。

<figure><img src="../../.gitbook/assets/image (305).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (306).png" alt=""><figcaption></figcaption></figure>

如果你想移除池子，可以点击你的交易对，选择 **`提取`** 流动性（如果想继续加池子，就选择 **`存入`**）。

<figure><img src="../../.gitbook/assets/image (307).png" alt=""><figcaption></figcaption></figure>

之后，按照页面需要，选择移除流动性比例，再点击 **`Withdraw`，** 钱包确认并支付gas即可。

<figure><img src="../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>

以上就是关于ORCA创建流动性/加池子/移除流动性的相关教程了。



[_**GTokenTool | 创建代币、批量空投和做市机器人等Solana工具集**_](https://sol.gtokentool.com)

**安全、开源，给Solana用户带来最便利的一站式体验。**



GTokenTool社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter:  [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)\
\
\
<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
