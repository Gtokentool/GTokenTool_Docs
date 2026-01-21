---
description: 👋 如果你是第一次接触“发币”这个概念，请放轻松——看完这篇，你就能从“币圈小白”变成“发币专家”。
icon: face-monocle
---

# 新人发币100问：打破壁垒，避开坑

区块链的世界看似复杂：各种术语、不同公链、费用机制、权限设置……&#x20;

但其实，发币这件事并不神秘。借助像 **GTokenTool** 这样的智能一键发币平台，你无需会代码，也不用担心安全与部署问题，只要几分钟，就能完成。

为帮新人打破信息壁垒，我们整理了《新人发币100问》：从基础认知到实操细节，从风险规避到合规要点，逐一拆解核心问题。不管你是想摸清发币逻辑，还是针对性解决难题，这份指引都能给你清晰答案。

## 一、基础认知篇：先搞懂“是什么”再动手

本板块聚焦发币的核心概念与底层逻辑，帮新人建立正确认知，避免因概念混淆踩坑。核心问题包括：

### 1. 我们常说的“发币”具体指什么？

* **发币：**&#x5C31;是在某条区块链上创建一个Token，这个代币的名称、数量全部由你来定义，你就是这个币的创始人。

### 2. 新手适合在哪种链上发币？

* **新手技术适配：**&#x4ECE;技术门槛、成本看，**币安智能链（BSC）、Solana 链** 更适合新手试水，GTokenTool 支持多条主流链。

### 3. 如何才能发币？

* 正常情况下，发币需要一个程序员写代码，然后将代码部署到区块链上。如果你不会写代码，就可以借助像 GTokenTool 这样的一键发币平台来完成。只需支付少量的服务费用，即可创建代币。

### 4. 发币平台有没有后门？

* 发币平台赚的是服务费，即创建费用。每次创建代币 GTokenTool 都会收取相应的费用。GTokenTool 的代码都是开源的，本地化运行。若有担忧，可自行审计合约代码。

### 5. 发币要支付多少服务费？

* 不同区块链的发币费用不一样，通常以该链本身代币支付。比如，在币安链发币，我们收取 BNB。在 Solana 链发币，收取 SOL作为服务费。具体每条链的费用可以参考[费用文档](https://docs.gtokentool.com/fu-wu-fei-yong)。

### 6. 发币了之后能不能交易？

* 只要为代币创建了流动性资金池（Liquidity Pool），就能交易。

### **7. 发的币能不能上币安、欧易？**

* 理论上不能，需要得到交易所的支持才可以。

### 8. 发的币能不能显示价格？

* 部分平台支持显示（如 Ave、GMGN、Dextool），部分平台不支持，具体需咨询对应平台客服。

### 9. 发的币，能不能看到代币的头像、简介等？

* 不同平台、钱包的规则不同 —— 部分可直接显示，部分需付费显示，部分不支持显示。

### 10. 我创建的代币能不能上GMGN、老鹰？

* 当然可以，只要创建流动性并完成交易，GMGN、Ave、Dextool、老鹰 DexScreener 等平台均可查询到代币。

### 11. 我发的币，风险监测是不是全绿？会不会高风险？

* 不同区块链、不同代币功能的风险各有不同。如果你特别在意风险这件事，那就不要创建功能代币，可以创建标准代币，风险检测全绿。因为只要带功能，就有可能有风险。

### 12. 什么是内盘？这个和一键发币有什么不同？

<table><thead><tr><th width="101.99996948242188">类型</th><th>资金池要求</th><th>代币归属</th><th>功能机制</th><th>项目方掌控权</th></tr></thead><tbody><tr><td>内盘发币</td><td>无需创建资金池</td><td>需购买，无初始代币</td><td>无任何功能</td><td>基本无掌控权</td></tr><tr><td>一键发币</td><td>需手动创建资金池</td><td>全部进入自己钱包</td><td>可创建多功能</td><td>掌控权更大</td></tr></tbody></table>

* 内盘发币：发币后不需要创建资金池，但是手里没有币，需要购买。而且内盘发币没有任何功能机制，项目方基本上没有掌控权。
* 一键发币：发币后代币全部进入自己的地址，但是需要手动创建资金池。项目方掌控权更大，可以创建不同功能的代币。

目前 GTokenTool 除了支持[一键发币](https://sol.gtokentool.com/zh-CN/Token/createToken)以外，还支持 [Pump 内盘发币](https://sol.gtokentool.com/zh-CN/pump/bundle)以及 [LetsBonk 发币](https://sol.gtokentool.com/zh-CN/LetsBonk/createToken)，并配备了多个捆绑交易工具，让交易更加高效。

### 13. 发的币权限在谁手里？怎么修改功能？

* 有些代币有权限，有些没有（例如标准代币）。假设你创建的代币拥有权限，那么这个权限默认就是支付发币费用的钱包地址。通过我们的控制台或者权限管理工具，就可以使用这些权限，或者放弃权限。
* [Solana 管理代币](https://sol.gtokentool.com/zh-CN/Token/management)、[BSC 多链代币控制台](https://www.gtokentool.com/managetokens)。

<figure><img src=".gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### 14. 发币要配备什么钱包？

* **钱包(软件/插件)：**&#x5982;果是电脑，需要安装谷歌浏览器，以及钱包插件，我们推荐小狐狸插件、OKX Web3 钱包插件。如果是手机，我们推荐 OKX 钱包软件、TP 钱包软件、小狐狸钱包软件等。
* **资产(代币)：**&#x94B1;包软件会生成钱包地址，钱包地址里要有相关的资产，以支付发币费用。例如你要在 BSC 链发币，钱包里至少得有0.05个 BNB。

## 二、技术实操篇：从0到1实现发币落地

本板块聚焦发币的技术流程，从公链选择到代币部署，用通俗语言拆解技术环节。核心问题包括：

### 1. 基础参数设置

* **全称：**&#x5C31;是这个代币的名称，例如 Bitcoin / 比特币这种，可以是中文、英文或者中英结合。
* **简称：**&#x5C31;是这个代币的符号，例如 BTC、ETH 这种，可以是中文、英文或者中英结合。
* **总供应量：**&#x4EE3;币的最大数量，建议在 10 亿 - 100 亿这个区间调整。（数量是一次性到账，无法分批或者挖矿产出）
* **精度：**&#x4EE3;币的最小分割单位，直接默认即可。
* **头像：**&#x6709;些区块链可以传头像，如 Solana。有些区块链不能传头像，如 BSC。即便传了头像之后，也并不意味着会显示出来。

### 2. 高级功能解读

* **增加功能：**&#x53EF;以随意增发代币，使得代币数量没有上限。
* **黑名单功能：**&#x5F53;一个地址被加入到黑名单之后，这个地址将无法转出或者卖出代币。
* **白名单功能：**&#x5F53;一个地址被加入到白名单之后，这个地址拥有豁免权限，例如可以豁免税率、豁免持仓限制等。
* **销毁手续费：**&#x4EA4;易中指定额度的代币将会被打入黑洞地址, 变相实现通缩机制。
* **营销手续费：**&#x4EA4;易中指定额度的代币将会自动转入营销钱包中, 用于项目方做其他营销。
* **回流手续费：**&#x4EA4;易中指定额度的代币将会自动添加到流动池内, 保证交易始终存在流动性。
* **持币分红手续费：**&#x4EA4;易中指定额度的代币, 用来购买分红代币, 并发送给持有者
* **加池分红手续费：**&#x4EA4;易中指定额度的代币, 用来购买分红代币, 并发送给LP持有者
* **最大持币量：**&#x4E00;个钱包地址最多可以持有多少代币，防止 “巨鲸” 控盘。
* **推荐返利：**&#x7528;户通过空投可绑定上下级关系，下级交易时，上级可获得推荐费用  。推荐返利只能新增至3级；推荐返利税单位为 %。
* **手动开启交易：**&#x521B;建流动性资金池后，需要手动打开此功能，代币才能进行交易，否则无法交易。
* **增加持币地址：**&#x7528;户交易时, 将会向随机地址空投最小单位代币以增加持币地址，不得超过10个。
* **杀机器人：**&#x5F00;启交易时，若检测到短时间内买入的地址，会判定为 “机器人” 并拉黑，防止机器人冲盘。
* **标准代币：**&#x6CA1;有任何功能/税率/权限，就是一个纯粹的代币，风险检测全绿。
* **持币分红：**&#x7528;户持有代币，即可获得另外一种代币的分红（如 USDT、BNB 等）。
* **营销回流代币：**&#x8BE5;模式允许设置税率自动添加流动性, 保证流动池永不枯竭. 还可以设置营销税率为项目方创造额外收益。
* **LP分红代币：**&#x6DFB;加流动性资金池成为LP的地址，可以额外获得代币奖励（一般是 USDT 或者 BNB 等）。
* **持币复利代币：**&#x7528;户持有代币，即可自动复利增发，使得余额越来越多（前几种分红来源于代币交易，复利来源于代币增发）。
* **NFT 分红+ LP 分红：**&#x8981;分红的代币(此代币必须存在与选择的交易对有相对应的池子，或者与底池一样的代币，U 池可分 U，BNB 池分 WBNB)。
* **黑洞分红：**&#x7528;户将代币转入到黑洞地址销毁后，即可获得分红资格。
* **314协议：**&#x4E00;个不通过 Swap 也能实现交易的代币合约。
* **符文：**&#x7528;户将 BNB 或 ETH 转入到预售地址进行 Mint，即可获得代币（项目启动前期筹集资金的一种方式）。
* **底池燃烧：**&#x6D41;动性资金池内每隔一段时间都会燃烧一部分代币，在池子内另一种代币（如USDT 或 BNB）不变的情况下，代币价格会自动上涨。
* **LP挖矿：**&#x7528;户添加流动性池成为 LP 之后，会获得挖矿奖励。

### 3. 不同区块链功能差异

* **EVM 系链（BSC、ETH、Base、X Layer 等）**
  * 优势：功能最丰富，适合实现复杂合约逻辑；
  * 劣势：成本与操作复杂度较高；
  * 特殊规则：通常不直接支持头像显示。
* **Solana 链**
  * 优势：热度高；可设置头像；支持创建价格稳定的代币；
  * 劣势：功能简单，仅标准代币、手续费代币 (Token2022)和持币分红三种机制；
  * 特殊规则：有黑名单、增发、更新代币资料等功能。
* **Sui 链**&#x20;
  * 优势：可以设置头像；支持创建价格稳定的代币；
  * 劣势：只有一种代币，无法设置税率；
  * 特殊规则：有黑名单、增发、更新代币资料等功能。
* **TRON 波场链**
  * 优势：可以设置并修改头像、简介等；
  * 劣势：发币费用高；功能单一，目前只有标准代币和纯手续费代币；
  * 特殊规则：名称为网址、仿币、中文币等容易被屏蔽。
* **TON 链**
  * 优势：有头像；
  * 劣势：功能单一，只支持一种代币类型；
  * 特殊规则：可以增发、更新代币资料。

## 三、上币与流通篇：让代币“活”起来

代币发行后需要流通才能产生价值，并非 “创建完成即结束”，后续的代币管理、交易支持、问题排查，直接决定项目能否顺畅运行 —— 这正是本部分的核心价值。

### 1. 发币后代币在什么地方？

* 所有代币会进入 “创建代币时连接的钱包地址”。

### 2. 为什么钱包里没有看到代币？

* 有些钱包不会直接显示代币，需要通过自定义添加代币的方式手动添加一下。

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

### 3. 发币后如何才能开源？验证合约代码？

* 不同区块链对合约验证要求不同：
  * EVM 系链（BSC、ETH、Base 等），默认开源，无需操作；
  * X Layer 区块链需要您手动开源（[开源教程](https://docs.gtokentool.com/fu-zhu-xin-xi/x-layer-dai-bi-kai-yuan-yan-zheng-jiao-cheng)）；
  * Solana 链、Sui、Ton 链暂时无需开源；
  * 波场链 TRON 需要手动开源（[开源教程](https://docs.gtokentool.com/tron/dai-bi-kai-yuan)）。

### 4. 发币后如何才能交易？

* 需要为代币创建一个流动性资金池，代币才能进行交易。不同区块链、不同交易平台，加池方式又有不同，可以详细阅读以下教程：
  * [Solana 链 Raydium AMM 创建流动性（加池子）教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-amm-create-liquidity)
  * [Solana 链 Raydium CPMM 创建流动性（加池子）教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-cpmm-create-liquidity)
  * [Solana 链添加稳定币（CLMM）流动性教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-clmm-create-liquidity)
  * [Solana 链 PumpSwap 创建流动性并买入教程](https://docs.gtokentool.com/solana/liquidity-management/pumpswap-create-liquidity-and-buy)
  * [Solana 链 Meteora DLMM 创建流动性教程](https://docs.gtokentool.com/solana/liquidity-management/meteora-dlmm-create-liquidity)
  * [币安链（BSC）创建流动性并100%提前买入教程](https://docs.gtokentool.com/kun-bang-zhuan-qu/create-liquidity-and-buy)
  * [Sui 链创建 Cetus 稳定池教程](https://docs.gtokentool.com/sui/create-cetus-stable-pool)

### 5. 不加池子可以转账吗？

* 可以，代币间的转账功能并不依赖是否有资金池，随时都能转账。

### 6. 为什么代币检测到有高风险？

* 标准代币是不会有任何风险的。许多风控或托管平台基于合约权限、资金池规模、持币分布等多种规则判断风险，不同检测平台的检测逻辑不一样，复杂功能（如增发、黑名单）更容易被标记。例如，同一个代币，OKX 检测没问题，币安检测就有问题。所以，如果大家比较在意风险的话，建议直接创建**标准代币**就可以。

### 7. 为什么代币看不到头像 Logo?

*   不同钱包、区块链、平台的显示规则不同：

    * **付费显示：**&#x90E8;分平台（如 Ave、TP 钱包）需付费才能显示；
    * **自动显示：**&#x90E8;分平台（如 OKX 钱包）可能会默认显示 Solana 链头像；
    * **手动上传：**&#x90E8;分区块链（如 BSC、ETH）需手动上传头像，并提供官网、社交媒体等资料审核；
    * **数据接入：**&#x90E8;分平台（如 PancakeSwap、Trust 钱包）会接入 CMC、CG 数据。
    * 上头像请找群管理员@xuxugege

    <figure><img src=".gitbook/assets/image (3).png" alt="" width="291"><figcaption></figcaption></figure>

### 8. 为什么代币没有价格？

* 价格显示由平台决定：
  * 支持显示：创建资金池并交易后，Ave、Dextool、GMGN 等平台可显示价格；OKX 钱包可能显示价格；
  * 不支持显示：TP 钱包等平台需满足 “高交易热度、多持币人数、大资金池” 才可能显示，无统一标准。

### 9. 要为代币制作官网、白皮书吗？

* 建议制作（若资金、技术允许）。成熟的代币项目需包含：官网、白皮书、Telegram 交流群、推特账号、Medium 博客、Discord。
* 进阶建议：
  * 联系审计公司获取代币审计报告；
  * 申请 CMC（CoinMarketCap）收录；
  * 申请 CG（CoinGecko）收录。

### 10. 我发的币，可以与线下的产业、公司或者 APP 结合起来吗？

* 具体得看结合的复杂度，总体来说不太可能。需要有专门的技术负责对接，同时代币本身也要合规才行。

### 11. 我发的币，可以在其他区块链使用吗？

* 从技术上来说，可以实现，但需要构建一个跨链桥。通过跨链桥将代币从一条链跨到多个区块链上。如果没有跨链桥支持，那是不行的。

### 12. 我发币后，没有钱加池子、上头像，可以先预售吗？

* 可以，预售本身就是用你的代币提前聚拢一部分资金，再通过这些资金去营销宣传代币。
* [符文预售](https://www.gtokentool.com/createInscription)、[IDO 私募预售](https://www.gtokentool.com/idov2?chainId=56)。

### 13. 谁可以创建资金池？

* 理论上，任何有代币的地址都可以创建，但一般来说是项目方自己创建。如果你启用了“手动开启交易”这个功能，那么除了项目方，别人无法创建。

### 14. **我创建了资金池之后，用户怎么交易呢？在哪里交易？**

* 一般来说，您在哪里创建的，用户去哪里交易。比如，BSC 链的可以在 PancakeSwap交易。ETH 链的可以在 Uniswap 交易。Solana 链的可以在 Raydium 交易等等。

### 15. **代币可以直接在OKX Web3钱包或者TP钱包的闪兑交易吗？**

* 不一定，钱包使用的是聚合 DEX，仅支持符合其要求的代币（例：TP 闪兑、Phantom 内置 Swap 对代币有明确要求）。如果您的代币无法在某些钱包交易，可以咨询一下钱包客服。

### 16. **创建资金池需要投入多少资金？有没有最低标准？**

* 首次创建流动性资金池时，并不存在一个全网统一的“最低门槛”——理论上你可以只放很少的钱。具体要放多少资金（如 USDT、BNB、ETH 等），完全取决于你的预算和项目目标，没有强制标准。

### 17. **那我投入的资金多或者少，有什么影响和区别吗？**

* 总的来说，投入的资金越多，可交易的代币数量就越多。
  * 投入 100 USDT，用户单次可买 100\~200 USDT 的代币；
  * 投入 10 USDT，用户单次仅可买 10 USDT 的代币。

### 18. 有没有一种方式，投入资金少，但用户可以买的多呢？

* 正常情况下，池子内需要有对等金额的 USDT，用户才能买入。但这种模式，在稳定池也可以实现。
* 如果是 Solana 区块链，可以通过[创建 CLMM 稳定池](https://docs.gtokentool.com/solana/liquidity-management/raydium-clmm-create-liquidity)的方式。只需通过“单币加池”的方式，添加您发行的土狗币，无需 USDT 这种价值币，也能让用户买入，这就实现了“小池子，大金额”的交易方式。

### 19. **创建资金池需要将代币加完吗？能不能预留？**

* 当然可以，假如您第一次创建流动性的时候，可以向流动性资金池内加入任意数量的代币（不能超过代币总量），无需全部进入流动性内。预留多少，完全凭自己的想法而定。

### 20. **池子里面的币会被买完吗？买完了怎么办？**

* 从资金池的合约逻辑来看，“池子里的币被买完”的情况不会出现。池子里的代币会随着买入减少，但价格会逐步升高。于是，池子里的代币无限趋近于0，代币价格不断上涨，趋近于无穷大。所以，池子代币数量不会完全变成0，只是会慢慢减少。而且随着代币价格越来越高，能买到的代币数量也会越来越少。如果想增加池子里的代币数量，可以通过增加流动性的方式实现。
* <mark style="color:blue;">重要提醒：</mark>不可直接向池子地址转账代币，否则会导致资金池内 USDT 被掏空。

### 21. **投入资金池的钱能不能取回来？**

* 创建流动性池时，你会获得一个 LP（流动性凭证）代币，代表你在池中的份额。 只要你没有销毁这个 LP 代币，就可以随时将资金池内的代币撤出。但具体能撤出多少，取决于当前池子内有多少币。

### 22. **别人买我的代币，钱去了哪里？是直接到我的地址吗？**

* 不是。别人购买你的代币，是把钱放到资金池里。然后资金池给他代币。如果是卖币，就是把币放到资金池里，资金池给他钱。所以，整个流程是依托于资金池运行的。如果你想获得用户买币的钱，将资金池撤了就可以。
  * 用户买币：将钱转入资金池，资金池向用户发放代币；
  * 用户卖币：将币转入资金池，资金池向用户发放钱；
  * 项目方收款：需撤出资金池才能获得用户买币的资金。

### 23. **别人买我的代币后，我能冻结让他不能卖吗？**

* 如果你发行的代币拥有黑名单功能，就可以实现。但是这种功能具有较高的危险性，拥有该功能的代币可能会被检测为高风险代币。

### 24. **代币价格是怎么定的？**

* 代币初始价格，由第一次加池的比例决定。如果你加100 U和100个币，那么代币的上线价格就是1 U。如果你加100 U和10000个币，代币的上线价格就是0.01 U，以此类推。
  * 加 100 USDT + 100 个币，初始价格 = 1 USDT / 个；
  * 加 100 USDT + 10000 个币，初始价格 = 0.01 USDT / 个。
* 价格涨跌只与买卖有关。当买盘大于卖盘，价格上涨，反之下跌。简单来说，买的越多价格越涨，卖的越多价格越跌。

### 25. **那代币价格能固定吗？**

* 通过创建稳定池，可以让代币的价格在一个较小的范围内波动，从而实现价格的相对稳定。
  * [Solana 链创建 CLMM 稳定池教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-clmm-create-liquidity)
  * [Solana 链 Meteora DLMM 创建流动性教程](https://docs.gtokentool.com/solana/liquidity-management/meteora-dlmm-create-liquidity)
  * [Sui 链创建 Cetus 稳定池教程](https://docs.gtokentool.com/sui/create-cetus-stable-pool)

### 26. **听说 Solana 创建资金池需要市场ID？是这样吗？**

* 不完全是这样。Solana区块链上面平台提供六种资金池类型，分别是AMM、AMM V4、CPMM、CLMM、PumpSwap 和 DLMM 稳定池。这六个，仅 AMM 需要市场 ID（创建 AMM 前需先创建市场 ID，且需支付成本）如果你不想出这个费用，可以选择其他类型创建，可以参考下面的教程：
  * [Solana 链 Raydium AMM 创建流动性（加池子）教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-amm-create-liquidity)
  * [Solana 链 Raydium CPMM 创建流动性（加池子）教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-cpmm-create-liquidity)
  * [Solana 链添加稳定币（CLMM）流动性教程](https://docs.gtokentool.com/solana/liquidity-management/raydium-clmm-create-liquidity)
  * [Solana 链 PumpSwap 创建流动性并买入教程](https://docs.gtokentool.com/solana/liquidity-management/pumpswap-create-liquidity-and-buy)
  * [Solana 链 Meteora DLMM 创建流动性教程](https://docs.gtokentool.com/solana/liquidity-management/meteora-dlmm-create-liquidity)

### 27. **那到底什么是市场ID呢？**

* Openbook Market ID是一个独特的ID，允许您的代币在defi平台上进行交易。通过这个ID，各大交易平台可以识别到你的流动性，所以一个ID只能用来对应一个交易对（如USDT/SOL）。属于历史产品，非必需操作。
* [创建市场 ID 工具](https://sol.gtokentool.com/zh-CN/liquidityManagement/createMarket)、[创建市场 ID 教程](https://docs.gtokentool.com/solana/liquidity-management/openbook-marketplace-id-creation)。

### 28. **为什么我已经创建了资金池，但是交易代币的时候还提示流动性不足？**

* 通常来说，流动性不足有两个原因：
  * DEX 不支持该流动性（例：OKX 钱包聚合 DEX 不支持部分池子）；
  * 交易数量大于资金池内代币数量，需增加流动性或降低交易金额。

### 29. 我创建的流动性是 BNB 交易对，可以用 USDT 购买吗？

* 没有问题，流动性资金池会自动将 USDT 换成 BNB 存在资金池里面的，所以无需担心，随意兑换。

## 四、常用工具篇：让交易更丝滑

### 1. 批量工具

* Solana：[批量转 SOL](https://sol.gtokentool.com/zh-CN/batchTool/batchTransfer/SOL) 、[批量转代币](https://sol.gtokentool.com/zh-CN/batchTool/batchTransfer/Token) 、[多对多转账](https://sol.gtokentool.com/zh-CN/batchTool/batchTransfer/ManyToManyTransfer)、[批量归集](https://sol.gtokentool.com/zh-CN/batchTool/gather)
* BSC：[批量发送代币](https://www.gtokentool.com/sendertoken)、[批量发送 NFT](https://www.gtokentool.com/sendernft)、[批量检查钱包余额](https://www.gtokentool.com/batchCheckBalance)、[批量归集](https://robotv2.gtokentool.com/#/collect)、[批量生成钱包](https://robotv2.gtokentool.com/#/createwallet)、[批量上传图片](https://www.gtokentool.com/uploadImage)、[增加持币地址](https://www.gtokentool.com/increaseAddr)

### 2. 市值机器人

* Solana: [Jup 市值](https://sol.gtokentool.com/zh-CN/market/jupMarket)、[Raydium 市值](https://sol.gtokentool.com/zh-CN/market/marketManagement)、[Pump 市值](https://sol.gtokentool.com/zh-CN/market/pumpMarket)
* [BSC 等多链通用市值](https://robotv2.gtokentool.com/#/marketbot)



GTokenTool 社群:

Telegram：[**https://t.me/gtokentool**](https://t.me/gtokentool)

Twitter: [**https://x.com/gtokentool**](https://x.com/gtokentool)

Gitbook：[**https://docs.gtokentool.com/**](https://docs.gtokentool.com/)

Github：[**https://github.com/Gtokentool/docs/blob/master/SUMMARY.md**](https://github.com/Gtokentool/docs/blob/master/SUMMARY.md)

YouTube：[**https://www.youtube.com/@GTokenTool**](https://www.youtube.com/@GTokenTool)&#x20;



<mark style="color:purple;background-color:orange;">**GTokenTool**</mark>_<mark style="color:purple;background-color:orange;">保留随时全权酌情因任何理由修改、变更或取消此公告的权利，无需事先通知。以上信息内容仅供参考，GTokenTool对本平台上的任何虚拟资产、产品或促销活动不做任何推荐或保证。虚拟资产的价格波动很大，投资交易虚拟资产将面临巨大风险。请谨慎投资。</mark>_
