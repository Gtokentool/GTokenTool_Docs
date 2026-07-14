---
icon: '3'
---

# 币安捆绑服务使用对接教程

GTokenTool实现了与Solana的Jito类似的服务，只需要加入小费，就可以捆绑并防止夹子机器人，单笔哈希仅需0.001 BNB，以下是具体使用教程。

## 请求参数

我们简化了请求载体，使用捆绑交易只需要传递两个参数，非常简单，也让请求更加迅速。

txs中最多包含有50条交易元数据。

maxBlockNumber最多设置为当前区块的后100个区块，不能小于当前区块。

请求地址：https://bundle.gtokentool.com/sendBundleWithoutKey

| 参数             | 必选 | 格式        | 示例                        | 备注                                                                                                                                                 |
| -------------- | -- | --------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| txs            | 是  | \[]string | \[ "0xf84a......e54284" ] | <p>raw tx 签过名的交易的元数据<br><mark style="color:red;">注：第一条raw tx,需要给我们的地址转账，每笔交易价格为0.001BNB，收费地址：</mark>0x3Dc20503e9E423201685AeE8687c94b6C4f8D846</p> |
| maxBlockNumber | 是  | uint64    | 39177941                  | 该 bundle 有效的最大区块号                                                                                                                                  |

### 请求示例 <a href="#qing-qiu-shi-li" id="qing-qiu-shi-li"></a>

**Raw Bundle**

```
curl -X POST -H "Content-Type: application/json" --data '{
	"txs": ["0xf84a8080808080808193a0437a5584216e68d1ff5bd7803161865e058f9bf4637fd1391213eac03ae64444a00df12bffe475d5dd8cc1544b72ee280471f1dcb5173827ba41eb25cfc3e54284"],
	"maxBlockNumber": 39177941,
}'<ETH_NODE_URL>
```

### 返回示例 <a href="#fan-hui-shi-li" id="fan-hui-shi-li"></a>

**正常**

```
{"jsonrpc":"2.0","id":1,"result": "0x11111111..."}
```

**异常**

```
{"jsonrpc":"2.0","id":1,"jsonerror":{"code":-38000,"message":"nonce too low: address 0x9Abae1b279A4Be25AEaE49a33e807cDd3cCFFa0C, tx: 0 state: 45"}}
```

1.常见问题：提示nonce too low

原因：单个地址使用多个绑定服务（如授权和买入一起），需要有不同的nonce。

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
