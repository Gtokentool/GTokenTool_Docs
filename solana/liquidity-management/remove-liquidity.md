---
icon: wave
---

# Solana移除流动性教程

## 准备事项

1. 一台电脑或者一部手机
2. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
3. 钱包准备充足余额

## Solana移除流动性池流程

### 1. 连接钱包

进入GTokenTool 移除流动性页面，右上角选择 Main 网络并连接钱包。

移除流动性： [https://sol.gtokentool.com/zh-CN/liquidityManagement/remove](https://sol.gtokentool.com/zh-CN/liquidityManagement/remove)

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-36-30.png" alt=""><figcaption></figcaption></figure>

### 2. 输入基础代币地址

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-51-13.png" alt=""><figcaption></figcaption></figure>

### 3. 选择对应的报价代币

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-51-00.png" alt=""><figcaption></figcaption></figure>

### 4. 选择对应的DEX

选择好后，下面会显示对应的池子信息以及我的持有量。（支持 Raydium AMM、Raydium CPMM、Raydium CLMM、PumpFun Swap流动性池)

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-57-29.png" alt=""><figcaption></figcaption></figure>

### 5. 输入移除数量

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-57-49.png" alt=""><figcaption></figcaption></figure>

### 4. 点击“移除流动性”

弹出钱包后，点击“`Confirm`”，完成交易。

<figure><img src="../../.gitbook/assets/Snipaste_2026-02-26_10-57-59.png" alt=""><figcaption></figcaption></figure>

## 常见问题 FAQ

### Q: 什么是移除流动性？

**A:** 退出资金池，销毁 LP，拿回自己的代币 + 报价代币。

### **Q:** 为什么拿到的币数量和当初不一样？

**A:** 受币价波动、交易手续费、滑点影响，数量会有浮动。选择波动性低的配对（如稳定币对）或者使用对冲工具（如期权）或仅在看好两种代币时提供流动性。

### **Q: 交易失败但扣除了 SOL 手续费？**

**A:** Solana 网络失败交易仍会消耗少量 Gas。检查网络状态（如 Solana Status），避开拥堵时段。确保钱包余额足够（建议预留 0.1 SOL）。

### Q: 为什么无法移除流动性？

**A:** LP 数量不足、钱包授权过期、RPC 卡顿、池子已枯竭、合约锁定 / 黑名单限制。

### Q: 部分移除和全部移除有什么区别？

**A:** 部分移除：保留部分流动性；全部移除：清空池子所有持仓。

### Q: 移除流动性后还能再加回去吗？

**A:** 可以，随时重新添加流动性。

### Q: 撤池失败交易报错怎么办？

**A:** 切换 RPC、清理缓存、重新连接钱包、小额尝试重试。



[_**GTokenTool | 创建代币、批量空投和做市机器人等Solana工具集**_](https://sol.gtokentool.com)

**安全、开源，给Solana用户带来最便利的一站式体验。**



GTokenTool社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter:  [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)\
\
\
<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
