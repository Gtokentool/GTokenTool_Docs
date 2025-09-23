---
description: 全网最好用的BSC和BASE多链批量转账空投工具
---

# 1️⃣ 批量转账-批量发送空投代币

## 批量转账工具介绍

GTokenTool多链批量转账工具，支持ETH、BSC、Base、Arbitrum等多条EVM公链，大大的简化了转账与空投流程，可以快速实现代币空投与转账等多种操作。

提示：请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)

## 批量转账工具使用流程

### 第1步，连接钱包

进入GTokenTool批量转账页面：[https://gtokentool.com/sendertoken](https://gtokentool.com/sendertoken)，点击右上角，连接小狐狸钱包，并切换到主网（这里以BSC测试网为例)。

<figure><img src="https://lh7-us.googleusercontent.com/gf3ho8iEOWdZ6l5WkDlPZxbKNT_CFjiCJbDjXO6u4bwHU8EKdz-Rl9XOw_-t4q89mr_46jo79lDkh3rGpR_JXNRamJfdb76fUuf22kCvDskV23QTiDusrdv9zHNvhcfGEp-Dg_mIB2BpCWVjbi_v_7E" alt=""><figcaption></figcaption></figure>

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="https://lh7-us.googleusercontent.com/WhMhizOEkTeTbsLmcjI91mKH9e6Z458de7d8osvO6Krv2VCG1Fv5cXdVHhEO8Ps2Z97_pPtF9Wkff3EdbGVCd4Zb7VQ4z1LF9-VK4R-nFm5PJHMROZJdLJZhF9MThLfCb4MQ9M34pdQrr4MoNlaShOs" alt=""><figcaption></figcaption></figure>

### 第2步，输入信息

假设我们给三个地址发送不同数量的代币，输入如下：

* 代币地址：0x0b29b9959e315e68c007b2cc376ea16f3c850951
* 收款地址和数量（逗号分隔）：
* 0x13FC5BD0A0ee0E1DD30176b833D436B95c9E2cD2,0.001
* 0x697FfC45A1bF65ca69601F06743219E86B94B0B1,1
* 0xAb8dF92b986b91A4964339BD044849DFfEA71AA8,3.45

输入完成后，点击 “下一步” 按钮。

<figure><img src="https://lh7-us.googleusercontent.com/B8UkNj3KS0pdAZDOeRAZdOKzbshvvk0_sviWrnGwxyAqSQqGaozP7To4uOFa8xCCSvoUAaQyM3QQZ0vTXawn7D1u2QqBBXNuvTKL-Elb5EdHs9Ubo1bjUf_wYRXjaIHmNXRnsImOZqU_W0DKzwjC-zo" alt=""><figcaption></figcaption></figure>

（不明白可以点击右下角 “查看例子”）

### 第3步，完成

点击 “发送” 按钮，在小狐狸上支付gas费（下一步>批准>确认），就完成了。

（注：因为每个用户网络速度不同，支付gas费用时可能会延迟1、2秒，属正常现象。）

<figure><img src="https://lh7-us.googleusercontent.com/1wCBsw9KQeTYUbULZfNh42zn2JAAIwC8Xf2GCYptwCt09DJGlV4HN1hmK4L7tEZNtV1mJOrPnMPv-mR-yFGnwMpccya7cfCc_xedSinm723gwLtSoEZ47xBB3jb8JkIXFnvYzYz94Fe-hdvkU6vaaXI" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-us.googleusercontent.com/7wFVCGer8aMcSieCQqD2_HYwmviyYPw9EZHq8pEdUdJdJ1Xw42oh65VZzGCPd-kx3rcsbzolLiAAw_WBa-DITJlMwNQh-pnQVHFyzG5Q5MRKOu1TYIX2wibuFb6d0PyAJc8eZlW9atq1-b9rW2CMylE" alt=""><figcaption></figcaption></figure>

### 参数说明  <a href="#can-shu-shuo-ming" id="can-shu-shuo-ming"></a>

1. **转账方式** :
   * **使用私钥** : 需要在`选择钱包`选项展开,并点击`导入钱包`将钱包导入进行批量转账操作。
   * **使用当前连接的钱包** : 使用当前连接网页的`小狐狸`(或者`TokenPocket`)进行确认交易操作。
2. **转账金额** :
   * **相同金额** : 向目标地址发起批量转账的**金额相同**(能够设置`统一金额`)。
   * **不同金额** : 向目标地址发起批量转账的**金额不同**(需要进行与模板格式`地址,数量`一致的格式化操作)。
3. **选择公链** : 选择`使用私钥`的转账方式才需要选择此项,用于选择你要操作的公链。
4. **选择钱包** : 选择`使用私钥`的转账方式才需要选择此项,用于选择你要操作的钱包。
5. **选择转账的币种** :
   * **转账BNB** : 转账BNB无需输入合约地址。
   * **转账合约代币** : 转账合约代币需要输入代币合约,随后会显示该代币基本信息方便核对。
6. **转账地址** : 需要发起批量转账交易的目标地址。
   * **相同金额** : 能够设置`统一金额` 。
   * **不同金额** : 需要进行与模板格式`地址,数量`一致的格式化操作。

## 常见问题解答 <a href="#chang-jian-wen-ti-jie-da" id="chang-jian-wen-ti-jie-da"></a>

### 1.、收款地址和数量必须用英文逗号分隔。

### 2、推荐使用PC端操作，更加方便快捷。

### 3、如往交易所地址进行转账，请务必确认交易所是否支持合约转账，否则你的转账将无法到账。

### 4、为保证转账顺利，一次转账的地址数请勿超过100个。

### 5、支持大部分EVM公链，切换到哪个钱包，就自动在哪个链上转账。

如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
