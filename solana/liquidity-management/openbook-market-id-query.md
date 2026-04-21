---
description: 最好用的OpenBook Market ID查询工具
---

# 🔍 OpenBook Market ID查询教程

**GTokenTool** 的 **Solana OpenBook Market ID查询** 工具主要用于帮助用户快速检索代币对应的市场 ID，以便进行流动性部署或交易对接。该工具具备**精准匹配、实时同步、多维度展示**等特点。其优势在于查询速度极快且信息详尽，能有效规避手动查找的繁琐与错误。它特别适用于需要获取底层合约数据以建立交易对或进行行情监控的 **Solana 项目方、DEX 运营者及流动性提供者**，是链上部署的重要辅助利器。

## 📌 核心摘要

* **功能定位：**&#x53;olana 链上流动性部署的关键信息检索引擎。旨在帮助用户通过代币地址快速定位并获取对应的 OpenBook Market ID，解决创建后遗忘或丢失 ID 的痛点。
* **技术特性：**
  * **全平台兼容查询：**&#x4E0D;仅支持在 GTokenTool 生成的 ID，亦可实时检索全网其他平台创建的存量市场 ID。
  * **多维度数据同步：**&#x4E0E; Solana 链上 OpenBook 程序实现秒级数据同步，确保检索结果的实时性与权威性。
  * **精准算法匹配：**&#x901A;过代币合约地址进行深度索引，消除手动在区块浏览器中翻找数据的繁琐流程。
* **应用价值：**&#x4F5C;为连接“代币发行”与“流动性池搭建”的数据桥梁，该工具极大简化了 DEX 运营及做市的前置准备工作，有效规避因数据丢失导致的部署中断。
* **目标受众：**&#x9700;在 Raydium 等平台部署流动性池的项目方、负责 DEX 交易对维护的运营者以及需要获取底层交易参数的量化交易员。

{% hint style="success" %}
考虑到用户在[创建OpenBook Market ID](https://docs.gtokentool.com/solana/openbook-shi-chang-id-chuang-jian-jiao-cheng)时，没保存ID就关闭了页面，以至于后面不好找，所以，[GTokenTool](https://www.gtokentool.com) 就开发了这款工具来查询市场ID。

不管你是在 GTokenTool 生成的ID，还是在其他平台创建的市场ID，都可以通过这个工具查询。
{% endhint %}

## OpenBook市场ID查询教程

OpenBook Market ID查询：[https://sol.gtokentool.com/zh-CN/liquidityManagement/searchId](https://sol.gtokentool.com/zh-CN/liquidityManagement/searchId)

### 1. 访问OpenBook市场ID查询

进入页面后，点击连接钱包，并选择 Main 网络节点，这里使用测试网演示。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-27_16-07-33.png" alt=""><figcaption><p>连接钱包并选择网络</p></figcaption></figure>

### 2. 输入代币地址并选择对应的基础代币

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-12_11-40-20.png" alt=""><figcaption><p>输入代币地址并选择对应的基础代币</p></figcaption></figure>

### 3. 点击查询，等待几秒钟，就可以复制您的ID

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-12_11-42-10.png" alt=""><figcaption><p>查询成功提示</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是OpenBook Market ID?

**A:** Solana OpenBook 订单簿专属市场唯一 ID，绑定代币交易对，用于 DEX 建池、上架展示。

### Q: 和代币 Mint、池子 ID 有什么区别？

**A:** Mint 是代币地址，Market ID 是订单簿交易对 ID，Pool ID 是流动性池地址，三者独立。

### Q: 查不到 Market ID 是什么原因？

**A:** 地址填反 / 输错、网络选错、未成功创建市场、使用新版 CPMM 池子（无需该 ID）。

### Q: 一个币多个 Market ID 怎么选？

**A:** 对应不同交易对（SOL/USDC），匹配自己创建的报价代币即可。

### Q: 查到 ID 但无法使用？

**A:** 复制带空格、市场未初始化、报价代币不匹配，重新核对或重建市场。

### Q: 查询需要付费、授权吗？

**A:** 免费只读查询，无需钱包授权，仅创建市场会扣手续费。

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
