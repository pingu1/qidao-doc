---
description: 在本指南中，我们将解释你开始使用 Cronos 链所需了解的一切。
---

# 如何开始使用 Cronos

### 什么是Cronos

如果不提及 Crypto.com，就很难解释 Cronos 是什么。 Crypto.com 是最大的中心化交易所（也称为 CEX）之一，正在构建自己的链集，包括 Crypto.org Chain 和 Cronos。 Crypto.org Chain 是具有专有技术的链，而 Cronos 是其 EVM（以太坊虚拟机）兼容的姐妹。它与专用于 CEX 的币安链和兼容 EVM 的币安智能链几乎相同。

除了其他优势之外，Cronos 还具有 **EVM 兼容性**，这意味着在其他 EVM 链上启动的大多数应用程序也可以部署到 Cronos，包括 Mai Finance 和**可扩展性**：Cronos 比以太坊主网更快、更便宜。

### 开始使用 Cronos

为了使用 Cronos 网络，你需要一个钱包地址。由于 Cronos 是一个与 EVM 兼容的网络，它将接受与其他 EVM 兼容链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用 Trezor 或 Ledger 等硬件钱包。

对于本教程，我们将像本网站上的所有其他指南一样坚持使用 Metamask。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon](../polygon/how-to-get-started-on-polygon.md) 的说明。

### 将 Cronos 添加到 Metamask

如果你已经安装了最新版本的 Metamask，你应该已经可以访问 Cronos 链，除了在 Metamask 顶部的网络下拉列表中选择 Cronos 之外，你无需其他任何东西。你还可以自己设置一个新的 RPC 以使用这些步骤访问 Cronos。打开 Metamask 弹出窗口，单击钱包图标，导航到设置，然后选择网络并找到 Cronos。你应该得到的数据如下：

* **网络名称:** Cronos
* **新的 RPC URL:** https://evm-cronos.crypto.org
* **Chain ID:** 25
* **货币符号:** CRO
* **阻止资源管理器URL:** https://cronos.crypto.org/explorer/

保存更改，Metamask 会自动将你切换到 Cronos 网络：

![恭喜！！你现在在 Cronos](../../.gitbook/assets/Cronos-onboarding-1.png)

## 桥接到Cronos

### 水龙头

没有任何官方水龙头可以在你的前几笔交易中获得你的第一个 CRO 代币。但是，如果你将一些资金桥接到 Cronos，或者只是在你需要一些 gas 时，某些应用程序将提供此服务：

* [Crystl 金融水龙头](https://cronos.crystl.finance/faucet): 连接你的钱包并完成验证码后，你可以请求一些 CRO 将其发送到你的钱包。
* [Elk金融](https://app.elk.finance/#/elknet):当你将 ELK 代币从一条链桥接到另一条链时，你可以选择将转移的 ELK 的一小部分交换到目标链的本地 gas 代币中。如果你是第一次将资产桥接到新链，这将特别有用。

![使用 ElkNet 桥将 1 美元转换为 gas 代币](../../.gitbook/assets/Cronos-onboarding-2.png)

* [Crypto.com](https://crypto.com): 不要忘记 Cronos 是与 Crypto.com 紧密相连的链。你可以在那里创建一个账户，通过链接银行账户直接购买你的 CRO 代币，然后将它们发送给 Cronos。

{% hint style="info" %}
记住，你将需要一些气体代币才能进行交易。这意味着，如果你在没有 CRO 代币的账户中将资产从另一条链桥接到 Cronos，你将被卡住，无法做任何事情。确保你的钱包有足够的资金来执行至少一笔 Gas 代币的交换交易。
{% endhint %}

### 桥接

* 如果你想将你的 MAI 桥接到 Cronos，[Relay Chain](https://app.relaychain.com/transfer#/) 是 Mai Finance 的官方合作伙伴。 RelayChain 现在支持从几个不同的链桥接 MAI，因此你将能够将你的资产从 Polygon、Moonriver、Avalanche 或 Shiden 发送到 Cronos。只需将目标链选择为 Cronos，并选择要发送的代币（大多数情况下以 MAI 命名，但有时也在 miMATIC 下）。选择要转账的金额并启动不超过 10 分钟的转账。注意转会费。然而，RelayChain 的一个好处是它会在接收端给你一些 CRO，这样你就可以将一些 MAI 换成 CRO。

![使用 RelayChain 将 MAI 从 Polygon 桥接到 Cronos](../../.gitbook/assets/Cronos-onboarding-3.png)

* 如果你想将一些资产转移到 Cronos，大多数链也可以使用 [AnySwap](https://anyswap.exchange/#/router)。作为旁注，AnySwap 还支持将 MAI 从 Polygon 转移到 Cronos。
* [ElkNet](https://app.elk.finance/#/elknet) 是一个特例，因为来自 Elk Finance 的桥将让你将 ELK 代币从任何与 EVM 兼容的链桥接到任何其他与 EVM 兼容的链上，并有可能将一小部分转移的金额转换为 gas令牌（请参阅上面专门介绍水龙头的部分）。

### MAI Hub

如果你通过中继链将一些 MAI 从 Polygon 桥接到 Cronos，你将获得 MAI 的 RelayChain 版本，而不是由 Cronos 上的应用程序铸造的本机 MAI。这 2 个代币（一个来自 RelayChain 和一个来自 Mai Finance）具有相同的价值和相同的名称，但合约地址不同，并且唯一可以在 Cronos 上种植收益的代币是来自 Mai Finance 的一个。

你可以使用[ Mai Finance 上的 hub](https://app.mai.finance/hub) 以 1:1 的比例从 Relay Chain 交换你的 MAI，然后你就可以在其他平台上使用你的真实 MAI。

![在 Hub 中的 Cronos 上将 MAI（RelayChain）交换为真正的 MAI](../../.gitbook/assets/Cronos-onboarding-4.png)

不要忘记，如果你想将它们从 Cronos 桥接到另一个链，则必须将你的真正 MAI 转换为中继链版本。

{% hint style="info" %}
看起来 AnySwap 支持将 MAI 从 Polygon 转移到 Cronos，但你将收到无法通过hub交换的 AnySwap 版本的 MAI。你可能会遇到无法使用的令牌，因此请确保你使用的是正确的网桥。
{% endhint %}

## Cronos上的DeFi

Cronos 与 Crypto.com 相关联，大量投资流入链中，DeFi 应用程序在那里支持流动性。因此，你也许可以在以下平台上种植产量：

* [CroDex](https://swap.crodex.app/#/swap): 这是 Cronos 上的顶级 DEX（去中心化交易所）和 AMM（自动做市商）之一，并且是类似于 QuickSwap 的 Uniswap v2 分支。你将能够交换你的资产，通过在农场提供 LP（流动性提供）对参与流动性挖掘，或质押平台的原生代币以获得更多奖励。 CroDex 也是 Mai Finance 在 Cronos 上的第一个官方合作伙伴，也是唯一可以将 MAI 换成其他资产的地方，以及通过种植 MAI-USDC 和 MAI-CRO 对来参与流动性挖矿计划.

![在 CroDex 上使用 MAI 进行农耕](../../.gitbook/assets/Cronos-onboarding-5.png)

当你在 CroDex 上耕作时，你将获得 CRX 代币的奖励，你可以将这些代币存入 Vault 以获得更多 CRX 代币，但还有其他（更好的）选项将在未来的教程中介绍。

* [VVS](https://vvs.finance) 和 [CronaSwap](https://app.cronaswap.org): 这些是其他 DEX/AMM，它们是 PancakeSwap（另一个 Uniswap fork）的forks，你将在其中获得与 CroDex 相同的功能。
* [Beefy Finance](https://app.beefy.finance/#/cronos), [Adamant](https://adamant.finance) 和 [Autofarm](https://autofarm.network/cronos/) 是许多网络上存在的著名聚合器/收益优化器，你可以在其中从大多数 DEX 存入你的 LP 代币，并让负责矿池的算法收获农场代币和化合物将奖励转化为更多 LP 代币。
* [Crystl Finance](https://cronos.crystl.finance) 是一个直鹅fork，首先在 Polygon 上推出，现在也可以在 Cronos 上使用。用户将能够将 LP 代币存入金库，以获得可以质押或耕种（或交换）的 CRYSTL 代币。
* [Fortune DAO](https://www.fortunedao.com/#/) 是 Cronos 上接受 DAI 和 USDC 的主要 Ohm (Olympus) fork。

## Cronos上的Mai Finance

目前该应用程序尚未完全启动，主要等待 ChainLink 预言机接受代币作为抵押品。该中心已经存在，因此你可以期待在 2022 年第一季度推出。

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
