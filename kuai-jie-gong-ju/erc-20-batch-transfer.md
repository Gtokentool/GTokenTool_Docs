# 🥨 ERC20批量转账

ERC20 批量转账是一种将多笔代币转账操作打包到单笔链上交易中一次性完成的技术。其核心原理是把多个接收地址和对应金额以数组形式作为参数传递给合约，由合约在一个循环中依次执行 transfer 或 transferFrom 操作。批量转账不仅将多次链上交互简化为一次，还能显著降低总 Gas 消耗，因为多笔交易共享一次「21000 Gas」的基础交易开销。

## GTokenTool批量转账工具介绍 <a href="#gtokentool-dai-bi-pi-liang-zhuan-zhang-gong-ju-jie-shao" id="gtokentool-dai-bi-pi-liang-zhuan-zhang-gong-ju-jie-shao"></a>

GTokenTool 批量转账工具，支持ETH、BSC、Base、Arbitrum等多条EVM公链，大大的简化了转账与空投流程，可以快速实现代币空投与转账等多种操作。

## 适用场景

*  项目上线空投：新币发行后快速向社区、KOL、早期投资者分发代币，提升持币地址数量和活跃度。
* 营销活动：空投奖励、测试网激励、合作伙伴分润。
* 团队/股东分红：批量向多地址发放收益。
* 钱包管理：多钱包归集或分发代币。

## ERC20批量转账流程 <a href="#pi-liang-zhuan-zhang-liu-cheng" id="pi-liang-zhuan-zhang-liu-cheng"></a>

### **第1步，连接钱包**

进入GTokenTool批量转账页面：[https://gtokentool.com/sendertoken](https://gtokentool.com/sendertoken)，点击右上角，连接小狐狸钱包，并切换到主网。

完成后，会看到 “链名称” 和 您的“钱包地址” ，如下图：

<figure><img src="https://docs.gtokentool.com/~gitbook/image?url=https%3A%2F%2F1523574308-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FaUD1j15UCzdjC6ftyzSr%252Fuploads%252FMe84PVEWqJNNWp9RUVZW%252F1.png%3Falt%3Dmedia%26token%3Decdbf597-c66c-4d2a-a7ab-801556817a5b&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=36e61d03&#x26;sv=2" alt=""><figcaption><p>连接钱包并选择公链</p></figcaption></figure>

### **第2步，输入转账信息**

假设我们给三个地址发送不同数量的代币，输入如下：

* 代币地址：BNB
* 收款地址和数量

<figure><img src="https://docs.gtokentool.com/~gitbook/image?url=https%3A%2F%2F1523574308-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FaUD1j15UCzdjC6ftyzSr%252Fuploads%252FBJLIw7to0g6VYPB8Ue3V%252F1.png%3Falt%3Dmedia%26token%3Dcd860495-0e2f-47b4-8e65-befb9f437b11&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=4ba7ae04&#x26;sv=2" alt=""><figcaption><p>输入转账信息</p></figcaption></figure>

### **第3步，完成转账**

输入完成后，点击 “`下一步`” 按钮。

<figure><img src="https://docs.gtokentool.com/~gitbook/image?url=https%3A%2F%2F1523574308-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FaUD1j15UCzdjC6ftyzSr%252Fuploads%252FDHdM0fCaYnglocNOa4Ko%252F1.png%3Falt%3Dmedia%26token%3D421935ea-1fb0-4f67-8ddd-9eab7451cc3f&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=45272ad2&#x26;sv=2" alt=""><figcaption><p>转账完成</p></figcaption></figure>

确认无误后，点击 “`发送`” 按钮，在小狐狸上支付gas费，就完成了。

ERC20批量转账工具的核心价值在于省时、省Gas、高效空投，特别适合项目方社区营销、团队分红等场景。

### 🤝 连接 GTokenTool <a href="#lian-jie-gtokentool" id="lian-jie-gtokentool"></a>

* **💬 Telegram社群**：[点击加入官方群组](https://t.me/gtokentool)
* **🐦 Twitter (X)**：[关注我们获取最新动态](https://x.com/gtokentool)
* **📚 官方文档**：[查看 Gitbook 文档](https://docs.gtokentool.com/)
* **💻 开源代码**：[访问 GitHub 仓库](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)
* **📺 视频教程**：[订阅 YouTube 频道](https://www.youtube.com/@GTokenTool)

> ⚠️ 风险提示与免责声明
>
> GTokenTool 保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。
>
> 以上信息内容仅供参考，GTokenTool 对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。**请谨慎投资。**
