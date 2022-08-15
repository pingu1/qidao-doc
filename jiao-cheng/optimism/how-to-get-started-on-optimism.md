---
description: 在本指南中，我们将解释你需要了解的所有内容，以便开始使用 Optimism 提供的不同 DApp。
---

# 如何在Optimism上开始

## 什么是 Optimism?

Optimism，或有时被称为 Optimistic Ethereum，是一种汇总扩展解决方案，允许用户在以太坊网络上提交交易并以更低的 gas 成本更快地执行交易。因此，Optimism 被称为以太坊第 2 层（简称 L2）。 Optimism 的名称来自它对乐观汇总技术的使用，该技术是指网络用于与以太坊主链（第 1 层或 L1）协同工作的证明类型。有关Optimism汇总和其他汇总解决方案如 ZK（零知识）的进一步阅读，请访问[此链接](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/)。

因为它是一种汇总技术，Optimism 不会产生自己的区块，因此不是区块链。此外，Optimism 网络 API 在很大程度上使用与以太坊相同的 JSON-RPC 规范，因此本质上是 EVM（以太坊虚拟机）等价物，允许为以太坊主网创建的应用程序在 Optimism 上运行，而基本无需更改其代码库。\
\
请注意，正因为如此，Optimism 不使用自己的 gas 代币，而是使用 Ether 作为 gas 来支付交易费用。

## 在Optimism上开始

在使用 Optimism 之前，你需要一个钱包地址。因为 Optimism 是一个 EVM 网络，它将接受与其他 EVM 链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用 Trezor 或 Ledger 等硬件钱包，但你可能需要额外关注能够将你的冷钱包连接到网络的步骤。

对于本教程，我们将坚持使用 Metamask，就像我们为本网站上所有其他指南所做的那样。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon](../polygon/how-to-get-started-on-polygon.md) 的说明。

### 添加 Optimism 到 Metamask

打开 Metamask 弹出窗口，单击钱包图标，导航到设置，然后选择网络并找到添加网络。你将在相关文本字段中使用以下信息：

* **网络名称:** Optimism
* **新 RPC URL:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **货币标志:** ETH
* **阻止资源管理器 URL:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

保存更改，Metamask 会自动将你切换到 Optimism：

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## 桥接到 Optimism

### 水龙头

Optimism 上没有 gas 水龙头，但如果你使用像 [ElkNet](https://app.elk.finance/#/elknet) 这样的 DApp，你可以选择在从任何受支持的网络桥接时将一些 Elk 代币交换为 gas。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### 桥接

* 如果你想将你的 MAI 或 QI 从任何其他网络转移到 Optimism，[Multi Chain](https://app.multichain.org/#/router) 是 Mai Finance 的官方合作伙伴。从你选择的网络中，你可以简单地选择目标链（Optimism）和你要发送的资产（MAI 或 ETH 的正确数量，然后单击“转账”按钮。注意直接在您的资产上收取的转账费用正在转移。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) 是一个受欢迎的桥接器，也是 Optimism 网络的官方桥接合作伙伴之一。
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) 是另一个流行的桥接器，也是 Optimism 网络的官方合作伙伴。仅支持少量代币，包括 ETH，以及 USDC、DAI 和 USDT 等各种稳定币，但它提供的桥接费用低于大多数其他解决方案。
* [Hashflow](https://app.hashflow.com/) 是一种较新的桥接技术，本质上是作为具有足够流动性的任何代币的跨链 DEX（去中心化交易所）。此外，Hashflow 用户目前可以通过交换或提供代币流动性来赚取 HFT（Hashflow 代币）。链目前仅限于 Ethereum、Avalanche、Arbitrum、Optimism、Polygon 和 BNB。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* 当你在 2 个网络之间转移 ELK 代币时，[Elknet](https://app.elk.finance/#/elknet) 将充当桥梁和水龙头。你将能够桥接你的 ELK，并且在接收端，你可以将一小部分 ELK 直接用作气体代币，在我们的例子中是 ETH，如上一节所述。

## Optimism 上的 DeFi

要开始使用 Optimism，以下是一些 DApp，你可能会发现它们对你的 MAI 和 QI 有用，包括：

* [Curve](https://optimism.curve.fi/factory/4/deposit): 这是目前 Optimism 上大部分 MAI 流动性存在的地方，因为 Curve 在执行稳定币互换方面非常有效。\
  \
  通过将 MAI 存入 Curve LP，你将收到 LP 代币，LP 代币可以存入 Mai Finance 的 [Farm 页面](https://app.mai.finance/farm)的 Curve 农场，以赚取 QI 代币的收益。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) 最近在 Optimism 上发布，在这里你可以找到 QI/WETH 流动资金池。它目前未被协议播种，但应该为 QI 提供额外的用例，直到 QI 质押在网络上启动。请注意，Arrakis 使用 Uniswap 池，因此你必须以指定的比率存入 QI 和 WETH 才能进入 LP。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019) 是官方认可的 Balancer 分叉，于 2022 年 6 月在 Optimism 上推出，并提供了一个名为“Come Together”的全新高流动性稳定币池，由 FRAX、USDC 和 MAI 组成。由于其包括 QI、BEETS 和 BAL 代币在内的巨额奖励，它肯定会成为 MAI on Optimism 的事实上的稳定币池。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Optimism 上的 Mai Finance

借贷平台已经在 Optimism 上可用，你可以在其中将 WETH（Wrapped Ether）或 WBTC（Wrapped Bitcoin）代币存入金库并借用 MAI。 MAI 可以存入 Curve 农场以赚取 QI，也可以在最近推出的 BeethovenX 上的新 FRAX/USDC/MAI 稳定池中获得 QI、BEETS 和 BAL 代币的奖励。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## 免责声明[Next - 教程Arbitrum](https://app.gitbook.com/o/-MgVaUztoRBw-4TjbJaB/s/-MgS6h4h2L6e5O5bUNqY-1608594363/\~/changes/6yqSM5HWBQksN5BKYc6i/jiao-cheng/arbitrum)

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
