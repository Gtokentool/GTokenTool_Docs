---
icon: landmark-flag
---

# Raydium CPMM 创建流动性（加池子）教程

## 📌 核心摘要

* **功能定位：**&#x53;olana 生态新一代**高效做市引擎**。支持项目方在 Raydium 平台部署 CPMM（恒定乘积做市商）V3 标准池，专为提升资金效率与降低交互成本设计。
* **技术特性：**
  * **成本结构优化：**&#x76F8;比传统的 AMM 模式，CPMM 显著降低了建立流动性池的链上成本，提供更具性价比的加池方案。
  * **扩展协议支持：**&#x539F;生支持 **Token 2022** 标准（如手续费代币/回流代币），解决了复杂代币协议在流动性池中的兼容性痛点。
  * **灵活参数配置：**&#x63D0;供可视化的流动性注入界面，支持自定义初始价格、代币配比及精准的市场参数控制。
* **应用价值：**&#x4F5C;为 Raydium 生态的先进做市方案，该工具通过更低的门槛与更强的兼容性，助项目方快速构建具备**可持续流动性**的交易环境。
* **目标受众：**&#x53D1;行 Token 2022 标准代币的项目方、对部署成本敏感的初创团队，以及寻求高效做市方案的 Solana 开发者。

## Raydium CPMM 流动性池介绍

Raydium CPMM 流动性池，也叫 V3 的池子，是 Raydium 提供的一种标准流动池。相比于 Raydium AMM 更便宜，支持 Token 2022 （手续费代币）。

## 视频教程

{% embed url="https://youtu.be/AYvua7dQyhg" %}

## 准备事项

1. 一台电脑或者一部手机
2. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
3. 钱包最少准备 **0.5 SOL** (Raydium官方将收取0.5 SOL)
4. 要创建流动性池的代币

## Solana 创建 Raydium CPMM 池子教程

### 1. 连接钱包

进入 GTokenTool 创建流动性页面，右上角选择 Main 网络并连接钱包。

创建流动性： [https://sol.gtokentool.com/zh-CN/liquidityManagement/CreatePool](https://sol.gtokentool.com/zh-CN/liquidityManagement/CreatePool)

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-13-45.png" alt=""><figcaption><p>连接钱包并选择网络</p></figcaption></figure>

### 2. 选择池子类型

GTokenTool 支持用户创建AMM池、 AMM V4 池、CPMM 池和 CLMM 稳定池四种，我们在这里选择 CPMM 池。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-15-22.png" alt=""><figcaption><p>选择池子类型</p></figcaption></figure>

### 3. 选择要创建流动性池的交易对 <a href="#id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui" id="id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui"></a>

* **基础代币：**&#x586B;写您创建的还没有任何价值的代币。
* **报价代币：**&#x5177;有市场价值的代币，通常是 SOL 、 USDC 或 USDT。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-16-46.png" alt=""><figcaption><p>选择交易对</p></figcaption></figure>

### 4. 具体参数填写

* **基础代币数量：**&#x586B;写你创建的代币数量，想填多少填多少，不要超过实际拥有量。
* **报价代币数量：**&#x586B;写价值币的数量，不要超过实际拥有数量。
* **初始价格：**&#x586B;写完基础代币数量和报价代币数量后会自动为您估算初始价格。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-17-30 (1).png" alt=""><figcaption><p>具体参数填写</p></figcaption></figure>

### 5. 创建 CPMM 流动性效果展示

参数填写好后，点击“`创建流动性`”。钱包弹出后，点击“`确认`”。

创建成功效果展示：

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-21-53.png" alt=""><figcaption><p>创建成功池子地址显示</p></figcaption></figure>

## ❓常见问题 FAQ

### Q: Raydium CPMM 是什么？

**A:** Raydium 新一代恒定乘积池子，替代旧版 AMM V4，是目前主流新建池子模式。

### Q: 创建 CPMM 需要 OpenBook Market ID 吗？

**A:** 不需要，**完全无需 Market ID**，步骤更简单、成本更低。

### Q: CPMM 支持 Token-2022 代币吗？

**A:** 支持，同时兼容传统 SPL 代币；旧版 AMM V4 不支持 Token-2022。

### Q: CPMM 可以设置初始价格吗？

**A:** 可以，通过填入代币配比，自定义池子开盘价格。

### Q: 为什么 CPMM 创建失败？

**A:** 代币授权未开启、钱包 SOL 余额不足、Token2022 权限限制、RPC 节点卡顿。

### Q: CPMM 流动性可以移除或燃烧吗？

**A:** 支持正常移除流动性取回资产，也可一键燃烧 LP 永久锁池。

### Q: 创建后可以修改池子参数吗？

**A:** 价格、手续费等核心参数上链锁定，无法修改，错误需重建池子。

### Q: CPMM 交易滑点、手续费高吗？

**A:** 手续费规则公开透明，滑点表现稳定，适合 MEME、土狗常规流通使用。

### Q: CPMM 会不会出现交易卡住、无法买卖？

**A:** 只要创建交易上链成功、流动性充足，即可正常自由交易。

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
