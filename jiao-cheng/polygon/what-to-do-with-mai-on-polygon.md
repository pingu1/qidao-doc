---
description: 本教程将介绍不同的选项，让你可以在 Polygon 上使用新铸造的 MAI。
---

# 如何在 Polygon 上使用 MAI

## 本教程的目标

本教程的目标不是详细介绍你可以使用 MAI 稳定币做什么，而是列出你可以在 Polygon 上使用的所有网站和 DeFi 应用程序，这些网站和 DeFi 应用程序可以让你直接或组合使用你的 MAI与其他稳定币。更多关于 MAI 的具体使用方法，可以参考本站其他教程，或者在 Discord 或 Telegram 上获取帮助。

请注意，该列表并不完整，并且永远不会完整，因为网络上每周都有新的 dapp 发布。我无法全部回顾，所以我只会介绍主要选项，或者最著名/最“安全”的选项。

如果你想要一个特定的项目被列出来，请加入 [Discord](https://discord.gg/mQq55j65xJ) 上的 Qi 社区。

{% hint style="info" %}
我不会介绍Mai Finance农场。这个主题值得拥有自己的教程，因为 Qi 与任何其他随机农场令牌不同。
{% endhint %}

## Blue Chip项目中 的安全农耕

Bluechip 项目是被证明是可靠且呈现风险较低的 DeFi 应用程序。他们通常会接受审计，并且他们背后的团队已经工作了很长时间。他们通常没有巨大的 APR（年百分比率），但他们值得信赖。

### Balancer

[Balancer](https://polygon.balancer.fi/#/) 是一个自动化的投资组合管理器、流动性提供者和价格传感器。在该平台上，你将能够借出你的加密货币，并向交易者收取费用，交易者通过追踪套利机会来重新平衡您的投资组合。如果您需要有关 Balancer 的更多详细信息，请阅读[官方文档](https://docs.balancer.fi/)。

在 Polygon 网络上，Balancer 提出了一个由 4 个主要稳定币组成的池：DAI、USDC、USDT 和 MAI（miMATIC）。这个稳定的矿池目前的 APR 相当稳定，约为 20%。

![截至 2021 年 8 月的稳定币池状态](../../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)

Balancer 的最大优点是你绝对不需要拥有 4 个硬币即可存入池中。 Balancer 将自动生成与你的存款的平衡组合。这意味着，如果你有价值 100 美元的 MAI，你可以简单地将它们存入 Balancer 池中，并让算法正确地将其滑入，根据存入时各自的价格为每个代币设置 25% 的比率。

池的奖励使用 BAL 代币支付，每周分发一次。除了 BAL 代币，还可以根据你输入的池授予额外奖励。你可以在此处查不同的激励项目。在我们的案例中，参与稳定池还将为你赢得 MATIC 和 Qi 奖励。

如果你需要有关如何使用 Mai Finance 借出你的加密货币和借入 MAI（而不是出售你的加密货币来购买 MAI）的更多详细信息，请阅读本网站上的其他指南。你甚至可以在循环中包含 AAVE 以赚取更多。

池的奖励使用 BAL 代币支付，每周分发一次。除了 BAL 代币，还可以根据你输入的池授予额外奖励。你可以在此处查不同的[激励项目](https://balancer-incentives.web.app/)。在我们的案例中，参与稳定池还将为你赢得 MATIC 和 Qi 奖励。

完整的流程是像这样的

![](../../.gitbook/assets/screen-shot-2021-08-11-at-11.34.45-am.png)

如果你需要有关如何使用 Mai Finance 借出你的加密货币和借入 MAI（而不是出售你的加密货币来购买 MAI）的更多详细信息，请阅读本网站上的其他指南。你甚至可以[在循环中包含 AAVE ](leverage-aave-tokens.md)以赚取更多。

### Curve finance

这里有一点点击诱饵。 [Curve](https://polygon.curve.fi) 是另一个平台，你可以在其中借出你的加密资产池，以产生收入，但不能直接借出 MAI（还没有？）。我们感兴趣的池是&#x20;

* AAVE 池将在稳定币三重奏 (DAI/USDC/USDT) 上产生 5% 到 15% 的 APR（APR 变化很大）。该池的工作方式与 Balancer 完全一样，你可以使用协议在 AAVE 上使用的单个资产进入池。
* 由稳定币三重奏组成的 atricrypto 池也包括 wETH 和 wBTC，以减轻无常损失。该池的 APR 介于 25% 和 30% 之间。 Mai Finance 团队目前也在尝试将 MAI 添加到此池中，这意味着你也许可以直接使用铸造的 MAI 进入它。

在等待 Curve 协议接受 MAI 作为其池中有效的稳定币时，你仍然可以按照以下步骤将你最喜欢的加密货币与 Curve 一起使用（以 MATIC 为例）

* 将你的 MATIC 代币存入 AAVE 并收集 amWMATIC
* 将你的 amWMATIC 存入 Mai Finance 并收集 camWMATIC（AAVE 奖励将复合到 camWMATIC 代币中）
* 使用 camWMATIC 作为 Mai Finance 的抵押品并借用 MAI
* 使用 Mai Finance 上的[调换页面](https://app.mai.finance/swap)来将你所有的 MAI 换成 USDC
* 然后你就可以
  * 用你的USDC进入Curve上的atricrypto池并获得25%到30%的奖励
  * 用你的USDC进入Curve上的AAVE池并获得5%到15%的奖励

曲线上的奖励在

* 自动复合的 USDC，增加你在池中的头寸（对于 atricrypto 池，它将是 USDC/USDT/DAI 和可能的 wBTC/wETH 的混合）
* 然后你可以使用 WMATIC 重复上述循环并增加你的贷款和投资资本
* CRV 代币，也可以用作 Mai Finance 的抵押品以借入更多 MAI 并增加你的投资资本

![](../../.gitbook/assets/screen-shot-2021-08-11-at-12.14.27-pm.png)

### AAVE

有一篇关于如何使用 Mai Finance[ 在 AAVE 上推广加密货币](leverage-aave-tokens.md)的完整指南。这不是 MAI 稳定币的直接使用，但我们可以想象，在未来，AAVE 还将拥有一个 MAI 池，你可以在其中借出你的加密货币。

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) 可能是 Polygon 上最著名的 DEX（去中心化交易所）之一，带有 SushiSwap 和 1Inch。它也是一个 AMM（自动做市商），允许用户使用流动性池在 Polygon 网络上进行有效率地交易。交易所的任何交易都需要支付一定的费用，该费用会部分重​​新分配给将流动性存入平台的用户。

你可以在 QuickSwap 上使用 MAI 的方式与[常规收益农场](secure-your-yield-farming-profits.md)非常相似，因此如果你需要获得在 QuickSwap上进入 MAI/USDC池的确切步骤，你最好阅读本文。

目前，如果你在 QuickSwap 上进入 MAI/USDC LP（流动性提供商）池，你将获得

* 交易费用
* QUICK 代币

![截至 2021 年 8 月 QuickSwap 上的 MAI/USDC 池的详细信息](../../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

## **Degen 农场和聚合器**

### Adamant

[Adamant](https://adamant.finance/home) 是一个聚合器，它在 Polygon 上列出所有“最佳”农场，并让你直接从他们的网站输入它们。通过将你的资产（LP 代币）存入 Adamant 的特定池中，算法将收获池授予的奖励，并自动将部分奖励复合到你的 LP 位置。

其余的奖励通常在 WMATIC 中转换，然后重新分配给 ADDY 代币（Adamant 的原生代币）的持有者。最后，您还可以获得 ADDY 代币的奖励，您可以收获和归属 90 天，从而赚取 WMATIC 一部分分红。

通常来说，如果你不太关心农场代币，并且不想每天手动多次复合奖励，那么 Adamant 是一个不错的去处。它还可以产生更多收入，因为除了池授予的奖励之外，你还可以获得一些 ADDY 奖励。

Adamant 目前支持一些接受 MAI/USDC LP 对的池。这些池在

* QuickSwap：QUICK 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励
* DinoSwap：Dino 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励
* Mai Finance：Qi 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励

![Adamant 上的 QuickSwap MAI/USDC 池](../../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)

{% hint style="info" %}
QuickSwap 网站上 QuickSwap 池的屏幕截图（见上面段落）和 Adamant 是在同一天拍摄的，但显示了不同的 APY（年收益率）。
{% endhint %}

可以直接看到，Adamant 上的 APY 比 QuickSwap 上的高一点。奖励细分如下

* 12.88% 自动复合QUICK（意味着QUICK奖励转化为更多LP代币）&#x20;
* 9.16% ADDY奖励（未复合）&#x20;
* 3.40%费用份额分红（每天获得ADDY）

这意味着，在 QuickSwap 授予的 20.92% 中，只有 12.88% 用于增加你的 LP 头寸，其余的用于互换 WMATIC 股息。你将可以每天（或任何时候）领取你的 ADDY 奖励并质押它们，这将反过来产生可领取的 WMATIC 分红。换句话说，Adamant 似乎是一个更好的选择，因为它具有更好的 APY 和自动复合奖励，但实际上它也涉及很多手动操作。

{% hint style="info" %}
使用 Adamant 也对原生代币价格产生很大影响。确实，由于 Adamant 不断地出售农场代币以产生更多的 LP 对和 WMATIC 作为其 ADDY 持有者的股息，因此农场代币的销售压力非常大，并且可以解释为什么它们的价格一直在下跌。
{% endhint %}

### **其他接受 MAI/USDC LP 对的农场**

MAI 在 Polygon 上越来越受欢迎，而且由于 QuickSwap 支持 MAI/USDC 对，现在很多农场也支持它。以下列表将展示一些你可以使用 MAI/USDC 赚取收益的项目

* DinoSwap
* Augury
* Polypup
* ...

其他农场也可能接受 MAI/USDC 池。如果你想随时了解新农场及其发布日期，我强烈建议你查看 Polygon 农场的 [RugDoc.io](https://rugdoc.io/calendar/) 日历，并可能查看他们网站的其余部分，该网站将提供每个农场的非常智慧的概述，如以及他们的潜在风险。

## Impermax

### 一点点解释

[Impermax](https://polygon.impermax.finance) 是一个让用户杠杆他们的 LP 代币获得更高收益的平台。目标非常简单：通过提供 LP 代币并将其用作抵押品，然后可以借入更多的 2 种标的资产以生成更多 LP 代币并重复循环。

![ Impermax 循环解释](../../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)

这样做时,用户暴露在无常的损失中，损失被循环重复的次数放大。当应用太多循环时，清算风险也会成倍增加。事实上，如果 APR 成倍的增加，构成货币对的两个代币的价格变化会被杠杆效应放大，从而导致更快的清算。

使用稳定币，清算风险较低，因为价格变化可以忽略不计。这也意味着抵押品债务比率 (CDR) 可能非常接近 100%，从而导致大量循环，所以导致高 APR。

注意，当你借入和杠杆你的头寸时，Impermax 会收取费用。费用相当于你最终头寸的 0.1%。例如，如果我拥有价值 100 美元的 MAI/USDC 并且我的杠杆率为 50 倍，那么我的最终头寸将价值 5,000 美元，并且我将支付与我借入的 4,900 美元相对应的 4.90 美元费用。

循环借贷组合的效果允许乘以最终的 APY。 MAI/USDC 对的初始 APY 为 20%，CDR 为 110%，运行循环 50 次，并使用公式

$$
等效APR = 初始APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

我们可以轻松获得 228% 的最终 APR。还有一些其他因素会影响最终的 APR，即借入 APR（借入更多 LP 代币的贷款利息），以及构成 LP 对的两种资产的供给和需求（直接驱动借入 APR）。

此外，因为所有费率都被应用循环的次数放大，因此 APR 会有巨大的变化，有时可能会在短时间内变为负数（你的 LP 代币将用于偿还负的 APR）。

### 我的 MAI/USDC 对的杠杆头寸

最后，你将基础 APR 用于一个更大的价值，这将获得更大的利息，从而增加你初始头寸的 APR。

![初始 MAI/USDC 对为 70.52 美元的Impermax 仪表板示例](../../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)

我可以很容易地看到我使用了多少作为抵押品，我最初投资了多少，杠杆比率是多少，以及由于杠杆比率导致的清算价值是多少。在撰写本文时，该寸头将为我提供以下比率

![在给定时间的收入和支出估算](../../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)

APR 以 IMX 代币授予，可以互换成更多的 MAI/USDC（使用 Mai Finance 的权力以 0% 的利息借入，RFTM），或用于为在 Impermax 上接受 IMX 的特定池提供流动性。

### **向借款人供应MAI**

确实，在应用程序上，你还可以为那些想要将杠杆循环应用于其头寸的人提供流动性（他们将需要基础资产来生成更多 LP 代币）。借贷资产是赚取收益并让借款人承担所有风险的好方法。还有，借款的用户越多，供应 APR 就越高。

![在给定时间 Impermax 上提供和借入 MAI 的利率](../../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)

这是优化你在 Mai Finance 上的 0% 贷款的另一种好方法。借 MAI 不仅无需支付任何费用，而且只需将其存入 Impermax上 即可赚取大量利息。

## 免责声明

一切都是本教程纯粹是教育性的。目标是为我认为值得在 Polygon 上的加密世界中发展的人们带来光明。我显然没有把Mai Finance说成一个农场，因为很快就会写出专用的教程。

最后，本指南绝对不能按原样应用，它不是任何财务建议，你不应该盲目遵循我写的内容。在考虑投资他们的平台之前，请阅读我提到的不同项目的文档。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
