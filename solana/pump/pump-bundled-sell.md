---
description: 此功能利用Jito技术，实现快速批量捆绑卖出，确保在Pump的交易过程畅通无阻，实现利益最大化。
icon: inbox-out
---

# Pump一键卖出教程

## 📌核心摘要

* **核心功能（一键砸盘）**：专为 **PumpFun** 平台设计的高效出货工具，支持将多地址代币独立卖出并打包为同一Bundle，毫秒级完成整批交易，实现快速清仓与砸盘。
* **技术架构（Jito 赋能）**：底层集成 **Jito 技术**，通过快速批量捆绑交易，有效规避网络拥堵与交易失败风险，确保大额卖单在 Pump 交易过程中的畅通无阻。
* **执行优势（利益最大化）**：通过自动化脚本实现毫秒级响应，大幅缩短出货时间窗口，降低滑点损耗，从而在激烈的市场博弈中**实现利润最大化**。

## 视频演示

{% embed url="https://youtu.be/-DFzeK39Wek" %}

## 准备事项

1. 一台电脑或者一部手机
2. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
3. 钱包私钥
4. 代币
5. GAS费用

## Pump一键卖出流程

### 1. 连接钱包

Pump一键卖出：[https://sol.gtokentool.com/zh-CN/pump/pumpSell](https://sol.gtokentool.com/zh-CN/pump/pumpSell)

进入 Solana 一键卖出页面，右上角支持切换成中文。选择 Main 网络并连接钱包。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-21_11-47-26.png" alt=""><figcaption><p>连接钱包并选择Main网络</p></figcaption></figure>

### 2. 输入代币合约地址

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-21_11-52-44.png" alt=""><figcaption><p>输入代币地址</p></figcaption></figure>

### 3. 选择DEX

选择要卖出代币的池子类型，若不清楚池子类型，直接选择Jup。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-21_11-53-40.png" alt=""><figcaption><p>选择对应的DEX</p></figcaption></figure>

### 4. 导入批量交易钱包

{% hint style="warning" %}
**注意：**&#x4EA4;易之前请刷新钱包，获取钱包最新余额。<mark style="color:red;">所有服务费将由导入的第一个地址支付。</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-21_11-54-15.png" alt=""><figcaption><p>导入钱包</p></figcaption></figure>

### 5. 设置捆绑小费

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-21_11-54-38.png" alt=""><figcaption><p>设置Jito小费</p></figcaption></figure>

{% hint style="success" %}
Jito EVM小费：Jito 小费可以简单理解为用户选择支付给矿工的“贿赂”费用，提高交易的优先级，费用越高，交易上链速度越快。
{% endhint %}

### 6. 点击“Pump一键卖出”

{% hint style="warning" %}
一键卖出功能最多支持 29 个地址同时捆绑卖出，每个地址的服务费最低仅为 0.005 SOL，所有服务费将由导入的第一个地址支付。<mark style="color:red;">请保证导入的第一个地址有足够 SOL 余额。</mark>
{% endhint %}

勾选钱包，并点击“Pump 一键卖出”。交易完成会弹出交易成功的提示。

<figure><img src="../../.gitbook/assets/Snipaste_2025-07-10_11-13-37.png" alt=""><figcaption><p>一键卖出成功提示</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是一键卖出？

**A:** 一键卖出是指一次性打包多个地址或交易指令，统一发送卖出请求，提高效率和优先级。

### Q: 使用一键卖出的优势是什么？

**A:** 可提升成交速度、减少滑点，并避免因手动延迟而错过最佳卖出时机。

### Q: Jito 技术在捆绑卖出中起什么作用？

**A:** Jito 可优先处理打包交易，有助于在高峰时段顺利完成卖出操作。

### Q: 最多支持多少个地址捆绑卖出？

**A:** 最多支持 29 个地址捆绑卖出，所有服务费由创建的钱包支付。

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
