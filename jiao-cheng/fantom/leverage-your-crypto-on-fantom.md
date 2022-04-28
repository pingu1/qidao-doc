---
description: 本指南建议对 Mai Finance 在 Fantom 上使用 Yearn vaults和 Beefy vaults提出的不同杠杆选项进行完整分析。
---

# 在 Fantom 上杠杆你的加密货币

## 介绍

Mai Finance 在 Fantom 上推出了具有多种不同vault类型的借贷平台，使你可以根据你将存放在vault中的资产来铸造 MAI 稳定币。这个想法是，你将能够保留你的加密货币并从它们的价格升值中受益，同时仍然能够以高 APR 购买其他代币和农场产量。如果你用你的贷款购买更多你已经存入的相同资产，这就是所谓的杠杆你的代币。我们将使用 Fantom 上的 2 个不同借贷平台向你展示该策略的好处，以杠杆我们的 DAI 代币。

## 利用你的 Yearn Vault 代币

### 将你的资产存入 Yearn Finance

[Yearn Finance](https://beta.yearn.finance/#/home) 是一组在以太坊主网和其他区块链上运行的协议，允许用户通过借贷和交易服务优化他们在加密资产上的收益。在 Fantom 上，我们将使用的产品是Yearn Finance的vaults。这是一个接受单一代币存款的工具，将使你从这笔存款中获得收益。作为存款证明，你将收到一个 yvToken。在我们的例子中，我们将存入 DAI 并获得 yvDAI 作为交换。

![在Fantom 网络上的Yearn vaults](../../.gitbook/assets/ftm-leverage-yv1.png)

{% hint style="info" %}
yearn finance在 Fantom 上仍处于测试模式。团队仍在平台上工作，APR/APY 没有显示。如果你前往 Iron Bank 选项卡，这是 yearn 平台上的借贷协议，你会看到借贷 DAI 的年利率约为 8%。请自行承担投资风险。
{% endhint %}

### 将你的 yvToken 存入 Mai Finance

一旦你将你的 DAI 存入了 yearn Finance，你的钱包里应该有 yvDAI。这就是我们所说的具有收益的代币：它本身没有任何价值，但代表了你在资产池中的份额，你的资产在该池中获得收益，并且奖励自动复利。换句话说，如果你的 DAI 的价值没有因为 DAI 与美元挂钩而发生变化，那么你的 yvDAI 代币的基础价值无论如何都会增加。

Mai Finance 接受许多不同的收益代币作为抵押品，包括 yvDAI。你现在可以存入此代币并借用 MAI。

![将你的 yvToken 存入 Mai Finance](<../../.gitbook/assets/ftm-leverage-yv2 (1).png>)

yvDAI vault的清算门槛为 110%，这意味着你可以借入 MAI，使你的抵押品价值与债务价值之间的比率为 110%。请注意，110% 实际上是你的vault将被清算的比率。你需要将比率保持在此最小阈值之上。由于 DAI 的价格变化不大（上下波动小于几美分），因此可以保持 115% 的“安全”CDR（抵押债务比率），但可以随意保持更高的水平。

与往常一样，要根据抵押品的价值和我们想要获得的目标 CDR 来计算我们可以获得的贷款价值，我们将使用以下公式：

$$
MAI_{available} = \frac{Collateral_{value} - Debt_{value} * Target_{CDR}}{Target_{CDR}}
$$

​抵押价值为 100 美元且没有债务，如果我们想保持 115% 的健康 CDR，我们最多可以借到

$$
MAI_{available}=\frac{100-0*1.15}{1.15}=86.95
$$

​​你现在的位置是，你的 DAI 收益存在于 Yearn vault中，并且你还可以使用一些 MAI 稳定币。由于我们想杠杆我们的 DAI 头寸，我们现在将我们的 MAI 换成更多的 DAI。

### 在 BeethovenX 上交换你的 MAI

在 Fantom 上，MAI 的主要流动性来源是 BeethovenX。这是你可以将你的 MAI 代币换成更多 DAI 用于我们的策略的主要场所。

![用 MAI 交换更多 DAI](../../.gitbook/assets/ftm-leverage-yv3.png)

这是我们循环的最后一步。现在你有更多的 DAI，你可以将它们存入 Yearn vault并重复循环。这样做会增加你在 Yearn vault中的资产数量，这意味着你将通过在该平台上借出 DAI 来获得更多奖励。 APR/APY 保持不变，但因为你拥有更多资产，你可以获得更多收益，如果你与初始投资相比，增加的是你的 APR。如果你想获得更多关于使用 yvDAI 循环可以实现什么 APR 的示例，请阅读我们的 Polygon [camDAI 代币指南](../polygon/camdai-beginner-strategy.md#main-strategy)，该指南使用完全相同的策略但不同的工具。

{% hint style="success" %}
BeethovenX 实际上是一个利用你借来的 MAI 来种植产量的绝佳机会。如果你无法使用杠杆循环获得更好的年利率，只需将你的 MAI 存入 MAI-DAI-USDC 池（截至 2021 年 11 月，年利率约为 30%）。
{% endhint %}

$$
MAI_
$$

## 在 Mai Finance 上利用你的mooScreamTokens

### 将你的资产存入 Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) 是一个去中心化的多链收益优化器平台，允许其用户从其持有的加密货币中赚取复利。换句话说，你可以在 Beefy Finance 上从其他平台存入一些资产或 LP 代币，让自动复合机收获农场代币并将它们复合成你存入的更多资产/LP 代币。例如，我们将在 Beefy 上使用单个 DAI 存款，并使用 Scream 作为底层平台。 Scream 是 Fantom 网络上的一个 Compound fork，你可以在该网络上借出你的资产并收集 SCREAM 代币。然后，Beefy 将出售 SCREAM 代币以获得更多 DAI。

要存入我们的 DAI，我们将访问 Beefy Finance 应用程序并选择 Scream 作为我们将在其上耕种产量的平台。你还可以添加 DAI 过滤器以获得直接 DAI 存款。

![使用 Scream 将 DAI 存入 Beefy](../../.gitbook/assets/ftm-leverage-beefy1.png)

如你所见，Beefy 已经在 DAI 单笔存款上提供了令人难以置信的 APY。将 DAI 存入 Beefy 后，你的钱包中应该有 mooScreamDAI 代币形式的存款证明。至于 yvDAI 代币，mooScreamDAI 代币是一种收益押金，这意味着你的资产仍然在 Scream 上使用并在 Beefy 上复利，赚取收益。但是你可以在 Mai Finance 上使用此代币向他们借 MAI。

### 将你的 mooScreamToken 存入 Mai Finance

一旦你将你的 DAI 存入了Yearn Finance，你的钱包里应该有 mooScreamDAI。你可以使用与上述 Yearn Vault 策略完全相同的步骤，唯一的区别是 mooScreamDAI 清算率为 135%。由于 DAI 是一种稳定币，因此仍然可以借用 MAI 并保持 CDR 非常接近清算比率。例如，我们的目标是 140% 的 CDR，使用与上述相同的公式，我们可以计算出我们可以用价值 100 美元的 DAI 铸造的 MAI 数量。

$$
MAI_{available}=\frac{100-0*1.4}{1.4}=71.43
$$

​由于我们借用更少，我们将能够执行更少的循环，最终等效的 APY 也会更低，但这仍然是一个不错的初学者策略。&#x20;

循环的其余部分与 yvDAI 相同，这意味着你必须在 BeethovenX 上将你的 MAI 换成 DAI 并重复直到你满意为止。

## 关于杠杆策略的一些说明

杠杆 DAI 被认为是一种初学者策略，因为它的风险很小（你使用的是稳定币），并且你最多可以使用 3 个协议获得一些不错的收益。但是，仍然存在一些风险。

### 清算风险

你将执行的循环越多，清算风险就越高。事实上，即使 DAI 价格的微小变化也会被你应用的杠杆放大，即使你将 CDR 保持在清算比率之上 5 个点，你的金库也可能面临风险。在你将资产存入 MAI 融资并且不借入额外的 MAI 以保持更好的 CDR 的步骤中停止杠杆循环始终是一个好主意。

此外，在清算的情况下，由于你在 MAI Finance的vault中包含更多资产，清算也会比你没有杠杆头寸产生更大的影响，因为你必须偿还的债务也更大.

### 技术风险

如果你在投资乐高积木中使用了很多协议，则需要确保这些协议是安全的。事实上，在我们的杠杆策略中，如果单个协议被黑客入侵，整个策略可能会崩溃。在投资 DeFi 项目之前，请务必进行尽职调查。

### 达到债务上限

由于这些策略易于设置且风险低，因此对它们的需求非常高。但是，你肯定注意到在杠杆过程中，借来的 MAI 被交换为 DAI（或其他代币）。如果在Beethoven上卖出过多的 MAI，其价格将缓慢下降，并且 MAI 存在失去挂钩的风险，这对于稳定币来说是非常不利的。为了让价格有时间稳定下来，Mai Finance有安全机制，最重要的是每个金库的债务上限。

债务上限表示可以为给定vault铸造的最大 MAI 数量。一旦达到上限，就不能再借 MAI。然后负责 MAI finance的核心团队可以决定提高上限或多等一点，以获得更好的 MAI 价格。

你可以随时在[vault创建页面](https://app.mai.finance/vaults/create)上验证可以铸造的 MAI 数量，但如果你收到以下错误消息，你通常会注意到没有更多的 MAI：

![达到债务上限时收到错误消息](../../.gitbook/assets/ftm-leverage-error.png)

即使你的健康因素正确，也会出现此错误消息。在大多数情况下，等待上限提高是唯一的解决方案。密切关注 twitter 或 Discord 以了解何时发生这种情况。

## 免责声明

本指南介绍了你可以在 Fantom 上使用资产并将 Mai Finance 纳入你的策略以增加收益的一些方法。但是，像往常一样，本教程不是财务建议，你应该在应用投资策略之前始终 DYOR，并以负责任的方式进行投资。

另请记住，此解决方案可能不是最佳策略，具体取决于你计划何时使用它。我们刚刚强调，BeethovenX 也为你的 MAI 提供了非常有趣的 APR，你还可以使用 Beefy Finance 将 BEETS 奖励复合成更稳定的硬币。

{% hint style="info" %}
请记住，在给定时间运作良好的策略可能在其他时间表现不佳（或让你赔钱）。请随时了解情况，监控市场，密切关注你的投资，并一如既往地进行自己的研究。
{% endhint %}
