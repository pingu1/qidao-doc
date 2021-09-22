---
description: >-
  Getting a good understading about how MAI works is crucial for any investor
  that really wants to understand Mai Finance, so in this article you will
  understand how MAI works.
---

# How does MAI work?

## What is a stablecoin?

Before getting into what is MAI, we have to understand what is a stablecoin, a stablecoin is a type of cryptocurrency that is designed to maintain a stable market price. Most of the stablecoins are pegged \(a currency where the price is designed to remain the same as a designated asset\) to the US dollar, but you can find other stablecoins pegged to other commodities such as gold \(like EGold\) or silver \(SilverCoin\).

However, there are 2 main categories in which all stablecoins can fit, **collateralized** or **non-collateralized.** The **collateralized** stablecoins are those that hold the assets against which their coin is pegged, meanwhile the **non-collateralized** make use of algorithms to control the supply of tokens in order to keep the price fixed at a predetermined level. 

## The IRON Finance disaster

If you've been around in crypto for some time, you may remember the disaster of the **TITAN** and **IRON** token, but for those of you who don't here is a quick recap. IRON Finance was a project that had 2 tokens, the _IRON_ stablecoin and the _TITAN_ token, however the IRON stablecoin **wasn't fully backed** with stablecoins, the proportion to mint IRON was **75% USDC** and **25% TITAN** token. So it was basically a recipe for disaster.

In June of 2021 the TITAN token reached an ATH of $65, which caused that a bunch of investors, who invested heavily in the coin, decided to sell. This caused a problem because TITAN is priced based on supply and demand. So as the available supply of TITAN increased, the price began to decrease. This caused a huge sell pressure so the price of TITAN fell even faster, so when TITAN began to fall rapidly, IRON lost its backing and eventually it’s peg.

![Price chart of the TITAN token](../.gitbook/assets/iron.jpg)

![Price chart of the IRON stablecoin](../.gitbook/assets/titan.jpg)

People started buying the IRON stablecoin to sell it for USDC and earn some quick bucks, in a huge arbitrage opportunity \(this means profiting in the price variations of tokens\) Long story short, it's been calculated that almost $1.75 billion were lost in this incident. Now, is there a difference between the IRON stablecoin and the MAI stablecoin?

## What is MAI?

MAI is a stablecoin that is backed by locked collateral tokens, the minting of MAI can be done either through **approved collateral** in vaults or through **Anchor.** 

When minting MAI depositing approved collateral, the **CDR** \(Collateral to Debt Ratio\) needs to be above 150%, this means that if you deposit $100 worth of collateral, the newly minted MAI can be at most worth $66.6667. We'll get to the reason behind this later in this article.

Another way to mint MAI is through the [Anchor](https://app.mai.finance/anchor),  this means that when you swap an stablecoin \(as September of 2021 you can mint MAI using **DAI**, **USDC** and **USDT**\) for MAI, new MAI is minted by the treasury and the deposited USDC is held in the treasury as collateral. Meanwhile, when you swap back your USDC, the MAI  that you provide will be burned.

![Stablecoins that can be swaped to mint MAI](../.gitbook/assets/image%20%289%29.png)

As you can see on the picture below, the price of the MAI stablecoin it's almost always close to $1, this is because as the [official documentation](https://docs.mai.finance/stablecoin-economics) says, the MAI stablecoin allows users to engage in risk-free arbitrage through Anchor when  the price of MAI falls below $0.99 or rises above $1.01. 

![Price chart of the MAI token in the last 90 days](../.gitbook/assets/image%20%287%29.png)

## Why is it always close to $1?

The peg to $1 is maintained by 2 mecanisms, via **Anchor** or by **depositing collatera**l in the vaults, in this section of the article, you'll understand why

### Anchor

Anchor allows users to mint MAI with stablecoins and redeem stablecoins from MAI. Also, as you can see on the picture below, there's a 1% fee when swapping your stablecoins for MAI or vice versa, there are two main reasons for these fee:

* The 1% minting fee to create MAI sets a price ceiling of $1.01.
* The 1% fee to redeem stablecoins from MAI sets a price floor of $0.99

![](../.gitbook/assets/image%20%288%29.png)

Having a price ceiling and a price floor helps MAI to not diverge from its peg too much, however as you've seen on the picture of the MAI chart, you can participate on low- risk arbitrage opportunities \(meaning that you can sell your stablecoins when MAI is under $1 or sell MAI when is above $1 to earn some quick bucks\). 

About what causes the fluctuation of the price of MAI, there could be two main reasons for this:

* If the **market is in a bearish trend**: people will sell their volatile assets and buy more stable coins to avoid losing value of volatile assets. This means that people want to buy MAI, increasing its price.
* If the **market is in a bullish trend**: people buy more volatile assets when their price is low, using their stable coins. This means that people sell their MAI, driving its price down.

### Depositing collaterals in vaults

In order to mint MAI using the vaults in Mai Finance, you need to deposit some collateral in there and have a **CDR** \(Collateral to Debt Ratio\) above a certain threshold, in this case is 150% \(however this percentage can change in the future if the community decides so\). This means that the vaults will always be overcollateralized \(by 150%\) to ensure that there is always collateral value to back the stablecoins minted. Remember that if a vault has less than a 150% CDR it could be partially liquidated by the community, so somebody could loose some of their collateral if a liquitador pays some of their debt.

As the value of the collateral rises, more stablecoins can be issued as a rise in collateral price will increase your collateral to debt ratio. Conversely, as the value of the collateral falls, fewer stablecoins can be issued, this is done to prevent that the CDR falls below the 150% mark.

## Afterword

As you've seen troughout this article, the MAI stablecoin is a type of stablecoin that is **over-collateralized,** meaning that there will always be enough collateral to back the price of the MAI token. This should give enough relief to those investors who hesitate about investing in projects that mint stablecoins. Also, keep in mind that if there is more MAI in the market, the more stable the price of MAI will be.

Recently, the vaults incentives have been introduced to Mai Finance, if you want to understand what that is, you can check this [article](https://app.gitbook.com/@qidao-qimps/s/mai-finance-tutorials/~/drafts/-MjoGweuRy7QzOmwfg7k/mai-eqi-qi-tutorials/mai-loans-and-vaults-incentives). This will help even more to the stability of the MAI price.

## Disclaimer 

You can find[ ](https://docs.mai.finance/stablecoin-economics)the original article of the Mai Finance team about MAI [here](https://docs.mai.finance/stablecoin-economics).

This guide is definitely not financial advice, it was made with an educational goal in mind. 

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly \(or make you lose money\) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}



