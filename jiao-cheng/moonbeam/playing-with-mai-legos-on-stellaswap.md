---
description: 在 Moonbeam 上使用 MAI 通过 StellaSwap 赚取收益。
---

# 在 StellaSwap 上玩 MAI 乐高积木

虽然 Mai Finance 不在 Moonbeam 上提供金库，但可以通过使用 Stella\_S\_wap 的新 MAI 库，使用链上一些你最喜欢的代币来铸造 MAI。通过利用你的抵押代币并借用 MAI，你可以通过涉及 xSTELLA 和 MAI 的循环策略获得丰厚的收益。

注意：本指南不作为财务建议。它的创建考虑到了教育目标。本指南的目的不是提出盲目遵循的策略，所以请做好功课和自己的模拟，只投资你准备好可能失去的东西。

[StellaSwap](https://stellaswap.com/) 是 Moonbeam 上领先的 DEX（去中心化交易所）。作为功​​能齐全的 DEX，StellaSwap 为用户提供了交换代币、在农场赚取收益以及参与协议治理的能力。让 StellaSwap 与众不同的是，它是第一个允许用户通过与 Mai Finance 合作直接从其界面本地铸造 MAI 的协议。

![Mint MAI 直接来自 StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### 在 StellaSwap 上铸造 MAI

Unlike MAI vaults on Mai Finance, StellaSwap's MAI vaults do charge interest for borrowing against your assets. Currently, users can borrow MAI against xStella, StellaSwap's revenue sharing staked token, at 12% interest, or against wGLMR, a wrapped version of Moonbeam's native gas token, at 8% interest. While users familiar with Mai Finance's 0% interest vaults might be taken aback by the higher interest rates, we'll go through a looping strategy in this guide to allow you to earn high yields on your borrowed stablecoins without ever leaving StellaSwap.

![StellSwap 上的 vaults](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. 首先，前往 StellaSwap 的 [MAI minting facility](https://app.stellaswap.com/mai).&#x20;
2. 从这里你将能够创建一个 xStella 或 wGLMR vault来借用 MAI。为了创建我们的循环策略，我们将创建一个 xStella vault。
3. 现在进入你新创建的vault并存入 xStella。请注意，xStella vault有 40% 的 LTV（贷款价值比），这意味着每价值 100 美元的 xStella，你将能够借入价值 40 美元的 MAI。
4. 接下来，你需要前往借阅部分，借阅 MAI。请记住你的 LTV 以避免被清算。

![xStella vault](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### 把乐高积木放在一起

现在你已经成功借用了 MAI，是时候使用它了！我们将利用我们的 MAI 将其存入 StellaSwap 的 MAI-Base4Pool 稳定币农场，并使用收益通过质押来赚取更多 Stella 代币。永远记住，如果你输入此策略，你将自担风险，如果你不进行尽职调查，你的vault可能会被清算！\
\
让我们首先在 StellaSwap [Farms](https://app.stellaswap.com/farm) 页面上找到 MAI-Base4Pool。

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

该农场目前提供非常有吸引力的 26% 稳定币收益率，其池由 MAI、FRAX、USDT、USDC 和 DAI 组成，收益率以 Stella 代币支付。请注意，该收益率主要抵消了我们目前为借入的 MAI 支付的利息（12%）。我们可以看看到目前为止我们的表现：

$$effective interest = (collateral * borrow interest)-(mai*farmingyield)$$

这为我们提供了 1.6% 的有效收益率来借入 MAI - 不错，但我们可以做得更好。我们现在可以拿走我们在 MAI-Base4Pool 中赚取的 Stella 代币，并将它们[质押以接收 xStella](https://app.stellaswap.com/xstella)。

![质押 xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

质押 xStella 有两个额外的好处。首先，它提供了 70% 的 Staking APR，从而增加了我们的收益，但更重要的是，随着用户之间共享来自协议的掉期收入，xStella 的价值会随着时间的推移而增加。这意味着我们在稳定币农场中相对安全的位置所获得的任何收益都在不断增加。然后，我们可以使用这些额外收益将额外的 xStella 存入我们的vault以增加我们的 LTV，或借用额外的 MAI。

## 免责声明

本指南不是财务建议，应仅被视为一种教育工具。总是做自己的研究。本指南中对项目的讨论不应被视为对该项目的认可。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
