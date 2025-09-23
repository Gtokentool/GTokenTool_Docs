# 6️⃣ 批量兑换(Swap)

与大多数交易所相比，在 gtokentool Swap 上进行交易非常容易。您不会被滑点所限制，所有计算都为您处理成最优的。

## 批量兑换流程 <a href="#kai-shi-jiao-yi" id="kai-shi-jiao-yi"></a>

在进行交易之前，您需要一个兼容 Web3区块链交互的钱包。 您可以使用metamask 等钱包插件。 您还需要一些 BEP20 代币才能进行交易。

### 1. 进入兑换页面

点击链接进入兑换页面。[https://www.gtokentool.com/batchSwap](https://www.gtokentool.com/batchSwap)

### 2. 连接钱包

如果您还没连接钱包，在您的右上角点击连接钱包。也可以通过[快捷网络添加](https://www.gtokentool.com)。快速的链接与区块链网络链接。

### 3. 选择交易代币

从按钮部分的位置选择您要交易的代币，默认选择为BNB。

<div align="center"><figure><img src="../.gitbook/assets/image (9).png" alt="" width="436"><figcaption></figcaption></figure></div>

<figure><img src="../.gitbook/assets/image (10).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="background-color:red;">**注意：**</mark><mark style="background-color:red;">（如上图所示）我们将上方的代币称为token0，下方的代币称为token1，无论您选择哪种代币，都是将token0 兑换成 token1。不管您是买还是卖都将设置好代币的顺序。以免兑换失败！</mark>
{% endhint %}

如图所示，选择您要交易的代币。接下来，通过输入框输入交易金额，**token0**代币输入1个金额。您的**token1**代币金额将自动估算，始终要记住通过token0=>token1的兑换顺序。

<figure><img src="../.gitbook/assets/image (12).png" alt="" width="426"><figcaption></figcaption></figure>

## 设置参数说明 <a href="#she-zhi-can-shu-shuo-ming" id="she-zhi-can-shu-shuo-ming"></a>

### **Gwei煤气费**

因此，首先要确保您有足够的BNB来支付链上的交易gas 费。通常gas fee 会根据链上打包的交易队列而波动，如果交易较多，则可能需要更高的 gas fee 才能推动交易。在这里可以了解更多关于[Gwei汽油费用的信息](https://academy.binance.com/en/glossary/gas)

### **滑点设置**

**BNB智能链上的代币在其合约中包含交易费**的情况并不少见，通常这些费用可用于燃烧，或进入项目方的营销钱包地址。 滑点将是对于一笔交易接收数量的容忍度，我们可以接受损失多少的代币数量，例如图中 1 USDT兑换成 0.996378....BUSD ，如滑点设置百分之**50%**。代表本次交易能容忍接受丢失百分之 **50%** 的代币，如果设置为1%，在交易发生时，丢失的代币数量大于超过1%那将会提示矿工回滚本次交易兑换操作。

### **接收地址**

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

您可以在交易对兑时设置一个固定的接收地址，批量兑换时可将token1的代币自动归集到接收地址，可节省在次归集。

### **交易截止时间**

交易上链打包等待的容忍时间，如Gwei 燃气费用突然飙升，您的交易可能在链上一直属于padding状态无法打包成功。

### **运行类型（模式）**

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

**并行执行：** 所有选中的地址将会在同一时间发起兑换交易，这样往往会出现所有的交易都在一个区块同时完成。

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

**串行执行：** 所有选中的地址会有序的进行交易，将按照从上往下的顺序一条条执行。

<figure><img src="../.gitbook/assets/image (17).png" alt="" width="466"><figcaption></figcaption></figure>

### **串行间隔时间**

1. 在串行模式下，每一个地址买入完成后，间隔停留等待一定时间在进行执行下一个地址。
2. 输入相同的2个值代表等待固定时间。

### **自定义交易模式**

1. 固定：选择自定义交易模式后，列表页面将会多出一列固定数量，根据固定金额买入。
2. 范围：列表页面将会多出一列范围输入框，范围表示根据地址的余额进行随机一个范围比例，（如输入：50～60）钱包地址中有1个BNB，将会随机0.5～0.6的BNB进行买入。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
