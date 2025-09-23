---
description: 黑名单功能升级版，根据自定义参数配置，自动禁止某些帐户执行如发送交易等特定操作，有助于防止恶意机器人行为对资产造成损害。
icon: file-lock
---

# Solana自动冻结教程

## 准备事项 <a href="#zhun-bei-shi-xiang" id="zhun-bei-shi-xiang"></a>

1. 一台电脑或者一部手机
2. Solana 钱包（[幻影钱包Phantom安装教程](https://docs.gtokentool.com/solana/auxiliary-tutorial/phantom-wallet-installation)）
3. 要进行监控的代币所属的钱包私钥
4. 要监控的代币
5. 请确保跟踪钱包有足够的 SOL 和代币，少量的 USDC

## Solana自动冻结具体操作流程

### 1. 连接钱包

进入Solana自动冻结页面：[https://sol.gtokentool.com/zh-CN/airdropSection/AutoFreeze](https://sol.gtokentool.com/zh-CN/airdropSection/AutoFreeze)，右上角点击连接钱包并选择 Main 网络。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_13-41-35.png" alt=""><figcaption></figcaption></figure>

### 2. 单钱包监控单代币（可选）

默认单钱包监控多代币，导入一个钱包监控多种代币。单钱包监控单代币时，请确保持有该代币的钱包和代币的序号对应，可以导入重复的钱包。

### 3. 自动冻结（可选）

默认通过 TG 机器人半自动冻结。

### 4. 自定义节点（可选）

打开后输入自己的 HTTP节点。

### 5. 打开“Telegram 通知”

根据[设置自动冻结播报教程](https://docs.gtokentool.com/solana/airdrop-section/set-up-auto-freeze-broadcasts-tutorial)设置跟卖播报，填写群ID。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_13-55-37.png" alt=""><figcaption></figcaption></figure>

### 6. 冻结条件设置（可选）

默认全部冻结，可对USDC买入数量和代币买入数量进行条件设置。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-06-16.png" alt=""><figcaption></figcaption></figure>

### 7. 冻结白名单（可选）

已添加白名单地址不会被冻结。

### 8. 新增代币

点击“`新增代币`”，添加需要监控的代币。

{% hint style="warning" %}
若要补充代币，请先关闭跟踪。如果关闭失败，请刷新网页。\
目前支持添加和跟踪 Raydium CLMM 的 USDC 池子，请确保跟踪钱包有足够的 SOL 和代币，少量的 USDC。
{% endhint %}

添加成功后，下面的表格里可以看到代币的信息。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-11-30.png" alt=""><figcaption></figcaption></figure>

### 9. 导入钱包

点击“`导入钱包`”，添加代币所属的钱包。<mark style="color:purple;">注意：导入钱包的顺序要与监控的代币一致。</mark>

导入成功后，可以看到钱包内SOL余额以及基础代币余额。可以点击“`刷新钱包`”获取当前钱包余额，<mark style="color:purple;">建议每次使用前刷新一次</mark>。也可点击`删除`按钮删除对应的钱包，或者点击“`全部删除`”按钮删除全部钱包。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-12-24.png" alt=""><figcaption></figcaption></figure>

### 10. 选择要监控的代币并点击“运行选中”

先勾选钱包，再选择要监控的代币，最后点击“`运行选中`”。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-13-40.png" alt=""><figcaption></figcaption></figure>

点击“`运行选中`”后，下面的日志会显示代币已监控。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-14-17.png" alt=""><figcaption></figcaption></figure>

代币的状态也会变成“激活”状态。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-14-44.png" alt=""><figcaption></figcaption></figure>

### 11. 等待其他人的买入操作，机器人会发送信息提醒

可以在日志中查看到监控情况。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-16-12.png" alt=""><figcaption></figcaption></figure>

同时，Telegram 中的机器人也会发送信息。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-16-45.png" alt=""><figcaption></figcaption></figure>

### 12. 取消监控

若要补充代币，请先关闭跟踪。点击“`停止选中`”可以关闭监控。日志中会显示代币已取消监控。代币状态会变回未激活。

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-18-50.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Snipaste_2025-09-05_14-18-59.png" alt=""><figcaption></figcaption></figure>

[_**GTokenTool | 创建代币、批量空投和做市机器人等Solana工具集**_](https://sol.gtokentool.com)

**安全、开源，给Solana用户带来最便利的一站式体验。**



GTokenTool社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter:  [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)\
\
\
<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
