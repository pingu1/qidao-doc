---
description: 本教程将详细展示当你用稳定币耕作时，如何在 Polygon 上使用不同的 DApp 来增加效益。
---

# 像乐高积木一样堆叠 DApp

**简介**

当你在给定农场上种植产量时，你通常会以原生农场代币的形式获得奖励。然后，你可以选择出售它们或保留它们并希望它们随着时间的推移会获得一些价值。本指南将介绍一些不同的 DApp（去中心化应用程序），以在不出售任何东西的情况下最大化你的收益，同时仍然可以复利。

这篇文章也将从稳定币开始，因为这被认为是一种相对安全的策略。但是，你需要记住，这不是财务建议，应该谨慎地遵循该指南，因为结果是绝对不能保证的。和往常一样，做你自己的研究。

![](../../.gitbook/assets/screen-shot-2021-08-30-at-10.52.20-am.png)

## QuickSwap

QuickSwap 是 Polygon 上最大的 AMM（自动做市商）之一。人们将成对的代币存入流动性池，并从使用该平台互换代币的其他用户那里赚取交易费。在掉期期间，QuickSwap 使用不同的流动性池自动选择最佳路线，每次从一个池子跳到另一个池子都要支付交易费用，这些费用会重新分配给流动性供应商。

## **稳定币耕种**

对于这个练习，我们将在 QuickSwap 上使用 MAI/USDC 对。这个流动性池是一个稳定的池，提出了一个 APY（年收益率在 20% 到 25% 之间变化）。收益由交易费用（累积到流动性池中）和 QUICK 奖励组成。

![ 截至 2021 年 8 月，QuickSwap 上的 MAI/USDC 流动性池](../../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

该池每天得到固定数量的 QUICK 代币，然后根据其在池中的份额分配给流动性提供者。例如，如果该池具有价值 1,000,000 美元的流动性，并且你已经存入了 1,000 美元的 LP（流动性提供者）代币，则你拥有池的 0.1%，这使你有权获得每日 QUICK 奖励的 0.1%。当你管理你进入的池时，你的Quick奖励将可以领取。

![以 20 美元的押金领取我的 QUICK 奖励](../../.gitbook/assets/screen-shot-2021-08-30-at-6.39.44-am.png)

你可以定期领取它们，为了让它们发挥作用。让我们看看如何。

### Dragon's Lair

Dragon's Lair 是一种优化 QuickSwap 收益的方法。你可以将你从流动性池中赚取的 QUICK 代币存入 Lair，它们将为你赚取额外的 QUICK 奖励。这是一个好主意如果你想保留 QUICK 代币而不是出售它们。当你的 QUICK 代币投入 Dragon's Lair 时，它们产生的奖励会自动复利，Lair 的 APY 约为 12%。

![截至 2021 年 8 月的 Dragon's Lair APY](<../../.gitbook/assets/image (7) (1).png>)

在你存入 QUICK 代币后，你将在钱包中获得一些 dQUICK 代币，这些代币代表你拥有的 QUICK 池的份额。注意，QUICK:dQUICK 的比率不是 1:1，因为 dQUICK 代表你在池中的份额，而QUICK的数量将随着时间的推移而增加，因为更多的奖励被添加到池中。

现在你把稳定币存入流动性池中，它们会产生快速奖励。多亏Dragon's Lair，奖励正在产生更多奖励。但是等等，还有更多……

### Dragon's Syrup

Dragon’s Syrup是QuickSwap为更多持有QUICK代币的用户提供的一种额外奖励方式。QuickSwap 团队设立了一个计划，合作伙伴可以通过向 QuickSwap 平台的用户授予他们自己的代币来推广他们的产品。然后你可以将你的 dQUICK 代币存入其中一个农场，以便在 Dragon's Lair 奖励之上赚取这些奇异的代币。我们感兴趣的一个是 ADDY 农场。

![Dragon's Syrup，一个通过 dQUICK 存款收集 ADDY 代币的农场](../../.gitbook/assets/screen-shot-2021-08-30-at-6.49.25-am.png)

当你将 dQUICK 存入农场时，它们将从 Dragon's Lair 消失（与你将它们存入 Vault 时你的 camToken 从 Mai Finance 的Yield页面上消失的方式非常相似）。但是你可以清楚地看到，来自 Lair 的 dQUICK APY 仍然适用，并且你还将获得额外的 ADDY 奖励。在这里，APR（年度百分比奖励）目前为 21.36%。

{% hint style="info" %}
你会注意到糖浆农场有一个到期日期。在这里，ADDY 场将在 50 天 11 小时后到期。一些新农场会随着一些旧农场的消失而出现。
{% endhint %}

在我们的这种情况，我们获得的 ADDY 奖励可以手动领取。你可以注意到，只有当我们将 QUICK 奖励手动复合成到 dQUICK 中，然后我们将其存入 QuickSwap 上的 ADDY 农场时，我们收集 ADDY 奖励的比率才能加快。

### 快速回顾

我们有 MAI/USDC LP 代币存入流动性池，我们赚取

* 调换费
* 池中的QUICK奖励，我们需要手动领取并添加到Dragon's Lair
* Dragon's Lair中的QUICK奖励会自动合成到我们现有的奖励中
* 我们可以领取的Dragon's Syrup中的 ADDY 奖励

## Impermax

Impermax是一个应用程序，允许用户自动杠杆他们的资产为了扩大他们在流动性池中的头寸。这是通过借用 Impermax 平台上提供的额外资产来完成的。

### 稳定币耕种

对于这个练习，我们还将使用 Impermax 中的 MAI/USDC 池。通过将一些 LP 代币存入 MAI/USDC 池，我们现在可以选择杠杆该存款一定次数，为了增加我们的暴露资本，并获得更多回报。在使用 Impermax 时你需要注意几点

* 你只能借用其他用户提供的资产
* 借入的资产越多，借款利率越高
* 如果借款利率变得太高，你的最终 APR 可能会变成负数，然后你会损失一些你的LP
* 杠杆越多，APR 越高，但借款利率越高

### 杠杆头寸

在 QuickSwap 上，我存入了价值 20 美元的 MAI/USDC 对。在 Impermax 上，我将只存入价值 10 美元的 MAI/USDC，并将对其应用 x2 杠杆以获得 20 美元的风险敞口。

![在给定时间Impermax上的杠杆窗口](../../.gitbook/assets/screen-shot-2021-08-30-at-7.11.10-am.png)

你可以在上面的截图中看到，如果我将我的杠杆增加到 x2.1，我会借

* 0.481269 USDC
* 0.487593 MAI

我们还可以看到我收取的交易费用会增加多少（+3.45%），以及QUICK奖励（+36.83%）、IMX奖励（+23.05%）和借贷利率（-37.20%）的增加最终估计 APR 为 26.13%。

注意在此示例中，借款费用是使用 QUICK 奖励和交易费用支付的，以防 QUICK 奖励不够。然后，如果还没有支付借款费用，IMX奖励会给到供应商，最后，如果供应商还有需要支付的东西，就会用押金支付给供应商。

我们在这的目标是匹配我们在 QuickSwap 上的存款，因此我们将坚持 x2 杠杆。这也确保我们不会有进入负 APR 的风险。我们的目标不是收集尽可能多的奖励，而是随着时间的推移增加我们的头寸，并收集 IMX 代币。

### 快速回顾

我们将 MAI/USDC 代币存入适当的池中

* 为了匹配 QuickSwap 中存入的金额，我们的仓位被杠杆化两次
* 我们收集 IMX 代币

## Adamant

Adamant 是一个收益优化器平台，可自动收集流动性池并将奖励自动复合到额外的 LP 代币中。 Adamant 上的大多数池都是来自 QuickSwap、SushiSwap 等大型流动性提供商的流行池。让我们看看如何使用 Adamant 来优化我们的收益。

### QUICK/IMX 耕作

我们在 QuickSwap 上赚取 QUICK 代币，我们在 Impermax 上赚取 IMX 代币。让我们使用 Adamant 从 QuickSwap 中耕作 QUICK/IMX 池。为什么这么做？因为农场实际上非常有利可图，正如你在此处看到的：

![来自 Adamant 上 QuickSwap 的 IMX/QUICK 池](../../.gitbook/assets/screen-shot-2021-08-30-at-7.27.26-am.png)

在撰写本文时，Adamant 上 IMX/QUICK 矿池的当前 APY 为 417.25%。奖励组成由



* 168.49% 自动复合 QUICK（出售来自 QuickSwap 的 QUICK 奖励以购买添加到你头寸的额外 IMX/QUICK LP 代币）
* 你可以在 Adamant 上索取 212.85% ADDY 代币（它们的归属期为 90 天，因此你无法立即访问它们）
* 如果你每天领取 ADDY，则在 WMATIC 中支付 35.91% 的费用股息

这意味着你的 IMX/QUICK 头寸会随着时间的推移而增长，并且你将获得 ADDY 奖励。你持有的 ADDY 越多，你收取的股息 (WMATIC) 就越多。

你还可以看到 Adamant 上的 APY 是Boostable。这意味着如果你质押额外的 ADDY 代币（不是既得的代币），你将应用额外的乘数来获得奖励。这实际上是一件好事，因为我们确实从 QuickSwap 上的 Dragon's Syrup 中获得了额外的 ADDY 代币！

### **收获ADDY和WMATIC**

你在 IMX/QUICK 池中获得从你的 LP 头寸收获的 ADDY 时，它们将被锁定 90 天，但将允许你以 WMATIC 的形式获得一些分红。根据你已授予的 ADDY 代币，当前的股息 APR 为 34%。

在 90 天归属期之后，你将有可能将它们锁定至少 90 天，为了增加从金库中挣得的 ADDY 代币并赚取额外的 ADDY 代币。

WMATIC 股息是我们所追崇的 QuickSwap + Impermax + Adamant 三重奏的实际输出，因为我们将能够使用它们将额外的 LP 代币重新注入 QuickSwap 和 Impermax。

### 快速回顾

我们以 IMX/QUICK LP 代币的形式存入从 Impermax 和 QuickSwap 赚取的 IMX 和 QUICK 代币。Adamant在赚取

* 对QuickSwap为IMX/QUICK池授予的QUICK代币的一部分进行自动复合，获得更多LP代币
* 用于提升 IMX/QUICK 奖励并使我们有资格获得分红的 ADDY 代币
* WMATIC 分红

## AAVE

有了在 Adamant 上赚取的 WMATIC 代币，我们现在可以将它们存入 AAVE 为了获得一些收益。这是[专门的文章](leverage-aave-tokens.md)中提到的正规的AAVE 代币杠杆。

## Mai Finance

随着AAVE 存款之后，我们的钱包中会收到 amWMATIC。我们可以使用 Mai Finance 上的Yield页面将AAVE 提供的奖励与 Matic 激励的奖励自动复合，并从我们在 Adamant 上赚取的 MATIC 获得额外的 4%。

然后，camWMATIC 可以通过将它们存入 camWMATIC 金库来用作 Mai Finance 的抵押品，这允许我们借入 MAI，并将一部分铸造的 MAI 互换成USDC。一旦我们的钱包中有更多的 MAI 和 USDC，我们就可以将 2 个稳定币组合成额外的 LP 代币，这些代币将存放在 QuickSwap 和 Impermax 上。再一次，如果你需要有关如何执行此操作的详细信息，请阅读[专门的文章](leverage-aave-tokens.md)。

## 引导系统

以下是对初始投资价值 1,000 美元的 MAI/USDC LP 代币进行的模拟，以及不同平台在 2021 年 8 月 30 日给出的当前 APR/APY。这不是我们上述描述内容的真正运用。费率会有所不同，代币价格会有所不同，一些程序会结束等等……因此，最终结果只是对如果一切保持稳定你可以获得的结果的估计，但情况永远不会如此。

### 第1天

由于你有价值 1,000 美元的 MAI/USDC，你想要在 QuickSwap 和 Impermax 之间拆分 LP 代币。因为 Impermax 允许我们杠杆我们的存款，我们实际上可以在 QuickSwap 上放入更多代币，并使用 Impermax 的杠杆选项来匹配你在 QuickSwap 中获得的东西。

为了降低 Impermax 上负利率的风险，拆分如下：

* 在 QuickSwap 上价值 900 美元的 MAI/USDC
* 在 Impermax 上价值 100 美元的 MAI/USDC 使用 x9 杠杆在 MAI/USDC 池中暴露 900 美元

模拟的其余部分，我们将考虑 QuickSwap 为以 QUICK 代币支付的 MAI/USDC 授予25.56% 的 APR，而 Impermax 在 x9 时为 MAI/USDC 提供 20% 的平均 APR，仅以 IMX 代币支付。这对应于每天的费率

* 在QuickSwap上 + 0.07%
* 在Impermax上 +0.05%

这意味着在第 1 天结束时，我们已经收集了

* 价值 0.63 美元的 QUICK
* 价值 0.49 美元的 IMX

从那里，我们可以将我们得到的所有 IMX 与一部分 QUICK 奖励组合成 IMX/QUICK LP 对，并将存入 Adamant。 LP 对的价值为 0.98 美元，我们仍有价值 0.14 美元的 QUICK，我们将其存入 Dragons's Lair 以换取 dQUICK。然后将 dQUICK 用于 Dragon's Syrup 以在第 2 天开始收集 ADDY。

| 奖励类型                   | 美元的价值 |
| ---------------------- | ----- |
| QuickSwap上的 dQUICK     | 0.14  |
| QuickSwap上的ADDY        | 0     |
| Adamant上的IMX/QUICK     | 0.98  |
| Adamant上的ADDY          | 0     |
| Adamant 上的 WMATIC      | 0     |
| Mai Finance上的camWMATIC | 0     |
| Mai Finance上的债务        | 0     |

### 第 2天

在 QuickSwap 和 Impermax 上仍然有相同的头寸，没有任何变化，我们再次获得价值 0.63 美元的 QUICK 和价值 0.49 美元的 IMX，用于在 QuickSwap 上的 ADDY 场中获得价值 0.98 美元的 IMX/QUICK 和 0.14 美元的 dQUICK。

然而，Adamant 的 IMX/QUICK 头寸在 IMX/QUICK 上的APR为 151.96%（或每天 +0.42%）。这意味着我们原始的 0.98 美元存款现在是 0.984 美元，我们通过 QuickSwap 和 Impermax 上的农耕增加了 0.98 美元。它还产生了 177.43% 的 APR（或每天 +0.49%）ADDY，相当于 0.005 美元。

在 QuickSwap 上，我们存入 Dragon's Syrup 的 dQUICK 正在以 12.26% 的APR（每天 +0.03%）产生额外的 QUICK 代币，并以 17.08% 的APR（每天 +0.05%）产生 ADDY 代币。这适用于价值 0.18 美元的 QUICK，这意味着在第 2 天结束时，我们已经生成了价值 0.00006 美元的 ADDY 和价值 0.000054 美元的 QUICK。 ADDY 奖励可以领取并添加到 Adamant 中，以开始提升 IMX/QUICK 头寸的 ADDY APR。

| 奖励类型                   | 美元的价值   |
| ---------------------- | ------- |
| QuickSwap 上的 dQUICK    | 0.274   |
| QuickSwap 上的 ADDY      | 0.00006 |
| Adamant上的**I**MX/QUICK |         |
| Adamant上的ADDY          | 0.005   |
| Adamant 上的 WMATIC      | 0       |
| Mai Finance上的camWMATIC | 0       |
| Mai Finance上的债务        | 0       |

### 第3天

继续前进，在 Adamant 上声称的 ADDY 奖励现在正在产生一些 WMATIC 奖励。收集的第一个价值 0.005 美元的 ADDY 可获得 56% 的 APR（每天 0.15%）或 WMATIC 股息，相当于价值 0.000007 美元的 WMATIC。请牢记，我们只是在这里启动引擎。

| 奖励类型                   | 美元的价值    |
| ---------------------- | -------- |
| QuickSwap上的dQUICK      | 0.411    |
| QuickSwap上的ADDY        | 0.00019  |
| Adamant上的IMX/QUICK     | 2.971    |
| Adamant上的ADDY          | 0.014    |
| Adamant上的WMATIC        | 0.000007 |
| Mai Finance上的camWMATIC | 0        |
| Mai Finance上的债务        | 0        |

### 第4天

我们现在可以在循环中添加 WMATIC。这笔股息将存入 AAVE，然后用于 Mai Finance 借入新的 MAI。

| 奖励类型                   | 美元的价值     |
| ---------------------- | --------- |
| QuickSwap上的dQUICK      | 0.548     |
| QuickSwap上的ADDY        | 0.00038   |
| Adamant上的IMX/QUICK     | 3.969     |
| Adamant上的ADDY          | 0.029     |
| Adamant上的WMATIC        | 0.000029  |
| Mai Finance上的camWMATIC | 0.000007  |
| Mai Finance上的债务        | 0.0000035 |

此时，Mai Finance 的“债务”将用于增加 QuickSwap 和 Impermax 上的 MAI/USDC LP 头寸，系统完全地启动。

## 农耕结果

![](../../.gitbook/assets/screen-shot-2021-08-30-at-11.33.34-am.png)

### 日常工作

日常工作由以下交易组成

* 在 Impermax 上收获 IMX
* 在 QuickSwap 上收获QUICK
* 在 QuickSwap 上创建新的 IMX/QUICK LP 对
* 将剩余的 QUICK 存入 Dragon's Lair 以获得 dQUICK
* 将 dQUICK 存入 Dragon's Syrup 以获得额外的 ADDY
* 在Dragon's Syrup上收获ADDY
* 在 Adamant 金库上存入收获的 ADDY
* 在 Adamant 上存入 IMX/QUICK LP 代币
* 从 LP 对中在 Adamant 上收获 ADDY
* 在 Adamant 上收获 WMATIC 股息
* 在 AAVE 上存入 WMATIC 并获得 amWMATIC
* 在Mai Finance存入amWMATIC并获得camWMATIC
* 将 camWMATIC 存入 Mai Finance 的金库
* 在Mai Finance 上借入50%的存款作为MAI稳定币
* 在 Mai Finance 上将 50% 的铸造 MAI 互换成 USDC
* 在 QuickSwap 上创建新的 MAI/USDC LP 对
* 将 90% 的新 LP 代币存入 QuickSwap 流动性池
* 将 10% 的新 LP 代币存入 Impermax 流动性池
* 杠杆 Impermax 上的新头寸来匹配 QuickSwap 上的头寸

**月复一月的原始结果**

| 月份 | dQUICK | IMX/QUICK | ADDY    | WMATIC | 债务     |
| -- | ------ | --------- | ------- | ------ | ------ |
| 1  | $4.25  | $32.56    | $2.32   | $0.03  | $0.02  |
| 2  | $8.36  | $68.34    | $9.65   | $0.28  | $0.15  |
| 3  | $12.48 | $108.86   | $22.30  | $0.98  | $0.49  |
| 4  | $16.59 | $154.78   | $41.34  | $2.41  | $1.20  |
| 5  | $20.71 | $206.83   | $67.50  | $4.86  | $2.42  |
| 6  | $24.84 | $265.83   | $101.73 | $8.70  | $4.34  |
| 7  | $28.97 | $332.74   | $145.11 | $14.31 | $7.15  |
| 8  | $33.12 | $408.63   | $198.87 | $22.14 | $11.06 |
| 9  | $37.29 | $494.73   | $264.40 | $32.70 | $16.34 |
| 10 | $41.48 | $592.45   | $343.28 | $46.57 | $23.26 |
| 11 | $45.71 | $703.39   | $437.33 | $64.40 | $32.19 |
| 12 | $49.97 | $829.37   | $548.59 | $86.94 | $43.46 |

### 第365天

一整年后，我们投资的最终状态将是

| 奖励类型                  | 美元的价值   |
| --------------------- | ------- |
| QuickSwap上的dQUICK     | 50.689  |
| QuickSwap上的ADDY       | 4.325   |
| Adamant上的IMX/QUICK    | 851.968 |
| Adamant上的ADDY         | 568.972 |
| Adamant上的WMATIC       | 91.209  |
| Mai Finance上的amWMATIC | 91.220  |
| Mai Finance上的债务       | 44.30   |

请注意，Adamant 中的 WMATIC 和每天收集，因此它们不是通过此过程产生的最终收入的一部分。此外，通过 QuickSwap 农场生成的 ADDY 并没有每天收获并添加以在此模拟中提高 Adamant 的 ADDY 奖励（它已经足够复杂了）。

最后，一年后，产生的收入价值 1,567.174 美元。如果我们认为初始投资是价值 1,000 美元的 MAI/USDC，那么我们的稳定货币对的最终 APY 为 156.71%。

## 结论

这款乐高游戏让我们能够从稳定的硬币种植中产生令人印象深刻的 APY，而且风险敞口很小。当然，这个模拟做出了一些 假设100% 不正确，但它说明了我们如何组合不同的 DApp 以最大限度地提高耕作产量。它还表明，出售我们种植的代币并不是必要的，如果你花时间研究可能性，就肯定有一个有效使用它们的方法。

## 免责声明

本指南绝对不是财务建议，它是出于教育目标而制作的。 目标不是提出可以盲目遵循的秘方，因此请做好功课和自己的模拟，并且只投资你准备好可能会失去的东西。你需要注意价格变化、供需、奖励计划结束日期、无常损失等......

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
