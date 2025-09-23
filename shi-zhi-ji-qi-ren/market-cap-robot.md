---
description: 全网最好的市值机器人，支持V2类型的swap
---

# 2️⃣ 市值机器人

## 市值机器人视频教程

{% embed url="https://youtu.be/G3C55Bg6iTA" %}

市值机器人支持以下链及Swap

* ETH、Arb、Base：Uniswap V2
* BSC：PancakeSwap V2
* Core：IceCreamswap、LFGswap、Archerswap

根据以下步骤，您可以在可支持的任意一条链上，进行代币市值管理。下面，以BSC测试链为例：

## 1、市值机器人介绍 <a href="#id-1-jie-shao" id="id-1-jie-shao"></a>

市值机器人（Market Cap Bot） 是一种基于人工智能（AI）和金融数据分析的工具，主要用于实时监控、分析和预测股票、加密货币或其他金融资产的市值变化。它通过自动化数据处理和算法模型，帮助投资者、交易员和机构用户快速获取市场动态，辅助投资决策。

## 2、选择公链 <a href="#id-1-xuan-ze-gong-lian" id="id-1-xuan-ze-gong-lian"></a>

目前GTokenTool市值管理机器人支持的公链有：

* BSC链（BNB Chain）
* BSC测试链（BNB Chain Test）
* Core链

## 3、选择交易所 <a href="#id-2-xuan-ze-jiao-yi-suo" id="id-2-xuan-ze-jiao-yi-suo"></a>

支持不同的去中心化交易所。BSC链和BSC测试链均支持PancakeSwap V2，Core链支持ShadowSwap。

## 4、网络节点 <a href="#id-3-wang-luo-jie-dian" id="id-3-wang-luo-jie-dian"></a>

GTokenTool会默认给出一个优质节点，用户也可以自行选择其他节点。

## 5、市值机器人操作步骤

提示：

* 请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)
* 请确保已经充值了市值机器人会员，充值教程：[https://docs.gtokentool.com/shi-zhi-ji-qi-ren](https://docs.gtokentool.com/shi-zhi-ji-qi-ren)

### **(1)** 市值机器人-**连接钱包**

进入创建页面：[https://robot-nuu.vercel.app/#/marketbot](https://robot-nuu.vercel.app/#/marketbot)，点击右上角，连接钱包。

<figure><img src="../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

### (2) 市值机器人-输入信息

* **选择公链：**&#x42;SC Test&#x20;
* **选择交易所：**&#x70;ancakeSwapTest
* **网络节点：**&#x68;ttps://bsc-testnet.publicnode.com

<figure><img src="../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

* **钱包使用方式：**&#x987A;序
* **模式：**&#x62C9;盘（拉升代币的价格）
* **合约地址：**&#x30;xB15815359E690fe0170435217927521209A02648
* **池子类型：**&#x54;BNB
* **花费代币：**&#x54;BNB（如果选择BNB，就表示买入或卖出代币，都是使用BNB来交易）
* **目标价格：**&#x30;.00004（因为我们选择的是拉盘，所以目标价格必须高于当前价格）

<figure><img src="../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

* **买入计算方式：**&#x91D1;额
* **买入金额（取两个数之间的随机数）：**&#x30;.0001 TBNB\~0.0002TBNB （如果填写100\~100，则表示每次使用100TBNB去购买代币；如果填写100\~200，则是取100\~200之间的随机数量的TBNB去购买代币）
* **时间间隔（取两个数之间的随机数）：**&#x31;00秒 \~ 200秒 （同理）

<figure><img src="../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

交易滑点(如果有夹子机器人，请设置滑点)

* 滑点%：1

Gas设置(如果有Gas设置需求，请开启该功能)

* gas(单位gwei)：0.2

钱包批量交易(如果有需要多个钱包同时买入卖出，请开启该功能)

* 执行次数(默认一次，如果需要多次请输入)：2

开始时间(如果有定时执行的需求，请开启该功能)：2024-07-20 20:00:00

<figure><img src="../.gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>

### (3) 市值机器人-导入刷单钱包

在右上角，点击“导入刷单钱包”。

<figure><img src="../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

输入私钥，一行一个，然后点击“导入”。

注：请放心，平台不会获取您的私钥。

<figure><img src="../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

在页面左下角可以查看钱包的具体详情。

<figure><img src="../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

### (4) 市值机器人-开始执行

买入授权：因为我们选择的是BNB买入，所以不用授权，如果是USDT批量买入就必须先授权。

点击“开始执行批量交易”。

<figure><img src="../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

### (5)市值机器人- 删除私钥

每次操作完成之后，点击导入刷“单钱包按钮”，先删除私钥，再点击“导入”。记住这里一定要点击“导入”，私钥就删除了。

<figure><img src="../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

## 市值机器人-常见问题

### 1. 批量买入/卖出的钱包，会被识别为夹子或者机器人吗？

不会，夹子以及机器人利用的是抢跑区块的原理，很容易判断。而市值管理系统的所有买卖都是正常的交易，不会被识别为机器人。

### 2.  平台会拿到你的私钥吗？

绝对不可能，你的私钥不会存储在平台上，所有操作都是基于前端执行的，请放心使用。

### 3. 最多可以导入多少钱包？

为了确保操作的稳定性和流畅性，一次性导入的钱包数量最好低于100个。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
