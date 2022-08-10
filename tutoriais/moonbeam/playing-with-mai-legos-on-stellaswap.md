---
description: Usando MAI na Moonbeam para gerar rendimentos com a StellaSwap.
---

# Brincando de LEGO na StellaSwap

While Mai Finance does not offer vaults on Moonbeam, it is possible to use some of your favorite tokens on the chain to mint MAI by using Stella\_S\_wap's new MAI vaults. By leveraging your collateral tokens and borrowing MAI against it, you can earn great yield through a looping strategy involving xSTELLA and MAI.&#x20;

_NOTE: This guide is not meant as financial advice. It was created with an educational goal in mind. The goal of this guide is not to propose a strategy to be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose._

[StellaSwap](https://stellaswap.com/) is the leading DEX (decentralized exchange) on Moonbeam. As a full-featured DEX, StellaSwap offers users the ability to swap tokens, earn yield on farms, and participate in protocol governance. What sets StellaSwap apart, is that it is the first such protocol that allows users to mint MAI natively directly from its interface through a partnership with Mai Finance.

![Mint MAI directly from StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### Minting MAI on StellaSwap

Unlike MAI vaults on Mai Finance, StellaSwap's MAI vaults do charge interest for borrowing against your assets. Currently, users can borrow MAI against xStella, StellaSwap's revenue sharing staked token, at 12% interest, or against wGLMR, a wrapped version of Moonbeam's native gas token, at 8% interest. While users familiar with Mai Finance's 0% interest vaults might be taken aback by the higher interest rates, we'll go through a looping strategy in this guide to allow you to earn high yields on your borrowed stablecoins without ever leaving StellaSwap.

![Vaults on StellSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. First, head off to StellaSwap's [MAI minting facility](https://app.stellaswap.com/mai).
2. From here you'll be able to create an xStella or wGLMR vault to borrow MAI against. To create our looping strategy, we will create an xStella vault.
3. Now enter your newly created vault and deposit xStella. Please note that xStella vaults have a 40% LTV (loan to value ratio) which means that for every $100 worth of xStella, you will be able to borrow $40 worth of MAI.
4. Next, you'll want to head to the borrow section, and borrow MAI. Please keep in mind your LTV to avoid being liquidated.

![xStella vault](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### Putting the legos together

Now that you've successfully borrowed MAI, it's time to put it to use! We'll be leveraging our MAI by depositing it into StellaSwap's MAI-Base4Pool stablecoin farm and using the yields to earn more Stella tokens by staking them. Always remember that if you enter this strategy you do so at your own risk and your vault may be liquidated if you do not do your due diligence!\
\
Let's first find the MAI-Base4Pool on the StellaSwap [Farms](https://app.stellaswap.com/farm) page.

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

This farm currently offers a very attractive 26% yield on stable coins with a pool comprised of MAI, FRAX, USDT, USDC, and DAI with a yield paid out in Stella tokens. Note that this yield is mostly offsetting the interest we are currently paying on our borrowed MAI (12%). We can take a look at our performance so far:

$$effective interest = (collateral * borrow interest)-(mai*farmingyield)$$

This gives us an effective yield of 1.6% to borrow MAI - not bad, but we can do better. We can now take the Stella tokens we are earning from being in the MAI-Base4Pool and [stake them to receive xStella](https://app.stellaswap.com/xstella).

![Staking xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

Staking xStella has two additional benefits. First, it provides a staking APR of 70%, thereby compounding our yields, but more importantly, xStella increases in value over time as swap revenue from the protocol is shared among users. This means that any yields we are earning from our relatively safe position in a stablecoin farm, are continuously increasing. We can then use these additional yields to deposit additional xStella into our vault to increase our LTV, or to borrow additional MAI against it.

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
