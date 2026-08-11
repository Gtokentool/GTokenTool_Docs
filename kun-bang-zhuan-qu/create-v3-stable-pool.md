---
description: 搭建 V3 稳定池，优化稳定币兑换深度与价格稳定性。
icon: water
---

# 创建 V3 稳定池教程

GTokenTool V3 稳定池搭建工具适配 PancakeSwap‑V3，底池固定选用 USDT等稳定币，池子手续费锁定 0.01%，专为稳定币、同质化代币创建窄区间集中流动性；可自定义初始开盘价，资金集中锚定平价位置，资金利用率远高于 V2 池子，降低交易滑点、积攒交易手续费收益。

## 📌 核心摘要

* **功能定位**：搭建 USDT等稳定币交易对的 V3 集中流动性池，适配平价类代币。
* **技术特性**：流动性区间可控、固定 0.01% 超低费率、集中流动性资本效率更高。
* **用户价值**：压低大额交易滑点，依靠高频交易赚取手续费，稳住代币市价。
* **适用人群**：稳定币项目方、流动性运维人员、链上做市商。

**备注：**&#x5E26;税费机制代币仅支持 V2 流动池，创建池子需要 0.02 BNB 手续费。

## **准备事项** <a href="#zhun-bei-shi-xiang" id="zhun-bei-shi-xiang"></a>

1. 一台电脑或者一部手机
2. BSC 钱包（[小狐狸MetaMask钱包安装教程](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)）
3. 钱包最少准备 0.021 BNB
4. 要创建流动性的代币地址

## 创建 V3 稳定池具体流程

### 1. 连接钱包

进入[创建 V3 稳定池](https://www.gtokentool.com/stableSwap)页面，右上角点击`连接钱包`并选择 BSC 主网。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-16_09-46-37.png" alt=""><figcaption><p>连接钱包并选择BSC链</p></figcaption></figure>

### 2.  选择DEX并选择底池代币

<figure><img src="../.gitbook/assets/Snipaste_2026-04-16_09-47-41.png" alt=""><figcaption><p>选择DEX并选择底池代币</p></figcaption></figure>

### 3. 输入代币地址

输入代币地址后，下面会显示代币简称以及代币余额。

{% hint style="success" %}
**注 :** 稳定池只支持标准代币，有机制的代币，请创建V2流动性池。
{% endhint %}

<figure><img src="../.gitbook/assets/Snipaste_2026-04-16_09-48-35.png" alt=""><figcaption><p>输入代币地址</p></figcaption></figure>

### 4. 输入交易价格和加池数量

<figure><img src="../.gitbook/assets/Snipaste_2026-04-16_09-49-17.png" alt=""><figcaption><p>输入交易价格和加池数量</p></figcaption></figure>

### 5. 点击“立即加池”

首次交易需要授权，弹出钱包后点击确认。交易成功后弹出成功提示。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-16_10-18-42.png" alt=""><figcaption><p>钱包确认</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是 V3 单币稳定池？

**A:** PancakeSwap V3 专为稳定币设计，可**只存一种币**做市，窄价格区间、低滑点、低无常损失。

### Q: 只能稳定币用吗？

**A:** 是的，适合 USDT/USDC 等 1:1 锚定资产，波动币不适用。

### Q: 建池要双币吗？

**A:** 不用，可**单币存入**，系统自动配比。

### Q: 池子安全吗？

**A:** 合约安全；风险主要看项目方是否锁仓、放弃权限。

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
