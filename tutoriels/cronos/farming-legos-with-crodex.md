---
description: >-
  Farming rewards with stable coins usually have low rates. Let's see how you
  can increase your gains with a new investment loop.
---

# Farming Legos with CroDex

Yield farming can be easy. You have 2 tokens, you combine them in a LP (**L**iquidity **P**roviding) pair, you deposit the LP token in a pool and you start getting swap fees and most of the time, rewards paid in the native token of the farm you are using. Most people will simply sell the reward for whatever asset they are looking for, which is most of the time, totally valid, but very far from an optimized solution. Today, we will see how you can profit from the very high APR (**A**nnual **P**ercentage **R**ate) proposed on Cronos on several DApps, which will transform a 30% APR on stable coin into a much higher rate.

![](../../.gitbook/assets/crodex-lego-1.png)

## CroDex

### Farming with MAI

Even if the lending application of Mai Finance is not deployed on Cronos yet, it is already possible to bridge MAI from other chains. One of the reason to do this is because there are not many MAI on Cronos, meaning that any application that proposes farming with MAI will also provide high APRs. This is the case of CroDex, currently the only place with MAI liquidity on Cronos. For this guide, we will use the MAI-USDC pool on CroDex to lower the risk of Impermanent Loss on your initial investment, but you can increase your gains by farming MAI-CRO.

![MAI-USDC LP pool on CroDex as of December 2021](../../.gitbook/assets/crodex-lego-2.png)

{% hint style="info" %}
Whenever you select an application to farm yields, it's important to note if the reward is displayed as an APR (**A**nnual **P**ercentage **R**ate) or APY (**A**nnual **P**ercentage **Y**ield). The latter assumes that all rewards you get are compounded daily for one complete year. In our example, 30% APR on the MAI-USDC pair corresponds to a 34.97% APY.

If you compare it to the MAI-USDC pool on Mai Finance, the APR given is 20.18% on Polygon, 22.10% on Fantom, and the MAI-av3CRV pool on Avalanche proposes 23.24% APR. CroDex proposes the best rate on MAI stable across all chains!
{% endhint %}

CroDex will pay you with their native token, the CRX. As of December 2021, 1 CRX = 127.56 USDC

### Single Staking CRX

This is where it gets interesting. CroDex has 2 different pools where you will be able to stake your CRX tokens for additional rewards. You can either stake to get more CRX, but we will use the pool where staking CRX will reward you with wCRO tokens. wCRO is the wrapped version of CRO, the gas token of the Cronos network.

![Single staking CRX on CroDex as of December 2021](../../.gitbook/assets/crodex-lego-3.png)

You can already see that you could very well sell your CRX for more MAI-USDC LP tokens and get almost 35% APY on the stable pair, but it's clearly better to stake your CRX to get CRO. Not only it can be used to pay transaction fees, but you can also farm MAI-CRO on CroDex. And the more CRX you get over time, the more CRO you'll get if you stake your CRX. But in this guide, we will explore Cronos a little more!

## CRYSTL Finance

CRYSTL Finance used to be known as Polycrystal on Polygon. It's a goose fork that proposes LP pair vaults and single staking pools, and it works exactly like Beefy Finance. We will be using both for our strategy.

### Farming CRYSTL with CRX-WCRO

We will be using the CRO tokens produced by the CRX staking to swap 50% of the reward into more CRX andcombine these two tokens into a CRX-WCRO pair on CroDex, then deposit the LP token in a vault on Crystl Finance. This will get you a high APY that will be compounded.

![Farming CRX-WCRO on Crystl Finance as of December 2021](../../.gitbook/assets/crodex-lego-4.png)

The rates displayed is an APY. A 1.21k% APY corresponds to a 258.17% APR, but you can also get the estimated daily gains directly on the vault info, and your CRX-WCRO farming will currently get you 0.71% daily gains. It's very important that you keep track of the daily reward because we will extract this portion of our LP position and break it into separate tokens. The CRX will be re-staked on CroDex to get more CRO tokens, and the CRO will be swapped for CRYSTL. Please also note that there is a withdraw fee for the gains we will extract each day.

### Single staking CRYSTL

With the CRYSTL token obtained in the previous step, you will be able to get USDC from the single-staking pool of CRYSTL Finance. Simply stake your CRYSTL token and you will be paid in USDC with a pretty high APR.

![Staking CRYSTL for USDC or SALEM as of December 2021](../../.gitbook/assets/crodex-lego-5.png)

Then you can simply swap 50% of the farmed USDC for MAI, and add back to your original position on CroDex.

Alternatively, we can use the same approach as above and stake CRYSTL tokens to earn SALEM tokens, which is the native token of Salem Finance.

## Salem Finance

Salem Finance is another goose fork where you'll be able to farm the SALEM token. Most LP pools have a deposit fee, but we will actually not use the LP farms since CRYSTL Finance is already giving us the SALEM tokens we need. Instead, we will stake SALEMs in the pools to earn additional WCRO with, once again, a very high APR.

![Staking SALEM for WCRO as of December 2021](../../.gitbook/assets/crodex-lego-6.png)

The (w)CRO token being the gas token of Cronos, it does have a lot of utility. You can also bridge it to the main Crypto.org chain if you want. In our case, and because we want to close our investment loop, we can simply sell the gains from Salem Finance and buy more USDC and MAI.

## Farming strategy

You can already see that with only 3 protocols, you have several options:

* Farming MAI-USDC to get CRX, staking CRX to get WCRO, selling WCRO for more MAI-USDC
* Farming MAI-USDC to get CRX, staking CRX to get WCRO, farming CRX-WCRO to get CRYSTL, staking CRYSTL to get USDC, swapping USDC for more MAI-USDC
* Farming MAI-USDC to get CRX, staking CRX to get WCRO, farming CRX-WCRO to get CRYSTL, staking CRYSTL to get SALEM, staking SALEM to get WCRO, selling WCRO for more MAI-USDC

For the rest of this guide, we will focus on the last strategy, which is the most complex and requires many manipulations, but it's also the one that offers the best overall result. Feel free to apply the one you prefer depending on your risk acceptance.

![](../../.gitbook/assets/crodex-lego-7.png)

### Bootstrapping the system

What follows is a simulation made with an initial investment of $1,000 worth of MAI-USDC LP tokens, and the current APRs/APYs presented in this document as of December 2021. Of course, rates and prices will change over time, so this simulation is only valid at the time of writing, and the simulation will only provide an estimation of what you could potentially get if you set up this system.

### Day 1

You deposit your MAI-USDC on CroDex in the appropriate pool and get 30% APR on it. At the end of the first day, once you collect your CRX rewards, you would have

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM | WCRO  |
| -------- | ---------- | -------- | ------ | ----- | ----- |
| 1,000.00 | 0.822      | 0.000    | 0.000  | 0.000 | 0.000 |

### Day 2

Your staked CRX is generating WCRO. You can harvest the reward and swap 50% into more CRX in order to create a CRX-WCRO L pair that you can then deposit on CRYSTL Finance. At the end of the second day you would have

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM | WCRO  |
| -------- | ---------- | -------- | ------ | ----- | ----- |
| 1,000.00 | 1.644      | 0.002    | 0.000  | 0.000 | 0.000 |

### Day 3

The CRX-WCRO pair locked in the CRYSTL Finance vault generated additional LP token. You will have to extract the daily gain and pay a 0.1% fee, and break the extracted LP portion into CRX and WCRO tokens. You can simply restake the CRX on CroDex, and swap the WCRO into CRYSTL. This can be done on [CroDex using the swap feature](https://swap.crodex.app/#/swap?outputCurrency=0xCbDE0E17d14F49e10a10302a32d17AE88a7Ecb8B). At the end of the day, you would have

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL  | SALEM | WCRO  |
| -------- | ---------- | -------- | ------- | ----- | ----- |
| 1,000.00 | 2.466      | 0.005    | 0.00003 | 0.000 | 0.000 |

{% hint style="info" %}
Note that the rewards on CRYSTL are very small and it may not be interesting to harvest the reward from day 1. This simulation is still displaying the rewards you should get and will assume you still compound daily, but this is done to simplify the results. Make sure you don't spend all your reward into transaction fees, and it may be more interesting to compound only weeekly of the first few weeks.
{% endhint %}

### Day 4

Your CRYSTL reward from Crystl Finance can be staked in order to earn SALEM tokens. At the end of the 4th day you'd get

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL  | SALEM     | WCRO  |
| -------- | ---------- | -------- | ------- | --------- | ----- |
| 1,000.00 | 3.288      | 0.010    | 0.00011 | 0.0000002 | 0.000 |

### Day 5

Final bootstrapping day when you will harvest the rewards from Salem Finance. The WCRO reward can be swapped for more MAI-USDC. However, as you can notice, the value of the reward is so small that you won't be able to harvest the WCRO from Salem Finance before Day 50 or so.

## Farming results

### Daily routine

Once the system is fully prepared, here's your daily routine

* harvest CRX from the MAI-USDC pool
* harvest the WCRO reward from the single staking pool on CroDex
* swap 50% of the WCRO reward for more CRX on CroDex, and create some CRX-WCRO LP token
* deposit your additional CRX-WCRO token on CRYSTAL Finance
* withdraw a portion of CRX-WCRO corresponding to your daily reward
* break the LP token into CRX and WCRO on CroDex
* stake the CRX into the single staking pool on CroDex that gets WCRO rewards
* swap the WCRO for CRYSTL on CroDex
* stake the CRYSTL token on Crytl Finance to get SALEM tokens
* harvest the SALEM token
* single stake the SALEM token on Salem Finance
* harvest the WCRO token from Salem Finance
* swap the WCRO for MAI and USDC and create more LP pair
* deposit the new MAI-USDC pair in the appropriate pool on CroDex

### Raw results month after month

| day | MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM  |
| --- | -------- | ---------- | -------- | ------ | ------ |
| 30  | 1,000.00 | 25.583     | 0.600    | 0.104  | 0.004  |
| 60  | 1,000.00 | 50.819     | 1.830    | 0.682  | 0.059  |
| 90  | 1,000.04 | 76.736     | 3.315    | 1.941  | 0.260  |
| 120 | 1,000.14 | 103.424    | 4.922    | 3.970  | 0.729  |
| 150 | 1,000.41 | 130.935    | 6.606    | 6.816  | 1.594  |
| 180 | 1,001.93 | 159.307    | 8.352    | 10.515 | 2.994  |
| 210 | 1,001.87 | 188.578    | 10.156   | 15.094 | 5.070  |
| 240 | 1,003.39 | 218.789    | 12.019   | 20.584 | 7.969  |
| 270 | 1,005.71 | 249.988    | 13.942   | 27.014 | 11.843 |
| 300 | 1,009.10 | 282.227    | 15.929   | 34.414 | 16.848 |
| 330 | 1,013.82 | 315.569    | 17.982   | 42.817 | 23.147 |
| 360 | 1,020.23 | 350.084    | 20.105   | 52.256 | 30.906 |

### Day 365

After a complete year of farming this system, you would have

* $1,021.49 worth of MAI-USDC on CroDex
* $355.96 worth of CRX single staked on CroDex
* $20.47 worth of CRX-WCRO deposited on CRYSTL Finance
* $53.93 worth of CRYSTL single staked on CRYSTL Finance
* $32.353 worth of SALEM single staked on Salem Finance

The WCRO from Salem Finance is actually included as the additional MAI-USDC position since it's fully sold to increase this pair.

This means that with an initial investment of $1,000, at the end of the year you would have $1,484.45 across all apps, for a total APY of 48.45%. And remember that this is done by farming only a stable pair as the root of the strategy. It's also good to note that the only token that is swapped over time is the CRO token.

### Alternative using Mai Finance

The Mai Finance application doesn't support vaults on Cronos, because tokens on Cronos don't have Chainlink Oracles yet. It's expected that during the first quarter of 2022, Chainlink will add oracles on Cronos, and you will be able to deposit your WCRO tokens in a Vault to borrow the MAI stable coin. This means that the strategy above can be modified to deposit WCRO and use MAI instead of selling the WCRO tokens, which will slightly increase your final reward rate.

![WCRO vault on Mai Finance (emulation)](../../.gitbook/assets/crodex-lego-8.png)

## Disclaimer

This guide was written to showcase that you can increase your reward rate withouth dumping the tokens that you farm. It's not simple to find the right fits when you're building feedback loops, but it's definitely feasable, and you will most of the time rewarded if you can find the right combo. However, this guide was written only to demonstrate how you can do that, and not to build a similar system. All transaction fees were purposedly discarded, and some rewards will not last for a complete year, meaning that you may want to consider more simple loops for your personal investments. However, CroDex is a very good starting point for that type of system.

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}
