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

[Balancer](https://polygon.balancer.fi/#/) 是一个自动化的投资组合管理器、流动性提供者和价格传感器。在该平台上，你将能够借出你的加密货币，并向交易者收取费用，交易者通过追踪套利机会来重新平衡您的投资组合。如果您需要有关 Balancer 的更多详细信息，请阅读[官方文档](https://docs.balancer.fi)。

在 Polygon 网络上，Balancer 提出了一个由 4 个主要稳定币组成的池：DAI、USDC、USDT 和 MAI（miMATIC）。这个稳定的矿池目前的 APR 相当稳定，约为 20%。

![截至 2021 年 8 月的稳定币池状态](<../../.gitbook/assets/Screen Shot 2021-08-11 at 11.06.59 AM.png>)

Balancer 的最大优点是你绝对不需要拥有 4 个硬币即可存入池中。 Balancer 将自动生成与你的存款的平衡组合。这意味着，如果你有价值 100 美元的 MAI，你可以简单地将它们存入 Balancer 池中，并让算法正确地将其滑入，根据存入时各自的价格为每个代币设置 25% 的比率。

池的奖励使用 BAL 代币支付，每周分发一次。除了 BAL 代币，还可以根据你输入的池授予额外奖励。你可以在此处查不同的激励项目。在我们的案例中，参与稳定池还将为你赢得 MATIC 和 Qi 奖励。

如果你需要有关如何使用 Mai Finance 借出你的加密货币和借入 MAI（而不是出售你的加密货币来购买 MAI）的更多详细信息，请阅读本网站上的其他指南。你甚至可以在循环中包含 AAVE 以赚取更多。

池的奖励使用 BAL 代币支付，每周分发一次。除了 BAL 代币，还可以根据你输入的池授予额外奖励。你可以在此处查不同的[激励项目](https://balancer-incentives.web.app)。在我们的案例中，参与稳定池还将为你赢得 MATIC 和 Qi 奖励。

完整的流程是像这样的

![](<../../.gitbook/assets/Screen Shot 2021-08-11 at 11.34.45 AM.png>)

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

![](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.14.27 PM.png>)

### AAVE

有一篇关于如何使用 Mai Finance[ 在 AAVE 上推广加密货币](leverage-aave-tokens.md)的完整指南。这不是 MAI 稳定币的直接使用，但我们可以想象，在未来，AAVE 还将拥有一个 MAI 池，你可以在其中借出你的加密货币。

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) 可能是 Polygon 上最著名的 DEX（去中心化交易所）之一，带有 SushiSwap 和 1Inch。它也是一个 AMM（自动做市商），允许用户使用流动性池在 Polygon 网络上进行有效率地交易。交易所的任何交易都需要支付一定的费用，该费用会部分重​​新分配给将流动性存入平台的用户。

你可以在 QuickSwap 上使用 MAI 的方式与[常规收益农场](secure-your-yield-farming-profits.md)非常相似，因此如果你需要获得在 QuickSwap上进入 MAI/USDC池的确切步骤，你最好阅读本文。

目前，如果你在 QuickSwap 上进入 MAI/USDC LP（流动性提供商）池，你将获得

* 交易费用
* QUICK 代币

![截至 2021 年 8 月 QuickSwap 上的 MAI/USDC 池的详细信息](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.37.56 PM.png>)

## **Degen 农场和聚合器**

### Adamant

[Adamant](https://adamant.finance/home) 是一个聚合器，它在 Polygon 上列出所有“最佳”农场，并让你直接从他们的网站输入它们。通过将你的资产（LP 代币）存入 Adamant 的特定池中，算法将收获池授予的奖励，并自动将部分奖励复合到你的 LP 位置。

其余的奖励通常在 WMATIC 中转换，然后重新分配给 ADDY 代币（Adamant 的原生代币）的持有者。最后，您还可以获得 ADDY 代币的奖励，您可以收获和归属 90 天，从而赚取 WMATIC 一部分分红。

通常来说，如果你不太关心农场代币，并且不想每天手动多次复合奖励，那么 Adamant 是一个不错的去处。它还可以产生更多收入，因为除了池授予的奖励之外，你还可以获得一些 ADDY 奖励。

Adamant 目前支持一些接受 MAI/USDC LP 对的池。这些池在

* QuickSwap：QUICK 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励
* DinoSwap：Dino 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励
* Mai Finance：Qi 奖励被互换成更多 MAI/USDC LP 和 WMATIC 奖励

![Adamant 上的 QuickSwap MAI/USDC 池](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.51.12 PM.png>)

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

### A little bit of explanation

[Impermax](https://polygon.impermax.finance) is a platform that let users leverage their LP tokens for higher yields. The goal is very simple: by providing LP tokens and using them as collateral, one can then borrow more of the 2 underlying assets to generate more LP tokens and repeat the loop.

![Impermax loop explained](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.15.21 PM.png>)

When doing so, the user is exposed to impermanent loss, and the loss is magnified by the number of times the loop is repeated. The risk of liquidation is also multiplied when too many loops are applied. Indeed, if the APR is multiplied, the price variation of the two coins forming the pair is amplified by the lever effect, leading to faster liquidation.

With stable coins, the risk of liquidation is lower though, because the price variation is negligible. This also means that the Collateral to Debt Ratio (CDR) can be very close to 100%, leading to a high number of loops, hence a high APR.

Note that Impermax is charging fees when you borrow and leverage your position. The fee corresponds to 0.1% of your final position. As an example, if I have $100 worth of MAI/USDC and I leverage 50x, my final position will worth $5,000 and I will pay a $4.90 fee corresponding to the $4,900 that I borrowed.

The effect of looping the lending/borrowing combination allows to multiply the final APY. With an initial APY of 20% for MAI/USDC pair with a CDR of 110%, operating the loop 50 times, and using the formula

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

We can easily get a 228% final APR. There are some other elements that will affect the final APR, namely the borrowing APR (loan interest for borrowing more LP tokens), and the supply/demand of both assets composing the LP pair (directly driving the borrowing APR).

Also, because all the rates are magnified by the number of times the loop is applied, the APR will vary drastically, and can sometimes become negative for short amount of times (your LP token will be used to repay the negative APR).

### Leveraged position of my MAI/USDC pair

In the end, you are using the base APR on a much bigger value, which is earning much bigger interests, increasing the APR of your initial position.

![An example of Impermax dashboard with an initial $70.52 MAI/USDC pair](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.38.33 PM.png>)

I can see very easily how much I'm using as collateral, how much I initially invested, what's the leverage ratio, and what are the liquidation values due to the leverage ratio. This position will give me the following ratios at the time of writing

![Earnings and spendings estimation at a given time](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.41.55 PM.png>)

The APR is granted in IMX token that can either be swapped for more MAI/USDC (use the power of Mai Finance to borrow at 0% interest, RFTM), or used to provide liquidity on specific pools accepting IMX on Impermax.

### Supplying MAI to borrowers

Indeed, on the app you can also provide liquidity to those who want to apply leveraging loops to their positions (they will need underlying assets to generate more LP tokens). Lending assets is a great way to earn yield and let the borrowers take all the risks. Also, the more users are borrowing, the higher the supply APR will be.

![Rates for supplying and borrowing MAI on Impermax at a given time](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.47.56 PM.png>)

This is another great way to optimize your 0% loan on Mai Finance. Not only you don't have to pay anything to borrow MAI, but you can earn a lot of interest just by depositing it on Impermax.

## Disclaimer

Everything is this tutorial is purely educational. The goal is to bring light to projects that I think are worthy for people evolving in the crypto world on Polygon. I obviously didn't talk about Mai Finance as a farm because a dedicated tutorial will be written very soon. Finally, this guide is ABSOLUTELY NOT meant to be applied as is, it's not any financial advice and you should not follow blindly what I wrote. Please read the docs of the different projects I mentioned before considering investing on their platforms.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
