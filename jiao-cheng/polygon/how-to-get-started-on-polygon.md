---
description: 在本指南中，我们将解释您需要了解的一切，以便开始使用在 Polygon 区块链上的不同的DApp。
---

# 如何开始使用Polygon

## **什么是Polygon？**

Polygon 网络是建立在以太坊区块链之上的网络，但它旨在解决以太坊主网的可扩展性问题。平均而言，Polygon 网络上一笔交易需要 3 到 5 秒，成本只有几分之一，可以让一个人每天用一个非常小的钱包进行数十笔交易。

Polygon也是第一个推出的“侧链”之一，与其他可用的链相比，Polygon 有一点先进性，它设法收集了：

* 不断增加的用户群
* 应用的不断增加
* 扎实的TVL目前稳定在40亿美元左右

Polygon 还设法建立了信任，并被证明是以太坊网络的可靠替代品，向愿意尝试去中心化金融的小型投资者打开了 DeFi 世界，而无需花费数百美元的交易费用。凭借这种信任和易用性，许多公司转向 Polygon来促进资产从一个网络桥接到另一个网络，增加安全性和匿名性，最终实现网络更强大。

## **创建钱包**

在使用 Polygon 区块链之前，你需要创建一个钱包地址，有不同的钱包类型、**软件**（Metamask、TrustWallet...）**和硬件（**Trezor 或 Ledger）。但是，在本指南中，我们将使用 _Metamask_ 来解释如何访问 Polygon 区块链。

### 下载 Metamask

要使用 Polygon 区块链你需要完成的第一步是在 Web 浏览器中下载 Metamask 扩展。你可以在他们的[网页](https://metamask.io/index.html)上下载。 Metamask 也可用于 iOs 和 Android 设备。

一旦你这样做了，你的浏览器上应该会有一个带有 Metamask 标志的扩展程序。当你第一次打开 Metamask 扩展时，它会问你是否有 Metamask 账户，如果有，你需要写你要加载的帐户的**种子短语**\*\*（稍后我们将谈到种子短语的重要性）。如果你没有帐户，则必须创建一个新帐户。这些是你需要遵循的步骤：

1. 首先，你需要为你的 Metamask 帐户选择一个密码。
2. 然后你应该观看关于如何保护你的钱包和种子短语重要性的视频。
3. 你会看到你的种子短语。创建新钱包时，你的种子短语是最重要的事情，因为如果你丢失种子短语并且计算机坏了，你将无法访问你的 Metamask 帐户。所以请小心你的种子短语，不要与任何人分享。

完成后，你应该会在浏览器上看到以下内容：

![ Metamask界面](<../../.gitbook/assets/image (18).png>)

### **添加Polygon Blockchain**

正如你在上图中看到的，我们使用的是Ethereum Mainnet，但是如果我们单击那里更改为不同的网络，你会看到 Polygon Mainnet不在那里。不用担心，我们需要做的是手动添加Polygon Mainnet，为此，你需要单击Custom RPC并编写以下内容：

![](<../../.gitbook/assets/image (20).png>)

一旦你完成后，你几乎可以在 Polygon Blockchain上使用 Metamask 钱包了，剩下的唯一一步是将Ethereum Mainnet切换到 Polygon Mainnet，为此你需要单击 Metamask extension顶部的下拉菜单。

## **获得免费 MATIC**

现在你已设置好使用 Polygon Blockchain的所有内容，但是你的钱包中没有任何 MATIC，因此你无法在 Polygon Blockchain上进行任何交易。交易基本上是 2 个地址之间的交换，需要一些时间来处理（这是由 Polygon 拥有的不同验证器完成的）并且有费用（该费用也称为 gas 并使用 MATIC 代币支付）。

幸运的是，此[页面](https://matic.supply)为你提供免费 MATIC 以在 Polygon 网络上进行你的第一笔交易（这些类型的页面可以称为水龙头）。你唯一需要做的就是将你的钱包连接到该页面并完成验证码。这些 0.002 MATIC (\~0,00223$) 将允许我们使用Polygon网络进行一些交易。

![获得免费 MATIC](<../../.gitbook/assets/image (23).png>)

有时由于网络拥塞，你在使用此页面时可能会遇到一些问题，因此只需稍等片刻，你就可以索取一些免费的 MATIC。此外，你可以尝试使用这个，以防另一个不起作用。

在我们进入文章的下一部分之前，你需要意识到这些水龙头不是供人们排水的。如果你的钱包有太多的 MATIC，它不会为你送达任何东西，或者如果你尝试在 24 小时内进行索取超过几次。所以，请小心，不要自私。

## **在 Metamask 中添加代币**

现在你的 Metamask 中有一些免费的 MATIC，你已准备好使用 Polygon 有的不同 DApp 和代币。你可以复制你想要用[PolygonScan](https://polygonscan.com) 使用的代币的地址。你到达那里后，你只需要写下你要添加的代币的名称。例如，如果我们在 Polygon 上搜索 QiDAO，我们将得到：

![在PolygonScan 上编写 QiDAO 的结果](<../../.gitbook/assets/image (24).png>)

现在，你需要复制合约的地址并在 Metamask上单击Add token。

![在 Metamask 上添加 Qi](<../../.gitbook/assets/image (25).png>)

## **如何在 Polygon 上购买代币**

现在我们已经准备好了我们的Metamask以及一些 MATIC来 支付 gas，我们可以开始在 Polygon 网络上购买一些代币。这么做，你需要使用 **DEX**（去中心化交易所），你可以选择很多 DEX，例如 [_Quickswap_](https://quickswap.exchange/#/swap)、[_Slingshot_](https://app.slingshot.finance/trade/m/MATIC/USDC)、[_Dexguru_](https://dex.guru)、[_Sushiswap_](https://app.sushi.com/swap) 等。

一旦你决定了你想要使用哪个 DEX，你就可以开始在 Polygon Blockchain上购买你最喜欢的代币。

![使用 Quickswap 购买 Qi 代币](<../../.gitbook/assets/image (26).png>)

{% hint style="info" %}
当你想购买代币时有另一个有趣的 DApp 是 [Zapper](https://zapper.fi/es/exchange)。 Zapper 理论上会搜索最便宜的平台来执行两个代币的互换，因此这是节省一些 MATIC 的好方法。
{% endhint %}

## 检查你的钱包历史记录

I了解如何查钱包历史记录很重要，这么做，你可以使用 [DeBank](https://debank.com)。 Debank 将允许你检查你在 Metamask 帐户中进行的不同交易，以及检查你使用的所有区块链上的投资组合或你拥有的 NFT 。如果你想比较的话这将会非常有用，例如，在质押一些Qi的期间你收到的不同的空投Qi。

![在我们新的 Metamask 地址中进行的所有交易](<../../.gitbook/assets/image (27).png>)

正如你所看到的，我的钱包里有 800,000 个 DxDex.io，但我没有做任何事情来让我的钱包里得到这些代币。你需要意识到这些类型的骗局，并且永远不要与你不知道的任何硬币互动。万一你授予他们访问权限，Debank 将允许你撤销它。请小心，如果你不知道那个代币，请不要触摸它。

## 有用的链接

以下是你在使用 Polygon Blockchain时可能会发现有用的一些链接：

* [Quickswap](https://quickswap.exchange/#/swap)
* [AAVE](https://app.aave.com)
* [PolygonScan](https://polygonscan.com/gastracker/): 此链接将有助于看 Polygon 网络上的 gas 价格。

## **免责声明**

本指南绝对不是财务建议，它是出于教育目标而制作的。

{% hint style="info" %}
请牢记在给定时间运行良好的策略可能在另一个时间表现不佳（或让你赔钱）。请保持消息灵通，监测市场，留意你的投资，并一如既往地，做你的研究。
{% endhint %}
