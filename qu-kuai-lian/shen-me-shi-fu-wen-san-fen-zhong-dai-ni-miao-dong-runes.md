---
description: Runes协议，是在比特币网络上基于UTXO特性发行同质化代币的协议
---

# 什么是符文？三分钟带你秒懂Runes

比特币符文是存在于比特币区块链上的独特的、可替代的代币。它们旨在代表具有独特特征元数据的可替代资产。由 Ordinals 协议的创建者 Casey Rodamor 提案，该方案被称为Runes。

Runes 旨在为 Ordinals、ORC-20、BRC-20 和 Stamps 等现有代币化协议提供一种用户友好的、基于 UTXO 的替代方案。符文是比特币网络上一种全新类型的可替代代币。这些代币在几个方面与现有替代品不同。首先，符文原生于比特币的未花费交易输出（UTXO）模型。这最大限度地减少了「垃圾」UTXO 的产生，从而实现更负责任的 UTXO 管理和更小的链上足迹。比特币区块链被设计为一个最小且高效的分类账，用于通过比特币交易转移价值。

在已有协议的背景下，每个协议都有其一系列挑战，Runes 应运而生——在复杂的景观中独具简洁之光。由 Ordinals 协议背后的创新者 Casey Rodamor 构想。

Runes 旨在解决许多先前协议（尤其是 BRC-20）的低效问题。 起源：这一切源自一篇粗糙的博客文章勾勒出的概念，Rodamor 在提出 Runes 后七小时内便已上线，也证明了加密社区的灵活性。

符文的核心愿望是修复 BRC-20 的缺陷。尽管 BRC-20 被广泛采用，但由于其依赖铭文而导致的低效问题让其颇受影响。这导致了执行基本操作时冗长的多步交易。相比之下，Runes 试图简化这个过程，简化代币操作并提高链上效率。

**其他协议的优缺点**

**BRC-20：**&#x56E0;其与铭文的关联而闻名，其设计更多地受到流行技术的驱动，而非高效工程。结果是一个效率极低的协议，执行基本操作，从发行代币到转移代币，需要多个交易。

**RGB：**&#x8FD9;一协议较为复杂，它在很大程度上依赖于链下数据，其开发一直跳票，并且应用范围有限。

**Omni Layer：**&#x8FD9;个协议都引入了一些操作所需的原生代币。虽然创新，但它们也带来了额外的复杂性，并减少了采用范围。

**Taproot Assets：**&#x8FD9;一协议虽然先进，但在很大程度上依赖于链下数据，在实施和用户体验方面可能遇到的障碍。

**Runes 发币协议的一些细节**

**deploy：**&#x901A;过构造 op\_return 中带有如下信息的交易来实现符文的部署

<figure><img src="../.gitbook/assets/1 (27).png" alt=""><figcaption></figcaption></figure>

在 Deploy 交易中，可以在 op\_return 中同时带有如下信息来实现部署的同时项目方预留代币

<figure><img src="../.gitbook/assets/2 (26).png" alt=""><figcaption></figcaption></figure>

**部署的符文有 3 种启动方式：**

term 设置为 0，带有 Edict，代表部署的符文全部在项目方手中

term 不为 0，不带有 Edict，代表项目方不预留符文，在满足 deadline 和 term 两个约束条件时可以 fair mint

term 不为 0，带有 Edict，代表项目方预留符文，在满足 deadline 和 term 两个约束条件时可以 fair mint

**Mint：**&#x6EE1;足约束条件下，只需要在 op\_return 中带有如下信息，即可实现 mint，mint 的数量在部署的时候已经进行了限定

<figure><img src="../.gitbook/assets/3 (22).png" alt=""><figcaption></figcaption></figure>

Transfer：输入利用带有符文的 utxo，然后利用 op\_return 带有 Edict 信息，指定转账到哪一个 utxo。

<figure><img src="../.gitbook/assets/4 (18).png" alt=""><figcaption></figcaption></figure>

目前许多符文项目方空投的条件一般都是持有龙头runestone，rsic还有一些指定的nft和一些质押者钱包及指定铭文持有者。



如有不明白或者不清楚的地方，请加入官方电报群：[https://t.me/gtokentool](https://t.me/gtokentool)
