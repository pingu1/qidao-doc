---
description: 在本指南中，我们将解释如何开始使用 Moonbeam。
---

# 如何在 Moonbeam 开始

## 什么是 Moonbean?

Moonbeam 于 2020 年 1 月推出，是一个在 Polkadot 网络上运行的与 EVM（以太坊虚拟机）兼容的智能合约平台，这就是所谓的 Polkadot 平行链。平行链是一组相互连接的链，它们从 Polkadot 的主中继链中受益，同时保持互操作性，从而在与主链并行运行的同时分享主链的好处和安全性。\
\
Polkadot 将平行链的好处描述如下：“平行链结束了孤立区块链的时代，创建了一个分散的、连接的区块链互联网，在此之前只存在具有自己部落社区的孤立网络。”

![Moonbeam, 一个 Polkadot 平行链](<../../.gitbook/assets/moonbeam (1).jpg>)

由于其 EVM 兼容层，Moonbeam 使 Solidity 开发人员能够更轻松地将其现有应用程序从其他 EVM 兼容网络移植到 Moonbeam，而只需少量代码更改。 Moonbeam 目前拥有 1.3 亿美元的 TVL，以及一个[充满活力且不断增长的](https://defillama.com/chain/Moonbeam)应用生态系统。

Moonbeat 还提供 Substrate 兼容性。 Substrate 是一个模块化的区块链框架，开发人员使用它来构建适合他们需要的区块链，使用称为托盘的可重复使用组件。它使用 Rust 编程语言，是大多数开发人员在为 Polkadot 网络构建平行链时使用的框架。

由于 Moonbeam 是基于 Substrate 的区块链，与其网络集成的应用程序受益于 Polkadot 和以太坊链以及比特币等其他链之间的互操作性。

开发者还可以使用以太坊上常用的兼容 Substrate 的生态系统工具，包括区块浏览器、前端开发库和钱包，以及 Truffle 和 Remix 等开发工具。

Moonbeam 的原生 gas 代币是 GLMR。

## 在 Moonbeam 上开始

在使用 Moonbeam 之前，你需要一个钱包地址。因为 Moonbeam 是一个 EVM 网络，它将接受与其他 EVM 链上相同的钱包，包括 Metamask 或 Nifty 等网络钱包，你将能够使用 Trezor 或 Ledger 等硬件钱包，但你可能需要额外关注能够将你的冷钱包连接到网络的步骤。

对于本教程，我们将坚持使用 Metamask，就像我们为本网站上所有其他指南所做的那样。如果你没有安装 Metamask，你可以找到有关[如何开始使用 Polygon ](../polygon/how-to-get-started-on-polygon.md)的说明。

### 添加 Moonbeam 到 Metamask

网络并找到添加网络。你将在相关文本字段中使用以下信息：

* **网络名称:** Moonbeam
* **新 RPC URL:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **Chain ID:** 128
* **货币标志:** GLMR
* **组织资源管理器 URL:** [https://moonscan.io/](https://moonscan.io/)

保存更改，Metamask 会自动将你切换到 Moonbeam：

![Moonbeam on Metamask](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## 桥接到 Moonbeam

### 水龙头

GLMR 是 Moonbeam 的原生 gas 代币，所以你需要在钱包里放一些来进行链上交易。幸运的是，官方 Moonbeam Faucet 将帮助你开始使用少量 GLMR，但请注意，如果网络拥塞，代币分散的金额有时可能不足以完成交易。

为了获得一些免费的 GLMR，你需要通过验证码机器人验证你是人类，并将你的 Metamask 钱包连接到该站点。少量（0.007 GLMR）将立即发送到你的钱包。

![GLMR.Supply Faucet](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

此外，用户可能希望使用 Solarflare 的“[Swap for gas](https://app.solarflare.io/bridge/gas-swap)”功能。这允许用户将包括 WETH、WBTC、USDC、DAI、USDT、BUSD、FLARE 和 BNB 在内的其他代币兑换成 Moonbeam 的原生 gas 代币 GLMR。

![Solarflare's "Swap for Gas"功能 ](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### 桥接

* [Multichain](https://app.multichain.org/#/router) 是 MAI 通过与 MAI Finance 合作的官方桥梁，你可以使用它轻松地将你的 MAI 发送到 Moonbeam。

![ Moonbeam 上的 Multichain](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) 是 Moonbeam 上的全功能 AMM（自动做市商），与 Uniswap 非常相似。 Solarflare 有一个内置的桥接器，允许用户将资产从以太坊主网以及 BNB 链桥接到 Moonbeam。如上面的水龙头部分所述，Solarflare 还具有“Swap for gas”功能。

![通过 Solarflare 桥接](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) 是一种流行的桥，也支持 Moonbeam。请注意，你可能无法从每条链桥接到 Moonbeam（例如，不支持 Polygon 到 Moonbeam 的桥接）。

![通过 Celer 桥接](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* 其他桥梁可用，但可能是特定于链的，例如 Cosmos 生态系统的 Nomad 或 Axelar。

## Moonbeam 上的 DeFi

[StellaSwap](https://app.stellaswap.com/farm) 目前是 Moonbeam 上 MAI 的主要流动性来源。 MAI-Base4Pool 由 MAI、FRAX、USDT、USDC 和 DAI 组成，目前的 TVL（锁定总价值）为 535,000 美元，为你的稳定币产生稳定的 26% APR（年百分比率）。

![ StellaSwap 上的 MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam 拥有一个充满活力的 DeFi 生态系统，有数十个 DApp（去中心化应用程序）可供使用，包括在[ Curve](https://moonbeam.curve.fi/) 和 [Beefy Finance](https://app.beefy.com/) 等其他链上发现的 DeFi 主食。有关可用 DApp 的完整列表，请查看[ DefiLlama 的 Moonbeam 页面](https://defillama.com/chain/Moonbeam)。

## Moonbeam 上的 Mai Finance

虽然 Moonbeam 上不提供 Mai Finance，但你可以在 StellaSwap 上创建vault并针对 xStella 和 wGLMR 借用 MAI。请注意，在 StellaSwap 上借用 MAI 会产生利息——xStella vault为 12%，wGLMR vault为 8%。你可以在下一个标题为“[在 StellaSwap 上玩 MAI 乐高积木](playing-with-mai-legos-on-stellaswap.md)”的部分中找到有关如何使用 StellaSwap 的 MAI vault的更多信息。

![StellaSwap 的 vaults](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
