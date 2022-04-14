---
description: >-
  本指南将介绍一项策略，凸显在 Mai Finance 和 QuickSwap 上推出新的 LP 池后，Mai Finance、QuickSwap 和
  Adamant 之间惊人的互动。
---

# 耕种还是质押？或两者？



![](../../.gitbook/assets/screen-shot-2021-09-03-at-9.24.12-am.png)

## 简介

当你使用 DeFi（去中心化金融）应用程序时，尤其是当你耕种收益时，你最终会得到农场授予的一堆原生代币。如果大多数人只是为了购买更多或他们最喜欢的代币而出售这些代币，为了增加收入，我们将展示能实际的保留和使它们投入工作一些方法。

为了这么做，我们将使用 2021 年 9 月初在 QuickSwap 上推出的新 LP 池（流动性提供池），它们使用来自 Mai Finance 的 Qi 代币。如果你需要很好地了解 QuickSwap 和 Adamant 应用程序是什么，请阅读 [Stacking DApps guide](stack-dapps-like-lego-bricks.md).

## **应用程序和池演示**

### 耕种方面

为了最大化我们的收益，我们将使用 3 种不同的应用程序

* Mai Finance
* QuickSwap
* Adamant

我们还将使用以下 LP 池

* Qi/MATIC on Mai Finance 生成 Qi
* QuickSwap 上的 Qi/WETH 生成 QUICK 和 ADDY
* Qi/QUICK on Adamant 生成 ADDY 和 MATIC

你已经可以看到，每个应用程序都在生成代币，这些代币可以为其他应用程序上使用的其他池提供资源。这个想法是将在 Mai Finance 上获得的 Qi 代币与在 QuickSwap 上获得的 QUICK 代币结合使用，并在 Adamant 上使用这两个。Adamant 将生成 ADDY 代币，让你可以领取 MATIC 股息。 MATIC 代币可以锁定在 WMATIC 金库中的 Mai Finance 以借入 MAI，然后买 MATIC 和 WETH，然后我们可以将其与 Qi 代币一起用于增加你在 Mai Finance 和 QuickSwap 的头寸。

### 质押方面

你还需要知道Mai Finance和QuickSwap上产生的多余代币是可以抵押的：

* Mai Finance 和QuickSwap上的Qi可用于对 QIP（QiDAO Improvement Proposals）进行投票。
* 在Mai Finance上的Qi可以被锁定。如果你锁定你的 Qi，你就有资格获得以 Qi 支付并在每周三分发的协议股息。很快就会有关于 Qi 抵押的更多细节。
* QuickSwap 上的 QUICK 也可以质押以在 Dragon's Lair 中生成额外的 QUICK 代币。
* 锁定的 QUICK (dQUICK) 也可用于 QuickSwap 以生成 Dragon's Syrup 中的其他代币，我们将使用的是生成 ADDY 代币的农场。
* Adamant 上的 ADDY 自动归属（锁定 90 天），但会产生 WMATIC 分红。
* 还可以锁定 Adamant 上的 ADDY，以提高你在网站上输入的池的 APR/APY（年度百分比奖励/年度百分比收益），以及产生更多ADDYs，并提高你的MATIC股息。

## 引导系统

![](../../.gitbook/assets/screen-shot-2021-09-08-at-6.54.08-am.png)

以下是对初始投资价值 1,000 美元的 Qi/MATIC 和 Qi/WETH LP 代币进行的模拟，以及不同平台在 2021 年 9 月 9 日给出的当前 APR/APY。这不是我们上述描述内容的真正运用。费率会有所不同，代币价格会有所不同，一些程序会结束等等……因此，最终结果只是对如果一切保持稳定你可以获得的结果的估计，但情况永远不会如此。

### 第1天

{% hint style="info" %}
**注意：**本指南中使用的池在发布前几个小时上线。 APR 和 APY 显然不会保持不变，几天后将对文档进行一些修订。请 DYOR 并谨慎使用指南。
{% endhint %}

由于我们有价值 500 美元的 Qi/MATIC LP 代币和 500 美元的 Qi/WETH LP 代币，我们会将它们存入 Mai Finance 和 QuickSwap。作为旁注，如果你对Qi 或 QuickSwap有偏好，你可以简单地将更多 LP 代币放在一个或另一个平台上，以生成更多你最喜欢的代币并质押更多。对于我们的示例，我们将坚持严格的 50% 拆分。

* 500 美元的 Qi/MATIC 将在 Mai Finance 上，年利率为 1160.65%
* 500 美元的 Qi/WETH 将在 QuickSwap 上进行，年利率为 1817.44%

我们还将在其余的模拟中使用以下 APR

* Dragon's Lair 的 dQUICK APR 为 17.28%
* Dragon's Syrup 的 ADDY APR 为 17.08%
* 自动复合 LP 代币在 Adamant 上的 Qi/QUICK APR 为 133%
* ADDY 代币在 Adamant 上的 Qi/QUICK APR 为 131%
* Adamant 上的 WMATIC APR 是锁定的 ADDY 代币的 35%

由于Mai Finance的APR低于 QuickSwap，我们将使用Mai Finance产生的 Qi 的 100% 来生成额外的 Qi/QUICK 代币（不出售，而是与 QuickSwap 上收到的 QUICK 代币结合），这意味着在一天结束时，我们还剩 0 Qi。当然，如果你以不同的方式平衡初始投资，你可以获得剩余的 Qi 和 0 QUICK。

因此，在第一天结束时，在我们的投资组合里有

| 奖励类型               | 美元的价值  |
| ------------------ | ------ |
| QuickSwap上的 dQUICK | 8.997  |
| QuickSwap上的ADDY    | 0      |
| Adamant上的Qi/QUICK  | 31.799 |
| Adamant上的ADDY      | 0      |
| Adamant上的WMATIC    | 0      |

### 第2天

在第 2 天，存入 QuickSwap 的 Dragon's Syrup 的 dQUICK 开始生成 ADDY 代币，以及 Adamant 上的 Qi/QUICK LP 对。在第 2 天结束时，我们将得到

| 奖励类型              | 美元的价值  |
| ----------------- | ------ |
| QuickSwap上的dQUICK | 17.998 |
| QuickSwap上的ADDY   | 0.0042 |
| Adamant上的Qi/QUICK | 63.713 |
| Adamant上的ADDY     | 0.114  |
| Adamant上的WMATIC   | 0      |

为了开始产生 WMATIC 股息，不要忘记每天在 Adamant 上领取你的奖励！

### 第3天

在第 3 天，在 Adamant 上收集的 ADDY 代币将开始产生 WMATIC 股息。这意味着在第 3 天结束时，我们将进入我们的投资组合

| 奖励类型              | 美元的价值  |
| ----------------- | ------ |
| QuickSwap上的dQUICK | 27.004 |
| QuickSwap上的ADDY   | 0.025  |
| Adamant上的Qi/QUICK | 95.743 |
| Adamant上的ADDY     | 0.343  |
| Adamant上的WMATIC   | 0.0001 |

从第 4 天开始，我们将能够

* 收集 WMATIC 股息
* 将WMATIC的一部分存入Mai Finance，并以此为抵押借款Mai
* 卖掉MAI 购买更多 WETH
* 将剩余的 MATIC 与 Qi 配对，并将 WETH 与 Mai Finance 上产生的更多 Qi 配对
* 将额外的 Qi/WMATIC 对存入 Mai Finance 并将 Qi/WETH 对存入 QuickSwap

到这时，农耕系统已完全准备就绪，我们可以开始估算收入。

## 农耕的结果

### 每日例行

每日例行由以下交易组成

* 在Mai Finance 上收获Qi
* 在 Adamant 上收获 WMATIC
* 将 66% 的 WMATIC 存入Mai Finance
* &#x20;借 MAI 支付 50% 的存款
* 将 MAI 互换成 WETH
* 在 QuickSwap 上创建 Qi/WMATIC 对
* 将 Qi/WMATIC 存入Mai Finance
* 在 QuickSwap 上创建 Qi/WETH 对
* 将 Qi/WETH 存入 QuickSwap
* 在QuickSwap上收获Quick
* 在 QuickSwap上创建 Qi/QUICK 对
* 将剩余的 QUICK 存入 Dragon's Lair
* 将 dQUICK 存入 Dragon's Syrup
* 从 Dragon's Syrup 中收获 ADDY 代币
* 从 Adamant 收获 ADDY 代币
* 在 Adamant 上存入新的 Qi/QUICK
* 将收获的 ADDY 存入到 Adamant（已锁定）



### 月复一月的原始结果

| 月份 | dQUICK    | Qi/QUICK   | ADDY       | Qi/MATIC  Qi/WETH |
| -- | --------- | ---------- | ---------- | ----------------- |
| 1  | $280.96   | $1,040.78  | $54.97     | $0.91             |
| 2  | $557.79   | $2,162.98  | $224.36    | $7.89             |
| 3  | $842.08   | $3,413.73  | $521.09    | $27.85            |
| 4  | $1,138.60 | $4,816.62  | $960.17    | $68.48            |
| 5  | $1,454.30 | $6,405.18  | $1,559.60  | $138.44           |
| 6  | $1,798.77 | $8,224.86  | $2,341.64  | $247.49           |
| 7  | $2,184.58 | $10,335.38 | $3,334.13  | $406.84           |
| 8  | $2,627.76 | $12,813.60 | $4,572.23  | $629.47           |
| 9  | $3,148.40 | $15,757.01 | $6,100.39  | $930.60           |
| 10 | $3,771.42 | $19,288.05 | $7,974.83  | $1,328.32         |
| 11 | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31         |
| 12 | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79         |

### 第365天

一整年后，我们投资的最终状态将是

| 奖励类型                  | 美元的价值     |
| --------------------- | --------- |
| QuickSwap上的dQUICK     | 5,628.29  |
| QuickSwap上的ADDY       | 365.25    |
| Adamant上的Qi/QUICK     | 29,733.58 |
| Adamant上的ADDY         | 13,587.56 |
| 附加的Qi/MATIC + Qi/WETH | 2,631.07  |

请注意，通过 QuickSwap 农场生成的 ADDY 并没有每天收获并添加以在此模拟中提高 Adamant 的 ADDY 奖励（它已经足够复杂了）。此外，我们只考虑既定的 ADDY。在最初的 90 天归属期后，如果你认领 ADDY 代币并锁定它们，你将提升你的 ADDY 奖励，并产生更多的 WMATIC。

最后，一年后，产生的收入价值 51,580.50 美元。如果我们考虑初始投资为价值 1,000 美元的 Qi/MATIC 和 Qi/WETH，则最终的 APY 为 5,087.39%。

## 免责声明

本指南绝对不是财务建议，它是出于教育目标而制作的。 目标不是提出可以盲目遵循的秘方，因此请做好功课和自己的模拟，并且只投资你准备好可能会失去的东西。你需要注意价格变化、供需、奖励计划结束日期、无常损失等......

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
