# Balancer添加流动性/删除流动性教程

在 Balancer 上添加流动性（成为流动性提供者，LP）的步骤如下：

***

## **一、添加流动性池**

#### **1. 准备工作**

* **钱包连接**：确保你已安装 Web3 钱包（如 [MetaMask](../../supplementary-information/metamask-installation.md)、WalletConnect），并连接到 Balancer 支持的区块链网络（如 [Ethereum](../../token-creation/eth-token-creation.md)、[Arbitrum](../../token-creation/arb-token-creation.md)、[Polygon](polygon-shi-shen-me-polygon-qu-zhong-xin-hua-shen-me-yi-si.md) 等）。
* **资金准备**：准备好要存入[流动性池](../../decentralized-trading/create-liquidity.md)的代币。Balancer 支持 **加权池**（不同代币权重不同）和 **稳定池**（如稳定币池），需按池要求的比例存入代币。

***

#### **2. 选择流动性池**

1. 访问 [Balancer 官网](https://balancer.fi/)。
2. 点击 **"Trade"** → **"Pools"**，浏览可用的流动性池。
3. 选择目标池（如 80/20 ETH/DAX 池），查看其：
   * **代币组成及权重**（如 50% USDC + 50% USDT）。
   * **手续费比例**（通常 0.01%\~1%）。
   * **当前 APR**（年化收益率）。

***

#### **3. 添加流动性**

1. 进入目标池页面，点击 **"Add Liquidity"**。
2. **输入存入金额**：
   * 系统会自动计算其他代币的所需数量（按池权重比例）。
   * 也可选择 **单边存入**（仅存一种代币），但会自动兑换部分代币以匹配池比例（可能产生滑点）。
3. **确认交易**：
   * 钱包会提示你授权代币转账和合约交互，需支付 Gas 费。
   * 成功后会收到 **Balancer LP 代币**（BPT），代表你的流动性份额。

***

#### **4. 注意事项**

* **无常损失（Impermanent Loss）**：当池内代币价格波动时，LP 可能面临损失（相比单纯持有代币）。
* **手续费收益**：交易手续费按 LP 份额分配，需权衡收益与风险。
* **锁定期**：部分池（如 Boosted Pools）可能有锁定期，需提前确认。

***

#### **5. 管理流动性**

* **查看头寸**：在 Balancer 的 "Portfolio" 页面或 DeBank 等工具中跟踪 LP 头寸。
* **退出流动性**：随时通过 **"Remove Liquidity"** 赎回代币（按当前比例返还）。

***

#### **常见问题**

* **Gas 费优化**：在以太坊主网费用较高时，可考虑使用 Layer2（如 Arbitrum）或侧链（Polygon）。
* **池安全性**：谨慎选择未经审计的第三方池，避免智能合约风险。

## **二、移除流动性**

在 Balancer 上删除流动性（即[移除流动性](../../solana/auxiliary-tutorial/raydium-v3-add-liquidity-remove-liquidity.md)并赎回代币）的步骤如下：

***

#### **1. 准备工作**

* **连接钱包**：确保你的 Web3 钱包（如 MetaMask）已连接到 Balancer 所在的区块链网络（如 Ethereum、Arbitrum 等）。
* **确认 LP 头寸**：在 Balancer 的 [Portfolio 页面](https://balancer.fi/portfolio/) 查看你持有的流动性池份额（BPT 代币）。

***

1. **进入池页面**：
   * 在 Balancer 官网点击 **"Trade" → "Pools"**，找到你提供流动性的池。
   * 或直接在 "Portfolio" 页面选择目标池。
2. **点击 "Remove Liquidity"**：
   * 选择移除比例（如 25%、50%、100%），或手动输入数量。
   * 系统会显示你将收到的各代币数量（按当前池比例计算）。
3. **选择赎回模式**：
   * **比例赎回**：按池的当前权重返还所有代币（默认选项）。
   * **单代币赎回**：将流动性全部兑换为单一币种（需启用“高级模式”，可能产生更高滑点）。
4. **确认交易**：
   * 钱包会提示你授权 BPT 代币销毁并接收赎回的代币。
   * 支付 Gas 费后，交易完成，代币将返回你的钱包。

***

#### **3. 注意事项**

* **价格影响**：大额移除可能因滑点导致实际到账代币减少，可调整滑点容忍度（默认 0.1%）。
* **无常损失**：若代币价格波动较大，赎回时的代币数量可能与存入时不同。
* **Gas 费**：在以太坊主网高峰期费用较高，可考虑 Layer2 网络（如 Arbitrum）降低成本。

***

#### **4. 常见问题**

* **找不到 LP 头寸？**\
  检查钱包是否连接正确，或尝试在 [Zapper.fi](https://zapper.xyz/) 等聚合平台查看持仓。
* **赎回后代币未到账？**\
  在区块链浏览器（如 Etherscan）查询交易状态，确认是否成功。
* **紧急退出池**：\
  某些池（如暂停交易的池）可能需要通过 Balancer 的 [紧急赎回界面](https://balancer.fi/emergency/) 处理。

如有不明白或者不清楚的地方，请加入官方电报群：[**https://t.me/gtokentool**](https://t.me/gtokentool)
