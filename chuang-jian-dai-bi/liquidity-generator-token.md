---
description: 交易手续费用于项目营销，实现资金回流反哺生态的代币
---

# 营销回流代币

## 营销回流代币视频教程

{% embed url="https://youtu.be/rp3SZZoEdU4" %}

## 1、介绍

该模式允许设置税率自动添加流动性, 保证流动池永不枯竭. 还可以设置营销税率为项目方创造额外收益。

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://www.gtokentool.com/tokenfactory](https://www.gtokentool.com/tokenfactory)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择 “营销回流代币”。

<figure><img src="../.gitbook/assets/image (224).png" alt=""><figcaption></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，填写如下：

* 代币全称：G TOKEN
* 代币简称：G T
* 供应总量：1000000（代币数量）
* 代币精度：18（小数点后的位数）
* 营销钱包地址：0x46ed16F6BCb78d05d38E4765C10CF89e2a542D43
* 选择池底：TBNB
* 选择交易所：pancakeSwapTest V2

<figure><img src="../.gitbook/assets/000 (10).jpg" alt=""><figcaption></figcaption></figure>

输入完成后，点击 “`创建`”。

### (4) 完成

点击 “`确认创建`” ，在小狐狸钱包支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/1kWxTs_DyVLEQZtRwEj8F2xnlf9wHXEuGPGBFqkDz0PSB6BVNcriMtfRX1Xtm8EbnmzgDi0i3wxWr8a5OxuR-SgmdZzEPNmKUJh7vL8voes-3V4j1yrJrpRJj-fz27t2whdoiXO_5q9KvHHuHqmPy-o" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">注意：</mark>

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

## 常见问题 FAQ

### Q: 什么是 BSC 营销回流代币？

**A:** 是带有**交易税负机制**的 BEP20 代币，每一笔买卖自动扣除手续费，按规则拆分：自动回流分红给持币用户；自动销毁代币通缩；营销 / 开发钱包税收（用于运营、推广）。

### Q: 和普通标准版代币有什么区别？

**A:** 普通代币无任何交易税收，转账免费；营销回流代币**每笔买卖扣税**，自带持币分红、自动销毁、营销扣费，适合土狗、MEME、长效运营项目。

### Q: BSC 回流代币安全吗？

**A:** 合约为开源标准模板，本身无漏洞；风险主要来自**管理员权限**，关闭黑名单、销毁权限、移除合约控制权后，就是安全版本。

### Q: 营销代币的税率一般设置多少？

**A:** 行业常规标准：买入税：3%\~8%；卖出税：5%\~12%。拆分自定义：分红、销毁、营销池、开发池可自由分配比例。

### Q: 回流代币能正常添加钱包吗？

**A:** 完全可以，和普通 BEP20 一样，小狐狸、TP、钱包手动添加合约地址即可显示余额与分红。

### Q: 带税代币转账会扣税吗？

**A:** 默认**仅 DEX 买卖扣税**，钱包点对点互转不扣税，不影响正常转账流通。若开启转账手续费，则需要扣税。

### Q: 为什么我卖出到手数量变少了？

**A:** 因为触发**卖出手续费**，扣除回流、销毁、营销税后，才是实际到账数量，属于合约正常机制。

### Q: 带税代币会不会无法交易？

**A:** 税率过高（卖出＞15%）会导致 DEX 路由报错、滑点异常；合理区间内配置税率，完全兼容 PancakeSwap 所有路由。

### Q: 营销代币有黑名单功能吗？

**A:** 模板自带黑名单可选，建议**部署后关闭黑名单权限**，避免限制用户交易、引发跑路质疑。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
