---
description: 在本指南中，我们将解释你开始使用 Harmony 链所需了解的一切。
---

# 如何开始使用 Harmony

## 什么是Harmony

Harmony 是一个试图解决以太坊主网面临的问题的区块链：在去中心化和可扩展性之间取得令人满意的平衡。该链的主要重点是高交易吞吐量、速度和能源效率。这是通过高度杠杆将被分组以同时处理交易的验证者的分片来完成的。支持可扩展性就像增加分片的数量一样简单，这也有助于实现更快的交易。随意在其[官方文档](https://docs.harmony.one/home/general/technology)中深入了解 Harmony 及其技术。

## 开始使用Harmony

为了使用 Harmony 网络，你需要一个钱包地址。由于 Harmony 是一个兼容 EVM 的网络（以太坊虚拟机），它将接受与其他 EVM 兼容链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用你的硬件钱包，如 Trezor 或分类帐。&#x20;

对于本教程，我们将像本网站上的所有其他指南一样坚持使用 Metamask。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon](../polygon/how-to-get-started-on-polygon.md) 的说明。

### 添加 Harmony 到 Metamask

如果你已经安装了最新版本的 Metamask，你应该已经可以访问 Harmony 链，除了在 Metamask 顶部的网络下拉列表中选择 Harmony One 之外，你无需其他任何东西。你也可以使用这些步骤自己设置一个新的 RPC 来访问 Harmony。打开 Metamask 弹出窗口，单击钱包图标，导航到设置，然后选择网络并找到 Harmony One。你应该得到的数据如下：

* **网络名称:** Harmony One
* **新的 RPC URL:** https://api.harmony.one
* **Chain ID:** 1666600000
* **货币标志:** ONE
* **阻止资源管理器URL:** https://explorer.harmony.one/

保存更改，Metamask 会自动将你切换到 Harmony 网络：

![ 恭喜！！你现在on Harmony了](../../.gitbook/assets/Harmony-onboarding-1.png)

## 桥接到Harmony One

### 水龙头

没有任何官方水龙头可以在你的前几笔交易中获得你的第一个 ONE 代币。你主要需要使用官方的 [Harmony 桥接](https://bridge.harmony.one/erc20)其他链上的一些代币，这将使你可以将某些特定资产从 Ehtereum Mainnet 或 Binance 桥接到 Harmony。你还可以从 Harmony 团队策划的[此列表](https://docs.harmony.one/home/developers/harmony-stack#bridges-fiat-gateways-exchanges)中获取一个项目列表，这些项目将让你通过 Fiat Gateways 或 Exchange Gateways 获得一些 ONE。

与往常一样，也你可以使用 [ElkNet](https://app.elk.finance/#/elknet) 将一些 ELK 代币从其他链转移到 Harmony。如果你这样做，请务必选中 Swap $ELK 1 框以将你转移的部分代币换成 ONE，这也可以让你将剩余的 ELK 代币换成更多的 ONE 或其他资产。

### 桥接

* [Multichain.org](https://app.multichain.org/#/router)（以前称为 AnySwap）是 Mai Finance 的官方合作伙伴，可让你将你的 MAI 代币从 Polygon 和其他链连接到 Harmony。附带说明一下，Multichain 一直与 Mai Finance 开发人员携手合作，以确保你连接到 Harmony 的 MAI 与你可以从借贷平台借到的 MAI 相同。 Harmony 上不需要 Hub。只需前往 Multichain 路由器，选择源网络、要传输的代币和目标网络，就完成了。请注意转账的最低金额、转账费用和过渡期限，但一旦完成，你将在 Harmony 上获得你的资产。

![将 MAI 从 Polygon 桥接到 Harmony One](../../.gitbook/assets/Harmony-onboarding-2.png)

* 如上一段所述，[官方 Harmony Bridge](https://bridge.harmony.one/erc20) 将允许你从以太坊主网或 BSC 转移特定资产。
* 如果你想将某些东西转移到 Harmony，[RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) 是另一种解决方案。检查他们的应用程序以查看哪些资产是可桥接的。
* [ElkNet](https://app.elk.finance/#/elknet) 是一个特例，因为来自 Elk Finance 的桥将让你将 ELK 代币从任何与 EVM 兼容的链桥接到任何其他与 EVM 兼容的链上，并有可能将一小部分转移的金额转换为 gas代币（请参阅上面专门介绍水龙头的部分）。

## Harmony上的DeFi

由于 Harmony One 是一个提供快速、安全交易以及非常便宜的 gas 的网络，因此许多与 EVM 兼容的 DApp（去中心化应用程序）已部署到该网络。下面的列表并未展示所有这些，请随意探索网络及其 DApp 列表。你可以在 [DefiLlama 上找到更详尽的列表](https://defillama.com/chain/Harmony)。

* [ViperSwap](https://viper.exchange/#/swap): 这是Mai Finance在Harmony One上的第一个合作伙伴。这是一个常规的 Uniswap v2 fork、一个 DEX（去中心化交易所）和 AMM（自动做市商），你将能够在其中交换你的资产、创建 LP（流动性提供）代币并通过向交易者提供流动性来获得奖励。奖励使用 VIPER 代币支付，你将能够在应用程序上质押以获得更多奖励。这是 DEX，你可以在其中找到一些 MAI 流动性来交换你的 MAI，或使用你的 MAI 耕种奖励。

![截至 2021 年 12 月，ViperSwap 上的 AI-ONE 和 MAI-VIPER 矿池](../../.gitbook/assets/Harmony-onboarding-3.png)

你会注意到矿池的 APR（年度百分比率）非常高。这主要是由于 ViperSwap 上的奖励格式：当你领取奖励时，5% 的 VIPER 代币可以直接使用，如果锁定到 2021 年 12 月 25 日，则可以使用 95%。在那之后，奖励将在整整一年内归属，这意味着你将无法立即获得你的农耕收益，而且它会非常缓慢地滴下。 ViperSwap 池还有另一个转折点：如果你长期质押你的 LP 代币，你将不得不支付减少的提款费。如果你在与存款交易相同的区块内取款（以对抗闪贷操作），则费用为 25%，如果你在 1 个月后取款，则费用为 0.01%。他们的官方文档中有关[农耕奖励](https://docs.venomdao.org/viper/tokenomics#bbd0)和 [LP 提款费用](https://docs.venomdao.org/viper/fees)的更多详细信息。

* [DeFi Kingdom](https://game.defikingdoms.com/#/): 这是一个特别有趣的项目，它混合了 DeFi 和Gamification。它的原生代币， JEWEL 代币，被用作提供流动性的用户的农耕奖励，但它可以在游戏或市场中使用。本指南解释 DeFi Kingdom（或 DFK）的整个宇宙需要花费太多时间，因此我们强烈建议你阅读[官方文档](https://docs.defikingdoms.com)。

![截至 2021 年 12 月的 DeFi Kingdom主图](../../.gitbook/assets/Harmony-onboarding-4.png)

* [SushiSwap](https://app.sushi.com) 是著名的 DEX/AMM，也出现在许多其他链上。交换，提供流动性，耕种 ONE 和 SUSHI 收益。
* [Curve Finance](https://harmony.curve.fi) 是另一个跨链应用程序，它可以让你提供流动性（3pool 和 tricrypto），并将用复合代币以及 ONE 和 CRV 奖励你。
* [Beefy Finance](https://app.beefy.finance/#/harmony) 是一个收益优化器，我们已经在我们的许多指南中介绍了它，因为它存在于许多链上。目前，你将能够从 Curve 和 SushiSwap 存入你的 LP 代币，并让 Beefy 合成器将农业平台提供的奖励聚合成更多的 LP 代币。
* [Euphoria DAO](https://app.euphoria.money/#/dashboard) 目前是 Harmony 上最大的 Ohm-fork，由 Venom DAO 开发，也落后于 ViperSwap。你可以结合一些不同的资产并获得它们的原生资产 WAGMI 代币。与大多数 OHM 项目一样，以疯狂的 APY（年度百分比收益率）为更多 WAGMI 质押 WAGMI。

## Harmony上的Mai Finance

Mai Finance 于 2021 年 12 月在 Harmony One 上推出，本指南非常接近推出日期，因此你阅读时可能已更新应用程序。&#x20;

你将可以在 Mai Finance (https://app.mai.finance/vaults/create) 上存入你的 WETH 或 ONE 代币，以借入 MAI 稳定币。然后，你将能够在 ViperSwap 上交换 MAI 以杠杆你的资产、保证金交易或农场收益。

![截至 2021 年 12 月的 MAI Finance vaults](../../.gitbook/assets/Harmony-onboarding-5.png)

## 免责声明

像往常一样，本指南不是财务建议，而应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
