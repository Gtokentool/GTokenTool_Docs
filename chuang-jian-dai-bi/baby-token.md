---
description: 按持币份额分配交易手续费 / 项目收益的分红型代币
---

# 持币分红代币

**GTokenTool** 的 **创建持币分红代币** 工具主要用于发行具备自动奖励机制的资产，通过交易税收向持有者分配主流代币。该工具具备**分红币种可选、门槛灵活配置、链上自动派发**等特点。其优势在于通过内生收益模型显著提升持币信心，通过利益共享凝聚社区共识。它特别适用于需建立强社区纽带、追求长期共赢的 **Web3 初创项目、DAO 组织及模因币运营团队**，是构建忠诚生态的利器。

## 📌 核心摘要

* **功能定位：**&#x4E00;站式自动化收益分配代币发行工具。支持用户发行能够根据持币比例，自动向持有者分发主流代币奖励（如 USDT、BNB 等）的资产。
* **技术特性：**
  * **分红币种自定义：**&#x652F;持自由选择分红的奖励代币类型，满足多样化的激励需求。
  * **智能分发阈值：**&#x53EF;配置起分门槛与持有量要求，确保分红机制的公平性与灵活性。
  * **全自动链上派发：**&#x5185;置自动化执行逻辑，无需手动操作即可实现收益的实时或定期链上发放。
* **应用价值：**&#x901A;过构建内生性的被动收益模型，将项目增长红利直接回馈给支持者，从而显著提升持币信心并降低资产抛压。
* **目标受众：**&#x9700;建立强利益绑定关系的 Web3 初创项目、追求高度凝聚力的 DAO 组织，以及希望通过分红机制吸引长期持有者的模因币（Meme）运营团队。

## 1、介绍

该模式可设置分红代币和持币门槛, 超过持币门槛的钱包, 将会自动分红指定代币, 需要注意的是, 由于逻辑复杂, 此类模版交易时使用的gas费较高, 不建议在ETH等过于昂贵的链上使用。

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://www.gtokentool.com/tokenfactory](https://www.gtokentool.com/tokenfactory)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption><p>连接钱包并选择网络</p></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择 “持币分红”。

<figure><img src="../.gitbook/assets/image (225).png" alt=""><figcaption><p>选择持币分红代币</p></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，填写如下：

* **代币全称：**&#x47; TOKEN
* **代币简称：**&#x47; T
* **供应总量：**&#x31;000000（代币数量）
* **代币精度：**&#x31;8（小数点后的位数）
* **营销钱包地址：**&#x30;x46ed16F6BCb78d05d38E4765C10CF89e2a542D43
* **选择池底：**&#x54;BNB
* **选择交易所：**&#x70;ancakeSwapTest V2
* **最小持币分红数量：**&#x31;0000
* **分红的代币：**&#x54;BNB

<figure><img src="../.gitbook/assets/000 (13).jpg" alt=""><figcaption><p>填写代币信息</p></figcaption></figure>

输入完成后，点击 “`创建`”。

### (4) 完成

点击 “`确认创建`” ，在小狐狸钱包支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/2gPB4235RA3JrxC7b2iAyy4Catfo71ipNYMGr_eKbHXgo6DmWEGozyuW-e7MgEyjbwFY2GmzgERXwGC-bwJkpapgVVb6pHep93nyDNYoxHq9q46sBgH-DDu1diIIRMlI3dN2yuJZxHe2x36mItxy6H8" alt=""><figcaption><p>确认创建</p></figcaption></figure>

<mark style="background-color:red;">注意：</mark>

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

## ❓常见问题 FAQ

### Q: 持币分红代币是什么原理？

**A:** 通过智能合约按用户持币比例，自动分配分红资产，无需用户手动操作。

### Q: 分红可以用什么代币发放？

**A:** 支持链上主流币、稳定币、项目自身代币等多种资产发放分红。

### Q: 可以设置最低持币分红门槛吗？

**A:** 支持自定义最低持币数量，不满足门槛的钱包无法获得分红。

### Q: 用户卖出代币后还能分红吗？

**A:** 卖出后持仓减少，不再计入分红统计，当期及后续分红自动停止。

### Q: 分红代币可以正常加流动性、上 DEX 吗？

**A:** 和普通代币完全一致，可正常添加流动性、设置交易税率、上线去中心化交易所。

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
