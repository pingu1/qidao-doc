---
description: >-
  This guide will explain in details how you can use your Qi, the native token
  from Mai Finance, on Polygon. We will also analyze if Qi is a good investment
  opportunity, and what drives its price.
---

# What to do with Qi on Polygon

## Intro

Qi (\[tʃ Í] or _chee_), is the native token of Mai Finance. Some use it to vote and QIP (**Q**iDAO **I**mprovement **P**roposals), some stake it to get even more of them, and some simply farm with it. You can find some very good info on how you can use Qi on the Mai Finance plateforme in the [guide dedicated to passive income](../MAI-university/earning-passive-income-with-qidao.md).

This guide, as most investment tutorials, will focus primarily on farming and harvesting yields, this time using the Qi token. We will see how you can generate a lot of Qi, and how you can use them on the different platforms on Polygon.

Humble farmers will sometimes tell you that you need to remain humble, sell what you harvest and take profits. But personally, I'll go with:

> Give a man a fish and you feed him for a day. Teach a man to fish and you feed him for a lifetime.

So grab your fish rods, and follow the guide.

## What to do with your Qi on Polygon

### Staking

I will not spend too much time on this part, there's already a complete guide on the subject. Just keep in mind that Mai Finance is collecting revenues, and redistributes a very large portion to Qi stakers. Staking your Qi on Mai finance is one of the best use for the token, and as of September 2021, 23% of all circulating Qi is locked on average for 2 years.

### LP pair Farming

Once again, there are already a few other pages presenting how you can include the Qi token in your farming strategy to generate yields and never sell any of your farm tokens. See [Stack DApps like Lego bricks](stack-dapps-like-lego-bricks.md) or [Farming or Staking ?](farming-or-staking-or-both.md) guides for details exampled.

As a quick reminder, Qi is paired to different tokens to form LP (**L**iquidity **P**rovider) pairs on [QuickSwap](https://quickswap.exchange/#/quick) so that you can farm

* Qi-WMATIC on Mai Finance and get rewarded with Qi tokens
* Qi-WETH on QuickSwap and get rewarded with QUICK tokens
* Qi-QUICK on QuickSwap and get rewarded with QUICK tokens

![LP pool on QuickSwap for the Qi-WETH pair](<../.gitbook/assets/image (19) (2).png>)

### Single Qi farming

Qi can also be used solely on [Impermax](https://polygon.impermax.finance). Impermax is a platform where you will be able to leverage a specific LP pair several times in order to increase your gains from QuickSwap.

The way it works, is that you will borrow the 2 tokens forming the pair that you want to farm, combine them into more LP tokens, and farm with a much higher position. In most cases, borrowing rates are largely compensated by farming APR, giving you some net positive rewards.

![Leveraged Qi-WETH position on Impermax](<../.gitbook/assets/image (20).png>)

We can see here that the final reward APR on Impermax is 393.88% after leveraging 5 times, based on an APY of 239.68% on QuickSwap.

{% hint style="info" %}
Note also that Impermax gives estimated APRs (**A**nnual **P**ercentage **R**ewards) while QuickSwap gives estimated APYs (**A**nnual **P**ercentage **Y**ields), meaning that QuickSwap assumes you compound your rewards daily. The 239.68% APY on QuickSwap corresponds to a 122.49% APR.
{% endhint %}

But then, on Impermax, in order to borrow Qi and WETH to leverage your position, you need to get them from somewhere. This is possible only because some other users (or yourself) also supply both tokens separately. The more token is borrowed, the higher the borrowing rate becomes, and the lower the final APR, sometimes going in the negatives.

![Qi and WETH statistics for the Qi-WETH market on Impermax](<../.gitbook/assets/image (11).png>)

For our example, we will focus on Qi. You can see that the total supply of Qi is $427.21 and the total amount used in leveraged position is $321.44, giving the utilization rate of 75.24%. Impermax has some internal mechanism that automatically calculates the supply APR (APR that people lending Qi will get) and the borrowing APR (percentage of the farmed reward that will be deduced to pay the loan).

This means that you can provide Qi solely on Impermax and get, in our example, 43.73% APR, at the moment of writing. As supply and demand varies, the supply APR will also increase / decrease. When you supply single tokens on Impermax, you will get rewarded with the token you provide, meaning that this strategy will make you accumulate more Qi over time.

While you are on Impermax, you can also use the leverage option to get IMX rewards. Please read the [Stacking guide](stack-dapps-like-lego-bricks.md) to get more details on how you can include Impermax in your farming strategy.

### Balancer

Balancer is a really nice toolbox for any strategy, especially the ones that include Qi and/or MAI. Balancer proposes an equivalent of LP pair mining, but with more than 2 tokens provided in a 1:1 ratio. The pool can have 3, 4 or 5 tokens (sometimes even more) with different weight, and the algorithm in charge of the pool makes sure that the ratio for each token is always respected, selling some and buying others to keep it balanced.

The pool that we want to use here is a pool that contains Qi, WMATIC, BAL, USDC and MAI. This pool will reward you with both Qi and BAL tokens, and you can already see that you will be able to compound both into the pool. Because another amazing advantage of pools on Balancer is that you don't need to provide all tokens forming the pool in the proper ratio, the algorithm will do it for you. This means that you can indeed only deposit Qi in the pool and let the algorithm do the rest to rebalance everything.

![Details of the pool as of September 2021](<../.gitbook/assets/image (17).png>)

As a side note, BAL tokens can (or will soon be) usable as collateral on Mai Finance, which mean that you will have the option to store your BAL tokens on the BAL vault on Mai Finance, and borrow MAI against then. In addition to that, borrowing MAI against your BAL tokens will make you eligible for Qi rewards that will feed the pool on Balancer.

![Closed loop using Mai Finance and Balancer](<../.gitbook/assets/image (18).png>)

The APR of BAL vaults will highly dictates how interesting it is to have the vault in the loop, or if compounding your Qi into the Balancer's pool will be better.

## Understanding the price of Qi

Getting a lot of Qi is one thing, however if the token loses value over time, is it really a good strategy to keep it? In this section, we will try to understand the different factors that impact directly the price of Qi so that, when you start investing your Qis, you will get a better idea of how its price may vary, and what impact you will get on the Qi ecosystem.

### Qi emission

One of the main factor that will affect the price of Qi is the rate at which they are created. Indeed, price is always driven by demand and supply. If there's a lot of supply and very low demande, the price will naturally collapse. Hence understanding how Qi is generated is crucial to estimate its value over time.

There are currently 2 sources of Qi emission: farming rewards and vault rewards.

![LP farms on Mai Finance in September 2021](<../.gitbook/assets/image (12).png>)

If you are farming yields on MAI finance, you have the choice between the MAI/USDC pair and the Qi/WMATIC pair (as of September 2021).

* The MAI/USDC pair is rewarded with 0.5 Qi / block
* The Qi/WMATIC pair is rewarded with 1 Qi / block

On Polygon, the expected block time is 2 seconds, and since there are 86,400 seconds in a day, this means that the MAI/USDC pool is rewarded with 21,600 Qi every day, and the Qi/WMATIC with 43,200 Qi.

The pools of Mai Finance alone are responsible for 64,800 new Qi daily.

As for Vaults, each vault gets an emission of 0.05 Qi / block, or a daily emission of 2,160 Qi, and there are currently 10 Vaults, for a total of 21,600 Qi allocated as Vault rewards.

This means that each day, the equivalent of 86,400 new Qi are minted and distributed to users.

### Yield optimizers

Yield optimizers are platforms that will automatically compound the rewards with some pre-defined strategies, and allocate additional rewards for you to choose their site. However, a big part of the reward harvested is sold directly, and re-used in another way on these platforms.

As an example, Adamant offers you to farm the Qi/WMATIC LP pair on their platform, with the following reward distribution

![Qi-WMATIC pool on Adamant](<../.gitbook/assets/image (15).png>)

![Details of the 179.23% APR granted by Adamant](<../.gitbook/assets/image (14).png>)

You will notice that if the overall APR is higher than on Mai Finance, it's solely because Adamant is allocating additional ADDY rewards to the farmers. The amount of Qi that is actually redistributed to the farmer is 98.45% compared to the 134.42% you can get on Mai Finance.

From these 98.45% Qi reward, half of it is directly sold to buy WMATIC and form additional LP tokens that is then given to the farmer.

With 100$ worth of LP token, assuming the APR and the token prices remain the same for a complete year, and assuming there's no compounding, you would get after one year of farming

* $134.42 worth of new Qi on Mai Finance
* $98.45 worth of new Qi/WMATIC token, or $49.23 worth of new Qi on Adamant

This means that, in the process, $85.20 worth of Qi is simply sold directly on the market, which is more than 60% of the total emission allocated to the pool on Adamant.

And Adamant isn't the only platform proposing the same type of service. Some other examples are Beefy Finance and Kogecoin. From the $4.9M TVL in the Qi/WMATIC farm on Mai Finance, $2.3M are coming directly from Adamant, $41k from Beefy and $12k from Kogecoin, representing for these 3 platforms more than 50% of the value locked on Mai Finance. A raw estimation is that more than 30% of the total daily Qi emission is dumped by these platforms, putting some very negative sell pressure on the token, decreasing its price, which partially explains why Qi has difficulties keeping a high price.

### Understanding LP pairs

When you farm yields by providing LP pairs, the LP token is actually used to provide liquidity to users who are swapping one token for another. In our example of Qi/WETH, when someone is buying WETH, some of the token can be taken off the LP pool and sold to the user requiring it.

At that point, because some WETH has been taken off the pool, there is a balance mismatch: less WETH for the same amount of Qi. The algorithm in charge of maintaining the pool ratio to 1:1 will then sell some Qi from this pool to buy back some more WETH and recreate a perfect 1:1 ratio. The opposite things also happen when someone buys Qi, i.e. WETH is sold to buy back some Qi.

The same phenomenon occurs when one of the 2 tokens composing the pair gains or loses value. As an example, we will assume that Qi price is $1 and ETH price is $1,000, and that we have a pool that has $100 worth of Qi and $100 worth of WETH. It means that the pools contains 100 Qi and 0.1 WETH.

Now, if the price of ETH goes up to $2,000, if the pool keeps the same amount of token, we would have $100 worth of Qi but $200 worth of WETH, and we would have lost the balance. Hence, the algorithm in charge of the pool will sell a little bit of ETH to buy some Qi. In our easy example, $50 worth of ETH will be sold to buy $50 worth of Qi, and the final state would be

* 150 Qi with a value of $150$
* 0.075 ETH with a value of $150

This also means that when the price of one of the 2 token goes up, the pool creates some demande for the other, also driving its price up. The opposite is also true: if one token loses value, the other one will be sold to maintain a 1:1 ratio, driving the price down. This also partially explains the price fluctuation of Qi when compared to the price fluctuation of WEHT and WMATIC (the 2 main tokens to which Qi is paired).

![Price of Qi (left) VS Price of WMATIC (right)](<../.gitbook/assets/image (13).png>)

### Lack of use case

Finally, the lack of use for Qi, or the lack of known use cases, can explain why the price of the token is going down. People collecting Qi from Vault rewards and/or farming on Mai Finance will just sell it while it still has "some" value in order to realize a profit, with no long-term vision, which is actually a pretty reasonable strategy. This guide tries actually to promote different ways to use your Qi tokens without selling them, but if the price doesn't go up, or if you can't generate benefits in other tokens (a.k.a profit leak), there's very little advantages stacking them.

### How can we help price to go up?

If we want the price of Qi to go up (and who wouldn't want to), there are a few options.

* Reduce emission: with 86,400 new Qi minted daily, the supply is very high. If we cut down this emission, the supply may be lower, and with less supply, price should in theory go up. However, the current emission for the farms need to remain the same because they're part of a current partnership with QuickSwap. Vault incentives have been launched, and are an amazing way to promote the lending platform, pushing people to take loans, so cutting these emissions is probably another bad idea.
* Farm responsibly: I'm not saying that Adamant is the main culprit or is a bad product. Indeed, I include this platform in most of my strategies and use it on a daily basis. However, I try to farm in pools for which I have less concerns that the token will be dumped. If you want to farm yields on Adamant in a pool that is using the Mai Finance farm, keep in mind that you participate in the Qi depreciation. If you are ok with that, that's totally fine.
* Understand how things work: prices of ALL crypto-currencies are highly volatile, and most of the time, the price of BTC and ETH dictate the price of all other tokens. This is not done magically. Also, please understand that when some people earn money, it's because some other are loosing some. There's no free money, and magical internet money is actually not that magical.
* Find new ways to use your Qi tokens. This guide will always provide ideas that will help you increase the volume of your portfolio, and sell as few tokens as possible. Closed loops are the best because the output of one product feeds the input of the next one, creating a nice bubble that will only grow over time.

Keep also in mind that

$$
Value = Quantity * Price
$$

When the price go down but your quantity goes up, your value may increase, or at least it won't decrease as fast.

## Disclaimer

This guide is actually a result of many discussion about Qi price on the Discord channel. I realized that some people complaining about the price depreciation didn't fully understand the reasons about why the price of Qi was on a consistant down trend. This leads to frustration and delusion, which is very negative for Qi, the Mai Finance product, and the whole DeFi ecosystem in general. However, there's absolutely no guarantee that the price will ever go up, so if you want to keep your Qis and invest them, please do your own research and do it at your own risk. Plan your strategy properly and stick to it.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
