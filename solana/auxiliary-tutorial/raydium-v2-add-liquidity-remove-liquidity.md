---
description: 全网最全的Raydium V2创建流动性添加池子教程
icon: files
---

# Raydium V2创建流动性 移除流动性教程

Raydium是SOL链上比较大的去中心化交易所，任何人都可以在上面创建流动性资金池。一旦创建了池子，就可以立即在Raydium交换界面上交易。

* 注意：Raydium V2添加池子前，需放弃拉黑（冻结）权限，不然会创建失败。放弃权限请前往G TOKEN代币管理页面进行操作→[https://sol.gtokentool.com/zh-cn/Token/management](https://sol.gtokentool.com/zh-cn/Token/management)

## Raydium V2创建流动性流程

### 1. 获取OpenBook市场ID

在此链接可创建廉价OpenBook市场ID:[https://sol.gtokentool.com/zh-cn/createMarket](https://sol.gtokentool.com/zh-cn/liquidityManagement)

请注意，创建ID的费用大概在0.55\~3个SOL之间（每个ID只能对应一个代币对，不可重复用）。

创建[OpenBook市场ID](https://docs.gtokentool.com/solana/openbook-shi-chang-id-chuang-jian-jiao-cheng)步骤请前往：[https://docs.gtokentool.com/solana/openbook-shi-chang-id-chuang-jian-jiao-cheng](https://docs.gtokentool.com/solana/openbook-shi-chang-id-chuang-jian-jiao-cheng)

创建完OpenBook市场ID后，将其复制保存，准备添加流动池。如果没有及时赋值保存ID,也可以在Solana浏览器搜索创建的哈希，在交易详情里寻找：

<figure><img src="../../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

### 2. 创建Raydium V2流动性

创建完OpenBook市场之后， 前往到Raydium V2的池子页面：[https://v2.raydium.io/pools/](https://v2.raydium.io/pools/)页面右上角点击连接钱包，之后选择“`创建池子`”(Create  Pool)按钮。

<figure><img src="../../.gitbook/assets/image (332).png" alt=""><figcaption></figcaption></figure>

点击之后，输入已经获取到的OpenBook市场ID。

<figure><img src="../../.gitbook/assets/image (322).png" alt=""><figcaption></figcaption></figure>

### 3. 初始化创建池子

* 设置要添加多少币和多少SOL代币到池子中。
* 设置您希望池在哪个日期和时间启动。
* 确保您的钱包中有足够的资金用于此初始流动性，然后单击“`确认并初始化流动性池`”。

**重要提示**：确认并初始化池后，您将无法再编辑起始价格、流动性或开始时间。注意，开始时间由链上的时间确定。

<figure><img src="../../.gitbook/assets/image (323).png" alt=""><figcaption></figcaption></figure>

* 单击确认后，需要在钱包中批准**两个单独的交易**。这些交易将创建池子，创建AMM帐户和ID，并从您的钱包中添加流动性。如果您没有看到其中一个交易，请检查您的钱包窗口是否隐藏在主浏览器窗口后面。如果您错过了确认交易，则该过程将失败，您需要再次单击确认，然后重新批准所有交易。
* 确认钱包中的两个交易后，新LP将已创建，您将获得新的AMM ID，并且底池将在设置的启动时间启动。
* 创建池子时需要0.4 SOL的手续费，钱包请确保预留足够多的手续费和加池子的费用。

### 4. 移除流动性

如果你确认自己已经添加池子，可以在Raydium页面选择Liquidity，然后页面往下拉一拉，就能看到自己的流动性了。

<figure><img src="../../.gitbook/assets/image (1).avif" alt=""><figcaption></figcaption></figure>

点击你的流动性，能看到一些选项，添加流动性或者交易，这时候请选择移除流动性，如下：

<figure><img src="../../.gitbook/assets/image (324).png" alt=""><figcaption></figcaption></figure>

然后填入你要移除的LP数量，点击“`Remove Liquidity`”，钱包确认后，就能撤出了。（如果选择MAX，就是全部撤出）

<figure><img src="../../.gitbook/assets/image (2).avif" alt=""><figcaption></figcaption></figure>

以上就是关于Raydium创建流动性/加池子/移除流动性/撤池子的全部教程了。

## 相关问题

### 1. 为什么钱包确认后半天没反应？

答：Raydium V2的UI页面一直比较卡，所以他们才会推出V3版本的。

### 2. 加了池子后能`锁池`吗？

答：Solana链目前支持锁池的平台不多，一般的做法都是`烧池子`，烧池子相当于百分百永久`锁池子`，就不能再撤池子了。

### 3. 为什么我看不到自己的流动性？

答：Raydium的流动性创建成功后，需要一段时间才会显示，最多24小时。此外，如果你设置了开盘时间，在开盘时间到来之前，的确是看不到流动性的。

### 4. 创建池子出现提示“base token freeze authority enabled”怎么办？

答：该提示是说，你的代币没有放弃`冻结权限`，请使用弃权工具将权限放弃：[https://sol.gtokentool.com/zh-cn/Token/management](https://sol.gtokentool.com/zh-cn/Token/management)

### 5. 创建池子出现提示“base lot size is zero”怎么办？

答：该提示是说，你的钱包里面没有足够的报价代币（如SOL）。



[_**GTokenTool | 创建代币、批量空投和做市机器人等Solana工具集**_](https://sol.gtokentool.com)

**安全、开源，给Solana用户带来最便利的一站式体验。**



GTokenTool社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter:  [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)

\
\
<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
