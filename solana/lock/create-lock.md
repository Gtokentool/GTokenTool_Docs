---
icon: lock-hashtag
---

# 创建锁教程

**GTokenTool** 的 **Solana 创建锁** 工具主要用于通过链上智能合约对代币或流动性进行限时锁定。该工具具备**定时解锁配置、锁定证明导出、数据实时可查**等特点。其优势在于通过去中心化托管增强项目透明度，有效防范团队砸盘或撤池风险。它特别适用于需向社区建立信任感、执行合规资产释放的 **Solana 项目方、代币开发者及风险管理团队**，是建立共识的安全基石。

## 📌 核心摘要

* **功能定位：**&#x53;olana 生态中关键的**去中心化资产托管与合规释放引擎**。支持项目方通过智能合约对代币或流动性持仓（LP）进行时间维度上的强制锁定。
* **技术特性：**
  * **自定义锁仓参数：**&#x652F;持灵活配置解锁时间点、分批释放比例及接收地址，满足多样化的归属计划（Vesting）需求。
  * **上链确权与证明：**&#x751F;成不可篡改的链上锁定存证，并支持锁定证明（Lock Proof）的实时导出与外部验证。
  * **数据实时索引：**&#x9501;定状态、剩余时长及资产数额实现全公开透明查询，确保外部监控及社区审计的即时性。
* **应用价值：**&#x4F5C;为构建项目**长期信任背书**的核心工具，通过物理限制“撤池”或“砸盘”行为，有效防止 Rug Pull 风险，是凝聚社区共识、稳定市场预期的安全基石。
* **目标受众：**&#x9700;向投资者展示长期运营决心的项目方、执行团队份额分发计划的初创团队，以及负责链上资产安全审计的合规机构。

## 准备事项

1.准备设备，一台电脑或手机

2.Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）

3.钱包内最少准备0.03 SOL

4.要锁定的代币

5.准备好翻墙软件（VPN/加速器），保证网络通畅

## 创建锁步骤

### 1. 连接钱包

进入创建锁页面（[https://sol.gtokentool.com/zh-CN/locks/createLock](https://sol.gtokentool.com/zh-CN/locks/createLock)），并且连接好钱包，选择 Main 网络节点。

<figure><img src="../../.gitbook/assets/Snipaste_2026-01-13_15-32-40.png" alt=""><figcaption><p>连接钱包并选择Main网络</p></figcaption></figure>

### 2. 选择代币

选择好代币后，下面会显示代币信息以及钱包内代币余额。

<figure><img src="../../.gitbook/assets/Snipaste_2026-01-13_15-37-57.png" alt=""><figcaption><p>选择代币</p></figcaption></figure>

### 3. 填写必要参数

**锁名称：**&#x4E3A;你的锁取一个名称。

**锁定数量：**&#x8BBE;置锁定代币数量（不能超过钱包余额）。

**解锁日期：**&#x8BBE;置解锁的日期。

<figure><img src="../../.gitbook/assets/Snipaste_2026-01-13_15-38-41.png" alt=""><figcaption><p>填写必要参数</p></figcaption></figure>

### 4. 点击“创建”

弹出钱包后，点击确认。

创建成功后可在[管理锁](https://sol.gtokentool.com/zh-CN/locks/managementLock)页面查看。

<figure><img src="../../.gitbook/assets/Snipaste_2026-01-13_15-41-11.png" alt=""><figcaption><p>锁列表</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是锁流动性？

**A:** 将 LP 代币托管锁定，无法随意转出、撤回资金，杜绝项目方撤池跑路。

### Q: 锁定后还能交易吗？

**A:** 可以，二级市场买卖正常，仅**不能移除流动性**。

### Q: 锁仓可以提前解锁吗？

**A:** 支持定时锁，到期可解锁，中途不可解。

### Q: 为什么需要锁流动性？

**A:** 增加项目信任度、减少砸盘风险、满足大盘收录基础条件。

### Q: 锁错了可以撤回吗？

**A:** 定时锁未到期**无法撤销**，操作前需核对。

### Q: 不同 DEX 的 LP 都能锁吗？

**A:** 主流全部支持：Raydium、CPMM、CLMM、Meteora、PumpSwap。

### Q: 锁定会影响代币本身吗？

**A:** 不会，只锁定 LP，代币转账、交易、持有完全不受限制。

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
