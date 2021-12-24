---
description: >-
  SpiritSwap recently launched a farm for MAI-WFTM, which is highlithing its
  mainstream adoption. This guide presents what you can do with this pool.
---

# Farming loop using SpiritSwap

When farming yields, the LP pair (**L**iquidity **P**roviding pair) is very important. Indeed, you want as little impermanent loss as possible so that you don't lose your initial investment. This initial pair will generate yield, and you can increase your gains by re-investing the token you farmed without additional risk on your initial. This is one of the reason why our guides propose strategies based on stables only, or on pairs that are composed by a stable coin and a blue chip token like Bitcoin, Ethereum, or the native gas token from the chain we are running the strategy.

Today, we will explore a relatively complex loop that will be based on the MAI-WFTM LP pair provided by SpiritSwap to celebrate its launch and current boost.

![](<../../.gitbook/assets/spiritswap-1.png>)

## Farming MAI on SpiritSwap

[SpiritSwap](https://app.spiritswap.finance/#/) is one of the main DEXes (**D**ecentralized **Ex**change) and AMM (**A**utomated **M**arket **M**aker) on Fantom. It's based on the Uniswap platform, so you will most certainly understand the core features of SpiritSwap, i.e. swapping assets, provide liquidity to earn yields. You will get rewards in the native token of the platform, the SPIRIT token that you will be able to stake and get inSPIRIT. The inSPIRIT token is particularly useful, it will let you vote for liquidity pools on which additional boost will be applied, and will allow you to earn extra yield from protocol revenue.

For our strategy, we will use the MAI-WFTM pool. As of December 2021, this pool can be found in the `Booster Farms` tab.

![MAI-WFTM pool on SpiritSwap as of December 2021](<../../.gitbook/assets/spiritswap-2.png>)

{% hint style="info" %}
When this guide has been created, the pool was in a very early stage (launched within the past 24h), which may explain the very high APR (**A**nnual **P**ercentage **R**ate). As always, before applying one of our strategies, do your own researches and verify the APR before investing. As comparison, USDC-WMATIC on Polygon is around 75%, and MAI-MOVR on Moonbeam is at 158%. Other pools like USDC-WFTM have stabilized around 50% on Fantom.

For the purpose of this guide, we will keep the lowest APR from the range, 152.98%, which may be a lot more than where it should stabilize.
{% endhint %}

When farming MAI-WFTM on SpiritSwap, you will get rewards paid in SPIRIT, the native token of the DApp (**D**ecentralized **App**lication). As of December 2021, 1 SPIRIT = 0.130 USDC.

## Farming using SPIRIT tokens on Liquid Driver

[Liquid Driver](https://www.liquiddriver.finance/) is another Uniswap fork that focuses on providing liquidity on Fantom. One of the feature that is the most interested on Liquid Driver is the fact that they can create linSPIRIT tokens from SPIRIT tokens. The linSPIRIT is a **l**iquid version of the inSPIRIT token. The ration between linSPIRIT and inSPIRIT is 1:1, it's really just a wrapped version of the inSPIRIT token, and you can trade both tokens for one another directly on Liquid Driver.

![LiquidSwapper on Liquid Driver](<../../.gitbook/assets/spiritswap-3.png>)

However, we will not use this feature. We will be farming the SPIRIT-linSPIRIT pool on Liquid Driver, but there's a nice little catch:

![Farming SPIRIT-linSPIRIT LP token on Liquid Driver](<../../.gitbook/assets/spiritswap-4.png>)

As you can see, you need to create the LP token on BeethovenX in order to get the 61% APR paid in LQDR tokens. As of December 2021, 1 LQDR = 4.560 USDC. Let's see how you can get this LP token.

## Create SPIRIT-linSPIRIT on BeethovenX

[BeethovenX](https://app.beets.fi/#/) has been recognized as the official Balancer pool on Fantom. As for Balancer, you don't need to deposit the same amount of both tokens to create a LP token. This means that you can directly deposit 100% of your SPIRIT tokens, and let the algorithm in charge of the pool to keep it balanced.

![Water Music By LiquidDriver on BeethovenX](<../../.gitbook/assets/spiritswap-5.png>)

In exchange, you'll get the LP token that you will be able to deposit on Liquid Driver.

{% hint style="info" %}
As you can see, this pool isn't incentivized on BeethovenX, you will not earn BEETS from it. The incentives are provided solely by Liquid Driver when you deposit the LP token on their platform, and the only reward you will get is paid in LQDR.
{% endhint %}

## Staking LQDR on Liquid Driver

Once you created your SPIRIT-linSPIRIT LP token on BeenthovenX and deposited it in the right pool on Liquid Driver, you will start earning LQDR tokens. You can then stake the LQDR tokens in order to earn a portion of the protocol's revenue. The cool thing is that you can choose the period of time during which your LQDR will be staked, and it will directly influence your APR (it's the same thing as when you stake Qi to earn protocol revenue). The average lock time is a little less than 2 years (max lock time) and rewards are paid in

* LQDR: you will be able to re-stake this reward
* WFTM: we will use this later
* BOO: we will use this later
* linSPIRIT: this can be used to increase your SPIRIT-linSPIRIT position on Liquid Driver
* SPELL: swap if for additional WFTM !!!

![Staking rewards when you stake LQDR as of December 2021](<../../.gitbook/assets/spiritswap-6.png>)

## Staking BOO on SpookySwap

[SpookySwap](https://spookyswap.finance) is the almost the last piece of our puzzle. Staking LQDR on Liquid Driver will make us earn BOO tokens, the native token from SpookySwap. SpookySwap is the biggest DEX/AMM on Fantom, so you can do pretty much the same thing as on SpiritSwap, except that their native token is the BOO token. This is particularly useful because you can stake your BOO tokens on SpookySwap to get xBOO tokens, and this staked version of BOO can be used to farm other tokens (it's a common feature for Uniswap forks). So, once you have xBOO, you will be able to deposit these tokens on SpookySwap to earn additional WFTM.

![Staking xBOO on SpookySwap to farm additional WFTM as of December 2021](<../../.gitbook/assets/spiritswap-7.png>)

## Getting more MAI-WTFM LP tokens

Liquid Driver and SpookySwap will produce WFTM tokens, so we're really missing MAI in order to add more LP tokens to our initial position in SpiritSwap. This can be done with a few different ways:

* swap 50% of your WFTM for MAI
* lend 66% of your WFTM on Beefy or Yearn Finance to get either mooScreamFTM or yvWFTM, then deposit the collateral tokens on Mai Finance and borrow MAI against them
* swap 66% of your WFTM for another asset and use the same strategy as above to borrow MAI

{% hint style="info" %}
If you need more details on the 2 last bullet points, we have a dedicated article on [leveraging your assets on Fantom](<leverage-your-crypto-on-fantom.md>).
{% endhint %}

For our guide, we will try to maximize our gains and use mooScreamDAI. This means that we will swap 66% of our WFTM for DAI on Spirit Swap, then deposit DAI directly on Beefy using SCREAM as the underlying platform to get mooScreamDAI. This token will then be deposited in a vault on Mai Finance and we will be able to borrow MAI. In order to lower the risk of liquidation, we will keep a CDR (**C**ollateral to **D**ebt **R**atio) of 200%, which means we will borrow half the value of our deposit. This is perfect since this corresponds to the same value of the WFTM we kept, so that it will be possible to create additional MAI-WFTM LP tokens.

![Getting mooScreamDAI on Beefy Finance](<../../.gitbook/assets/spiritswap-8.png>)

At the end of the loop, we'll get more MAI-WFTM and a yield bearing token used as collateral in Mai Finance.

## Farming Strategy

The following simulation is made assuming a few things:

* All rates and prices remain the same for the entire period of the simulation, 1 year in our case
  * 153% APR on MAI-WFTM farming on SpiritSwap
  * no reward on linSPIRIT
  * 61% APR on SPIRIT-linSPIRIT on Liquid Driver
  * 139% APR on staking LQDR
    * 26% APR in LQDR
    * 6% in WFTM
    * 30% in BOO
    * 74% in linSPIRIT
    * 3% in SPELL
  * 36% APR for staking xBOO
  * 21% APR for mooScreamDAI
* All rewards and programs are also running for an entire year
* The initial investment is $1,000 worth of MAI-WFTM LP token

![](<../../.gitbook/assets/spiritswap-9.png>)

### Day 1

On day 1, simply deposit your MAI-WFTM pair on SpiritSwap. At the end of the day, harvest your SPIRIT tokens and combine them into a SPIRIT-linSPIRIT pair on BeethovenX, then deposit this LP token on Liquid Driver. At the end of the day, you'd get

| MAI-WFTM | linPIRIT-SPIRIT | LQDR | xBOO | mooScreamDAI |
|----------|-----------------|------|------|--------------|
| 1,000.00 |            4.19 | 0.00 | 0.00 |         0.00 |

### Day 2

On day 2, yourr MAI-WFTM is still generating SPIRIT tokens that you'll deposit in the linSPIRIT-SPIRIT pool on Liquid Driver, but you will also be able to harvest your first few LQDR tokens, and stake them for the multi-rewards. At the end of the day, you'll get

| MAI-WFTM | linPIRIT-SPIRIT |  LQDR | xBOO | mooScreamDAI |
|----------|-----------------|-------|------|--------------|
| 1,000.00 |            8.38 | 0.007 | 0.00 |         0.00 |

### Day 3

On day 3, same thing except your LQDR will have produced your first few exotic tokens from protocol revenues. Don't forget you will actually stake your BOO, add your linSPIRIT to the pool, your LQDR will be restaked, and the rest will be swapped for WFTM. The resulting WFTM is then partially swapped for DAI and then mooScreamDAI deposited in a Vault to borrow MAI, form additional MAI-WFTM that is then deposited on SpiritSwap. At the end of Day 3, you'd get

| MAI-WFTM | linPIRIT-SPIRIT |  LQDR | xBOO | mooScreamDAI |
|----------|-----------------|-------|------|--------------|
| 1,000.00 |           12.58 | 0.021 | 0.00 |         0.00 |

{% hint style="info" %}
xBOO and mooScreamDAI position are too small to be displayed, so you may skip these steps for the first few days. Also, for simplicity, I'm not taking transaction fees in consideration, which may have an impact on your gains.
{% endhint %}

At this point, the system is primed, it's time to sit down and profit.

## Farming  Results

### Daily routine

Once the system is fully bootstrapped, here's the daily routine you'll have to follow:

* harvest SPIRIT tokens from MAI-WFTM pool on SpiritSwap
* harvest rewards from Liquid Driver staking pool
* harvest rewards from SpookySwap staking pool
* deposit the SPIRIT from SpiritSwap and the linSPIRIT from Liquid Driver into the pool on BeethovenX
* deposit the SPIRIT-linSPIRIT LP token on Liquid Driver
* stake your BOO on SpookySwap to get xBOO
* stake your xBOO to farm WFTM
* swap your SPELL for WFTM
* swap 66% of your WFTM for DAI
* deposit the DAI generated on Beefy to get mooScreamDAI
* deposit the mooScreamDAI tokens on Mai Finance
* borrow MAI and keep a CDR of 200% (50% of what you deposited)
* provide liquidity for the MAI-WFTM pool on SpiritSwap

### Raw results month after month

| day |  MAI-WFTM | linPIRIT-SPIRIT |   LQDR  |  xBOO  | mooScreamDAI | MAI debt |
|-----|-----------|-----------------|---------|--------|--------------|----------|
|  30 | 1,000.004 |         130.010 |   3.281 |  0.026 |        0.005 |    0.002 |
|  60 | 1,000.039 |         256.218 |  13.014 |  0.210 |        0.041 |    0.021 |
|  90 | 1,000.140 |         383.220 |  29.369 |  0.712 |        0.147 |    0.074 |
| 120 | 1,000.349 |         511.436 |  52.538 |  1.698 |        0.364 |    0.182 |
| 150 | 1,000.708 |         641.302 |  82.741 |  3.338 |        0.738 |    0.369 |
| 180 | 1,001.268 |         773.275 | 120.224 |  5.810 |        1.323 |    0.661 |
| 210 | 1,002.081 |         907.835 | 165.263 |  9.295 |        2.175 |    1.088 |
| 240 | 1,003.207 |       1,045.486 | 218.165 | 13.984 |        3.360 |    1.680 |
| 270 | 1,004.710 |       1,186.759 | 279.268 | 20.075 |        4.947 |    2.473 |
| 300 | 1,006.659 |       1,332.316 | 348.947 | 27.773 |        7.014 |    3.507 |
| 330 | 1,009.130 |       1,482.451 | 427.613 | 37.296 |        9.645 |    4.823 |
| 360 | 1,012.205 |       1,638.095 | 515.717 | 48.870 |       12.935 |    6.467 |

### Day 365

After a complete year of farming the syste, you would get

* $1,012.782 worth of MAI-WFTM on SpiritSwap
* $1,664.608 worth of linSPIRIT-SPIRIT on Liquid Driver
* $531.353 worth of LQDR staked on Liquid Driver
* $51.015 worth of xBOO on SpookySwap
* $13.554 worth of mooScreamDAI on Mai Finance in a vault
* $6.777 worth of MAI debt

Considering an initial investment of $1,000 this would be equivalent to an APY of 227.096%

### Small tweaks to the strategy

If you want to get a lower risk exposure, you can possible start with your initial investment being $1,000 worth of mooScreamDAI in a vault, borrow $500 worth of MAI and swaap 50% for WFTM to get the starting block on SpiritSwap. This will considerably lower your risk of loosing part of your initial in case the price of FTM goes down too much.

Currently, the highest rate is given by the SpiritSwap pool, so a possibible simplification of the loop would be to simply swap all the LQDR tokens you get on Liquid Driver for more MAI-WFTM.

## Disclaimer

This guide is a theoretical version of something you could implement on Fantom. When we're exposing loops in our tutorials, we're actually trying to never dump tokens and always try to find the best way possible to use everything we collect. This is a good way to keep price rising since farming and dumping a token usually resuslts in the price of the farmed token to go down, making the yields less and less attractive. If everyone was keeping their farmed tokens, their price would only go up with time.

In any case, the guide is also based on a lot of assumptions (price don't change, reward rates don't change) and doesn't count transaction fees, so if you want to implement this type of closed loop, make sure to be profitable at the end of the day, or compound your gains only once a week. And as usual, DYOR!

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}
