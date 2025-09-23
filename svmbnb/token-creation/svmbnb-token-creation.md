# SVMBNB一键发币教程

[_<mark style="color:orange;">GTokenTool-SVMBNB工具集</mark>_](https://sol.gtokentool.com)

S链上近期热度持续高升，很多用户都想尝试在 Solana 链上发行属于自己的代币，但是发币需要了解相关代码逻辑，门槛较高。[GTokenTool](https://www.gtokentool.com)实现了可视化的操作页面，支持用户在 Solana上轻松创建和管理代币。本文将详细介绍如何在 GTokenTool 上1分钟创建您的专属SOL发币流程。

## Solana发币视频演示

{% embed url="https://youtu.be/10d8ZWXfUro" %}

## Solana发币准备事项

1.安装好幻影（Phantom）钱包插件，安装教程（[https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）

2.钱包内最少准备0.13个SOL

3.准备好翻墙软件（VPN/加速器），保证网络通畅

4.发币Logo和相关信息

5.手机Solana发币也使用Phantom钱包或欧易web3钱包，不要用TP钱包，TP不能传logo

## Solana发币教程步骤

### 1.连接幻影钱包Phantom

打开Solana发币链接地址：[https://sol.gtokentool.com](https://sol.gtokentool.com) 点击连接钱包，并选择你的节点。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-41-37 (1).png" alt=""><figcaption></figcaption></figure>

点击"连接钱包"后会弹出钱包选择页面，点击幻影钱包（Phantom），即可连接钱包钱包里面需要有0.03SOL用作支付。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-45-31 (1).png" alt=""><figcaption></figcaption></figure>

连接后可以看到右上角显示的钱包地址。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-46-59 (2).png" alt=""><figcaption></figcaption></figure>

### 2.填写Solana发币相关信息并上传LOGO文件

完成钱包连接之后，先选择发币模式，接下来就是填写Solana发币信息，具体如下：

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-50-37 (2).png" alt=""><figcaption></figcaption></figure>

**代币全称：**&#x53D1;币的名称信息（如GT），支持英文、中文以及中英文混合，最多32个字符。

**代币简称：**&#x53D1;币的简称信息（如G），支持英文、中文以及中英文混合，最多10个字符。

**代币精度：**&#x4EE3;币精度定义了代币可以分割到多小的单位。 SPL代币的最大精度是9，常见的精度设置是6（实用代币）和9（高精度应用），0精度通常用于NFT。可参考以下数值设置：

<figure><img src="https://docs.slerf.tools/~gitbook/image?url=https%3A%2F%2F4224157678-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4xjUClsdH3VznI0Aws3J%252Fuploads%252F60ZDrvO0VnA1jOtAwlvi%252Fimage.png%3Falt%3Dmedia%26token%3D6ea135ca-037f-4519-8741-7e33c7a8f773&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=f0232ea0&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**总供应量：**&#x53D1;币的总供应量，当精度为9时，总供应量不能超过100亿；当精度为8时，总供应量不能超过1000亿，以此类推。

**Logo：**&#x53;olana发币的头像，可在钱包中显示logo代币图片（上传图片大小最大不超过2M）。

### 3.添加选填内容

如果你想添加联系方式等，可以点击选填内容按钮，展开选填内容模块。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-52-19 (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_18-52-51 (1).png" alt=""><figcaption></figcaption></figure>

**官网：**&#x5B98;网链接地址。

**电报：**&#x7535;报（Telegram）链接地址。

**推特：**&#x63A8;特（Twitter）链接地址。

**Discord:** Discord链接地址。

**简介：**&#x586B;写你的代币简介。

**标签：**&#x6700;多添加5个标签，通过输入后点击"添加"按钮来进行添加标签，觉得不合适的标签也可以删除。

### 4.设置靓号（非必须）

如果您想要自定义代币合约，创建靓号代币。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-05-37.png" alt=""><figcaption></figcaption></figure>

### 5.权限设置（非必须）

代币元数据修改权限、冻结权限、铸币权限设置。

* **元数据更改权：**“放弃所有权”意味着您将无法修改令牌元数据。
* **冻结权：**&#x5982;果您放弃冻结权限，则意味着您将无法冻结持有者钱包中的代币。
* **铸币权：**“放弃铸币权”对于让投资者感到更加安全和作为代币的成功是必要的。如果您放弃铸币权，则意味着您将无法铸造更多代币供应。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-08-20.png" alt=""><figcaption></figcaption></figure>

### 6.使用jito（非必须）

当网络节点卡顿的时候，可以使用jito，可以大大提高发币的成功率。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-10-02.png" alt=""><figcaption></figcaption></figure>

### 7.点击"确认创建"，创建Solana发币

确认信息之后，点击"确认创建"按钮，之后会跳出钱包提示，点击去"确认"支付费用，即可完成创建。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-11-24.png" alt="" width="389"><figcaption></figcaption></figure>

### 8.查看Solana发币的信息

创建成功后会弹出一个提示框提示创建成功，并展示你的发币的地址。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-13-20.png" alt=""><figcaption></figcaption></figure>

点击确认后会前往管理代币列表，可以进行进一步的Solana发币管理。

<figure><img src="../../.gitbook/assets/Snipaste_2025-03-08_19-14-57.png" alt=""><figcaption></figcaption></figure>

或者前往SOL区块链浏览器（[https://solscan.io](https://solscan.io)）去查看发币信息。

<figure><img src="../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

此时，Solana发币的流程就算是基本创建完成了，大家可以根据需求去做池子，然后就能交易了。

* Raydium加池教程：[https://docs.gtokentool.com/solana/raydium-v2-jia-chi-zi-jiao-cheng](https://docs.gtokentool.com/solana/raydium-v2-jia-chi-zi-jiao-cheng)
* Orca加池教程：[https://docs.gtokentool.com/solana/orca-jia-chi-zi-jiao-cheng](https://docs.gtokentool.com/solana/orca-jia-chi-zi-jiao-cheng)
* Meteora加池教程：[https://docs.gtokentool.com/solana/meteora-jia-chi-zi-jiao-cheng](https://docs.gtokentool.com/solana/meteora-jia-chi-zi-jiao-cheng)

推荐产品：

[<mark style="color:orange;">**创建 OpenBook 市场 ID**</mark>](https://sol.gtokentool.com/#/liquidityManagement)　　[<mark style="color:orange;">**创建流动性池**</mark>](https://sol.gtokentool.com/#/liquidityManagement/CreatePool)　　[<mark style="color:orange;">**批量转账**</mark>](https://sol.gtokentool.com/#/batchTool/batchTransfer/SOL)

## Solana发币常见问题

### 1.Solana发币需要合约开源吗？

答：不需要。Solana上的代币是通过官方发布好的合约创建出来的账户，所有的SPL代币用的都是一个合约。

### 2.为什么发币之后钱包显示未知代币/不显示logo?

答：Phantom钱包有时候信息有延迟，需要一段时间才能显示logo和代币名称等信息。可以在Solana浏览器上搜索代币信息进行查看。

### 3.什么情况下丢弃权限？

答：如果需要在 Raydium 添加的代币需要放弃冻结和铸币权限，元数据修改权限可以自行选择丢弃，丢弃之后将不能修改元数据信息。

### 4.上传logo需要收费吗？

答：不需要，平台采用的是IPFS存储方案，免费上传。

### 5.如果你发现代币Logo不见了,可能是由于代币不符合要求

要让用户看到Logo必须在coingecko或Birdeye.so上列出令牌。

Phantom钱包会优先考虑效率和资源管理,因此并非所有代币都会显示其logo,尤其是如果代币是新代币，或TVL较低或资本化较低的话。

### 6.代币符号是什么？

代币符号是代币的简短标识，通常由几个大写字母组成，例如 SOL 或 USDC。

### 7.代币精度是什么，怎么填写？

代币精度定义了代币可以分割到多小的单位。SPL代币的最大精度是9，常见的精度设置是6（实用代币）和9（高精度应用），0精度通常用于NFT。

### 8.为什么要放弃元数据修改权？

放弃元数据修改权意味着一旦设置，代币的基本属性（如名称、符号、图像等）将无法更改。这通常用于增强项目的透明度和信任，显示项目方对代币和其未来计划的承诺。

### 9.什么是放弃冻结权？

放弃冻结权表明创建者无法随意冻结或解冻代币，增强了代币网络的去中心化特性和用户对代币的信任。

### 10.什么是放弃铸币权？

放弃铸币权意味着一旦代币发行完成，将无法增发新的代币。这通常用于限制供应量，防止通货膨胀，确保代币的稀缺性和价值。

### 11.如何保证我创建的代币的安全？

GTokenTool 提供的代币创建工具遵循 Solana 网络的标准安全实践。确保您的私钥安全，避免共享给不可信的第三方，是保护您代币安全的关键。

### 12.在 GTokenTool 上创建代币需要多长时间？

创建过程本身通常很快，只需要几分钟。一旦您提交了所有必需的信息并支付了相关费用，代币几乎可以立即在 Solana 网络上生效。

### 13.可以增发 Solana SPL 代币吗？

可以，但需要您在创建代币时保留增发权限。如果您选择放弃这一权限，那么将无法对该代币进行后续增发。



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
\
&#xNAN;_<mark style="color:purple;">GTokenTool</mark><mark style="color:purple;background-color:yellow;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
