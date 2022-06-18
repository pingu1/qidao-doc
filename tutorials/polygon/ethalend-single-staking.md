---
description: >-
  Most people will use their MAI loan to buy other assets. However, some very
  interesting strategies can be used with MAI directly, and the one using
  Ethalend is a very good one.
---

# MAI single-staking with Ethalend

## Intro

One of the missions of this website and the collection of tutorials that are offered is to make DeFi user friendly by demystifying the most complex protocols. This vision is also shared by the team behind [Ethalend](https://www.ethalend.org/), and this guide will present a perfect way to use this platform in conjunction with Mai Finance to amplify your stable farming yields.

## Ethalend presentation

![](../../.gitbook/assets/Ethalend-1.png)

### What is Ethalend

Ethalend is a composable protocol that abstracts the complexity in DeFi to provide algorithmically optimal yield. It is not a yield aggregagor, but a yield optimizer. You will be able to deposit your assets on the platform, and the algorithm in charge of the pool in which you deposit your assets will actually invest them in the best way possible. Yields are then distributed in the native token of Ethalend, the ETHA token, as well as some partner tokens, including Qi from Mai Finance that you can get by depositing your MAI in the MAI-USDT eVault. You can read more about Ethalend via their [official documentation](https://docs.ethalend.org/), or by reading this excellent [interview of the co-founder](https://ambcrypto.com/un-complicating-defi-an-interview-with-ethalend-co-founder-danny-b/).

### Create your Ethalend wallet from your web3 wallet

One of the very interesting things about Ethalend is that the application is using a dedicated on-chain wallet that is not linked to your web3 wallet. This can be considered as

* an advantage since all contract risk is limited to what is exposed in this private wallet. Also, some interaction between the Ethalend application and the private wallet are directly included into the platform use, which may save you some transaction fees. As a side note, the ETHA smart wallet is non-custodial, meaning that only you will have access to the wallet, it's not like a master centralized wallet controlling the share corresponding to your wallet.
* a disadvantage, because it adds complexity in your routine, and the ETHA smart wallet isn't compatible with physical devices.

It's going to be up to you to decide if the pros are bringing enough value to surpass the cons. When you are ready to create your wallet, simply click on the `Create Wallet` button in the top right corner of your screen.

![Create your ETHA smart wallet](../../.gitbook/assets/Ethalend-2.png)

There you go, ready to use the protocol!

## Strategy overview

This strategy can be added to your bucket of relatively safe strategies since it will be using stable coin farming at its root, and additional yields will be provided thanks to more volatile assets from the rewards of the stable position.

### MAI single staking and gains

![Ethalend MAI-USDT eVault as of November 2021](../../.gitbook/assets/Ethalend-3.png)

One of the big advantages of Ethalend, and one of the key feature that allows DeFi simplification, is that you don't need to provide a LP (**L**iquidity **P**roviding) pair composed of 2 assets with a ratio of 1:1. The algorithm that manages the pool (or eVault in our case) will do it automatically for you. Also, once you deposit your assets in a eVault, they will be re-routed automatically to the best protocol that will maximize your yield. The reward tokens will be farmed and converted for you regularly.

![Depositing 100 MAI in the MAI-USDT eVault from our MetaMask wallet](../../.gitbook/assets/Ethalend-4.png)

As you can see, details of the rewards are displayed in the right part of the screen. The ETHA rewards are not displayed, but you get an estimation of the Qi rewards associated with your deposit. If you scroll down the page, you will also get a good understanding of the underlying strategy that is using QuickSwap in our case. QUICK rewards will be converted into Qi rewards. ETHA rewards are minted by the protocol to incentive you to use their platform instead of QuickSwap.

{% hint style="info" %}
Pay attention to the 0.10% withdrawing fees. As of writing, with a deposit of 100 MAI, I will have to pay a 0.1 MAI exit fee, which roughly corresponds to 10 days of farming in the eVault. Make sure you understand this point before investing anything.
{% endhint %}

### Staking ETHA: Ethalend or QuickSwap

The main reward you will get by lending your MAI on Ethalend will be paid in ETHA, the native token from Ethalend. One of the main advantage of Ethalend is that you will be able to single stake your ETHA tokens directly on the platform and magnify your yields.

![Staking your ETHA on Ethalend directly](../../.gitbook/assets/Ethalend-5.png)

As you can see, the best option is to deposit the ETHA you earned in the ETHA-QUICK pool. Because of the nature of the 2 assets (very volatile), the reward is really high. You can possibly reduce the impermanent losses by depositing your ETHA in the ETHA-USDT pool if you prefer. In both cases, you will be rewarded with QUICK tokens. And of course, if you are really bullish on ETHA, you can stake your rewards in the ETHA pool for additional ETHA.

The staking vaults on Ethaland are actually a convenience offered by Ethalend. When you deposit your tokens in the pool, the balancing algorithm will sell a few of the deposited tokens to buy the other side of the LP pair, and use this pair in QuickSwap. As a side note, you can totally do this manually: claim your ETHA tokens, withdraw in your web3 wallet, sell 50% for QUICK tokens, create some LP tokens, and deposit them in the QuickSwap pool:

![QuickSwap pools for ETHA as of November 2021](../../.gitbook/assets/Ethalend-6.png)

{% hint style="info" %}
QuickSwap promotes a 223.1% APY on the ETHA-QUICK pair, while Ethalend displays a 116.73% APR on the same pair. This is due to the difference between APY (**A**nnual **P**ercentage **Y**ield, or autocompounded rewards) and APR (**A**nnual **P**ercentage **R**evenue, or rewards without auto-compounding). The 2 percentages are actually exactly the same, so it doesn't matter which platform you chose to use your ETHA tokens.
{% endhint %}

### The dQUICK Mai Vault

The best way to use the QUICK rewards you will get from staking your ETHA is to convert them into dQUICK. dQUICK can be created in the Dragon's Lair on QuickSwap. It's the way QuickSwap is incentivizing users to stake their QUICK by rewarding them with additional QUICK: by locking your QUICK tokens on QuickSwap, you will earn extra tokens.

![Dragon's Lair APY on QuickSwap as of November 2021](../../.gitbook/assets/Ethalend-7.png)

{% hint style="info" %}
The dQUICK APY varies a lot between 20% and 40%, depending on the amount of QUICK tokens that are actually staked on the Platform
{% endhint %}

But one of the best thing about dQUICK is that it's a "proof of deposit" token that can be used on Mai Finance as a collateral. This means that, after you deposited your QUICK rewards from Ethalend on QuickSwap and received dQUICK, you can head to Mai Finance and deposit the dQUICK tokens into a dQUICK Vault to borrow MAI against them.

![dQUICK Vault on Mai Finance as of November 2021](../../.gitbook/assets/Ethalend-8.png)

A few things about the dQUICK vaults:

* They have a liquidation ratio of 130%, which means you will be able to borrow a lot of MAI against your dQUICK tokens. However, if you want to collect borrowing rewards too, you will need to keep a CDR (**C**ollateral to **D**ebt **R**atio) between 155% and 400%. This is a good idea since the QUICK token is pretty volatile, and as a general rule, this website strongly promote a CRD 100% above the liquidation ratio (or 230% for dQUICK).
* dQUICK Vaults are among the ones with the highest APR when you borrow MAI against dQUICK. As of writing, you can get up to 39.40% APR paid in Qi tokens based on the amount of MAI you will borrow against your MAI.

You can already see that, providing dQUICK is very interesting since you will have an asset that gets compounded QUICK rewards from QuickSwap, you will get Qi rewards for your loan, and you will be mint MAI that can then be added back into the eVault on Ethalend, increasing your stable farming position.

### What to do with your Qi rewards

This subject is explained in [a dedicated article](what-to-do-with-qi-on-polygon.md). For the sake of this tutorial, we will simply deposit your Qi in the Qi-BAL pool on Balancer to benefit from a solid APR, paid in additional Qi and BAL tokens that you can compound in the exact same pool.

![State of the Qi-BAL pool on Balancer as of November 2021](../../.gitbook/assets/Ethalend-9.png)

## Bootstrapping the system

![](../../.gitbook/assets/Ethalend-10.png)

What follows is a simulation made with an initial investment of $100 worth of MAI that you can either borrow from an existing vault, or buy from a DEX platform. It assumes that all current APRs and APYs stay the same over the span of 1 year, and that all tokens keep the same price, which will (of course) never be the case.

### Day 1

On day 1, you will deposit your MAI on Ethalend in the MAI-USDT pool, then you will get the reward in both Qi and ETHA at the end of the day.

| Reward type        | Value in dollars |
| ------------------ | ---------------- |
| Mai on Ethalend    | 100.000          |
| Qi+BAL on Balancer | 0.032            |
| ETHA on Ethalend   | 0.070            |
| dQUICK on Mai      | 0.000            |
| debt on Mai        | 0.000            |

### Day 2

On day 2, you can stake your ETHA from day 1 on Ethalend, which will generate QUICK rewards that you can then convert to dQUICK on QuickSwap, deposit on Mai Finance, and you will be able to borrow MAI against these tokens. You can also deposit your Qi in the Balancer pool. At the end of day 2 you will get:

| Reward type        | Value in dollars |
| ------------------ | ---------------- |
| Mai on Ethalend    | 100.000          |
| Qi+BAL on Balancer | 0.065            |
| ETHA on Ethalend   | 0.141            |
| dQUICK on Mai      | 0.000            |
| debt on Mai        | 0.000            |

From there, the system is bootstrapped, and you will be able to grow your stable position of MAI, as well as get rewards in Qi, BAL, ETHA and dQUICK. Note that some values are too low to be significant at this point, and since you won't be able to borrow less than 0.01 MAI, you will have to accumulate dQUICK for 14 days before being able to borrow MAI.

## Farming Results

### Daily routine

The daily farming routine is composed of

* Harvesting the Qi and ETHA rewards from the MAI-USDT pool on Ethalend
* Deposit the Qi tokens in the Balancer pool on Balancer
* Deposit the ETHA tokens in the ETHA-QUICK pool on Ethalend
* Harvest QUICK rewards from the ETHA-QUICK pool on Ethalend
* Convert QUICK into dQUICK on QuickSwap
* Deposit dQUICK into the dQUICK vault on Mai Finance
* Borrow MAI from the dQUICK vault on Mai Finance
* Deposit additional MAI borrowed in the MAI-USDT pool on Ethalend

Additionally, you will be able to harvest and compound the Qi and BAL rewards weekly.

### Raw results month after month

Below are the raw results at the end of each month:

| day | Mai on Ethalend | Qi on Balancer | ETHA on Ethalend | dQUICK on Mai | MAI debt |
| --- | --------------- | -------------- | ---------------- | ------------- | -------- |
| 30  | 100.046         | 1.015          | 2.186            | 0.099         | 0.049    |
| 60  | 100.196         | 2.116          | 4.303            | 0.406         | 0.203    |
| 90  | 100.453         | 3.315          | 6.424            | 0.926         | 0.463    |
| 120 | 100.819         | 4.624          | 8.553            | 1.666         | 0.833    |
| 150 | 101.297         | 6.058          | 10.690           | 2.631         | 1.315    |
| 180 | 101.892         | 7.632          | 12.838           | 3.828         | 1.914    |
| 210 | 102.606         | 9.361          | 15.001           | 5.263         | 2.632    |
| 240 | 103.443         | 11.264         | 17.179           | 6.945         | 3.473    |
| 270 | 104.406         | 13.360         | 19.377           | 8.881         | 4.441    |
| 300 | 105.501         | 15.671         | 21.597           | 11.079        | 5.540    |
| 330 | 106.731         | 18.220         | 23.841           | 13.548        | 6.774    |
| 360 | 108.100         | 21.032         | 26.113           | 16.297        | 8.149    |
| 365 | 108.343         | 21.528         | 26.495           | 16.783        | 8.392    |

### Day 365

At the end of one year, you would have

* $108.343 worth of MAI in the MAI-USDT pool on Ethalend
* $26.495 worth of ETHA in the ETHA-QUICK pool on Ethalend
* $21.528 worth of Qi in the Qi-BAL pool on Balancher
* $16.783 worth of dQUICK in the dQUICK vault on Mai Finance
* $8.392 worth of MAI debt on Mai Finance

This sums up as $173.149 worth of assets, and an outstanding debt of $8.392, which corresponds to an equivalent APY of 64.757%. This is achieved with an initial investment of $100 worth of MAI and using a stable pool as basis for farming. Note that transaction fees haven't been taken in account, but may influence the final result. This is also assuming you are compounding daily for 1 complete year.

## Disclaimer

Everything presented in this tutorial is educational content made to illustrate how you can use your MAI without selling them, and still generate an APY of more than 60% using different protocols as lego bricks. However, this tutorial should not be considered as financial advice.

Also, the strategy here is presenting a closed loop that doesn't sell any token and each system is feeding the next one. However, as you can see, the dQUICK final position isn't very high, and the MAI loan will probably not generate a lot of Qi. You can probably achieve the same equivalent APY (if not better) by selling the QUICK rewards granted by the ETHA-QUICK pool, buy MAI and add it to your MAI-USDT position.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
