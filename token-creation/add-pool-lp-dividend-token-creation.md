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

输入完成后，点击 “创建”。

<figure><img src="../.gitbook/assets/000 (14).jpg" alt=""><figcaption></figcaption></figure>

### (4) 完成

点击 “确认创建” ，在小狐狸钱包支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/yWjc92x3CtS5eHZwU90XKNwQjefbU53bAA_npiyP6AF1G5z1SlQv2Ke7QvwP0w809kWgfOhHlwRS0-GE--_Z8WlWuIw-DojrAFMsecuSiaz0zdrhjGUG7vwCFkexWrebB7LLZYulqwLp7dyjeb6sTo4" alt=""><figcaption></figcaption></figure>

<mark style="background-color:red;">注意：</mark>

1.LP分红代币发成功之后可以在控制台设置加，撤池子手续费（注意：加池子手续费最好跟卖税一样，不然用户可以通过机器人将卖税设置成与加池子手续费一样，比如卖税100，加池子手续费0，用户可以通过机器人将卖税变成0卖出代币）。

2.<mark style="color:purple;">尾号前缀需要设置成e(小写，不要填0X,就写e)。</mark>

3.撤池子手续费默认进合约地址后按设置的买卖手续费进行分红，有需要设置指定地址的可在控制台中-》移除LP接收地址处，输入你想接收的地址，比如填黑洞，那么移除LP的税就会进黑洞地址。

4.如果需要设置不能设置撤池子，那移除LP的税就需要调整到100以上。

5.对主币池子无效（比如BNB）。

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
