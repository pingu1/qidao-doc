---
description: >-
  This tutorial will try to cover some DeFi solutions
  enabled by Jarvis for people who want to invest with
  synthetics assets pegged to non-USD Fiats.
---

# From Traditional Finance to DeFi with Jarvis

Not all stable coins are equal. For most DeFi (**De**centralized **Fi**nance) users, stable coins represent a cryptocurrency that is pegged to the U.S. dollar. This is the case for assets like:

* USDC or USDT that are issued by centralized entities and backed by U.S. dollars
* over-collateralized assets like DAI or MAI that are softly pegged to the U.D. dollar but backed by a basket of different cryptocurrencies
* algorithmic stable coins like UST or MIM that are partially backed and for which the $1 peg is maintained using a specific algorithm

But did you know that you can find other stable coins? As an example, TOMB is a token that is pegged to the FTM price (the native gas token of the Fantom network) using algorithms.

In this article, we'll focus on stable coins that are pegged to FIATs (government-issued currencies), and we will try to explain why they are important for your investment strategies.

![](<../../.gitbook/assets/Jarvis-0.png>)

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

## Why do we need synthetic FIATs ?

Let's consider you are living in a European country and use Euro daily. If you were to buy crypto assets, you would most likely buy them with your Euros. For volatile assets like Bitcoin, it doesn't really matter because you'll be focusing on the price of Bitcoin in Euros to assess whether or not you are making money. And hopefully, you will make some.

But what if you want to invest in DeFi and yield farming instead? And what if, to mitigate the risks, you want to provide liquidity using stable coins only? Most of the stable liquidity on many chains is provided as USD-pegged assets, which means you will have to purchase USDC/USDT/DAI/MAI using your Euros. At this point, you should check that the liquidity you provide is generating interest, but also that the price difference between the US Dollar and the Euro isn't working against you.

![EUR/USD over the last year](<../../.gitbook/assets/Jarvis-1.png>)

If you bought 100€ worth of USDC on the 20th of September 2021, you would have had $117.29 worth of USDC because the ratio EUR:USD was 1:1.1729 at that time. If you were to convert $117.29 worth of USDC in Euros today (March 24th, 2022) with a ratio 1:1.0994, you would get 106.69€, or a gain of 6.69%.

But if you bought CAD 100 (100 Canadian Dollars) worth of USDC on the same day (September 20th, 2021) with a ratio of 1:0.7796 you would have had USD 77.96 worth of USDC. Converting these today to CAD with a ratio of 1:0.7972, would be worth CAD 97.79, or a loss of 2.21%.

However, 1 CAD always equals 1 CAD no matter what, like 1 USD = 1 USD and 1 EUR = 1 EUR.

Every currency of every country varies according to the geopolitical situation, internal and international politics, micro and macroeconomic decisions. This is why you need to pay attention to the price variation of your crypto assets, even if they are "stable".

## Jarvis Network and Mt. Pelerin

### What is Jarvis Network

[Jarvis Network](https://jarvis.network/) is a specialized application that allows users [to swap their crypto assets](https://app.jarvis.exchange/) for synthetics FIATs. A synthetic FIAT is a cryptocurrency that is pegged to the price of an existing FIAT. As such, Jarvis will let you swap your USDCs for

* jCAD: the crypto version of the Canadian Dollar
* jEUR: the crypto representation of Euro
* jJPY: the crypto version of the Japanese Yen
* jSGD, jCHF, jGBP, and many more

As such, Jarvis really is an On-Chain Forex (**For**eign **Ex**change) that is live on the Ethereum Mainnet, but also on Polygon, BNB Chain, Gnosis Chain, and Avalanche.

But it doesn't stop there. Jarvis proposes incentivezed liquidity pools that inclue jFIATs. This is done to attract users to deposit their jFIATs and earn yields on their stablecoins (with the hability to deposit a single asset via Curve pools), help other protocols that offer stable coins while not having a lot of liquidity, and make it easy for DeFi users to off-ramp their gains.

![Liquidity pools on Jarvis as of March 2022](<../../.gitbook/assets/Jarvis-2.png>)

{% hint style="info" %}
You can see in the screenshot above that the 2CAD pair is composed of jCAD and CADC. The CADC token is actually another version of the Canadian Dollar provided by [DFX](https://app.dfx.finance/), another decentralized Forex solution.
{% endhint %}

### Mt. Pelerin

[Mt. Pelerin](https://www.mtpelerin.com/bridge-wallet) is a non custodial fiat-crypto OTC desk. It allows users to purchase crypto from their bank account directly, and to have them directly deposited in their crypto wallet. It's also a direct partner of Jarvis and lets you buy jFIATs.

{% hint style="info" %}
The easiest way to use Mt. Pelerin is via the Bridge Wallet mobile application. Note that because it's a centralized service, you will have to provide personal information to prove your identity if you want to be able to use the service. You also need to have a bank that allows you to make bank transfers to Switzerland. However, it's always possible to use their website on which you will find a widget allowing you to buy cryptocurrencies from a bank transfer or using a Credit Card. This isn't subject to any KYC but has some limitations. Note that by using the website, your purchase will be sent directly to your web wallet. For the rest of this guide, we will present the Birdge Wallet solution though.
{% endhint %}

![Buying some jEUR with a EUR bank transfer](<../../.gitbook/assets/Jarvis-3.png>)

Bank transfers may be subject to fees, and will most likely take some time to complete, but overall, Mt. Pelerin allows you to easily buy and sell your synthetic FIATs for their FIAT counterparts. They also have an internal [fee structure](https://www.mtpelerin.com/pricing) that you can read in more detail, and depending on the asset you buy, you may be able to buy and sell up to $100,000 per year free of charge.

![Selling some jCAD to my bank account](<../../.gitbook/assets/Jarvis-6.png>)

{% hint style="info" %}
If you bought jFIATs, your bank account is automatically linked to your Bridge Wallet account and you will be able to select it from the dropdown list of recipients. If not, you will have to create a new account from an IBAN.
{% endhint %}

### Link your Polygon wallet to your Mt. Pelerin account (Bridge wallet address)

Linking your wallet to your Mt. Pelerin / Bridge Wallet account is as easy as

* Opening the Bridge Wallet application
* Open the Addresses tab at the bottom
* Click on `Link an address`
* Take a photo of the QR code of your Polygon wallet, or copy and paste the complete address in the field
* Send a few MATICs to the Bridge Wallet address to validate it

![](<../../.gitbook/assets/Jarvis-5.png>)

![Linking my Polygon wallets to my Mt. Pelerin application](<../../.gitbook/assets/Jarvis-4.png>)

{% hint style="info" %}
Once again, you can use the widget on the Mt. Pelerin website to [buy](https://www.mtpelerin.com/buy-ehtereum) and [sell](https://www.mtpelerin.com/sell-ethereum) your crypto using your web wallet (or hardware wallet) directly without using the Bridge Wallet. Please refer to the Mt. Pelerin website.
{% endhint %}

### Sending jFIATs to your Polygon wallet

Sending your jFIATs to your wallet on Polygon (or any supported chain) is very easy. From the Wallet tab, make sure you are on the network you want to use as a destination and load your jWallet Currencies.

![Sending jCAD to Polygon](<../../.gitbook/assets/Jarvis-8.png>)

After you selected the jFIAT you want to send, simply click on send, fill up the different fields, then initiate the transaction and enjoy low gas and fast processing!

{% hint style="info" %}
You can get a full recap of all your transactions in the activity section of each jFIAT, as well as on the Activity tab on the main screen.
{% endhint %}

![Checking that I received my jCAD on DeBank.com](<../../.gitbook/assets/Jarvis-7.png>)

{% hint style="success" %}
Mt. Pelerin is a very good solution to buy and sell cryptocurrencies and synthetic FIATs. But you can also use this service to send money to your friends and family if they are also using the application and possibly bypass complex bank transfers or limitations.
{% endhint %}

## Getting the best of your stable jFIATs

You have synthetic FIATs on Polygon, so now we need a clever way to use them. In the intro, we saw that it may be a better idea to use them as-is instead of swapping them (selling them) for USD-pegged stable coins.

Think also about this scenario: you have Canadian dollars and want a little bit of exposure to Ethereum. Wouldn't it be nice if you could buy Ethereum without taking the risk of actually buying it? Well, this is what lending markets are for !!!

### Market.xyz

[Market.xyz](https://www.market.xyz/) is a lending protocol where you will be able to use some of your crypto assets as collateral to borrow other assets. They recently launched a new pool 100% dedicated to Jarvis synthetic FIATs: https://polygon.market.xyz/pool/7.

![Jarvis Forex locked on Market.xyz as of March 2022](<../../.gitbook/assets/Jarvis-9.png>)

As you can see, you can lend your jFIATs and earn interest from borrowers. The locker also accepts some LP (**L**iquidity **P**roviding) tokens as collateral. This means that you can lend your m2CAD or m2JPY and still earn ~27% APY (**A**nnual **P**ercentage **Y**ield) on them, and borrow other jFIATs like jCAD or jJPY to leverage your position. You can also borrow some MAI, the USD-pegged stable coin created by the QiDAO protocol behind Mai Finance. The QiDAO community agreed to provide new MAI on a regular basis to maintain a low interest rate on MAI loans from the Jarvis locker on Market.xyz.

{% hint style="danger" %}
There's a minimum borrowing amount of 0.05 ETH on Market.xyz lockers, which is equivalent to $150 as of March 2022. Since you need to keep a healthy Collateral to Debt Ratio, make sure that you deposit enough collateral if you want to take a loan on the platform.
{% endhint %}

As for any lending platform on Polygon, Market.xyz will enforce a healthy Collateral to Debt Ratio. This is what the LTV of each collateral represents (**L**oan **T**o **V**alue, the inverse of the CDR). As an example, the LTV of m2CAD is 60%, meaning that the ratio between your debt and your collateral value needs to remain above 60%.

In the case of m2CAD, the collateral is pegged to the Canadian Dollar which can vary compared to the MAI you will borrow (pegged to the US dollar). However, the variation is very small, so you can in theory borrow very close to the threshold of 60%. For our guide, we will try to stick to a CDR of 200%, which corresponds to a LTV of 0.4 (1 / 2.5 = 0.5). To be able to borrow the required 0.05 ETH worth of MAI, we will need a collateral value of

$$
AvailableCollateral = \frac{Debt Value}{LTV} = \frac{0.05 ETH}{0.4} = 300\$
$$

Since today the USD:CAD ratio is 1:0.7972, I will need an initial investment of

$$
InvestmentCAD = \frac{300}{0.7972} = 376.32 CAD
$$

{% hint style="info" %}
Assuming I invest $300 worth of CAD and borrow $150 worth of MAI, I will currently earn 27% APY (23.91% APR) on my collateral and will have to pay 11.28% interest on my loan. Over the span of 1 year, that represents a growth of $81 of my collateral and $16.92 worth of interest to pay.
{% endhint %}

Now let's see what to do with your USD-pegged loan.

### Uniswap V3

[Uniswap V3](https://app.uniswap.org/) is the latest version of Uniswap, the parent project of many DEXes (**D**ecentralized **Ex**changes) where users will be able to swap their assets for other cryptocurrencies, as well as provide liquidity to support these swaps.

Uniswap V3 isn't incentivized on Polygon (yet), but offers a new way to provide liquidity: concentrated liquidity! You select the range on which you want to provide liquidity, and if the range is very narrow, you earn more fees than users who provide liquidity on a broader range. You can learn how to provide liquidity pairs on Uniswap V3 with [their official guide](https://help.uniswap.org/en/articles/5391541-provide-liquidity-on-uniswap-v3), and you can also watch the truly amazing [video by Finematics on UniswapV3](https://youtu.be/Ehm-OYBmlPM).

For this tutorial, we will focus on the MAI-USDC pair since we borrowed some MAI and we want to limit risk exposure by farming stable coins.

The first thing to do is to define a target range. Now that the price of MAI is a lot more stable due to ever-increasing liquidity, more pools, and some mechanisms like the Curve pool that help keep the price very stable), we will target a 1:1 rate for MAI:USDC. In reality, 1 MAI is closer to 0.998 USDC. 

The expected price range is between 0.99 and 1.01 USDC for 1 MAI, depending on the market conditions. When volatile assets are surging, people have more borrowing power and tend to swap a lot of MAI, decreasing its price. The opposite effect occurs when the market shrinks and people need to repay their loans to prevent liquidation: MAI is bought from the market to repay loans, increasing its price. In fact, the actual price range tends to be between 0.994 and 1.004 USDC per MAI.

![Spreading your LP on a broad or narrow position will have a great impact on the fees you collect](<../../.gitbook/assets/Jarvis-10.png>)

What you really need to understand though, is

* If you select a broad range, you will collect fewer fees than if you select a narrow range because your liquidity is spread on a bigger range
* If the select a narrow range and the price goes out of that range, you will not collect fees
* Your liquidity is not adjusted based on price. If you select a [0.99;1.01] range for MAI:USDC and the price of MAI is 0.99 USDC, you will have 100% MAI and 0% USDC. On the other hand, if the price is 1.01 USDC per MAI, you will have 100% USDC and 0% MAI
* You can exit your liquidity pool anytime and create a new one with a broader / narrower range if you see that your first setup isn't collecting enough fees
* For stablecoins, it's better to set a 0.05% fee range so that aggregators like [zapper](https://zapper.fi/) or [1inch](https://app.1inch.io/#/137/) pick your pool when users are swapping their stablecoins

For the simplicity of this guide, we will set a range centered on 1.000 with a 1% spread between 0.995 and 1.005 USDC per MAI.

![Creating a concentrated liquidity pool for MAI-USDC pair](<../../.gitbook/assets/Jarvis-11.png>)

{% hint style="info" %}
Pay attention to the token order for your pair. Indeed, the price range will not be the same if you select MAI (mimatic) first and USDC second, or USDC first and MAI second !!!
{% endhint %}

Depending on your setup, you can expect between 8% APR (broad range) and 20% APR (narrow range) on your LP paid in MAI and USDC. This will highly depend on the price action and volume of trades operated on UniswapV3. Keep in mind that you can also use this tool to operate your trades with a very low price impact and collect fees from your own trades!

## Farming Strategy

For this strategy, we will be using Jarvis as our starting point. We will be using jCAD bought via Mt. Pelerin for this. The jCAD will be deposited on Curve Finance into the appropriate pool to get a 2CAD LP token. This LP token will be deposited on Beefy so that swap fees and reward tokens provided by Jarvis can compound into additional 2CAD. As a proof of deposit, we will receive mooJarvis2CAD tokens that we can then use on Market.xyz as collateral to borrow some MAI with a CDR of 200% (50% LTV). The MAI loan will be used to create a liquidity-providing token on UniswapV3 so that it can collect swap fees at 12% APR.

This initial setup ensures that you don't get impacted by the price variation of the USD in regard to the CAD. Also, the borrowed amount is secured in the UniswapV3 pool and can be repaid at any time.

Both gains from the 2CAD and the UniswapV3 pools will be added to a "reward booster", i.e. a pool that will have 0 impact on the initial investment or the loan but will actually increase the gains from a high reward rate. You can use pretty much any pool with a reward rate higher than the 2CAD pool. It can be a liquidity pool on QuickSwap like the cxDOGE/cxETH (44.24% APY as of March 2022), or even an ohm-fork like Klima (944% APY as of March 2022). For our simulation, we will be using the JRT-MAY22-USDC pool directly on Jarvis Network. The liquidity can be bought/added on [Kyber Network](https://kyberswap.com/#/add/0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174/0xF5f480Edc68589B51F4217E6aA82Ef7Df5cf789e/0xdaa2c66b06b62bad2e192be0a93f895c855484ee) and uses USDC and a native token from the Jarvis Network. This LP token is currently getting 143% APR.

This strategy is focusing on stable coins, but also presents a lot of possible variations:

* You can use 2JPY or 2SGD if you prefer these FIATs over jCAD
* You can lend your jCAD (or any jFIAT) on Market.xyz and collect borrowing fees from borrowers
* You can swap your loan from Market.xyz into any token for which you will provide liquidity on UniswapV3. Pick the pool you prefer, but pay attention to potential impermanent losses
* You can swap the fees you collect on UniV3 to anything accepted on [Mai Finance](https://app.mai.finance) (BTC, CRV, LINK, GHST ...) and repay your loan on Market.xyz using the loan taken on Mai Finance, actually transferring your loan at 11% into a loan at 0%
* You can also use the fees collected to repay your loan on Market.xyz faster
* Possibilities are endless

As always, we will assume a few things for the simulation:

* The APY for 2CAD is 27% APY (23.91% APR)
* The interest rate for the loan on Market.xyz is 11.28%
* The APR of your position on UniswapV3 is 12% because you make it quite large (more secure but less efficient)
* You will get 143% APR on the JRT-MAY22-USDC reward booster on Jarvis Network

![](<../../.gitbook/assets/Jarvis-12.png>)

{% hint style="info" %}
If you want to run simulations for this system, you can use the [Google Spreadsheet linked to this strategy](https://docs.google.com/spreadsheets/d/10-n5IyZLl0GZyjM16SNuVOONNsfJ15pm2GL0e2MagzE/edit?usp=sharing). Simply change the different reward rates or desired CDR to estimate the final APY you can get from this loop.
{% endhint %}

### Day 1

You need to bootstrap your system. To do so

* swap $300 worth of USDC for jCAD on Jarvis Network (or purchase jCAD directly via Mt. Pelerin)
* deposit the jCAD on Curve Finance in [pool #23](https://polygon.curve.fi/factory/23/deposit)
* deposit the 2CAD LP token on [beefy finance](https://app.beefy.finance/#/polygon/vault/jarvis-2cad)
* deposit the beefy receipt token on Market.xyz
* borrow MAI with a CDR or 200% (LTV of 50%)
* swap a part of your MAI for USDC on Uniswap V3 and deposit MAI and USDC into a new liquidity pool with parameters of your choice

After the 1st day of farming, you should have

|     position     |  value ($) |
|------------------|------------|
| mooJarvis2CAD    |    300.000 |
| 2CAD rewards     |      0.197 |
| MAI-USDC UniV3   |    150.000 |
| UniV3 fees       |      0.049 |
| JRT-MAY22-USDC   |      0.000 |
| Jarvis rewards   |      0.000 |
| MAI debt         |    150.000 |

You are all set, the rest is simple maintenance and moving the rewards into the Jarvis pool

### Daily maintenance

Time to put your gains into the reward booster:

* harvest MAI and USDC on Uniswap V3
* extract a small portion of your mooJarvis2CAD corresponding to what has been compounded
* harvest reward on Jarvis Network
* swap everything for JRT-MAY22 and USDC on Kyber Network, and create LP tokens
* deposit the LP token on Jarvis Network

At the end of Day 2, you will have

|     position     |  value ($) |
|------------------|------------|
| mooJarvis2CAD    |    300.000 |
| 2CAD rewards     |      0.197 |
| MAI-USDC UniV3   |    150.000 |
| UniV3 fees       |      0.049 |
| JRT-MAY22-USDC   |      0.246 |
| Jarvis rewards   |      0.001 |
| MAI debt         |    150.000 |

### Raw results month after month

Here are raw results month after month, as you can get them in the Google SpreadSheet linked above.
 
| day | mooJarvis2CAD | MAI-USDC  | JRT-MAY22-USDC |  MAI debt |
|-----|---------------|-----------|----------------|-----------|
|  30 |       300.000 |   150.000 |          7.534 |   151.350 |
|  60 |       300.000 |   150.000 |         16.282 |   152.760 |
|  90 |       300.000 |   150.000 |         26.118 |   154.182 |
| 120 |       300.000 |   150.000 |         37.179 |   155.618 |
| 150 |       300.000 |   150.000 |         49.616 |   157.067 |
| 180 |       300.000 |   150.000 |         63.601 |   158.530 |
| 210 |       300.000 |   150.000 |         79.326 |   160.007 |
| 240 |       300.000 |   150.000 |         97.009 |   161.497 |
| 270 |       300.000 |   150.000 |        116.893 |   163.001 |
| 300 |       300.000 |   150.000 |        139.252 |   164.519 |
| 330 |       300.000 |   150.000 |        164.393 |   166.051 |
| 360 |       300.000 |   150.000 |          7.343 |     0.000 |

### Day 365

With a CDR of 200%, you will repay your entire debt during the 11th month, liberating the initial CAD that you can transfer back into your bank account if you want, and you will still have

* $150 worth of MAI-USDC
* $7.343 worth of LP on Jarvis

For a grand total of 52.91% APY.

{% hint style="info" %}
If you take the profits from your 2CAD liquidity pool and invest them directly into the JRT-MAY22-USDC pool on Jarvis, without adding Market.xyz in the middle, you would get a total APY of 52.68%. You can see the 2nd sheet on the Google Spreadsheet for details, or set the CDR to 1,000,000 (no loan).
{% endhint %}

## Disclaimer

This guide has been written mostly to illustrate how you can convert your FIATs into crypto assets (and vice versa) using Mt. Pelerin and Jarvis Network. For non-US residents, this is a very nice opportunity to transfer money from one "world" to the other with very little impact and almost no fees. The fact that you can also get your synthetic FIATs on Polygon makes it particularly efficient since gas cost and transaction time remain among the best for DeFi.

It's also interesting to note that more and more first-grade applications are using jFIATs, especially [AAVE v3](https://app.aave.com/markets/) that started to propose jEUR and EURS lending markets, facilitating the transition from TradFi (**Trad**itional **Fi**nance) to DeFi.

The strategy proposed in this guide, it's assuming all prices and rates remain the same, which is obviously not what happens in real life. Make sure you pay attention to the reward borrowing rates before you invest anything so that you can repay your loan.

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs, end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}
