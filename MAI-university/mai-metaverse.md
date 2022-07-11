---
description: 本指南将概述可以使用 MAI 稳定币的不同链以及如何将原生货币桥接到其他网络。
---

# MAI Metaverse

![](../.gitbook/assets/MAI.png)

## 介绍

MAI，有时被称为 miMATIC，是第一个来自 Polygon 网络的稳定币。它与 1.00 美元软挂钩，其价值可能在 0.99 美元和 1.01 美元之间波动。你可以在[官方文档](https://docs.mai.finance/stablecoin-economics)中获得有关如何维护挂钩的更多详细信息。但这并不是因为 MAI 是 Polygon 原生的，所以它只能在该网络上找到。确实，就像你可以在不同的网络上找到 DAI 一样（DAI 实际上是另一种来自以太坊主网的稳定币），MAI 也在缓慢但肯定地扩展到其他网络。本文将突出可以找到它的不同网络，以及如何将 MAI 从一个网络转移到另一个网络。

## Polygon

### 在Polygon上获取MAI

正如所解释的，MAI 是 Polygon 原生的，这是你可以铸造 MAI 的唯一地方（截至 2021 年 9 月）。这由以下情形完成

* 以你之前存放在 Mai Finance 上的金库中的某些抵押品借入 MAI
* 在 [Mai Finance](https://app.mai.finance/anchor) 上用 USDC 互换成 MAI
* 出售另一种资产并在 Polygon 上的任意 DEX（Decentralized EXchange）上购买 MAI，最有效的是 [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) 或 [Inc](https://app.1inch.io/#/137/classic/swap)

### 在Polygon上使用MAI

MAI 稳定币正在 Polygon 上越来越多的项目中使用，尤其是现在它被用作 QuickSwap 等大项目的其他稳定币。截至 2021 年 9 月，QuickSwap 上有 3 个稳定的农场，总数为 18,327,604 美元：

* MAI-DAI 为 6,553,255 美元
* MAI-USDT 为 6,316,026 美元
* MAI-USDC 为 5,458,323 美元

可以在其他的项目/产量农场/产量优化器上找到额外的池。你可以在[专门的文章](../jiao-cheng/polygon/what-to-do-with-mai-on-polygon.md)中阅读有关如何处理 MAI 稳定币的更多信息。&#x20;

## Solana

### **在Solana获取MAI**

Solana 是一个用于去中心化应用程序的区块链平台。该网络的目标是提出低费用（低于 0.01 美元）和快速（低于 400 毫秒）的交易。这背后的想法是为以太坊主网及其侧链创建一些替代方案。然而，并不是因为 Solana 是以太坊网络的直接竞争对手，所以它不支持相同的资产。确实，Solana 现在支持可以从 Polygon（可以铸造）桥接的 MAI 稳定币。

\
为了将你的 MAI 代币发送到 Solana，你可以使用 [AllBridge](https://allbridge.io/)，一个允许你将代币从一个链转移到另一个链的桥接平台。 AllBridge 支持以下网络：

* 以太坊主网
* Polygon
* Solana
* 火币
* 币安智能链

从某种意义上说，该界面是非常直观的，你仅仅需选择两个网络以及要在这两个网络之间传输的资产。

![将 MAI 从 Polygon 桥接到 Solana](../.gitbook/assets/screen-shot-2021-09-13-at-1.52.23-pm.png)

下一步是指出你的 Solana 钱包地址和你要转账的金额。请意识到，MetaMask 不支持 Solana 钱包（还未？），你将不得不在该网络上创建一个单独的钱包。它可以是像 MetaMask 这样的网络钱包，也可以是应用程序钱包。在选择之前，请阅读 [Solana 的官方建议](https://docs.solana.com/wallet-guide)。

{% hint style="info" %}
请注意，Solana 不提供任何让你获得第一个 SOL（用于支付交易费用的原生代币）的水龙头。你需要先购买一些 SOL 并将它们放在你的钱包中，以便你可以将 MAI 转移到你的钱包中。
{% endhint %}

### **在Solana使用MAI**

与你可以在 Polygon 上使用 MAI 提供流动性和农耕作收益的方式相同，你也可以在 Solana 上做同样的事情。你可以使用 MAI 的主要地方是 [Saber](https://app.saber.so/)，在 MAI/USDC 池中。&#x20;

![截至 2021 年 9 月，Saber 上的 MAI/USDC 池状态 ](../.gitbook/assets/screen-shot-2021-09-13-at-2.11.10-pm.png)

知道saber 上 MAI/USDC 池的好事之一是，与 QuickSwap 上的 LP（Liquidity Providing）池不同，你不需要提供比率为 1:1 的 LP 对。你可以简单地存入单一资产（**MAI** 或 **USDC**）或两种稳定币的（不）平衡比率。

![MAI 和 USDC 在 Saber池中不平衡](../.gitbook/assets/screen-shot-2021-09-13-at-2.13.51-pm.png)

这意味着你实际上可以使用来自 Mai Finance 的 100% MAI 存款，而无需将任何资金互换成 USDC。它特别方便，可以防止受到 2 个稳定币之间微小价格差异的影响。注意，如果在 Polygon 上的 QuickSwap 上耕种，你将获得以原生农场代币支付的奖励，就像在 QUICK 中获得报酬一样。然后，你可以出售你的 saber代币以增加你的 MAI/USDC 头寸。

{% hint style="info" %}
在 Solana 上，你还可以使用[ Sunny](https://app.sunny.ag/)，这是一个聚合器，可以自动复合 Saber 的奖励。请注意，Sunny 聚合器未经 Mai Finance 团队验证。 AllBridge 和 Saber 已成为Mai Finance的官方合作伙伴，但不保证结果。请像往常一样，做你自己的研究。.
{% endhint %}

## Avalanche

### **在 Avax 上获取 MAI**

Avalanche 是一个区块链网络，设计旨在为启动 DeFi 应用程序和企业区块链解决方案提供开源平台和第 1 层协议。它是以太坊主网的另一种替代解决方案，也支持与以太坊主网、Polygon 和 Solana 相同的资产。像这样，你现在可以使用[Relay Chain](https://app.relaychain.com/#/transfer)将你的 MAI 从 Polygon（截至 2021 年 9 月是唯一可以铸造MAI 的地方）发送到 Avax。

至于 AllBridge，用户界面非常简单。N 只需选择资产将作为桥接的网络、目的地和要转移的资产。

![将 MAI 从Polygon桥接到Avalanche
](../.gitbook/assets/screen-shot-2021-09-13-at-2.52.31-pm.png)

Metamask 确实支持 [Avax 钱包](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche)，因此你不需要像 Solana 那样的任何额外钱包。

### **在Avax上使用MAI**

与在 Polygon 上使用 MAI 农耕产量的方式相同，你也可以在 Avalanche 上使用 MAI。这样做的主要场所是 [Trader Joe 的农场](https://www.traderjoexyz.com/#/farm)，在那里你可以找到 MAI/USDC 池。

![截至 2021 年 9 月，Trader Joe 上的 MAI/USDC 池状态](../.gitbook/assets/screen-shot-2021-09-13-at-3.07.19-pm.png)

Avalanche 上的农场运作方式与 Polygon 上的农场非常相似。因此，你可以像使用 QuickSwap 一样使用 Trader Joe 的应用程序。你首先需要使用相同比例的 MAI 和 USDC 在站点上创建 LP 对，然后将 LP 对存入农场。与你在 QuickSwap 上耕种时获得 QUICK 报酬的方式相同，在 Trader Joe 上耕种时你将获得 JOE 代币奖励。然后，你可以在其他池中使用这些代币，或出售它们以增加你的 MAI/USDC 对。

## Fantom

### 在 Fantom上获取 MAI

Fantom 是一个区块链/智能合约平台，其目的是解决其他网络的可扩展性问题，即以太坊区块链。开发人员可以在该网络上创建他们的 DApp（去中心化应用程序）并使用与其他网络相同的资产。因此，你已经可以使用 [AnySwap](https://anyswap.exchange/#/bridge) 的桥接器将 MAI 从 Polygon 桥接到 Fantom。

如果 AnySwap 是另一种桥接解决方案，它的 用户界面与 AllBridge 和 Relay Chain 的非常相似。在 Polygon 上，你必须先连接你的 MetaMask 钱包，然后选择要桥接的资产 (MAI) 和目的地网络 (Fantom)。

![将 MAI 从多边形桥接到 Fantom](../.gitbook/assets/image.png)

Metamask **确实**支持 [fantom 钱包](https://docs.fantom.foundation/tutorials/set-up-metamask)，因此很容易设置它以在 Fantom 上获取你的 MAI 并马上开始使用它。

### 在 Fantom 上使用 MAI

目前，Mai Finance 团队与 Fantom 上的任何收益农场没有任何合作关系。一旦团队知道正在使用 MAI 的项目，就会更新此文档。敬请关注。

## 免责声明

本指南中提供的详细信息纯粹是教育性的，未经维护本指南的团队直接测试。 Discord 服务器上的一些用户已经尝试将他们的资产桥接到 Solana 和/或 Avalanche，因此你可以加入 Discord 社区提出你的问题。请不要忘记做自己的研究，不同的网络会有不同的交易费用和执行时间，不同的奖励计划，桥接费用等......如果你将 MAI 发送到其他网络，请确保你可以将它们桥接回来以防万一你需要它在多边形上。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
