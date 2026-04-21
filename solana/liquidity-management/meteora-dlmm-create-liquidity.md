---
icon: meteor
---

# Meteora DLMM 创建流动性教程

**GTokenTool** 的 **Solana Meteora DLMM 创建流动性** 工具专为 **Meteora** 设计，用于精准部署动态流动性。该工具具备**Bin 级区间自定义、多种波动率策略选择、极高资金效率**等特点。其优势在于能通过集中流动性获取更高手续费收益，并有效降低交易滑点。它特别适用于追求极致收益、需灵活管理动态头寸的 **Solana 专业做市商、流动性提供者及进阶 DeFi 玩家**，是精准管理资本的专业利器。

## 📌 核心摘要

* **功能定位：**&#x9488;对 **Meteora DLMM（动态流动性做市商）** 协议设计的**高阶流动性精细化管理引擎**。支持用户在 Solana 链上实施具备动态收益捕获能力的流动性部署策略。
* **技术特性：**
  * **Bin 级区间自定义：**&#x5F15;入离散流动性分档（Bin）技术，允许用户在极窄的价格区间内精准锁定资金分配。
  * **动态策略驱动：**&#x9884;设多种基于波动率的流动性策略，通过调整价格分布模型，实现不同市场环境下的收益最大化。
  * **极致资本效率：**&#x5229;用集中流动性算法，以更小的资金消耗实现更高的交易深度，并显著提升手续费分成比例。
* **应用价值：**&#x901A;过**波动率捕获与低滑点交易**设计，该工具为用户提供了超越传统 AMM 的盈利空间，是实现链上资产增值与高阶做市的核心利器。
* **目标受众：**&#x5BFB;求高额手续费回报的专业做市商、需精准对冲价格风险的流动性提供者，以及对资本效率有极高要求的进阶 DeFi 交易员。

## Meteora DLMM 流动性池介绍

Meteora DLMM（Dynamic Liquidity Management Module）是 Solana 生态中基于动态流动性管理机制的去中心化交易协议，其流动性池设计旨在解决传统 AMM（如恒定乘积模型）中流动性利用率低、滑点高的问题，核心特点是通过**动态调整流动性分布**优化资本效率，尤其适合波动较大的加密资产交易场景。

## 准备事项

1. 一台电脑或者一部手机
2. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
3. 钱包最少准备 **0.24 SOL**
4. 要创建流动性池的代币

## Solana 创建 Meteora DLMM 池子教程

### 1. 连接钱包

进入 GTokenTool 创建流动性页面，右上角选择 Main 网络并连接钱包，这里用测试网演示。

创建流动性池： [https://sol.gtokentool.com/zh-CN/liquidityManagement/CreatePool](https://sol.gtokentool.com/zh-CN/liquidityManagement/CreatePool)

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-02-09.png" alt=""><figcaption><p>连接钱包并选择Main网络</p></figcaption></figure>

### 2. 选择池子类型 <a href="#id-2-xuan-ze-clmm-chi-zi" id="id-2-xuan-ze-clmm-chi-zi"></a>

GTokenTool 支持用户创建AMM池、 AMM V4 池、CPMM 池、 CLMM 稳定池、PumpSwap池和 DLMM 稳定池，我们在这里选择 DLMM 稳定池。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-13-06.png" alt=""><figcaption><p>选择池子类型</p></figcaption></figure>

### 3. 选择要创建流动性池的交易对 <a href="#id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui" id="id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui"></a>

* **基础代币：**&#x586B;写您创建的还没有任何价值的代币。
* **报价代币：**&#x5177;有市场价值的代币，通常是 SOL 、 USDC 或 USDT。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-17-51 (1).png" alt=""><figcaption><p>选择交易对</p></figcaption></figure>

### 4. 选择加池模式 <a href="#id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui" id="id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui"></a>

GTokenTool 为您提供了两种加池模式（默认为单币加池）：

* **双币加池：**&#x540C;时加入用户创建的代币和价值币。
* **单币加池：**&#x53EA;添加用户创建的代币。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-20-34.png" alt=""><figcaption><p>选择加池模式</p></figcaption></figure>

### 5. 双币加池参数填写

* **初始价格：**&#x8BBE;置池子的初始价格。
* **存入数量：**&#x8BBE;置存入价值币（比如USDT）的数量，<mark style="color:purple;">系统会自动为你计算出需要存入的基础代币数量</mark>。如果弹出钱包爆红，可能是你的代币数量太少，可以减少存入数量再次尝试。
* **钱包预留余额估算：** 钱包余额需要大于（Meteora 官方收取 + 服务费用 0.23 SOL，入池数量，预留0.01 SOL）的总和。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-40-37 (1).png" alt=""><figcaption><p>双币加池参数填写</p></figcaption></figure>

### 6. 双币加池效果展示

参数填写好后，点击“`创建流动性`”。钱包会弹出两次，第一次创建池子，第二次添加池子，钱包弹出后，点击“`确认`”。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-46-50.png" alt=""><figcaption><p>创建池子钱包确认</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-47-06.png" alt=""><figcaption><p>添加池子钱包确认</p></figcaption></figure>

创建成功效果展示：

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-47-15.png" alt=""><figcaption><p>创建成功池子地址显示</p></figcaption></figure>

### 7. 单币加池参数填写

* **单币加池：**&#x6253;开单币加池开关。
* **初始价格：**&#x8BBE;置池子的初始价格。
* **存入数量：**&#x8BBE;置存入基础代币的数量，不需要存入价值币（比如USDT）。
* **钱包预留余额估算：**  钱包余额需要大于（Meteora 官方收取 + 服务费用 0.23 SOL，预留0.01 SOL）的总和。

<mark style="background-color:$warning;">**温馨提示：**</mark><mark style="background-color:$warning;">单币加池代币是无法卖出的，只能买入。如果你希望代币可以卖出，需要往池子里加入价值币才行，通过我们的</mark>[<mark style="background-color:$warning;">市值机器人</mark>](https://sol.gtokentool.com/zh-CN/market/jupMarket)<mark style="background-color:$warning;">买入一笔就行。</mark>

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-26-52.png" alt=""><figcaption><p>单币加池参数填写</p></figcaption></figure>

### 8. 单币加池效果展示

参数填写好后，点击“`创建流动性`”。钱包会弹出两次，第一次创建池子，第二次添加池子，钱包弹出后，点击“`确认`”。

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-34-16.png" alt=""><figcaption><p>创建池子钱包确认</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-34-35.png" alt=""><figcaption><p>添加池子钱包确认</p></figcaption></figure>

创建成功效果展示：

<figure><img src="../../.gitbook/assets/Snipaste_2025-11-14_14-35-01.png" alt=""><figcaption><p>创建成功池子地址显示</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: 什么是 DLMM？

**A:** 动态流动性做市商（**Dynamic Liquidity Market Maker**），将流动性分散到**离散价格 Bin**，自动集中在活跃价格，**资本效率更高**。

### Q: 支持 Token-2022 吗？

**A:** ✅ 支持，但部分扩展（如转账钩子）需项目方申请 Badge。

### Q: 加流动性要选区间吗？

**A:** ❌ 不用手动设区间。**输入金额 + 价格范围**，自动分 Bin。

### Q: 能部分撤池吗？

**A:** ✅ 支持**部分赎回**，灵活管理仓位。

### Q: 在 GTokenTool 用 DLMM 有什么不同？

**A:** ✅ **无需手动选区间**✅ **仅填初始价格 + 存入数量**✅ **支持单币一键加池**✅ **自动分 Bin、自动再平衡**

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

