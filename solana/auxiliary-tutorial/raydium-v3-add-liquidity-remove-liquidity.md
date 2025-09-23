---
description: 全网最好的Raydium V3添加流动性 移除流动性教程
icon: files
---

# Raydium V3添加流动性 移除流动性教程

## Raydium V3添加流动性 移除流动性教程视频演示

{% embed url="https://youtu.be/AEkgk44asBI" %}

V3是Raydium最新推出的一个流动性产品，具有以下特点：

* **新的做市逻辑：**&#x91C7;用了新的 CPMM 做市模式，有别于之前V2的AMM
* **不需要市场ID：**&#x43;PMM不再需要Openbook市场ID，可省去一笔ID创建费用
* **创池成本更低：**&#x56;3的池子创建收费0.2 SOL，是原先V2池子的一半
* **支持度不够：**&#x4F8B;如PEPE机器人、Ave等尚不支持V3版本，只有我们的市值机器人支持
* **交易问题 ：**&#x52A0;了V3池子之后，可能会出现无法卖出的情况

## 1. 添加流动性

打开RaydiumV3的官网：[https://raydium.io/liquidity-pools/](https://raydium.io/liquidity-pools/)，可以点击右上角的设置切换语言：

<figure><img src="../../.gitbook/assets/image (319).png" alt=""><figcaption></figcaption></figure>

之后点击“`创建`”按钮。

<figure><img src="../../.gitbook/assets/image (309).png" alt=""><figcaption></figcaption></figure>

打开之后，选择**标准AMM池**，然后`继续`下一步。

(集中池创建麻烦，且价格不能波动太大，所以一般我们推荐创建标准AMM池)

<figure><img src="../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

## 2. 确定价格和比例

在新的页面，我们需要填写相应的代币与数量，进行流动性创建。

<figure><img src="../../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

* **代币数量：**&#x4F60;要添加到池子里面的代币数量（你发行的代币）。
* **SOL数量：**&#x4F60;的交易对代币（报价代币）。
* **开盘时间：**&#x4EE3;币开始交易的时间。这个时间之前，池子无法交易（UTC时间，与北京时间有8个小时时差）。
* **开盘价格：**&#x4E5F;就是代币初始价格，取决于你的代币数量与Sol数量。例如，我初始放入1亿枚代币和1个SOL进入池子，那么我的开盘价格就是：0.00000001 SOL，换算成USDT就是0.00000182 U。

例如：

<figure><img src="../../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

关于开盘时间这一块，在设置的时候，Raydium很人性化的给予了自动转换时区的功能，UTC时间与北京时间自动转换，所以设置起来就比较方便了，例如：

<figure><img src="../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>

确定好没问题之后，点击初始化流动性，钱包确认支付费用就可以了。（注意：加池手续费大概0.2 SOL左右）

<figure><img src="../../.gitbook/assets/image (314).png" alt=""><figcaption></figcaption></figure>

池子创建成功后，会有个提示给你，如下图所示：

<figure><img src="../../.gitbook/assets/image (315).png" alt=""><figcaption></figcaption></figure>

## 3. 移除流动性

同样我们打开Raydium，页面链接：[https://beta.raydium.io/portfolio/](https://beta.raydium.io/portfolio/)找到“`我的投资组合`”，选择标准流动池，就可以看到自己的池子。

<figure><img src="../../.gitbook/assets/image (316).png" alt=""><figcaption></figcaption></figure>

* 注：如果你设置了开盘时间，那要等到开盘后，才能看到池子。

此时，如果你想移除流动性，选择那个“`-`”按钮就可以了，如下所示：

<figure><img src="../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

选择你要撤池子的比例，点击`移除流动性`，然后钱包确认，就可以了。

以上就是关于Raydium V3添加流动性/加池子/撤池子/移除流动性的全部教程了。

## 相关问题

### 1. `V3`有什么优点/缺点？

答：V3的优点就是不用创建市场ID，省了笔钱。缺点就是一些狙击机器人不支持V3，没法用。

### 2. 加了V3池子后能`锁池`吗？

答：同样通过燃烧池子实现。

### 3. 代币没有关闭冻结权限，怎么办？

需要去代币管理工具那里前往权限管理放弃冻结权限：[https://sol.gtokentool.com/zh-cn/Token/management](https://sol.gtokentool.com/zh-cn/Token/management)，方可继续操作。如果还是有提示，可能是raydium有缓存，需要更换网络或者刷新重试。





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
