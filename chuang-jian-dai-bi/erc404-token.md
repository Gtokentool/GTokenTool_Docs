---
description: G TOKEN官网：https://www.gtokentool.com
---

# ERC404

## 1、介绍

是一种新的标准，NFT与代币的结合，当用户在去中心化交易所购买一个代币时，会自动生成一个NFT。

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://www.gtokentool.com/tokenfactory](https://www.gtokentool.com/tokenfactory)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择 “ERC404”。

<figure><img src="../.gitbook/assets/image (229).png" alt=""><figcaption></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，点击上传图片，并填写如下：

* 代币全称：G TOKEN
* 代币简称：G T
* 代币精度：18（小数点后的位数）
* 总供应量：1000000（代币数量）
* 选择交易所：pancakeSwapTest V2

<figure><img src="../.gitbook/assets/000 (18).jpg" alt=""><figcaption></figcaption></figure>

输入完成后，点击 “`创建`”。

### (4) 完成

点击 “`确认创建`” ，在小狐狸钱包支付gas费，就完成了。

（注：因为每个用户网络速度不同，支付gas费用时可能会延迟1、2秒，属正常现象。）

<figure><img src="https://lh7-us.googleusercontent.com/DlgfMu8mPTlR_aNQgEinJJhHoCjN1Qry1P_YMPQ0p28PpNO1p-iRJOopJuHRx6EohVvGOGNR8J4EaVjhW2WL65C18LLKzJOQJtmsCdtMIyNyGhMwA1zdrcQ__wrp5k3eTXMg6_zzWT6-Cw4-os5k4ys" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">注意：</mark>

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

## 常见问题 FAQ

### Q: 什么是 ERC404 代币？

**A:** ERC-404 是实验性混合代币标准，核心是ERC20 代币与 ERC721 NFT 自动双向绑定、互转，实现 “持币即持 NFT、碎片可交易、整币出 NFT”。<mark style="color:purple;">1 个完整 ERC404 代币 = 1 个对应 NFT；持有 ≥1 个代币自动得 NFT；卖出 / 拆分代币则 NFT 自动销毁。</mark>

### Q: ERC404 和普通代币、NFT 有什么区别？

**A: ERC20**：可拆分、无 NFT、流动性好、无收藏属性；**ERC721 NFT**：唯一、不可拆分、流动性差、有收藏 / 稀有度；**ERC404**：**同时具备两者**：可拆分交易（币）+ 满 1 枚自动出 NFT（藏品）。

### Q: 我卖了一部分代币，NFT 怎么没了？

**A:** 机制就是如此：余额从 1.0 → 0.9：**<1 → NFT 自动销毁，**&#x518D;买回到 ≥1：**自动重新 mint 新 NFT（属性 / 稀有度可能变）。**

### **Q:** 可以只交易 NFT、不交易代币吗？

**A:** 不行。**ERC404 是强绑定**：交易代币 → 自动影响 NFT；转移 NFT → 代币也会一起走；不能单独卖 NFT、单独留币。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
