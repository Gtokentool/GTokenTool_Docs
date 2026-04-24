# ⚡ 代币批量转账

代币批量转账是一种通过智能合约或特定工具，在一次交易中向多个不同钱包地址发送代币的技术方案。

### 代币批量转账视频

{% embed url="https://youtu.be/7WbdDzfv_20" %}

### GTokenTool代币批量转账工具介绍

GTokenTool代币批量转账工具，支持ETH、BSC、Base、Arbitrum等多条EVM公链，大大的简化了转账与空投流程，可以快速实现代币空投与转账等多种操作。

### 批量转账费用

Bsc链：0.01 BNB / 200个地址\
Sol链：0.004 SOL\
SUI链：每次收取2 SUI\
TON链：0.02 TON/每地址\
OKB链：每次收取0.1OKB

### 为什么需要批量转账？

* **节省 Gas 费用：**&#x867D;然发送的总代币量不变，但由于合并了交易头部信息并减少了与合约多次交互的固定开销，总的手续费通常比逐个转账低 30% - 60%。
* **节省时间：**&#x624B;动发送 100 笔转账可能需要一小时，而批量工具只需几秒钟配置。
* **确保同步性：**&#x5728;空投或发放奖励时，所有接收者几乎能在同一时间收到代币，避免了因时间差导致的二级市场价格波动风险。

### 批量转账应用场景

* **项目空投 (Airdrop)：**&#x52A0;密货币项目方为了推广，向成千上万个活跃用户地址派发代币。
* **工资/奖励发放：**&#x44;AO 组织或区块链公司定期向成员发放代币化薪水。
* **流动性激励：**&#x5411;提供流动性的质押者分发收益。
* **分销与营销：**&#x5728;社交媒体活动后向中奖名单分发奖品。

### 批量转账流程

#### 第1步，连接钱包 <a href="#di-1-bu-lian-jie-qian-bao" id="di-1-bu-lian-jie-qian-bao"></a>

进入GTokenTool代币批量转账页面：[https://gtokentool.com/sendertoken](https://gtokentool.com/sendertoken)，点击右上角，连接小狐狸钱包，并切换到主网。

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="../.gitbook/assets/1 (67).png" alt="连接钱包"><figcaption></figcaption></figure>

#### 第2步，输入信息 <a href="#di-2-bu-shu-ru-xin-xi" id="di-2-bu-shu-ru-xin-xi"></a>

假设我们给三个地址发送不同数量的代币，输入如下：

* 代币地址：BNB
* 收款地址和数量

<figure><img src="../.gitbook/assets/1 (68).png" alt="输入信息"><figcaption></figcaption></figure>

#### 第3步，完成 <a href="#di-3-bu-wan-cheng" id="di-3-bu-wan-cheng"></a>

输入完成后，点击 “`下一步`” 按钮。

<figure><img src="../.gitbook/assets/1 (69).png" alt="完成转账"><figcaption></figcaption></figure>

确认无误后，点击 “`发送`” 按钮，在小狐狸上支付gas费，就完成了。

### 注意事项

1. **权限授权：**&#x5728;使用批量转账工具时，通常需要先授权智能合约动用你钱包里的特定额度。
2. **地址校验：**&#x7531;于是一次性发送，一旦地址列表出现格式错误或包含错误地址（如不支持该代币的合约地址），可能导致部分转账失败或资产丢失。
3. **链上限制：**&#x4E0D;同的区块链（如 Ethereum、Solana、BNB Chain）对单个区块能容纳的交易指令有上限。如果一次性批量发送数千个地址，可能需要分批次进行（例如每 200 个地址为一个批次）。

{% hint style="info" %}
如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
{% endhint %}
