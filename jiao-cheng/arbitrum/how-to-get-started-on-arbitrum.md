---
description: 在本指南中，我们将解释你需要了解的所有内容，以便开始使用 Arbitrum 提供的不同 DApp。
---

# 如何在 Arbitrum上开始

## 什么是Arbitrum?

Arbitrum 是一种汇总扩展解决方案，允许用户在以太坊网络上提交交易并以更低的 gas 成本更快地执行交易。因此，Arbitrum 被称为以太坊第 2 层（简称 L2）。与其兄弟网络 Optimism 一样，Arbitrum 使用optimistic汇总技术，该技术是指网络用于与以太坊主链（第 1 层或 L1）协同工作的证明类型。有关optimistic汇总和其他汇总解决方案（如 ZK（零知识））的进一步阅读，请访问[此链接](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/)。

因为它是一种汇总技术，所以 Arbitrum 不会产生自己的区块，因此不是真正的区块链。 Arbitrum 背后的开发者 Offchain Labs 旨在使网络 EVM（以太坊虚拟机）与未来升级等效。\
\
请注意，正因为如此，Arbitrum 不使用自己的 gas 代币，而是使用 Ether 作为 gas 来支付交易费用。

## 开始使用 Arbitrum

在使用 Arbitrum 之前，你需要一个钱包地址。由于 Arbitrum 是一个 EVM 网络，它将接受与其他 EVM 链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用 Trezor 或 Ledger 等硬件钱包，但你可能需要额外关注能够将你的冷钱包连接到网络的步骤。

对于本教程，我们将坚持使用 Metamask，就像我们为本网站上所有其他指南所做的那样。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon](../polygon/how-to-get-started-on-polygon.md) 的说明。

### 添加 Arbitrum 到 Metamask

打开 Metamask 弹出窗口，单击钱包图标，导航到设置，然后选择网络并找到添加网络。你将在相关文本字段中使用以下信息：

* **网络名称:** Arbitrum
* **新 RPC URL:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **Chain ID:** 4216
* **货币标志:** ETH
* **阻止资源管理器 URL:** [https://arbiscan.io/](https://arbiscan.io/)

保存更改，Metamask 会自动将你切换到 Arbitrum：

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## 桥接到 Arbitrum

### 水龙头

Arbitrum 上没有 gas 水龙头，但如果你使用像 [ElkNet](https://app.elk.finance/#/elknet) 这样的 DApp，你可以选择在从任何受支持的网络桥接时将你的一些 Elk 代币交换为 gas。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### 桥接

* 如果你想将你的 MAI 或 QI 从任何其他网络转移到 Arbitrum，[Multi Chain](https://app.multichain.org/#/router) 是 Mai Finance 的官方合作伙伴。从你选择的网络中，你可以简单地选择目标链（Arbitrum）和你要发送的资产（MAI 或 ETH 的正确数量，然后单击“转账”按钮。注意直接在你的资产上收取的转账费用正在转移。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) 是一种流行的桥接器，可让你将代币从大约 15 个不同的网络转移到 Arbitrum。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) 是另一个流行的桥接器。仅支持少量代币，包括 ETH，以及 USDC、DAI 和 USDT 等各种稳定币，但它提供的过桥费用低于大多数其他解决方案。
* [Hashflow](https://app.hashflow.com/) 是一种较新的桥接技术，本质上是作为具有足够流动性的任何代币的跨链 DEX（去中心化交易所）。此外，Hashflow 用户目前可以通过交换或提供代币流动性来赚取 HFT（Hashflow 代币）。链目前仅限于 Ethereum、Avalanche、Arbitrum、Optimism、Polygon 和 BNB。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* 当你在 2 个网络之间转移 ELK 代币时，[Elknet](https://app.elk.finance/#/elknet) 将充当桥梁和水龙头。你将能够桥接你的 ELK，并且在接收端，你可以将一小部分 ELK 直接用作gas代币，在我们的例子中是 ETH，如上一节所述。

## Arbitrum上的 DeFi

* [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) 目前拥有 Arbitrum 上唯一具有 MAI 流动性的池。通过将你的 MAI 存入 MAI/USDC/USDT 池，用户可以获得大约 13% 的稳定币收益率。请注意，此池将很快迁移，以修复现有的流动性错误。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## &#x20;Arbitrum上的 Mai Finance

该借贷平台已在 Arbitrum 上可用，你可以将 WETH（Wrapped Ether）或 WBTC（Wrapped Bitcoin）代币存入vault并借用 MAI。然后，你可以将借来的 MAI 存入 Balancer 以赚取收益。

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
