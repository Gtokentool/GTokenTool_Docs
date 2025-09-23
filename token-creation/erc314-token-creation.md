---
description: 席卷全球创新玩法、无需swap即可兑换、交易冷却防夹子（G TOKEN官网：https://www.gtokentool.com）
---

# ERC314代币

## 视频教程

{% embed url="https://youtu.be/EJruZv9vP_w" %}

## 1、介绍

314协议是一种新的实验性代币标准，该协议旨在降低用户交易时高昂的交易费用与繁琐的授权流程。和传统的Swap不同，314协议实现了“转账即交易”的新型功效。

* 买币：用户将BNB转入合约地址，即可获得代币
* 卖币：用户将代币转入合约地址，即可获得BNB
* 交易冷却：用户在30S内只能交易一笔
* 锁池：在设定的区块范围内，项目方无法撤池子

## 2、操作步骤

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

### (1) 连接钱包

进入创建页面：[https://token.gtokentool.com/#/](https://token.gtokentool.com/#/)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

注：公链默认为钱包所在的公链。

<figure><img src="https://lh7-us.googleusercontent.com/FDuKRIyAoUBC7fd20VlNJ09LBIRXyrEnlD8_DbxZ5Cc8mkJU_Qu-gZz9vxdtsKORj1-SaL74miqmeYPXwoj24p57nzc3rjRch24A_SYD9G9JucckSaKBK6jNJE-61EjJ-raFF-TLqiiu6vU3VsdMT8U" alt=""><figcaption></figcaption></figure>

完成后，会看到您的  “钱包地址” ，如下图：

<figure><img src="https://lh7-us.googleusercontent.com/2gNL5Tmk66SC-5n-yP0q19PqA9mMByVVBFVPL06RtlpuPGp4dEzc1c7pNFsAV9SFE-9jfi-XGST3CXL4XZ524Jd2rHHPLsjaObZ-2doNmmVO4DZvMmjZDrlrcwKdYdLDnH4a9hUHSpjFIUreeHG3dF4" alt=""><figcaption></figcaption></figure>

### (2) 选择代币模式

点击下拉框，选择“ERC314”。

<figure><img src="https://lh7-us.googleusercontent.com/qvc8KnVqywG9WzZDdcABeWpjHI5qO6CEHBQbDGj4r3lxOMc7HRcIUpQeqBqp-OecfoB6W6m2fbnxEX1OuJfHmIPE1PKqx_9oI9DZGUrUTJfRWHC-2dmQi6oOytQRWcorwnctEYmX3mEAlXYV5Pd4PlI" alt=""><figcaption></figcaption></figure>

### (3) 填写您的代币信息

依次填写代币信息，假设我们创建一个代币叫——“G TOKEN”，填写如下：

* 代币全称：G TOKEN
* 代币简称：G T
* 代币精度：18（小数点后的位数）
* 供应总量：10000（代币数量）
* 营销手续费（%）：2（需为整数）
* 燃烧手续费（%）：2（需为整数）
* 营销钱包地址：0x89ed16F6BCb78d05d38E4765C10CF89e2a782D77
* 请输入流动性代币余额：2000（池子需要添加多少代币，不要超过代币总量）
* 锁N个小时：37025
* 持币分红手续费(%)：3（需为整数）
* 最小持币分红数量：1000
* 每小时燃烧底池（‰）：5

输入完成后，点击“创建代币”并支付gas费，就完成了。

<figure><img src="https://lh7-us.googleusercontent.com/8b8YwuccKdRGR7aP1j0k-ae-xjdyBDw7Ylspd1UZQxkG86WRUVu49i5MNrK_ELZVMN3nT9rgsuXcSGAar794UxHt2rLLULRwZ9ovb1BLUmQFREvBTo2qtaAOWrej4rQOCxFalzf9LgOJfAACh_KEaHk" alt="" width="563"><figcaption></figcaption></figure>

## 3、注意事项

### 1. 能转账不能交易

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要前往PancakeSwap创建一个流动性资金池才可以。教程：[https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity](https://docs.gtokentool.com/qu-zhong-xin-hua-jiao-yi/create-liquidity)

### 2. 营销钱包分红什么币？

营销钱包，持币分红，分该链的gas币（币安链则分BNB）。

### 3. 权限丢弃后，营销钱包功能还在吗？

假设营销钱包和权限钱包是同一个，在你丢弃了权限之后，并不影响营销钱包功能的使用，同样可以加池子、撤池子、控制流动性。

### 4. 怎么计算初始代币价格？

初始价格 = “流动性代币余额”：“首次打BNB的数量”

### 5. 314协议可以用USDT或者wBNB交易或配对吗？

不支持，314协议交易只能通过BNB进行。

### 6. 为什么Ave不显示K线？

由于ave有延迟，加池子之后，需要交易数笔，才能显示K线。



如有不明白的地方，请加入官方电报群：[@](https://t.me/maleduck666)[https://t.me/gtokentool](https://t.me/gtokentool)
