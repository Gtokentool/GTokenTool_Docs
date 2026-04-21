---
icon: fire
---

# Solana代币燃烧教程

**GTokenTool** 的 **Solana代币燃烧工具** 主要用于实现代币供应量的永久缩减，支持用户通过销毁特定数量的代币来执行通缩策略。该工具具备**操作极简、即时链上生效**等特点，用户无需编写智能合约即可安全执行燃烧任务。相比其他平台，其优势在于**完全透明的交互流程与极低的手续费损耗**，并能有效提升项目的市场信誉度。它特别适用于需要通过通缩模型回馈社区、减少流通压力或进行销毁活动的 **Solana 项目方、社区治理团队及代币持有者**，是资产价值管理的高效利器。

## 📌核心摘要

* **功能定位**：Solana 代币通缩与价值管理工具。它通过将代币永久发送至不可恢复的销毁地址，减少流通中的代币总量，从而提升代币的稀缺性与潜在价值。
* **核心价值（通缩经济模型）**：
  * **价值提升**：通过减少供应量，在需求不变或增加的情况下，理论上可以推高代币的市场价格。
  * **信任建立**：项目方通过主动销毁代币，向社区展示其长期承诺，增强投资者信心。
  * **生态激励**：部分项目将交易手续费的一部分用于销毁，形成通缩闭环，激励用户长期持有。
* **操作前置条件**：
  * **钱包准备**：需安装并配置好 Solana 钱包（如 Phantom），并确保钱包内有足够的 SOL 用于支付 Gas 费。
  * **代币信息**：需明确要销毁的代币合约地址和要销毁的代币数量。
  * **资金准备**：操作钱包内需有至少 0.05 SOL 用于支付交易费用。

## 准备事项

1. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
2. 钱包最少准备 0.05 SOL
3. 要冻结的代币合约和要冻结的账户地址信息

## Solana代币燃烧教程

### 1. 连接钱包

进入[GTokenTool](https://www.gtokentool.com)代币燃烧页面，右上角连接钱包，选择Phantom钱包，并选择 Main 网络节点，这里使用测试网演示。

Solana代币燃烧：[https://sol.gtokentool.com/zh-CN/liquidityManagement/burnToken](https://sol.gtokentool.com/zh-CN/liquidityManagement/burnToken)

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_15-08-11.png" alt=""><figcaption><p>连接钱包并选择网络</p></figcaption></figure>

### 2. 选择要燃烧的代币

选择代币后，可以查看到代币的相关信息。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_15-11-22.png" alt=""><figcaption><p>代币信息显示</p></figcaption></figure>

### 3. 输入想要燃烧的代币数量

关闭`全部销毁并关闭账户`的开关，可以设置想要燃烧的比例或数量。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_15-14-41.png" alt=""><figcaption><p>输入燃烧数量</p></figcaption></figure>

### 4. 提交完成代币燃烧

点击“`燃烧代币`”，执行操作。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_15-16-41.png" alt=""><figcaption><p>钱包确认</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-25_15-17-14.png" alt=""><figcaption><p>燃烧成功提示</p></figcaption></figure>

{% hint style="danger" %}
在进行代币燃烧之前，请确保您完全理解燃烧的目的和对项目经济模型的潜在影响。燃烧代币是不可逆的操作，一旦执行，被燃烧的代币将永久从流通中移除。在提交燃烧操作前，务必仔细检查将要燃烧的代币数量。错误的数量可能导致意外的经济损失。
{% endhint %}

## ❓常见问题 FAQ

### Q: 关闭账户是什么意思？

**A:** 你每收到一个新的代币，Solana系统会自动在你的地址里开设一个代币存储账户。所谓“关闭账户”，就是把代币全部销毁，账户也关掉的意思。关闭账户并不影响你自己的钱包，因此不用担心。

### Q: NFT可以销毁吗？

**A:** 在 Orca 加池子获得是 NFT，这个暂时是不支持销毁/烧池的。目前可以销毁的是 Ryadium 和 Meteora 的 LP。

### Q: 烧池后还能撤回流动性吗？

**A:** 烧池后，永久无法撤出流动性。

### Q: 燃烧操作是否可以撤销？

**A:** 不可以，燃烧后代币被永久移除，无法恢复。

### Q: 燃烧是否会直接拉升价格？

**A:** 燃烧本身不保证价格上涨，但减少供应可能产生稀缺效应。

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
