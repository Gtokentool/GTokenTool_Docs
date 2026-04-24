---
description: 可同时从一个地址向多个接收者发送代币。支持导入 CSV 文件，并可自定义等额或可变分配。在单笔交易中完成多次转账，节省高达 90% 的 Gas 费用。
---

# 1️⃣ 代币批量转账-批量发送空投代币

批量转账工具专为需要高频、大批量处理代币分发的开发者及项目方设计。通过简洁的交互界面，用户可在一分钟内完成从地址导入到转账确认的全流程。

## 批量转账工具介绍

GTokenTool多链批量转账工具，支持ETH、BSC、Base、Arbitrum等多条EVM公链，大大的简化了转账与空投流程，可以快速实现代币空投与转账等多种操作。

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

## 注意事项 <a href="#chang-jian-wen-ti-jie-da" id="chang-jian-wen-ti-jie-da"></a>

* 收款地址和数量必须用英文逗号分隔。
* 推荐使用PC端操作，更加方便快捷。
* 如往交易所地址进行转账，请务必确认交易所是否支持合约转账，否则你的转账将无法到账。
* 为保证转账顺利，一次转账的地址数请勿超过100个。
* 支持大部分EVM公链，切换到哪个钱包，就自动在哪个链上转账。

## 批量转账工具使用流程

### 第1步，连接钱包

进入GTokenTool批量转账页面：[https://gtokentool.com/sendertoken](https://gtokentool.com/sendertoken)，点击右上角，连接小狐狸钱包，并切换到主网。

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/Snipaste_2026-01-04_14-50-09.png" alt=""><figcaption><p>连接钱包并选择公链</p></figcaption></figure>

### 第2步，输入转账信息

假设我们给三个地址发送不同数量的代币，输入如下：

* 代币地址：BNB
* 收款地址和数量（逗号分隔）：
* 0x13FC5BD0A0ee0E1DD30176b833D436B95c9E2cD2,0.01
* 0x697FfC45A1bF65ca69601F06743219E86B94B0B1,0.02
* 0xAb8dF92b986b91A4964339BD044849DFfEA71AA8,0.03

<figure><img src="../.gitbook/assets/Snipaste_2026-01-04_14-55-29.png" alt=""><figcaption><p>输入转账信息</p></figcaption></figure>

（不明白可以点击右下角 “查看例子”）

### 第3步，完成

输入完成后，点击 “`下一步`” 按钮。

<figure><img src="../.gitbook/assets/Snipaste_2026-01-04_14-56-53.png" alt=""><figcaption><p>发送交易</p></figcaption></figure>

确认无误后，点击 “`发送`” 按钮，在小狐狸上支付gas费，就完成了。

（注：因为每个用户网络速度不同，支付gas费用时可能会延迟1、2秒，属正常现象。）

### 优势

| **特性** | **传统手动转账** | **GTokenTool 批量转账** |
| ------ | ---------- | ------------------- |
| 效率     | 极低（一个一个转）  | 极高（一键分发数千人）         |
| 错误率    | 高（手动复制易出错） | 低（系统自动核验地址）         |
| 成本     | 费时费力       | 节省时间与人力成本           |
| 门槛     | 需要耐心       | 零代码基础，小白即用          |

## ❓常见问题 FAQ

### Q: 批量转账是什么？

**A:** 一次给多个地址同时发送代币，高效省 Gas。

### Q: 手续费怎么算？

**A:** 每200个地址需要0.01 BNB，比单笔转账便宜。

### Q: 可以转 BNB 吗？

**A:** 支持代币和 BNB 批量转账。

### Q: 发送失败会退回吗？

**A:** 失败金额自动退回，已成功部分不撤回。

GTokenTool 是一款高效、安全的 Solana 链上自动化工具，旨在帮助用户无需代码即可快速实现 SOL 及 SPL 代币的大规模空投和多地址分发。

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
