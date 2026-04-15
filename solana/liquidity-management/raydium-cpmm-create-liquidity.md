---
icon: landmark-flag
---

# Raydium CPMM 创建流动性（加池子）教程

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

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-13-45.png" alt=""><figcaption></figcaption></figure>

### 2. 选择池子

GTokenTool 支持用户创建AMM池、 AMM V4 池、CPMM 池和 CLMM 稳定池四种，我们在这里选择 CPMM 池。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-15-22.png" alt=""><figcaption></figcaption></figure>

### 3. 选择要创建流动性池的交易对 <a href="#id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui" id="id-2.-xuan-ze-yao-chuang-jian-liu-dong-xing-chi-de-jiao-yi-dui"></a>

* **基础代币：**&#x586B;写您创建的还没有任何价值的代币。
* **报价代币：**&#x5177;有市场价值的代币，通常是 SOL 、 USDC 或 USDT。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-16-46.png" alt=""><figcaption></figcaption></figure>

### 4. 具体参数填写

* **基础代币数量：**&#x586B;写你创建的代币数量，想填多少填多少，不要超过实际拥有量。
* **报价代币数量：**&#x586B;写价值币的数量，不要超过实际拥有数量。
* **初始价格：**&#x586B;写完基础代币数量和报价代币数量后会自动为您估算初始价格。

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-17-30 (1).png" alt=""><figcaption></figcaption></figure>

### 5. 创建 CPMM 流动性效果展示

参数填写好后，点击“`创建流动性`”。钱包弹出后，点击“`确认`”。

创建成功效果展示：

<figure><img src="../../.gitbook/assets/Snipaste_2025-08-20_15-21-53.png" alt=""><figcaption></figcaption></figure>

## 常见问题 FAQ

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



[_**GTokenTool | 创建代币、批量空投和做市机器人等Solana工具集**_](https://sol.gtokentool.com/)

**安全、开源，给Solana用户带来最便利的一站式体验。**



GTokenTool社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter: [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)&#x20;



<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
