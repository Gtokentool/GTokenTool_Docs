# 3️⃣ Springboard市值机器人

## 视频教程

{% embed url="https://www.youtube.com/watch?v=dXYv6_jl-PM" %}

## 介绍 <a href="#id-1-jie-shao" id="id-1-jie-shao"></a>

市值机器人，直接调用智能合约，策略/私钥本地保存，资产安全；7\*24小时运行，项目方无须长时间盯盘，合理利用时间，可节省成本；钱包地址本地批量生成，支持多地址同时导入，支持归集/空投功能，方便资产管理，刷量、拉/砸盘多策略设定，可自定义设置参数；多地址交易记录，k线自然真实。

## 操作步骤

提示：

* 请先安装小狐狸钱包插件，教程：[https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation](https://docs.gtokentool.com/fu-zhu-xin-xi/metamask-installation)
* 请确保已经充值了市值机器人会员，充值教程：[https://docs.gtokentool.com/shi-zhi-ji-qi-ren](https://docs.gtokentool.com/shi-zhi-ji-qi-ren)

### 1. 连接钱包

进入创建页面：[https://robot-nuu.vercel.app/#/marketbot](https://robot-nuu.vercel.app/#/marketbot)，点击右上角，连接钱包。

<figure><img src="../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

### 2. 输入信息

* **选择公链：**&#x42;SC&#x20;
* **选择交易所：**&#x73;pringboard
* **网络节点：**&#x68;ttps://bsc-dataseed.binance.org/

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

* **钱包使用方式：**&#x987A;序
* **模式：**&#x62C9;盘（拉升代币的价格）
* **合约地址：**&#x30;xB15815359E690fe0170435217927521209A02648
* **池子类型：**&#x42;NB
* **花费代币：**&#x42;NB（如果选择BNB，就表示买入或卖出代币，都是使用BNB来交易）
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

### 3. 导入刷单钱包

在右上角，点击“导入刷单钱包”。

<figure><img src="../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

输入私钥，一行一个，然后点击“导入”。

注：请放心，平台不会获取您的私钥。

<figure><img src="../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

在页面左下角可以查看钱包的具体详情。

<figure><img src="../.gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

### 4. 开始执行

买入授权：因为我们选择的是BNB买入，所以不用授权，如果是USDT批量买入就必须先授权。

点击“开始执行批量交易”。

<figure><img src="../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

### 5. 删除私钥

每次操作完成之后，点击导入“刷单钱包按钮”，先删除私钥，再点击“导入”。记住这里一定要点击“导入”，私钥就删除了。

<figure><img src="../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
