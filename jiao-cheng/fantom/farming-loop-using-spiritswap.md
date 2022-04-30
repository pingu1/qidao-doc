---
description: SpiritSwap 最近为 MAI-WFTM 推出了一个农场，它正在高度重视其主流采用。本指南介绍了你可以使用此池执行的操作。
---

# 使用 SpiritSwap 的农场循环

在耕种产量时，LP对（流动性提供对）非常重要。事实上，你希望尽可能少的无常损失，这样你就不会失去你的初始投资。这个初始对将产生收益，你可以通过重新投资你种植的代币来增加收益，而不会增加初始风险。这就是为什么我们的指南仅基于稳定币或由稳定币和blue chip代币（如比特币、以太坊或我们正在运行该策略的链中的本地天然气代币）组成的对提出策略的原因之一。

今天，我们将探索一个相对复杂的循环，该循环将基于 SpiritSwap 提供的 MAI-WFTM LP 对，以庆祝其推出和当前的提升。

![](../../.gitbook/assets/spiritswap-1.png)

### 在 SpiritSwap 上耕种 MAI

[SpiritSwap](https://app.spiritswap.finance/#/) 是 Fantom 上主要的 DEX（去中心化交易所）和 AMM（自动做市商）之一。它基于 Uniswap 平台，所以你肯定会了解 SpiritSwap 的核心功能，即交换资产，提供流动性以赚取收益。你将在平台的原生代币中获得奖励，你将能够质押并获得 inSPIRIT 的 SPIRIT 代币。 inSPIRIT 代币特别有用，它可以让你投票支持将应用额外提升的流动性池，并让你从协议收入中获得额外收益。

对于我们的策略，我们将使用 MAI-WFTM 池。截至 2021 年 12 月，此池可在 Booster Farms 选项卡中找到。

![截至 2021 年 12 月，SpiritSwap 上的 MAI-WFTM 池](../../.gitbook/assets/spiritswap-2.png)

{% hint style="info" %}
创建本指南时，该池处于非常早期的阶段（在过去 24 小时内启动），这可能解释了非常高的 APR（年度百分比率）。与往常一样，在应用我们的一种策略之前，请在投资前进行自己的研究并验证 APR。相比之下，Polygon 上的 USDC-WMATIC 约为 75%，Moonbeam 上的 MAI-MOVR 为 158%。 USDC-WFTM 等其他矿池在 Fantom 上稳定在 50% 左右。

出于本指南的目的，我们将保持该范围内的最低 APR 为 152.98%，这可能远高于应稳定的水平。
{% endhint %}

在 SpiritSwap 上耕种 MAI-WFTM 时，你将获得 DApp（去中心化应用程序）的原生代币 SPIRIT 支付的奖励。截至 2021 年 12 月，1 SPIRIT = 0.130 USDC。

### 在 Liquid Driver 上使用 SPIRIT 代币进行农耕

[Liquid Driver](https://www.liquiddriver.finance) 是另一个 Uniswap 分叉，专注于在 Fantom 上提供流动性。 Liquid Driver 最感兴趣的功能之一是他们可以从 SPIRIT 代币创建 linSPIRIT 代币。 linSPIRIT 是 inSPIRIT 代币的流动版本。 linSPIRIT 和 inSPIRIT 之间的比例是 1:1，它实际上只是 inSPIRIT 代币的包装版本，你可以直接在 Liquid Driver 上将两个代币相互交易。

![Liquid Driver上的 LiquidSwapper](../../.gitbook/assets/spiritswap-3.png)

但是，我们不会使用此功能。我们将在 Liquid Driver 上耕种 SPIRIT-linSPIRIT 池，但有一个不错的小问题：

![在 Liquid Driver 上种植 SPIRIT-linSPIRIT LP 代币](../../.gitbook/assets/spiritswap-4.png)

如你所见，你需要在BeethovenX 上创建LP 代币才能获得以LQDR 代币支付的61% APR。截至 2021 年 12 月，1 LQDR = 4.560 USDC。让我们看看如何获​​得这个 LP 代币。

### 在 BeethovenX 上创建 SPIRIT-linSPIRIT

[BeethovenX](https://app.beets.fi/#/) 已被公认为 Fantom 上的官方Balancer池。至于 Balancer，你不需要存入相同数量的两个代币来创建 LP 代币。这意味着你可以直接存入 100% 的 SPIRIT 代币，并让负责矿池的算法保持平衡。

![Beethoven X上LiquidDriver的Water Music](../../.gitbook/assets/spiritswap-5.png)

作为交换，你将获得可以存入 Liquid Driver 的 LP 代币。

{% hint style="info" %}
如你所见，BeethovenX 没有激励这个池，你不会从中获得 BEETS。当你在他们的平台上存入 LP 代币时，奖励仅由 Liquid Driver 提供，你将获得的唯一奖励是以 LQDR 支付。
{% endhint %}

### 在 Liquid Driver 上质押 LQDR

一旦你在 BeenthovenX 上创建了你的 SPIRIT-linSPIRIT LP 代币并将其存入 Liquid Driver 的正确池中，你将开始赚取 LQDR 代币。然后，你可以质押 LQDR 代币以赚取协议收入的一部分。很酷的一点是，你可以选择质押 LQDR 的时间段，这将直接影响你的 APR（这与质押 Qi 以获得协议收入是一回事）。平均锁定时间略低于 2 年（最长锁定时间），奖励支付

* LQDR: 你将能够重新质押此奖励
* WFTM: 我们稍后会使用它
* BOO: 我们稍后会使用它
* linSPIRIT: 这可用于增加你在 Liquid Driver 上的 SPIRIT-linSPIRIT 位置
* SPELL: 交换如果换取额外的 WFTM ！！！

![截至 2021 年 12 月质押 LQDR 时的质押奖励](../../.gitbook/assets/spiritswap-6.png)

### 在 SpookySwap 上质押 BOO

[SpookySwap](https://spookyswap.finance) 几乎是我们拼图的最后一块。在 Liquid Driver 上质押 LQDR 将使我们获得来自 SpookySwap 的原生代币 BOO 代币。 SpookySwap 是 Fantom 上最大的 DEX/AMM，所以你可以做与 SpiritSwap 几乎相同的事情，除了它们的原生代币是 BOO 代币。这特别有用，因为你可以在 SpookySwap 上质押你的 BOO 代币以获取 xBOO 代币，并且这种质押版的 BOO 可用于种植其他代币（这是 Uniswap forks的常见功能）。因此，一旦你拥有 xBOO，你就可以将这些代币存入 SpookySwap 以赚取额外的 WFTM。

![截至 2021 年 12 月，在 SpookySwap 上质押 xBOO 以增加 WFTM](../../.gitbook/assets/spiritswap-7.png)

### 获得更多 MAI-WTFM LP 代币

Liquid Driver 和 SpookySwap 将产生 WFTM 代币，因此我们确实缺少MAI，以便将更多 LP 代币添加到我们在 SpiritSwap 中的初始位置。这可以通过几种不同的方式来完成：

* 将 50% 的 WFTM 换成 MAI
* 将 WFTM 的 66% 借给 Beefy 或 Yearn Finance 以获得 mooScreamFTM 或 yvWFTM，然后将抵押代币存入 Mai Finance 并借用 MAI
* 将你的 WFTM 的 66% 换成另一种资产，并使用与上述相同的策略来借入 MAI

{% hint style="info" %}
如果你需要有关最后两个要点的更多详细信息，我们有一篇关于[在 Fantom 上杠杆你的资产](leverage-your-crypto-on-fantom.md)的专门文章。
{% endhint %}

对于我们的指南，我们将尝试最大化我们的收益并使用 mooScreamDAI。这意味着我们将在 Spirit Swap 上将 66% 的 WFTM 换成 DAI，然后使用 SCREAM 作为底层平台将 DAI 直接存入 Beefy 以获得 mooScreamDAI。然后，该代币将存放在 Mai Finance 的vault中，我们将能够借用 MAI。为了降低清算风险，我们将保持 200% 的 CDR（抵押债务比率），这意味着我们将借入存款价值的一半。这是完美的，因为这对应于我们保留的 WFTM 的相同值，因此可以创建额外的 MAI-WFTM LP 代币。

![在 Beefy Finance 上获得 mooScreamDAI](../../.gitbook/assets/spiritswap-8.png)

在循环结束时，我们将获得更多的 MAI-WFTM 和作为 Mai Finance 抵押品的收益代币。

### 农耕策略

以下模拟是在假设一些事情的情况下进行的：

* 在整个模拟期间，所有费率和价格都保持不变，在我们的案例中为 1 年
  * 153% APR onSpiritSwap 上的 MAI-WFTM 农业年利率为 153%
  * &#x20;SpiritSwap 上的 MAI-WFTM 农耕
  * linSPIRIT 没有奖励
  * Liquid Driver上 SPIRIT-linSPIRIT 的 61% APR
  * 质押 LQDR 的年利率为 139%
    * LQDR 年利率为 26%
    * 6% 在 WFTM
    * 30% 在 BOO
    * 74% 在 linSPIRIT
    * 3% 在 SPELL
  * 抵押 xBOO 的年利率为 36%
  * mooScreamDAI 的 21% 年利率
* 所有奖励和计划也将运行一整年
* 初始投资为价值 1,000 美元的 MAI-WFTM LP 代币 is $1,000

![](../../.gitbook/assets/spiritswap-9.png)

### 第1天

第一天，只需将你的 MAI-WFTM 对存入 SpiritSwap。在一天结束时，收获你的 SPIRIT 代币并将它们组合成 BeethovenX 上的 SPIRIT-linSPIRIT 对，然后将该 LP 代币存入 Liquid Driver。在一天结束时，你会得到

| MAI-WFTM | linPIRIT-SPIRIT | LQDR | xBOO | mooScreamDAI |
| -------- | --------------- | ---- | ---- | ------------ |
| 1,000.00 | 4.19            | 0.00 | 0.00 | 0.00         |

### 第2天

在第 2 天，你的 MAI-WFTM 仍在生成 SPIRIT 代币，你将存入 Liquid Driver 上的 linSPIRIT-SPIRIT 池中，但你也将能够收获你的前几个 LQDR 代币，并将它们质押以获得多重奖励.在一天结束时，你会得到

| MAI-WFTM | linPIRIT-SPIRIT | LQDR  | xBOO | mooScreamDAI |
| -------- | --------------- | ----- | ---- | ------------ |
| 1,000.00 | 8.38            | 0.007 | 0.00 | 0.00         |

### 第3天

在第 3 天，除了您的 LQDR 之外，同样的事情将从协议收入中产生你的前几个奇异代币。不要忘记你实际上会质押你的 BOO，将你的 linSPIRIT 添加到池中，你的 LQDR 将被重新质押，其余的将被交换为 WFTM。然后将生成的 WFTM 部分交换为 DAI，然后将 mooScreamDAI 存放在vault中以借用 MAI，形成额外的 MAI-WFTM，然后存放在 SpiritSwap 上。在第 3 天结束时，你将获得

| MAI-WFTM | linPIRIT-SPIRIT | LQDR  | xBOO | mooScreamDAI |
| -------- | --------------- | ----- | ---- | ------------ |
| 1,000.00 | 12.58           | 0.021 | 0.00 | 0.00         |

{% hint style="info" %}
xBOO 和 mooScreamDAI 头寸太小而无法显示，因此你可以在前几天跳过这些步骤。另外，为简单起见，我没有把交易费用考虑在内，这可能会影响你的收益。
{% endhint %}

此时，系统已准备就绪，是时候坐下来获利了。

## 耕种结果

### 日常

系统完全启动后，你必须遵循以下日常程序：

* 从 SpiritSwap 上的 MAI-WFTM 池中收获 SPIRIT 代币
* 从 Liquid Driver 质押池中收获奖励
* 从 SpookySwap 质押池中收获奖励
* 将 SpiritSwap 的 SPIRIT 和 Liquid Driver 的 linSPIRIT 存入 BeethovenX 的池中
* 将 SPIRIT-linSPIRIT LP 代币存入 Liquid Driver
* 在 SpookySwap 上质押你的 BOO 以获得 xBOO
* 将你的 xBOO 抵押到农场 WFTM
* 将你的 SPELL 换成 WFTM
* 将 66% 的 WFTM 换成 DAI
* 将 Beefy 上生成的 DAI 存入即可获得 mooScreamDAI
* 将 mooScreamDAI 代币存入 Mai Finance
* 借入 MAI 并保持 200% 的 CDR（你存入金额的 50%）
* 为 SpiritSwap 上的 MAI-WFTM 池提供流动性

### 月复一月的原始结果

| 天   | MAI-WFTM  | linPIRIT-SPIRIT | LQDR    | xBOO   | mooScreamDAI | MAI debt |
| --- | --------- | --------------- | ------- | ------ | ------------ | -------- |
| 30  | 1,000.004 | 130.010         | 3.281   | 0.026  | 0.005        | 0.002    |
| 60  | 1,000.039 | 256.218         | 13.014  | 0.210  | 0.041        | 0.021    |
| 90  | 1,000.140 | 383.220         | 29.369  | 0.712  | 0.147        | 0.074    |
| 120 | 1,000.349 | 511.436         | 52.538  | 1.698  | 0.364        | 0.182    |
| 150 | 1,000.708 | 641.302         | 82.741  | 3.338  | 0.738        | 0.369    |
| 180 | 1,001.268 | 773.275         | 120.224 | 5.810  | 1.323        | 0.661    |
| 210 | 1,002.081 | 907.835         | 165.263 | 9.295  | 2.175        | 1.088    |
| 240 | 1,003.207 | 1,045.486       | 218.165 | 13.984 | 3.360        | 1.680    |
| 270 | 1,004.710 | 1,186.759       | 279.268 | 20.075 | 4.947        | 2.473    |
| 300 | 1,006.659 | 1,332.316       | 348.947 | 27.773 | 7.014        | 3.507    |
| 330 | 1,009.130 | 1,482.451       | 427.613 | 37.296 | 9.645        | 4.823    |
| 360 | 1,012.205 | 1,638.095       | 515.717 | 48.870 | 12.935       | 6.467    |

### 第365天

经过一整年的耕作系统，你会得到

* SpiritSwap 上价值 1,012.782 美元的 MAI-WFTM
* Liquid Driver 上价值 1,664.608 美元的 linSPIRIT-SPIRIT
* 价值 531.353 美元的 LQDR 质押在 Liquid Driver 上
* SpookySwap 上价值 51.015 美元的 xBOO
* Mai Finance 上价值 13.554 美元的 mooScreamDAI 在vault中
* 价值 6.777 美元的 MAI 债务

考虑到 1,000 美元的初始投资，这相当于 227.096% 的 APY

### 策略的小调整

如果你想获得较低的风险敞口，你可以从你的初始投资开始，将价值 1,000 美元的 mooScreamDAI 在保险库中，借入价值 500 美元的 MAI 并为 WFTM 交换 50% 以获得 SpiritSwap 的起点。如果 FTM 的价格下跌太多，这将大大降低你损失部分初始资金的风险。

目前，最高费率由 SpiritSwap 池提供，因此循环的一个可能简化是简单地将你在 Liquid Driver 上获得的所有 LQDR 代币换成更多 MAI-WFTM。

## 免责声明

本指南是您可以在 Fantom 上实现的理论版本。当我们在教程中公开循环时，我们实际上是在尝试从不转储代币并始终尝试找到使用我们收集的所有内容的最佳方式。这是保持价格上涨的好方法，因为种植和抛售代币通常会导致种植代币的价格下跌，从而使收益率越来越不具吸引力。如果每个人都保留他们的代币，他们的价格只会随着时间的推移而上涨。

无论如何，该指南也是基于很多假设（价格不变，奖励率不变）并且不计算交易费用，所以如果你想实现这种类型的闭环，请确保在一天结束时盈利，或者每周只复合一次你的收益。和往常一样，DYOR！

{% hint style="info" %}
本指南绝对不是财务建议，它是出于教育目标而制定的。你需要注意价格变化，供需，奖励计划结束日期，无常损失等......目标不是提出可以盲目遵循的食谱，所以请做好功课和自己的模拟，只有投资你准备好可能失去的东西。
{% endhint %}

