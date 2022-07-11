---
description: 在本指南中，我们将解释开始使用 Avalanche 链所需了解的一切。
---

# 如何开始使用Avalanche

## **什么是 Avalanche？**

Avalanche 是一个第一层区块链，用作去中心化应用程序和自定义区块链网络的平台。Avalanche 网络由三个独立的区块链组成：X 链、C 链和 P 链。每条链都有一个显著的目的，这与其他的方法完全不同，也就是让所有节点验证所有交易。Avalanche区块链甚至根据其用例使用不同的共识机制。

Avalanche 与现有的以太坊工具链 100% EVM 兼容，其 C 链提供与以太坊相同的功能，但具有更高的吞吐量、亚秒级确定性和更低的交易费用。 AVAX 是 Avalanche 网络的原生 gas 代币。

## 上Avalanche

在使用 Avalanche 网络之前，你需要创建一个钱包地址。可以使用不同的钱包类型，包括\*\*软件钱包\*\*，例如 Metamask 或本机[Avalanche Wallet](https://wallet.avax.network/), 以及\*\*硬件钱包 \*\*，例如 [Trezor](https://trezor.io/coins/) 或者 [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true). &#x20;

出于本教程的目的，我们将使用 Metamask。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon ](https://guide.qidao.community/tutorials/polygon/how-to-get-started-on-polygon#downloading-metamask)的说明

### **将Avalanche添加到 Metamask**

为了使用 Avalanche 网络，你需要将其添加到 Metamask。为此，请单击网络下拉菜单（如果这是你第一次设置它，它将显示Ethereum Mainnet），然后选择自定义 RPC。然后，你可以在弹出的表单上添加以下值：

* **网络名称**: Avalanche Network
* **新的RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **标志**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

保存更改，Metamask 会自动将你切换到 Avalanche 网络。

![成功！你现在在Avalanche！](../../.gitbook/assets/avax\_MM.png)

## 桥接到Avalanche

### 水龙头

Avalanche 主网上目前没有可用的水龙头。如果你需要一些 AVAX 来支付 gas 费用，你必须将 AVAX 直接从中心化交易所发送到你的钱包，或者通过 Elknet 网桥桥接代币。在下面的[网桥](https://guide.qidao.community/tutorials/avalanche/how-to-get-started-on-avalanche#bridges)部分中更多地了解第二个选项。

### 网桥

* [官方 Avalanche 网桥](https://bridge.avax.network/)**-**Avalanche有自己的网桥，​​可用于将资产从以太坊主网桥接到 Avalanche。 Gas 费用在桥接代币中支付，并且由于你是从以太坊桥接的，所以费用可能会很高。
* [Anyswap](https://anyswap.exchange/#/bridge)  还允许将资产桥接到许多不同的链。桥接的最低代币数量变化将取决于代币，但桥接成本是固定费用。
* [Celer Bridge](https://cbridge.celer.network/#/transfer) 为许多具有出色用户界面的连锁店提供桥接服务。 Avalanche 的桥接费约为 3%。
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) 以低成本提供易于使用且直观的界面。作为旁注，Relay Chain是官方支持的将[MAI 连接到 Avalanche](https://guide.qidao.community/mai-university/mai-metaverse#avalanche)的解决方案。
* [Elknet ](https://app.elk.finance/#/elknet)是由 Elk Finance 提供的桥接服务，这是一种在多个网络上可用的去中心化交易所，包括 Avalanche、Binance、Fantom、Polygon 和 xDai。 使Elknet 与此列表中的其他桥接器的不同之处在于桥接不需要 AVAX，但我们将在下面讨论一个问题。桥接成本只是交易的gas费用。
* 为了通过 Elknet 将你的代币转移到 Avalanche，你必须首先将它们转换为 Elk Finance 的原生代币 Elk。
* 然后，你可以使用网桥将你的 ELK 从支持的网络移动到 Avalanche，如果你选中“Swap $ELK 1 for gas”，你的一部分转移将转换为 AVAX。
* 桥接完成后（通常不到 10 分钟），你可以将钱包切换到 Avalanche 网络，你将看到你的 ELK 和一些 AVAX 准备好部署。你现在可以直接在网站上将你的 ELK 互换成 Avalanche 上任何受支持的代币。
* 可以反向完成相同的操作以移回 Polygon 或任何其他支持的链**。**

![Elknet界面](../../.gitbook/assets/AVAX\_elkswap.png)

## Avalanche上的DeFI

Avalanche 最近几个月出现了大量的增长，这不仅导致了伟大的本地项目的开发，而且大型 deFi 蓝筹股也开始转向网络，包括尚未在那里推出的 Curve。

* [Aave](https://app.aave.com/dashboard) 最近在 Avalanche 上推出，并且已经锁定了 4b 美元的总价值。 Avalanche 上支持的抵押代币包括 Aave、Avalanche、Dai、Tether、USDC、WBTC 和 WETH。 camAVAX 代币将被接受作为 Mai Finance 金库的抵押品。
* [Beefy Finance](https://app.beefy.finance/#/avax) 可能为大多数 deFI 用户所熟知，因为它可以在其他链上使用，包括 Binance、Fantom、Harmony、Polygon 等。 Beefy 是所谓的自动合成器，目前为单代币和双代币农场提供了很好的农业 APY。 Beefy 确实为 Trader Joe 上的 [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) 和[MAI/USDC.e ](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e)LP 提供了自动复合功能。
* [Benqi](https://app.benqi.fi/markets) 是一种类似于 Aave 的市场协议，是网络上同类协议中的第一个。支持的抵押代币包括 Avalanche、Dai、Link、Tether、USDC、WBTC 和 WETH。

![BenQI界面](../../.gitbook/assets/AVAX\_benqi.png)

* [TraderJoe](https://www.traderjoexyz.com/#/home) 是一个去中心化的交易所，并已成为 Avalanche 上的顶级项目之一，具有直观的用户界面和出色的跳频功能，允许用户将代币直接转换为流动性池代币。 TraderJoe 还是[Avalanche 上 MAI-USDC LP 池](https://guide.qidao.community/mai-university/mai-metaverse#using-mai-on-avax)的官方合作伙伴**。**

![](../../.gitbook/assets/AVAX\_joe.png)

* [YieldYak](https://yieldyak.com/farms) 是另一种自动复合器，它也提供高农耕APY。它的单一代币农场与BenQI 共同合作以杠杆更高的回报，因此被认为是有风险的。

![](../../.gitbook/assets/avax\_yak.png)

## 其他有用链接

* [alanche Network](htts://avax)
* [Avalanche 社区链接](https://www.avax.network/community)（Discord、Medium、Reddit、Twitter 等）
* [Debank](https://debank.com), 投资组合经理

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做你自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。
