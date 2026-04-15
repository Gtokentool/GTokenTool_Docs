---
description: 加池参与分红、池子越来越厚，币价螺旋上涨（G TOKEN官网：https://www.gtokentool.com）
---

# 加池（LP分红代币）

## 1、介绍

用户在去中心化交易所（如薄饼swap）添加流动性之后，用户可以获得LP代币，该模式分红可将奖励按比例直接分发到持有LP的地址，鼓励用户多多添加流动性。

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://www.gtokentool.com/tokenfactory](https://www.gtokentool.com/tokenfactory)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择 “LP分红代币”。

<figure><img src="../.gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，填写如下：

* 代币全称：G TOKEN
* 代币简称：G T
* 总供应量：1000000（代币数量）
* 代币精度：18（小数点后的位数）
* 营销钱包地址：0x46ed16F6BCb78d05d38E4765C10CF89e2a542D43
* 选择池底：TBNB
* 选择交易所：pancakeSwapTest V2
* 分红的代币：TBNB

<figure><img src="../.gitbook/assets/000 (14).jpg" alt=""><figcaption></figcaption></figure>

输入完成后，点击 “`创建`”。

### (4) 完成

点击 “`确认创建`” ，在小狐狸钱包支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/yWjc92x3CtS5eHZwU90XKNwQjefbU53bAA_npiyP6AF1G5z1SlQv2Ke7QvwP0w809kWgfOhHlwRS0-GE--_Z8WlWuIw-DojrAFMsecuSiaz0zdrhjGUG7vwCFkexWrebB7LLZYulqwLp7dyjeb6sTo4" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">注意：</mark>

1. LP分红代币发成功之后可以在控制台设置加，撤池子手续费（注意：加池子手续费最好跟卖税一样，不然用户可以通过机器人将卖税设置成与加池子手续费一样，比如卖税100，加池子手续费0，用户可以通过机器人将卖税变成0卖出代币）。
2. <mark style="color:purple;">尾号前缀需要设置成e(小写，不要填0X,就写e)。</mark>
3. 撤池子手续费默认进合约地址后按设置的买卖手续费进行分红，有需要设置指定地址的可在控制台中->移除LP接收地址处，输入你想接收的地址，比如填黑洞，那么移除LP的税就会进黑洞地址。
4. 如果需要设置不能设置撤池子，那移除LP的税就需要调整到100以上。
5. 对主币池子无效（比如BNB）。

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

## 常见问题 FAQ

### Q: **什么是 LP 分红？**

**A:** 用户在去中心化交易所加池后，除了流动性奖励，还可按比例获得额外代币分红。分红只对自己加池激活的 LP 地址有效。

### Q: 如何获得 LP 分红资格？

**A:** 必须自己加池并产生买卖交易才能激活分红，转账获得的 LP 或仅买入而不卖出都无法获得分红。

### Q: 分红是如何计算的？

**A:** 按照用户**LP 持仓数量占全网总 LP 数量的比例**瓜分奖励池，LP 持有量越多，每期分红收益越高，结算规则链上公开可查。

### Q: **分红币种如何选择？**

**A:** 创建代币时可选择主流币（如 BNB、USDT、USD1、BUSD、U、DOGE、FIST）作为分红币，所选币必须与底池代币有交易对且流动性充足。

### Q: **黑名单和白名单的作用是什么？**

**A: 黑名单**被加入的地址无法卖出或转账，可设置分红黑名单屏蔽分红；**白名单**不受交易暂停、税率限制，开盘前可交易或加池。

### Q: **哪些情况无法分红？**

**A:** 分红代币没有与 BNB 的交易对或池子流动性过小，地址是 MetaMask 智能合约地址，白名单地址（如发币地址、营销钱包地址）交易等这些情况都是不会触发分红的。

### Q: 移除流动性后还能获得分红吗？

**A:** 不能。一旦赎回 LP、移除流动池，LP 凭证会被销毁，立刻失去分红权益，仅重新添加流动性后恢复资格。

### Q: 可以多地址分散持有 LP 叠加分红吗？

**A:** 支持。多个钱包分别持有 LP，会独立计算各自份额，分红独立发放，份额可累加。

### Q: 正常交易代币会影响分红吗？

**A:** 不影响。单纯买卖、转账原生代币不会改变分红资格，**只看 LP 持仓状态**，和代币现货持仓无关。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
