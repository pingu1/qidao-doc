---
description: 本页介绍了如何将流动性挖矿与Mai Finance提供的借贷奖励相结合，以增加你的整体利益。
---

# 如何结合耕种和借贷奖励

## 简介

2021 年 9 月，Mai Finance推出了金库奖励，以促进其借贷业务，并让人们使用他们的代币来借入 MAI。它不仅可以用少量还款费用获得 0% 的利息贷款，现在人们还可以通过借钱获得报酬。本指南将提出一种基于稳定币种植的策略，使用 Augury Finance 作为代币来源，这些代币将为 Mai Finance 的金库提供资金，从而获得高额借贷激励，然后将额外的 MAI 重新注入农场。

![](<../../.gitbook/assets/image (29).png>)

## 应用程序和池演示

### Augury Finance

Augury Finance 是一个收益聚合器，不专注于自动复合你的 LP（流动性池）代币。取而代之的是，Augury 将自动出售其用于买其输液中的其他代币的农场的代币。

例如，你可以在 Augury 上耕种 DFYN-WETH对

![Augury Finance 上的 DFYN-WETH 矿池示例](<../../.gitbook/assets/image (30).png>)

这个 Infusion 使用 DinoSwap 作为底层农场，以及一个可以在 DFYN 上获得的 LP 代币。 APR为123.43%，用户在此池中存入流动性将奖励

* WETH的30%&#x20;
* LINK的20%
* WBTC的20%
* USD的15%
* WMATIC的15%

如果你在 DinoSwap 上耕种，你将获得 DINO 代币的报酬，其价格非常的反复无常。在其他聚合器（如 Adamant 或 Beefy）上，你会增加你的 LP 头寸，但使用 Augury，你可以通过获得不太可能具有非常高波动性的代币来“确保”你的头寸。缺点是你的初始头寸不会随着时间的推移而增长，因为 100% 的收获 DINO 被转换为由奖励构成的一套代币

{% hint style="info" %}
Augury Finance 使用 3 个不同的注入层，它们具有不同的存款费用和表现费。请阅读你想要使用的层类型，并确保你了解它们对你的耕作策略的影响。
{% endhint %}

在我们的策略中，我们将使用 USDT-UST tier2 农场，以 WETH/WBTC/LINK/WMATIC/USDC 的混合奖励用户，因为 Mai Finance 为我们将获得的 5 个代币中的 4 个提出了 4 个金库作为奖励。为了最大化我们的利润，我们将在 Augury 的输出和 Mai Finance 的金库之间添加 AAVE，因为我们将收获的 5 个代币中有 3 个可以借给 AAVE。

![稳定币耕种USDT-UST 用于我们的策略](<../../.gitbook/assets/image (31).png>)

### Curve

Curve 是一个蓝筹项目，将奖励借出蓝筹代币的用户。奖励由自动合成代币（添加回投资）、WMATIC 代币和 CRV 代币组成，这两种代币Mai Finance上接受为抵押品。

关于 Curve 及其池需要注意的一件非常有趣的事情是，人们不必为给定的池存入确切数量的每个代币。相反，可以提供单个代币，管理池的算法将通过出售一部分存款并购买其他代币来自动调整其他代币，以保持池中的正确比率。

我们将使用接受 WBTC/WETH/USDC/USDT/DAI 的任意组合的 atricrypto3 池，我们将在 Augury 池中添加将由池生成的 USDC。

![截至 2021 年 9 月，Curve 上的 atricrypto3 池的详细信息](<../../.gitbook/assets/image (32).png>)

### AAVE

正如在关于 Augury 的段落中提到的，在我们在 Mai Finance 上使用它们之前，AAVE 用于为在 Augury 上种植的代币添加一个小奖励。而不是将我们的 WBTC、WETH 和 WMATIC 直接放在Mai Finance上，我们将这些代币存入 AAVE，并使用Mai Finance的收益工具将 AAVE 的奖励自动复合到 amToken 池中，并使用 camToken 作为金库的抵押品。你可以通过阅读[利用你的 Aave 市场代币](leverage-aave-tokens.md)来获得有关这部分的更多详细信息。

![截至 2021 年 9 月的 AAVE贷款奖励](<../../.gitbook/assets/image (33).png>)

### Balancer

Balancer 是另一个像 Curve 一样的蓝筹项目。你将能够将某些代币存入由2个以上代币组成的池中，并且存入一个代币。池将自动平衡以获得组成池的每个代币的相等比例。

对于我们的策略，我们将使用 WETH/BAL/Qi/MAI/USDC 池。该矿池将接受从 Mai Finance 的金库中收集的 Qi 代币，并将奖励我们额外的 Qi 和 BAL 代币，我们将能够将这些代币存入 BAL 金库中的 Mai Finance，让我们能够铸造更多的 MAI 和增加我们在Augury时的耕作头寸。

![截至 2021 年 9 月的Balancer 5-池](<../../.gitbook/assets/image (34).png>)

## 引导系统

![](<../../.gitbook/assets/image (35).png>)

下面是一个模拟，初始投资价值 1,000 美元的 ETH 存入 camWETH 金库，借入价值 500 美元的 MAI，转换为价值 500 美元的 USDT-UST。该模拟假设不同系统有以下奖励

* USDT-UST 农耕 APR 为 22.53%
* amWBTC APR为0.39%
* amWETH APR 为1.71%
* amWMATIC APR 为3.80%
* atricrypto3 APR 为 3.86% 自动复合 LP 代币，13.09% WMATIC 和 17.63% CRV
* 5-代币Balancer 池，APR 为 43.46%，BAL:Qi 比率为 1:6

Vault 奖励 APR 为

* camWBTC 23.28%
* camWETH 21.52%
* camWMATIC 32.93%
* LINK 24.51%
* CRV 116.71%
* BAL 62.38%

这些 APR 在不同平台上都可能发生变化，并且不能保证它们会持续一整年，但是我们将在本次模拟中采用它们，以便了解系统可能的整体 APR。为了进一步“简化”模拟，我们不会考虑价格变化，也不会考虑交易费用。也请注意，此模拟考虑了 Mai Finance 上的 Vault 奖励和 Balancer 奖励每天而不是每周复合，但这些奖励目前每周空投到用户的钱包。最后，为了进行模拟，我们将假设 CDR（抵押品与债务比率）始终为 200%，这意味着我们只借入了存款的一半来继续获得奖励，但要防止轻松清算。

### 第1天

如果你还有价值 1,000 美元的 WETH，请将其存入 AAVE 以获得 amWETH，然后将你的 amWETH 存入 [Mai Finance](../../) 以获得 camWETH，最后将你的 camWETH 存入相应的金库，以便能够借入 500 MAI。

使用[anchor](https://app.mai.finance/anchor) 将你的 MAI 转换为 USDT（或者，如果Anchor中没有流动性，你可以使用另一个 DEX，例如 [QuickSwap](https://quickswap.exchange/#/)），然后你可以使用 [DFYN](https://exchange.dfyn.network/#/) 将你的 USDT 的 50% 互换成 UST 并形成一个 USDT-UST 对，然后你可以在[Augury](https://augury.finance/infusions/)上存款。请注意，你还需要一些 OMEN，你也可以在 QuickSwap 上购买。

因此，在第一天结束时，我们收获了以下奖励

| 奖励类型          | 美元的价值 |
| ------------- | ----- |
| 来自农耕的WBTC     | 0.123 |
| 来自农耕的WETH     | 0.031 |
| 来自农耕的WMATIC   | 0.031 |
| 来自农耕的LINK     | 0.031 |
| 来自农耕的USDC     | 0.092 |
| 来自vaults的Qi奖励 | 0.295 |

这些只是我们在第一天结束时从耕种和借贷中获得的奖励。

### **第**2天

获得奖励，WBTC、WETH和WMATIC通过AAVE和Mai上的收益仪器后，将被发送到相应的Mai金融金库。 LINK 直接存入 LINK 金库，USDC 发送到 atricrypto3 池中的 Curve。

Qi 奖励被发送到 Balancer。在这一点上，我们可以从 3 个 camToken 保险库和 LINK 保险库（准确地说价值 0.13 美元的 MAI）借用更多的 MAI，我们可以从我们借用的 MAI 创建更多的 USDT-UST对。

因此，在第 2 天结束时，我们收获了以下奖励

| 奖励类型                | 美元的价值   |
| ------------------- | ------- |
| 来自农耕的WBTC           | 0.123   |
| 来自农耕的WETH           | 0.031   |
| 来自农耕+ Curve的WMATIC  | 0.031   |
| 来自农耕的LINK           | 0.031   |
| 来自农耕的USDC           | 0.093   |
| 来自Curve的CRV奖励       | 0.00004 |
| BAL奖励               | 0.00005 |
| 来自vaults的Qi奖励       | 0.296   |

在这一点上，系统已准备好，奖励以一种方式流动，每一步都在为下一个步骤提供支持，从而创建一些不错的小循环。

## 农耕结果

### 每日例行

每日例行由以下交易组成

* Augury上收获奖励
* 在 AAVE 上存入WBTC、WETH 和 WMATIC
* 将 amWBTC、amWETH 和 amWMATIC 存入 Mai Finance 的收益仪器中
* 将 camWBTC、camWETH 和 camWMATIC 存入 Mai Finance 的各自的金库中
* 将 LINK 存入 Mai Finance 的 LINK 金库
* 将 USDC 存入 Curve 的 atricrypto3 池中
* 从 Curve 收获WMATIC 并在 camWMATIC 金库中使用它们
* 从 Curve 获取 CRV 并在 CRV 金库中使用它们
* 从不同的金库借用 MAI
* 通过Anchor在Mai Finance上将MAI转换为USDT
* 在 DFYN 上将 50% 的 USDT 兑换成 UST
* 在 DFYN 上创建新的 USDT-UST LP 对
* 在 Augury 上存入新的 LP 代币

### 每周例行

此外，你将获得 每周BAL 奖励（来自你在 Balancer 上的 Qi 存款）和 Qi 代币（来自金库奖励）。你不得不

* 将 Qi 代币存入 Balancer
* 将 BAL 代币存入 Mai Finance 的 BAL 金库
* 从你额外的 BAL 存款中借用 MAI，并将它们转换为 USDT-UST 对，在 Augury 上进行农场

### **月复一月的原始结果**

| 月份 | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| -- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1  | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2  | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3  | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4  | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5  | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6  | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7  | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8  | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9  | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10 | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11 | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12 | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

一些注意事项：

* USDT-UST 池的增长是从金库借入额外 MAI 的唯一结果
* 由于 Curve 上存入的 USDC 数量非常少，CRV 池几乎不存在
* BAL 金库并不重要，因为 Balancer 奖励的 14.28% 以 BAL 代币支付，其余以 Qi 代币支付
* Balancer池中的数量是最大的收益，只是Vault奖励和Balancer奖励的结果

### 第365天

一整年后，我们投资的最终状态将是

| 头寸          | 美元价值     |
| ----------- | -------- |
| USDT-UST    | 553.24   |
| atricrypto3 | 36.20    |
| Balancer    | 137.62   |
| camWBTC     | 47.45    |
| camWETH     | 1,029.19 |
| camWMATIC   | 14.39    |
| LINK        | 11.84    |
| CRV         | 0.017    |
| BAL         | 3.93     |

总债务实际上是整个 USDT-UST 头寸，因此为 553.24 美元，产生的总奖励为 280.63 美元，对应于最终的 APY 为 28.06%。

### **与其他策略的比较**

在稳定代币农耕中获得 28% 的 APY 并不算太糟糕，但是与我们可以用初始价值 1,000 美元的 ETH 应用的其他更简单的策略相比，这如何？让我们检查以下策略的最终 APY

* 通过 AAVE 杠杆amWETH 8 次：为此，我们将使用[利用你的 Aave 市场代币](leverage-aave-tokens.md)中描述的确切流程。
* Augury 上完全稳定的农耕：对于此策略，我们在 Augury 上以相同的输注出售 WETH 和价值 1,000 美元的 USDT-UST
* QuickSwap 上完全稳定的耕作：对于此策略，我们将使用 camWETH 金库从金库奖励中受益，并在 QuickSwap 上耕作价值 500 美元的 MAI（MAI-DAI，APY 为 19.78%），使用 Mai Finance 上的 dQUICK 金库借入额外的 MAI 并重新投资到农耕池中（dQUICK 金库的 APR 为 55.72%）

| 策略                       | 最终APY  |
| ------------------------ | ------ |
| 本指南中介绍的策略                | 28.06% |
| 杠杆 AAVE 代币 8 X           | 46.46% |
| 在Augury上只有稳定的农耕          | 22.53% |
| Quickswap 农耕 + dQUICK 金库 | 35.96% |

## 免责声明

这个策略真的很有趣，并且使用了 Mai Finance 的大部分保险库，编写本指南主要是为了展示，截至 2021 年 9 月，这是在耕作稳定币时会产生更多奖励的部分。但是，这种策略可能不是最有趣的一种，并且涉及对数个平台的大量操作。最后，Augury 是一个极出色的工具，可以生成可以包含在多种策略中的特定代币，但可能不仅仅是稳定的农耕。作为旁注，在计算最终 APY 时，没有考虑存款费用或绩效费用。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
