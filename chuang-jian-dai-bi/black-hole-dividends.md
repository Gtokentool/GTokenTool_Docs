---
description: 交易手续费打入黑洞地址销毁，间接为持币者分红的通缩型代币
---

# 黑洞分红代币发币教程

## 黑洞分红视频教程

{% embed url="https://www.youtube.com/watch?v=N_6A1fiSdr8" %}

## 1、介绍

* **分红权重**：转入黑洞地址的代币将转换为分红权重，让您的每一笔投入都能带来更多回报。
* **免费发币**：我们为用户提供免费发币服务，助您轻松发行自己的代币，无需任何费用。
* **透明收费**：我们的手续费与 PancakeSwap 一致，保证透明、公平的交易环境。

&#x20;需要注意的是, 由于逻辑复杂, 此类模版交易时使用的gas费较高, 不建议在ETH等过于昂贵的链上使用。

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://www.gtokentool.com/tokenfactory](https://www.gtokentool.com/tokenfactory)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择 “黑洞分红”。

<figure><img src="../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，填写如下：

* 代币全称：G TOKEN
* 代币简称：G T
* 供应总量：1000000（代币数量）
* 代币精度：18（小数点后的位数）
* 营销钱包地址：0x46ed16F6BCb78d05d38E4765C10CF89e2a542D43
* 选择池底：TBNB
* 选择交易所：pancakeSwapTest V2
* 黑洞分红阈值：10000（用户转入黑洞地址达到这个数量开始分红（首次转入黑洞数量必须要达到这个值，不然后续无累加））
* 分红的代币：TBNB

<figure><img src="../.gitbook/assets/000 (13).jpg" alt=""><figcaption></figcaption></figure>

输入完成后，点击 “`创建`”。

### (4) 完成

点击 “`确认创建`” ，在小狐狸钱包支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/2gPB4235RA3JrxC7b2iAyy4Catfo71ipNYMGr_eKbHXgo6DmWEGozyuW-e7MgEyjbwFY2GmzgERXwGC-bwJkpapgVVb6pHep93nyDNYoxHq9q46sBgH-DDu1diIIRMlI3dN2yuJZxHe2x36mItxy6H8" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">玩法：</mark>玩家买币之后将代币转入黑洞地址，可享受分红权益，自此，静待分红即可（黑洞地址：**0x000000000000000000000000000000000000dEaD**）。

<mark style="background-color:red;">注意：</mark>

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

## 常见问题 FAQ

### Q: 什么是 BSC 黑洞分红代币？

**A:** 黑洞分红代币是用户将持有的代币转入黑洞地址后，才能获得分红资格。具体分红哪种代币，可以在创建合约的时候填写。

### Q: 黑洞代币和普通代币有什么区别？

**A:** 普通 BEP20 无手续费、无销毁、无分红；黑洞分红代币**每笔链上交易自动扣税**，自带销毁通缩、持币躺赚，适合长效持仓模式。

### Q: 分红是如何计算的？

**A:** 按照**用户销毁数量占全网总销毁量的比例**加权分配，销毁越多，分红份额越高，每日 / 每周期自动结算发放。

### Q: 黑洞分红代币会不会每笔交易都扣税？

**A:** 是的，**仅 DEX 买卖交易扣税**，钱包点对点转账一般不扣税，不影响正常互转。若开启了转账手续费，转账也需要扣税。

### Q: 税费如何分配？

**A: 营销手续费：**&#x4EA4;易中指定额度的代币将会自动转入营销钱包中, 用于项目方做其他营销；**销毁手续费：**&#x4EA4;易中指定额度的代币将会被打入黑洞地址, 变相实现通缩机制；**回流手续费：**&#x4EA4;易中指定额度的代币将会自动添加到流动池内, 保证交易始终存在流动性；**黑洞分红手续费:** 交易中指定额度的代币, 用来购买分红代币, 并发送给持有者。

### Q: 可以更换分红币种吗？

**A: 合约部署完成后，分红币种不可修改**，保证公平防后台篡改。

### Q: 黑洞销毁是永久的吗？

**A:** 完全永久。黑洞地址无私钥、无法转账、无法找回，销毁后永久减少流通量，降低抛压。

### Q: 销毁多少代币才有分红门槛？

**A:** 可设置黑洞分红阈值，也可设置分红时间（默认一小时）。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
