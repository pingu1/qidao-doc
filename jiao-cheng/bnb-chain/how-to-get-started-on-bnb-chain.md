---
description: 在本指南中，我们将解释你开始使用 BNB 链必须提供的不同 DApp 所需了解的一切。
---

# 如何在BNB Chain上开始

## 什么是 BNB Chain?

BNB Chain是一个与 EVM（以太坊虚拟机）兼容的网络，它是原始Binance Smart Chain的升级版，它提供低交易费用，并且比以太坊（它所基于的链）更快的出块时间。\
\
正因为如此，BNB Chain 是全球最受欢迎的链之一，年交易量超过 45 亿，拥有极其活跃和成熟的[ DApp 生态系统](https://dappbay.bnbchain.org/)。

BNB Chain 使用 Binance 的 BNB 代币来支付gas费，因此请务必在你的钱包中有一些以执行交易。 Binance 提供了有关如何购买或将代币转移到其 BNB 链的[易于遵循的指南](https://www.binance.com/en/support/faq/85a1c394ac1d489fb0bfac0ef2fceafd)。

## 在 BNB Chain上开始

在使用 BNB Chain 之前，你需要一个钱包地址。因为 BNB 链是一个 EVM 网络，它将接受与其他 EVM 链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用 Trezor 或 Ledger 等硬件钱包，但你可能必须遵循能够将你的冷钱包连接到网络的额外步

对于本教程，我们将坚持使用 Metamask，就像我们为本网站上所有其他指南所做的那样。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon ](../polygon/how-to-get-started-on-polygon.md)的说明。

此外，你可以使用币安自己的币安钱包，以更轻松的方式开始网络。

### 添加 BNB Chain 到 Metamask

打开 Metamask 弹出窗口，单击钱包图标，导航到设置，然后选择网络并找到添加网络。你将在相关文本字段中使用以下信息：

* **网络名称:** BNB Chain
* **新 RPC URL:** [https://docs.binance.org/smart-chain/developer/rpc.html](https://docs.binance.org/smart-chain/developer/rpc.html)
* **Chain ID:** 0x38
* **货币标志:** BNB
* **组织资源管理器 URL:** [**https://bscscan.com/**](https://bscscan.com/)\*\*\*\*

保存更改，Metamask 会自动将你切换到 BNB：

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.28.44 AM.png>)

如果你想搜索具有较低延迟的其他 RPC，请查看 [ChainList](https://chainlist.org/) 以获取其他端点。

## 桥接到 BNB Chain

### 水龙头

BNB Chain 上有免费的水龙头，但作者认为使用 ElkNet 之类的东西来获取免费的 gas 代币会更安全。如果你选择使用在网上找到的水龙头，请自行承担风险。使用 [ElkNet](https://app.elk.finance/#/elknet)，你可以选择在从任何受支持的网络桥接时将你的一些 Elk 代币交换为 gas。

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.29.50 AM.png>)

### 桥接

* 如果你想将你的 MAI 或 QI 从任何其他网络转移到 BNB Chain，[Multi Chain](https://app.multichain.org/#/router) 是 Mai Finance 的官方合作伙伴。从你选择的网络中，你只需选择正确数量的目标链（BNB 链）和要发送的资产（例如 MAI 或 QI），然后单击“转移”按钮。请注意直接在你转移的资产上收取的转移费用。

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.32.07 AM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) 是一种流行的桥接器，可让你将代币从大约 15 个不同的网络转移到 BNB 链。

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.31.15 AM.png>)

* [Hashflow](https://app.hashflow.com/) 是一种较新的桥接技术，本质上是作为具有足够流动性的任何代币的跨链 DEX（去中心化交易所）。此外，Hashflow 用户目前可以通过交换或提供代币流动性来赚取 HFT（Hashflow 代币）。链目前仅限于 Ethereum、Avalanche、Arbitrum、Optimism、Polygon 和 BNB。

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.33.51 AM.png>)

* 当你在 2 个网络之间转移 ELK 代币时，[Elknet ](https://app.elk.finance/#/elknet)将充当桥梁和水龙头。你将能够桥接你的 ELK，并且在接收端，你可以将一小部分 ELK 直接用作 gas 代币，在我们的例子中是 BNB，如上一节所述。

## BNB Chain 上的 DeFi

* [Ellipsis Finance](https://ellipsis.finance/pool/0x68354c6E8Bbd020F9dE81EAf57ea5424ba9ef322) 是 BNB 链上 MAI 流动性的去处。 Ellipsis 上的 MAI 池（MAI+val3EPS）由四种稳定币组成，包括 BUSD（Binance USD）、USDC、USDT（Tether）和 MAI。通过存入稳定币，然后将 LP 质押到 Ellipsis，用户可以通过 Ellipsis 的 EPS 代币、Vallas 的 VAL 代币以及交易费用获得 6% 到 15% 的可变收益。

![MAI+val3EPS pool on Ellipsis](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.07.42 AM.png>)

## &#x20;BNB Chain 上的 Mai Finance

借贷平台已经在 BNB 链上可用，你可以在其中将你的 WBNB（Wrapped BNB）和 CAKE（PancakeSwap）代币存入vault并借用 MAI。然后，你可以将借来的 MAI 存入 Ellipsis 以赚取 MAI 收益。

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.11.26 AM.png>)

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
