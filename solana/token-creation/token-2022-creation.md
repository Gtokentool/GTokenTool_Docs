---
description: 无需编写代码，即可轻松创建符合 Token2022 标准的 Solana 代币。自定义交易税率，满足更多样化的项目需求，享受更加灵活的市场策略定制。
icon: coin-vertical
---

# Solana SPL Token 2022手续费代币创建教程

## 📌 核心摘要

* **功能定位**：**Solana Token 2022 标准代币创建指南**。不同于传统的 SPL 代币，本教程专注于创建支&#x6301;**“原生交易手续费”**（Transfer Fee）的新型代币。
* **核心差异（Token 2022 vs 普通 SPL）**：
  * **交易税率自定义**：允许在合约层面设定**转账手续费率**。每当代币发生转移时，自动扣除一定比例的手续费（可用于项目分红、回购或营销）。
  * **无需代码**：尽管 Token 2022 涉及更复杂的指令，但本工具实现了可视化配置，降低了技术门槛。
* **适用场景**：
  * 希望实现**持币分红**或**自动流动性获取**的项目。
  * 需要更灵活的市场策略（如通过费率调控交易频率）的高级代币模型。

## 视频演示

{% embed url="https://youtu.be/_uG2YfnkbbM?si=LS8sMWPd410f9K1-" %}

## 准备事项

1.准备设备，一台电脑或手机

2.Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）

3.钱包内最少准备0.07个SOL

4.准备好翻墙软件（VPN/加速器），保证网络通畅

## 创建手续费代币（Token-2022）操作步骤

### 1.连接幻影钱包Phantom

打开发币链接地址：[https://sol.gtokentool.com/zh-CN/Token/createToken](https://sol.gtokentool.com/zh-CN/Token/createToken)

点击连接钱包，并选择 Main 网络节点，这里使用测试网演示。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-23_15-20-20.png" alt=""><figcaption><p>连接钱包并选择网络</p></figcaption></figure>

### 2.填写代币相关信息并上传LOGO文件

完成钱包连接之后，先选择代币模式，接下来就是填写代币信息，具体如下：

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-42-40 (1).png" alt=""><figcaption><p>填写代币基础信息</p></figcaption></figure>

**代币名称：**&#x4EE3;币的名称信息（如GTOKENTOOL），支持英文、中文以及中英文混合，最多32个字符。

**代币简称：**&#x4EE3;币的简称信息（如GTOKEN），支持英文、中文以及中英文混合，最多10个字符。

**代币精度：**&#x4EE3;币的精度位数，默认为9，精度与你能填写的最大总供应量有关。

**总供应量：**&#x4EE3;币的总供应量，当精度为9时，总供应量不能超过100亿；当精度为8时，总供应量不能超过1000亿，以此类推。

<figure><img src="../../.gitbook/assets/image (492).png" alt=""><figcaption><p>参数参考</p></figcaption></figure>

**简介（选填）：**&#x586B;写你的代币简介。

**Logo：**&#x4EE3;币头像，可在钱包中显示logo代币图片（上传图片大小最大不超过2M）。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-45-22.png" alt=""><figcaption><p>转账费率设置</p></figcaption></figure>

**转账费率：**&#x6BCF;次交易或转账所需的手续费率，单位为百分比。

**最高费用：**&#x5355;笔转账或交易时的最大手续费用上限（不填默认为供应量）。

**所有权地址：**&#x63A7;制此代币的所有权限，默认为当前连接的钱包地址。

**提现钱包地址：**&#x4EE3;币所产生的手续费，有权限进行提现的地址，默认为当前连接的钱包地址。

### 3.添加联系方式（选填）

如果你想添加联系方式等，可以点击打开“`添加联系方式`”按钮，选择需要填写的内容进行填写。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-23_15-23-45.png" alt=""><figcaption><p>添加联系方式</p></figcaption></figure>

**官网：**&#x5B98;网链接地址。

**电报：**&#x7535;报（Telegram）链接地址。

**推特：**&#x63A8;特（Twitter）链接地址。

**Discord:** Discord链接地址。

### 4. 高级设置填写

**提示：如果您不了解高级功能设置，请勿输入或修改。**

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-48-36.png" alt=""><figcaption><p>高级设置</p></figcaption></figure>

**权限委托**：将您的代币权限委托给另一个地址，该地址将能够燃烧或转移任意数量的代币。

**计息利率%(0.00 - 100)**：为您的代币设定利率，模仿债券等现实世界的资产，并随时获得利息。需要先设置交易费率。

**不可转账（灵魂绑定代币）**：默认关闭，使代币不可转让给其他地址，通常适用于独特成就等类型项目。

### 5. 高级选项设置

如果您想要自定义代币合约，可以使用靓号合约功能创建代币。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-23_15-24-43.png" alt=""><figcaption><p>靓号合约生成</p></figcaption></figure>

代币更新权限、冻结权限、增发权限设置。

* **放弃更新权限：**“放弃更新权限”意味着您将无法修改令牌元数据。
* **放弃冻结权限：**&#x5982;果您放弃冻结权限，则意味着您将无法冻结持有者钱包中的代币。
* **放弃增发权限：**“放弃增发权限”对于让投资者感到更加安全和作为代币的成功是必要的。如果您放弃铸币权，则意味着您将无法铸造更多代币供应。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-49-34.png" alt=""><figcaption><p>权限设置</p></figcaption></figure>

### 6.点击"确定"，创建代币

确认信息之后，点击"`确定`"按钮，之后会跳出钱包提示，点击去"`Confirm`"支付费用，即可完成创建。

<figure><img src="../../.gitbook/assets/Snipaste_2026-04-20_11-34-31.png" alt=""><figcaption><p>钱包确认</p></figcaption></figure>

### 5.查看代币

创建成功后会弹出一个提示框提示创建成功，并展示你的代币地址。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-51-59.png" alt=""><figcaption><p>代币合约地址显示</p></figcaption></figure>

创建成功后可以前往`管理代币`，在手续费代币列表下可以找到刚才创建的代币，可以进行进一步的Solana发币管理。或者直接在上方的搜索框内输入代币地址进行查找。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-53-30.png" alt=""><figcaption><p>代币列表</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_10-54-10.png" alt=""><figcaption><p>代币查询结果</p></figcaption></figure>

或者前往SOL区块链浏览器（[https://solscan.io](https://solscan.io)）去查看代币信息。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_11-02-03.png" alt=""><figcaption><p>区块链浏览器代币信息显示</p></figcaption></figure>

如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)

## ❓常见问题 FAQ

### Q: Solana上发币需要合约开源吗？

**A:** 不需要。Solana上的代币是通过官方发布好的合约创建出来的账户，所有的SPL代币用的都是一个合约。

### Q: 为什么发币之后钱包显示未知代币/不显示logo?

**A:** Phantom钱包有时候信息有延迟，需要一段时间才能显示logo和代币名称等信息。可以在Solana浏览器上搜索代币信息进行查看。

### Q: 上传logo需要收费吗？

**A:** 不需要，平台采用的是IPFS存储方案，免费上传。

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
