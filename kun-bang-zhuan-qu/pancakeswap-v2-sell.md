---
description: 通过多个地址同步卖出持有的代币，避免单笔大额交易对价格造成冲击。支持自定义卖出数量，一键捆绑卖出，实现平稳止盈策略。
icon: up-from-bracket
---

# PancakeSwap V2一键卖出教程

**GTokenTool** 的 **PancakeSwap V2一键卖出工具** 专为 BSC 生态设计，助力用户极速出清资产。该工具具备**全币种自动识别、秒级链上交互、支持多地址同步**等特点。其优势在于能规避手动交易的繁琐延迟，在剧烈波动中精准锁定利润。它特别适用于追求操作效率的 **Web3 交易员、模因币玩家及项目运营团队**，是玩家在 PancakeSwap 市场博弈中抢占先机、快速落袋为安的必备神器。

## 📌 核心摘要

* **功能定位：**&#x4E13;为 **BSC (币安智能链)** 交易者打造的**资产极速套现引擎**。支持通过多个钱包地址同步执行卖出操作，实现持仓资产的批量、平稳清退。
* **技术特性：**
  * **全币种自动识别：**&#x667A;能扫描并列出钱包内持有的代币，无需繁琐的手动添加，大幅缩短交易准备时间。
  * **多地址同步抛售：**&#x652F;持一键控制多个关联地址同步卖出，有效分散交易压力，规避单笔大额卖单对币价造成的剧烈负面冲击。
  * **秒级链上交互：**&#x6DF1;度优化合约交互路径，提供毫秒级的响应速度，确保在行情波动剧烈时能够精准锁定目标收益。
* **用户价值：**&#x5F7B;底告别了手动切换地址、逐一授权、重复输入数量的低效模式。通过**自动化、捆绑式**的清仓操作，助您在分秒必争的市场博弈中抢先落袋为安，显著降低因操作延迟导致的利润回撤。
* **适用群体：**&#x8FFD;求极致操作效率的 **Web3 活跃交易员**、深度参与 BSC 生态的 **Meme/模因币玩家**，以及需统筹管理多个持仓钱包的**项目运营团队**。

## **准备事项** <a href="#zhun-bei-shi-xiang" id="zhun-bei-shi-xiang"></a>

1. 一台电脑或者一部手机
2. BSC 钱包（[小狐狸MetaMask钱包安装教程](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)）
3. 要交易的代币地址
4. 要卖出代币的钱包私钥和充足的BNB

## PancakeSwap V2一键卖出具体流程

### 1. 连接钱包

进入页面：[https://www.gtokentool.com/FourSell](https://www.gtokentool.com/FourSell)，点击右上角，连接[小狐狸钱包](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)，并切换到币安链主网。完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-03-34.png" alt=""><figcaption><p>连接钱包并选择BSC链</p></figcaption></figure>

### 2. 输入代币地址

输入代币地址后，选择对应的DEX，否则可能导致交易失败。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-04-35.png" alt=""><figcaption><p>输入代币地址并选择对应DEX</p></figcaption></figure>

### 3. 选择对应的底池代币

可选择已提供的代币，也可自行输入底池代币地址。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-05-31.png" alt=""><figcaption><p>选择对应底池</p></figcaption></figure>

### 4. 设置滑点

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-05-40.png" alt=""><figcaption><p>设置滑点</p></figcaption></figure>

### 5. 导入钱包

导入钱包后请刷新钱包，以获取最新的钱包余额以及代币余额。

{% hint style="success" %}
**注意：**<mark style="color:$success;">全部费用由导入的第一个钱包支付。</mark>全网最低费用，阶梯收费低至0.005 BNB/地址。10个以下地址0.008 BNB/地址，10个钱包以上0.005 BNB/地址。
{% endhint %}

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-06-33.png" alt=""><figcaption><p>导入钱包</p></figcaption></figure>

### 6. 设置卖出数量

可手动输入也可批量添加。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-07-04.png" alt=""><figcaption><p>设置卖出数量</p></figcaption></figure>

### 7. 点击“确认”

点击“`确认`”后，交易成功会弹出成功提示。你也可以点击`刷新`，获取钱包最新代币余额。

<figure><img src="../.gitbook/assets/Snipaste_2026-04-09_10-24-00.png" alt=""><figcaption><p>确认交易</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是多地址捆绑卖出？

**A:** 指多个钱包同时卖出同一代币，以批量执行交易，提高交易成功率与速度。

### Q: 为什么卖出地址的BNB余额必须大于 0.001？

**A:** 每个钱包至少保留 0.001 BNB 以上余额，以确保足够支付交易 Gas 费用。

### Q: 代币地址输入错误怎么办？

**A:** 请在执行前确认代币合约地址正确无误。

### Q: 是否支持自定义卖出金额？

**A:** 支持。你可以为不同钱包单独设定卖出金额，也可以统一设定同样的卖出数额。

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
