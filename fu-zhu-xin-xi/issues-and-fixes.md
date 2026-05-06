---
icon: gear-code
---

# 常见错误排查

下面把常见问题按场景列出，每项给出快速排查步骤与可行解决方法。遇到紧急问题时先按本页检查，仍未解决再到社区 [Telegram 官方群](https://t.me/gtokentool) 寻求帮助。

{% hint style="warning" %}
在动任何“Reset”或“Remove”操作之前，请确保您有正确的助记词/私钥备份！任何误操作都可能导致资产无法恢复。
{% endhint %}

### 1. 钱包连接问题

**问题表现：**&#x44;App 无法连接钱包 / 收不到弹窗授权。

**排查步骤：**

1. 确认当前钱包已解锁并且在正确的浏览器（或移动 App）上运行。
2. 检查是否处于正确网络（查看 MetaMask 顶部网络选择）。
3. 关闭并重新打开浏览器扩展或移动 App；若仍不行，尝试切换 RPC（使用备用公共节点）。
4. 若使用浏览器插件，清除页面缓存或在无痕模式/另一个浏览器试试。
5. 检查是否有广告拦截器或隐私插件阻止弹窗（禁用后重试）。

### 2. 交易失败 / revert（合约回退）

**问题表现：**&#x4EA4;易被打包但状态为失败（reverted），提示 revert 或内含错误说明。

**排查步骤：**

1. 在区块浏览器查看该 tx 的详细失败原因（有时返回了 revert 的字符串消息）。
2. 检查输入参数：目标地址、数量、合约方法名是否正确。
3. 对 ERC20 转账：确认发送者已批准（approve）足够额度给合约。
4. 若是合约调用，确认合约逻辑（例如：合约有白名单、最小持仓、暂停开关等）。联系合约开发者或检查合约公开文档。
5. 对代币创建/部署失败，注意合约部署的初始化参数与 constructor 是否正确。

**解决建议：**

* 在测试网先复现（强烈推荐）。
* 如果是 allowance 问题，先调用 approve，再执行转账/交换。
* 若是合约自身逻辑导致，需开发者修复或按合约要求操作。

### 3. Gas 不足 / Gas 估算失败

**问题表现：**&#x53D1;送交易被拒绝（insufficient funds）、估算 Gas 失败、或一直处于 pending。

**排查步骤：**

1. 确认账户中有足够的原生代币（链的 Gas 代币，例如 ETH/BNB/OKB/XPL），并非代币余额。
2. 对于支持代付或稳定币支付的链，确认是否需要额外的原生代币作为最小手续费。
3. 如果交易 pending 太久，可在钱包里使用“Speed up”（加价替换）或“Cancel”（发送一笔 nonce 相同、Gas 更高的空 tx 来替换）功能。
4. 若钱包无法估算 Gas，尝试更换 RPC（临时切换到 Infura/Alchemy/公共节点）并重新发送。
5. 若频繁出现估算失败，可能是 RPC 节点问题或合约有大量计算导致估算超时，建议使用付费节点或分步调用合约（减少单次复杂度）。

### 4. 交易卡在 pending（挂单）

**问题表现：**&#x4EA4;易一直 pending，既不失败也不确认。

**排查步骤：**

1. 在区块浏览器查看交易的 Gas Price 与当前链的平均 Gas Price 是否偏低。
2. 如果偏低，使用钱包的 Speed Up 功能以更高 Gas Price 替换；或在高级钱包中“替换交易”（same nonce, higher fee）。
3. 若想取消，发送 nonce 相同、Gas Price 更高但不做实际操作的“取消”交易（注意风险，并确保操作前已备份助记词）。
4. 若 RPC 节点有问题（节点不同步），请切换节点再查询。

### 5. 代币转账但余额未显示 / 合约未验证

**问题表现：**&#x74;x 显示成功，但钱包页面没有显示代币余额，或合约在浏览器上未验证。

**排查步骤：**

1. 确认在正确网络下查看余额（有时会把代币发到其他链）。
2. 如果是新代币，手动在钱包中“添加代币”（使用合约地址与链的 token 标准）。
3. 合约未验证：在浏览器（Etherscan / BaseScan / BscScan / PlasmaScan）搜索合约地址，若未验证，可联系发行方或按浏览器指引提交源码验证。
4. 若合约地址是 0x...，但交易显示成功且日志有 Transfer，说明链上已经有转账，只是钱包未显示该 token 的元数据。

**解决建议：**

* 手动添加 token 合约与小数位（decimals）信息。
* 推荐项目方在链上发布并验证合约源码以提高用户信任度。

### 6. 授权（approve）与被盗风险

**问题表现：**&#x6388;权给合约后无法撤回或担心被盗。

**排查步骤与建议：**

1. 使用 Revoke.cash / Etherscan Token Approvals 查看并撤销大额或不再使用的授权。
2. 对不熟悉的合约不要授予 unlimited（无限）授权，优先设置最小额度或一次性授权。
3. 定期检查授权列表，必要时撤销高风险授权。

### 7. 钱包显示“网络不匹配”或链参数错误

**问题表现：**&#x4D;etaMask 报错“已连接到错误的网络”或交易失败提示链 ID 不符。

**排查步骤：**

1. 检查钱包网络设置中的 RPC URL 与 Chain ID 是否与您要操作的链一致。
2. 若使用自定义 RPC，确认填入的 RPC 与 Chain ID、Symbol 匹配。
3. 对新链（如 Plasma、X Layer）一定要检查是否需要额外的 Gas 代币（OKB、XPL 等）。

### 8. 硬件钱包（Ledger/Trezor）常见问题

**问题表现：**&#x7B7E;名一直等待 / 设备未检测到签名请求。

**排查步骤：**

1. 确保硬件钱包的固件与管理应用（Ledger Live）已更新到最新版。
2. 在连接硬件钱包时，使用官方提供的桥接软件（如 Ledger Live 或相应的浏览器插件）。
3. 若签名被拒绝，检查硬件钱包上是否正确显示交易详情（金额、接收地址、链）。
4. 某些复杂合约调用需要在硬件钱包上手动确认额外数据；仔细阅读并确认。

### 9. 常用快速自救命令（高级用户）

* 更换 RPC：在钱包网络设置里添加/切换到稳定节点（Infura/Alchemy/QuickNode）。
* 重置 MetaMask 账户（仅清除本地交易历史，不会删除资产）：「Settings → Advanced → Reset Account」。在重置前务必确认已备份助记词。
* 查看 nonce 与替换交易：使用区块浏览器查看最新 nonce 并发送 nonce 相同的新交易覆盖旧交易。

***

⚠️注意：使用 GTokenTool 时，90% 问题来自 **钱包配置** 或 **网络问题**。

{% hint style="success" %}
1. 刷新页面 + 切换网络。
2. 清空钱包缓存 (MetaMask: Settings > Advanced > Reset)。
3. 检查 Tx Hash 在浏览器中状态。
{% endhint %}

### 📌 错误列表与解决方案速览

|                错误消息               |      原因      |                   解决方案                  |
| :-------------------------------: | :----------: | :-------------------------------------: |
|           **Out of Gas**          | Gas Limit 太低 | 手动加 Gas Limit 至 500k+。GTokenTool 默认安全值。 |
|       **Nonce Too Low/High**      |   Nonce 冲突   |     钱包等待上一笔确认，或手动设置下一个 Nonce (浏览器查)。    |
|       **Insufficient Funds**      |     余额不足     |    确认 Gas 代币 (BNB/ETH/OKB)，预留 0.1 单位。   |
|    **Replacement Transaction**    |     重复签名     |       取消上一笔，或加速 (加 Priority Fee)。       |
| **RPC Error / Network Not Found** |    RPC 失效    |              切换备用 RPC 资源列表。             |
|         **User Rejected**         |     签名拒绝     |               确认弹窗无误，重连钱包。              |
|   **Contract Deployment Failed**  |    合约代码问题    |        检查参数 (总供应 >0，无特殊字符)。测试网验证。       |
|         **Low Gas Price**         |     小费太低     |        提高 Priority Fee 至 1 Gwei+。       |
|       **Execution Reverted**      |     合约逻辑错    |           查看详情 Tx，常见于 LP 池不存在。          |
|         **MetaMask Stuck**        |  Gas 估算 Bug  |         启用 "Advanced Gas"，手动设置。         |

**仍未解决？👉🏻**加入 [Telegram 官方群](https://t.me/gtokentool) 截图求助。

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
