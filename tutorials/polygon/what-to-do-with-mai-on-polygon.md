---
description: >-
  This tutorial will present the different options that will let you use your
  freshly minted MAI on Polygon.
---

# What to do with MAI on Polygon

## Goal of this tutorial

The goal of this tutorial is not to present in details what you can do with your MAI stable coin, but have a list of all the websites and DeFi application that you can use on Polygon that will let you use your MAI directly, or in combination with other stable coins. For more details about specific ways to use MAI, you can refer to other tutorials on this site, or get help on Discord or Telegram.

Please note that the list is not complete, and will never be since there are new dapps launching every week on the network. I can't review them all, so I will only present the main options, or the most famous / most "secured" options.

If you want a particular project to be listed, please join the Qi community on [Discord](https://discord.gg/mQq55j65xJ).

{% hint style="info" %}
I will not present Mai Finance farms. This subject deserves its own tutorial, because Qi is not like any other random farm token.
{% endhint %}

## Farming safely on bluechip projects

Bluechip projects are the DeFi applications that proved to be solid and present a lower risk. They are usually audited and the team behind them have been working on then for a long time. They usually don't have huge APRs (**A**nnual **P**ercentage **R**ate) but they can be trusted.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) is an automated portfolio manager, liquidity provider, and price sensor. On the platform, you will be able to lend your crypto and you collect fees from traders, who rebalance your portfolio by following arbitrage opportunities. If you need more details about Balancer, please go read [the official doc](https://docs.balancer.fi).

On Polygon network, Balancer proposes a pool composed of the 4 main stable coins: DAI, USDC, USDT and MAI (miMATIC). This stable pool has currently a pretty steady APR of \~20%.

![Stable coin pool state as of August 2021](<../../.gitbook/assets/Screen Shot 2021-08-11 at 11.06.59 AM.png>)

The best thing about Balancer is that you absolutely don't need to own the 4 coins to deposit into the pool. Balancer will automatically generate a balanced combination with whatever deposit you make. This means that if you have 100$ worth of MAI, you can simply deposit them into the Balancer pool and let the algorithm slip it properly to have a 25% ratio for each coin depending on their respective price at the moment of the deposit.

Rewards for the pool are paid using the BAL token, distributed on a weekly basis. In addition to the BAL token, additional rewards can be granted depending on the pool you entered. You can check the different [incentives program here](https://balancer-incentives.web.app). In our case, participating in the stable pool will also earn you MATIC and Qi rewards.

The complete flow would be something like this

![](<../../.gitbook/assets/Screen Shot 2021-08-11 at 11.34.45 AM.png>)

If you need more details on how you can use Mai Finance to lend your crypto and borrow MAI (instead of selling your crypto to buy MAI), read other guides on this site. You can even [include AAVE into the loop](leverage-aave-tokens.md) to earn even more.

### Curve finance

A little bit of click-bait here. [Curve](https://polygon.curve.fi) is another platform where you will be able to lend your crypto assets in pools that will generate revenues, but not MAI directly (not yet?). The pools we are interested in are

* the AAVE pool that will generate between 5% and 15% APR (APR varies a lot) on a stable coins trio (DAI/USDC/USDT). The pool works exactly like Balancer in the way that you can enter the pool using a single asset that will be used on AAVE by the protocol.
* the atricrypto pool that is composed of the stable coin trio and includes wETH and wBTC too to mitigate impermanent losses. This pool has an APR ranging between 25% and 30%. The Mai Finance team is currently trying to have MAI added to this pool too, meaning that you may be able to enter it with your minted MAI directly.

While waiting for the Curve protocol to accept MAI as a valid stable coin in their pools, you can still use your favourite crypto with Curve by following these steps (example with MATIC)

* Deposit your MATIC token on AAVE and collect amWMATIC
* Deposit your amWMATIC on Mai Finance and collect camWMATIC (the AAVE rewards will be compounded into the camWMATIC tokens)
* Use the camWMATIC as a collateral on Mai Finance and borrow MAI against it
* Use the [swap page](https://app.mai.finance/anchor) on Mai Finance to swap all of your MAI for USDC
* Then you can
  * Enter the atricrypto pool on Curve with your USDC and get 25% to 30% reward
  * Enter the AAVE pool on Curve with your USDC and get 5% to 15% reward

Rewards on Curve are granted in

* Auto-compounded USDC that increase your position in the pool (it will be a mix of USDC/USDT/DAI and possibly wBTC/wETH for the atricrypto pool)
* WMATIC that you can then use to repeat the loop above and increase your loan and invested capital
* CRV token, that can also be used as collateral on Mai Finance to borrow more MAI and increase your invested capital

![](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.14.27 PM.png>)

### AAVE

There's a complete guide on how you can use Mai Finance to [lever up your crypto on AAVE](leverage-aave-tokens.md). This is not doing a direct use of MAI stable coin, but we can imagine that, in the future, AAVE will also have a MAI pool where you will be able to lend your crypto.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) is probably one of the most famous DEX (Decentralized EXchange) on Polygon with SushiSwap and 1Inch. It's also an AMM (Automated Market Maker) that allows users to efficiently trade on the Polygon network using liquidity pools. Any trade on the exchange is subject to a fee that is partially redistributed to users who deposit their liquidity on the platform.

The way you can use MAI on QuickSwap is very similar to a [regular yield farm](secure-your-yield-farming-profits.md) so if you need to get exact steps to enter the MAI/USDC pool on QuickSwap, it's probably better for you to read this article.

Currently, if you enter the MAI/USDC LP (**L**iquidity **P**rovider) pool on QuickSwap, you will earn

* trading fees
* QUICK tokens

![Details of the MAI/USDC pool on QuickSwap as of August 2021](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.37.56 PM.png>)

## Degen farms and aggregators

### Adamant

[Adamant](https://adamant.finance/home) is an aggregator that is listing all the "best" farms on Polygon and let you enter them directly from their website. By depositing your assets (LP tokens) on a specific pool on Adamant, the algorithms will harvest the rewards granted by the pool and automatically compound part of the reward into your LP position. The rest of the reward is usually converted in WMATIC that is then redistributed to the holders of the ADDY token (native token of Adamant). Finally, you get a reward in ADDY tokens as well that you can harvest and vest for 90 days, earning you part of the WMATIC dividends.

In general, Adamant is a good place to go if you don't really care about the farm token, and if you don't want to compound your rewards manually several times a day. It also generates more revenue since you get some ADDY rewards in addition to the reward granted by the pool.

Adamant currently supports a few pools that accept the MAI/USDC LP pair. The pools are on

* QuickSwap: QUICK reward is swapped into more MAI/USDC LP and WMATIC rewards
* DinoSwap: Dino reward is swapped into more MAI/USDC LP and WMATIC rewards
* Mai Finance: Qi reward is swapped into more MAI/USDC LP and WMATIC rewards

![QuickSwap MAI/USDC pool on Adamant](<../../.gitbook/assets/Screen Shot 2021-08-11 at 12.51.12 PM.png>)

{% hint style="info" %}
The screenshots of the QuickSwap pool on QuickSwap website (see paragraph above) and Adamant have been taken the same day, but are showing different APYs (**A**nnual **P**ercentage **Y**ield).
{% endhint %}

You can see that the APY on Adamant is a little bit higher than on QuickSwap directly. The reward breakdown is as follows

* 12.88% Auto-compounded QUICK (meaning the QUICK reward is transformed into more LP tokens)
* 9.16% ADDY reward (not compounded)
* 3.40% fee share dividend (claiming ADDY daily)

This means that, out of the 20.92% granted by QuickSwap, only 12.88% is used to increase your LP position, the rest is swapped into WMATIC dividends. You will be able claim your ADDY reward daily (or anytime) and stake them, which will will in turn generate claimable WMATIC dividends. In other words, Adamant _seems_ a better option because it has better APYs and compound rewards automatically, but in reality it involves a lot of manual actions too.

{% hint style="info" %}
Using Adamant also has a strong impact of native token prices. Indeed, because Adamant is constantly selling the farm tokens to generate more LP pairs and WMATIC as dividends to their ADDY holders, the sell pressure is very high on farm tokens and can explain why their price is consistently decaying.
{% endhint %}

### Other farms accepting MAI/USDC LP pair

MAI getting more and more popularity on Polygon, and because QuickSwap supports the MAI/USDC pair, a lot of farms are now supporting it too. The following list will present a few projects on which you can earn yield using MAI/USDC

* DinoSwap
* Augury
* Polypup
* ...

Other farms may also accept the MAI/USDC pool. If you want to stay informed about new farms and their launch date, I strongly recommend taking a look at the [RugDoc.io calendar](https://rugdoc.io/calendar/) for Polygon farms, and possibly to the rest of their website which will present a very smart overview of each farm, as well as their potential risks.

## Impermax

### A little bit of explanation

[Impermax](https://polygon.impermax.finance) is a platform that let users leverage their LP tokens for higher yields. The goal is very simple: by providing LP tokens and using them as collateral, one can then borrow more of the 2 underlying assets to generate more LP tokens and repeat the loop.

![Impermax loop explained](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.15.21 PM.png>)

When doing so, the user is exposed to impermanent loss, and the loss is magnified by the number of times the loop is repeated. The risk of liquidation is also multiplied when too many loops are applied. Indeed, if the APR is multiplied, the price variation of the two coins forming the pair is amplified by the lever effect, leading to faster liquidation.

With stable coins, the risk of liquidation is lower though, because the price variation is negligible. This also means that the Collateral to Debt Ratio (CDR) can be very close to 100%, leading to a high number of loops, hence a high APR.

Note that Impermax is charging fees when you borrow and leverage your position. The fee corresponds to 0.1% of your final position. As an example, if I have $100 worth of MAI/USDC and I leverage 50x, my final position will worth $5,000 and I will pay a $4.90 fee corresponding to the $4,900 that I borrowed.

The effect of looping the lending/borrowing combination allows to multiply the final APY. With an initial APY of 20% for MAI/USDC pair with a CDR of 110%, operating the loop 50 times, and using the formula

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

We can easily get a 228% final APR. There are some other elements that will affect the final APR, namely the borrowing APR (loan interest for borrowing more LP tokens), and the supply/demand of both assets composing the LP pair (directly driving the borrowing APR).

Also, because all the rates are magnified by the number of times the loop is applied, the APR will vary drastically, and can sometimes become negative for short amount of times (your LP token will be used to repay the negative APR).

### Leveraged position of my MAI/USDC pair

In the end, you are using the base APR on a much bigger value, which is earning much bigger interests, increasing the APR of your initial position.

![An example of Impermax dashboard with an initial $70.52 MAI/USDC pair](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.38.33 PM.png>)

I can see very easily how much I'm using as collateral, how much I initially invested, what's the leverage ratio, and what are the liquidation values due to the leverage ratio. This position will give me the following ratios at the time of writing

![Earnings and spendings estimation at a given time](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.41.55 PM.png>)

The APR is granted in IMX token that can either be swapped for more MAI/USDC (use the power of Mai Finance to borrow at 0% interest, RFTM), or used to provide liquidity on specific pools accepting IMX on Impermax.

### Supplying MAI to borrowers

Indeed, on the app you can also provide liquidity to those who want to apply leveraging loops to their positions (they will need underlying assets to generate more LP tokens). Lending assets is a great way to earn yield and let the borrowers take all the risks. Also, the more users are borrowing, the higher the supply APR will be.

![Rates for supplying and borrowing MAI on Impermax at a given time](<../../.gitbook/assets/Screen Shot 2021-08-11 at 1.47.56 PM.png>)

This is another great way to optimize your 0% loan on Mai Finance. Not only you don't have to pay anything to borrow MAI, but you can earn a lot of interest just by depositing it on Impermax.

## Disclaimer

Everything is this tutorial is purely educational. The goal is to bring light to projects that I think are worthy for people evolving in the crypto world on Polygon. I obviously didn't talk about Mai Finance as a farm because a dedicated tutorial will be written very soon. Finally, this guide is ABSOLUTELY NOT meant to be applied as is, it's not any financial advice and you should not follow blindly what I wrote. Please read the docs of the different projects I mentioned before considering investing on their platforms.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
