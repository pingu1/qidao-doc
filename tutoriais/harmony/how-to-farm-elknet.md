---
description: >-
  Este guia apresenta diferentes maneiras de fazer farming com um único par LP
  para ilustrar as diferenças entre staking e .
---

# Um par LP, farming de varias formas

## Introduction

Providing liquidity on a DEX (**D**ecentralized **EX**change) and farming reward is one of the most common way to farm yields in DeFi (**De**centralized **Fi**nance). However, many users are only paying attention to the rates of the LP (**L**iquidity **P**roviding) pool they enter, without really checking if the rate is an APR (**A**nnual **P**ercentage **R**eward) or an APY (**A**nnual **P**ercentage **Y**ield). There are many ways to farm a pool and manage the reward tokens. We will see in this guide some of the different way you can farm one of the latest pools on Harmony, MAI-ELK, and see what you can do with the ELK tokens that you will get as a reward.

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs, end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}

![](../../.gitbook/assets/elk-farming-1.png)

## Elk Finance

[Elk Finance](https://app.elk.finance/#/) is a DEX forked from Uniswap v2, as well as an AMM (**A**utomoated **M**arket **M**aker). You will find all the usual features of Uniswap forks: trading your assets, combine your different crypto currencies into LP tokens, farm some LP pairs, and stake their native token, the ELK.

What makes Elk Finance a totally different project though is its presence on many blockchains, and not only the EVM-compatibles chains (**E**thereum **V**irtual **M**achine). Indeed, Elk Finance is currentl present on 16 chains and they have plans to expand to many others. They managed to build a bridge between all those chains to let users transfers the ELK token: The ELKNET.

![Bridging some ELK from Harmony to Moonriver using the ElkNet](../../.gitbook/assets/elk-farming-2.png)

Also, one cool feature proposed by the ElkNet is the possibility to swap a portion of the transferred asset for some gas token on the destination. This is particularly useful if you are going for the first time on a block chain where there is no available faucet.

{% hint style="success" %}
Except for chains where gas is high (only Avalanche and Cronos at time of writing), using ElkNet to bridge your ELK tokens from one chain to another is done at no expense. You read that right, you don't pay any bridging fees!
{% endhint %}

Finally, Elk Finance provides Impermanent Loss protection. You can read all the details about the Impermanent Loss program in [their official documentation](https://docs.elk.finance/features/impermanent-loss-protection), but basically, all you need to know is that if the price of ELK changes between the moment you deposit and the moment you withdraw, you'll be pay extra ELK in order to cover the impermanent loss. Because MAI is pegged to 1 USD, the impermanent loss is only linked to the price movement of ELK, so you're always a winner when you're entering LP pools on Elk Finance DEX.

## Farming the MAI-ELK LP Pair

Elk Finance partnered with Mai Finance in January 2022 to propose token farming using the MAI-ELK LP pair on their DEX. The MAI-ELK pair can be used on 3 different networks for now: Harmony, Moonriver and Gnosis. Some additional pools may be launched later on Polygon, Cronos and Fantom. Let's see the different strategies that you can apply for this new pool.

{% hint style="info" %}
We are proposing this guide for Harmony because the gas fees are very cheap, which allows you to compound your reward manually on a daily basis. This makes it a very good blockchain for beginners who have only a few dollars to invest as play money. However, everything presented in this guide can be also applied to any other chain.
{% endhint %}

### Farming and Staking

The very first strategy is pretty straightforward:

* combine your LP pair
* deposit the LP in the MAI-ELK pool and get 200% APR
* harvest your rewards daily
* stake them at 32.53% APR

If you start with an initial $100, here are the results you can get month after month for a complete year of farming, assuming the rates given above remain the same for the entire farming period.

| day | MAI-ELK ($) | staked ELK ($) |
| --- | ----------- | -------------- |
| 30  | 100.000     | 16.653         |
| 60  | 100.000     | 33.756         |
| 90  | 100.000     | 51.323         |
| 120 | 100.000     | 69.366         |
| 150 | 100.000     | 87.897         |
| 180 | 100.000     | 106.930        |
| 210 | 100.000     | 126.479        |
| 240 | 100.000     | 146.557        |
| 270 | 100.000     | 167.180        |
| 300 | 100.000     | 188.360        |
| 330 | 100.000     | 210.115        |
| 360 | 100.000     | 232.458        |

At the end of the year, you would have

* $100.00 worth of MAI-ELK LP tokens in the pool
* $236.24 worth of staked ELK tokens

Which corresponds to an overall APY of 236.24%. It's not exactly APR because part of the reward is compounded (the staked ELK).

{% hint style="info" %}
You can find all the results and the formula used to build this table in [the following Google Sheet](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) in the first tab. You can copy this file to your own drive and adjust rates and initial investment to see the overall APY change with the number you enter.
{% endhint %}

### Farming and Compounding directly

Compounding means that you harvest your rewards, and use it to create additional LP tokens. In our case, you would:

* harvest your ELK rewards
* sell 50% for MAI
* combine into some additional MAI-ELK LP token
* deposit in the pool

If you start with the same initial investment of $100, the results you can expect for a complete year of farming, assuming the rates given remain the same for the entire farming period, are as follows:

| day | MAI-ELK ($) |
| --- | ----------- |
| 30  | 117.172     |
| 60  | 138.044     |
| 90  | 162.635     |
| 120 | 191.607     |
| 150 | 225.739     |
| 180 | 265.952     |
| 210 | 313.328     |
| 240 | 369.143     |
| 270 | 434.901     |
| 300 | 512.374     |
| 330 | 603.647     |
| 360 | 711.179     |

And at the end of the year, you would have

* $730.878 worth of MAI-ELK LP tokens in the pool

Which corresponds, for an initial investment of $100, to an overall APY of 630.88%. Since we are compounding the reward, this is the exact APY you would get from an APR of 200%.

As a side note, the formulas to calculate the APY from an APR with daily compounding (or an APR from an APY) are as follows:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

$$
APR = N * (( 1 + APY)^\frac{1}{N} - 1)
$$

With `N` being the number of times you compound your rewards. In our case, the 2 formula would give us

$$
APY = ( 1 + \frac{2}{365})^{365}-1 = 634.88\%
$$

$$
APR = 365 * (( 1 + 6.3488)^\frac{1}{365} - 1) = 199.99\%
$$

It's easy to see and understand that if you apply an APR of 200% (the APR of the LP pool) to your reward, you will get better yields than if you apply an APR of 32.53% (staking APR). In that sense, compounding is way better than staking while the farming APR remains above the staking APR. This may obviously change with the amount of liquidity in the pool.

{% hint style="info" %}
As for the previous section, the simulation can be found in the same [Google SpreadSheet](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) in the second tab.
{% endhint %}

### Farming and Compounding using Mai Finance

If staking and compounding are giving good yields, both methods are directly linked to the price of the ELK token, so the value of your investment will vary with the price of ELK. We already saw that compounding gives better options compared to staking. Now we will see how you can capture some value from your farming rewards, and continue investing in the same pool using Mai Finance. The daily routine would be as follows:

* Harvest the ELK rewards
* Sell 66% of the reward to buy some blue chip token accepted as collateral on Mai Finance. For our exemple, we will be using the ONE token here
* Deposit the ONE tokens in your vault on Mai Finance
* Borrow additional MAI at 200% CDR (**C**ollateral to **D**ebt **R**atio), which value will correspond to your remaining ELK tokens
* combine into some additional MAI-ELK LP token
* deposit in the pool

{% hint style="info" %}
Converting your reward tokens to ONE may not be the safest way to protect your assets, one of the best ways to do it is to convert to stable coins. However, options on Mai Finance on Harmony as of writing this article are pretty limited. You may get better options in the future (after January 2021), like staking Stake DAO LP tokens as collateral (see our [dedicated article for Polygon](../polygon/the-elephant-and-the-otter.md) to see how you may be able to use Stake DAO tokens on Mai Finance).
{% endhint %}

If you start with the same initial investment of $100, the results you can expect for a complete year of farming, assuming the rates given remain the same for the entire farming period, and that your vault isn't liquidated, are as follows:

| day | MAI-ELK ($) | ONE ($) | Mai debt ($) |
| --- | ----------- | ------- | ------------ |
| 30  | 111.154     | 11.560  | 5.780        |
| 60  | 124.003     | 24.456  | 12.228       |
| 90  | 138.337     | 38.842  | 19.421       |
| 120 | 154.328     | 54.892  | 27.446       |
| 150 | 172.168     | 72.797  | 36.398       |
| 180 | 192.070     | 92.772  | 46.386       |
| 210 | 214.273     | 115.055 | 57.528       |
| 240 | 239.042     | 139.915 | 69.958       |
| 270 | 266.674     | 167.648 | 83.824       |
| 300 | 297.501     | 198.588 | 99.294       |
| 330 | 331.891     | 233.106 | 116.552      |
| 360 | 370.257     | 271.609 | 135.805      |

And at the end of the year, you would have

* $377.069 worth of MAI-ELK LP tokens in the pool
* $278.446 worth of ONE token in your ONE vault
* $139.223 worth of debt from your vaule
* a CDR of 200%, as expected

Starting from an original position of $100 worth of MAI-ELK, this would represent an overall APY of 416.29%. Here we're getting a little less gains compared to pure compounding, however we also extracted a good portion of our gains into ONE, which may be less volatile than ELK, hence may present less risk.

{% hint style="info" %}
Once again, the simulation can be found in the same [Google SpreadSheet](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) in the third tab.
{% endhint %}

Alternatively, you can also sell all your ELK rewards for tokens that are accepted on Mai Finance, borrow MAI and sell part of it to buy additional ELK in order to increase your position in the MAI-ELK pool. By doing so, you increase your exposure to ONE, but also increase your debt. You would end up with $270.715 worth of MAI-ELK, $352.913 worth of ONE and $171.457 worth of debt for an overall APY of 342.17%.

## Influence of the frequency at which you compound

Whether you decide to stake your rewards or compound, it's important to understand that your reward will change depending on the frequency at which you perform your harvest + invest routine. As a reminder, the formula that links APY and APR is as follows:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

In this equation, `N` represents the number of times you compound your rewards in a year. So, and APR of 200% as above would give you the following APY depending on the frequency you compound:

| Compounding frequency | equivalent APY |
| --------------------- | -------------- |
| daily                 | 634.88 %       |
| twice in a week       | 625.01 %       |
| weekly                | 611.71 %       |
| twice in a month      | 609.55 %       |
| monthly               | 535.86 %       |
| quarterly             | 406.25 %       |
| twice in a year       | 300.00 %       |

Manually compounding more than once a day can be expensive depending on the chain you're on. But basically, it's clear that the more often you compound, the better the reward. This is also explaining why yield optimizer / auto-compounder are popular. Keep in mind that by compounding, you add sell pressure to the token you farm, which will have a negative impact on the price of that token. If that's also the token you are using to farm (in our exemple ELK), you may be impacted by impermanent losses, unless you're using Elk Finance DEX, which protects you from impermanent losses.

## Choosing the right pool

The MAI-ELK pair has been deployed to several chains, so it's possible for you to deploy your capital to the chain that offers the best rates.

![MAI-ELK pools on Gnosis (top), Moonriver (middle) and Harmony (bottom) as of January 2021](../../.gitbook/assets/elk-farming-3.png)

{% hint style="info" %}
The MAI-ELK pool may also be deployed to other chains in a near future, possibly on Polygon, Cronos and Fantom. This is not guaranteed and there's no ETA for that, so stay updated by checking the difference Discord servers of both projects, of following them on twitter.
{% endhint %}

Besides the reward rate on each chain, you may also have to consider the price of the ELK token on each chain. Indeed, if the price is almost the same on all chains, the tiny difference may also be a factor for you to choose the chain where you want to farm the ELK token.

![Price of the ELK tokens on all the chains where it's present](../../.gitbook/assets/elk-farming-4.png)

As you can see, the MAI-ELK pool on Moonriver gives a better reward rate, and the ELK token also has a higher price on that chain. This means that, at time of writing, it may be better to farm the MAI-ELK pool on Moonriver than on Harmony or Gnosis, especially if you plan to sell a part of the farmed tokens. Note that this may not be true all the time, so make sure you choose your chain properly and that you do your own researches before joining a LP pool. Finally, it is strongly recommended to read the [documentation about IL protection](https://docs.elk.finance/features/impermanent-loss-protection) because the insurance is highly dependant on the number of days your LP tokens are deposited in the pool.

As a side note, because bridging ELK is free, you can possibly move from one chain to another in order to always benefit from the best rates. Make sure that you understand that by doing so, you will also influence the reward rates of the pool you exit and the one you join (less liquidity will increase the APR, more liquidity will lower it).

## Disclaimer

This guide has been written in order to illustrate the different ways to farm yields using liquidity providing tokens. You will highly influence your gains with the strategy that you pick, as well as your exposure to risk. Of course, all the notions pointed in this document are also applicable to any LP pair, and it's highly recommended to run your own simulations before picking a strategy, a LP pair, a pool or even a DEX.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
