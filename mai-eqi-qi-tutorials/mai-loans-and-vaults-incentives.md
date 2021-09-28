---
description: >-
  This article is a detailed explanation of how you can use Mai Finance to
  borrow MAI at 0% interest, and get paid to do so, transforming your 0%
  interest loan into a negative interest loan.
---

# MAI loans and Vaults incentives

## Intro

The core business of Mai Finance is a lending platform. Instead of selling their crypto to buy other assets, people are able to lock their funds on Mai Finance and borrow against them. This presents the opportunity to keep high value assets \(WBTC, WETH ...\) while still being able to get other assets and farm yields. In that case, the loan is used to generate revenue, while the collateral is gaining value.

One of the other big advantage of using Mai Finance is that there's no repayment schedule. In other words, you borrow MAI stable coin against your crypto, you don't pay any interests, and you can repay your debt whenever you want. See the different articles on [debt management](../debt-management-tutorials/debt-repayment-why-and-when.md) for more details. The only fee that you would ever pay is a repayment fee corresponding to 0.5% of the money you borrowed that you pay when you repay your loan, and that is taken out of your collateral.

As an example, if you deposited $200 worth of WETH to borrow $100 worth of MAI, when you repay your loan you would have to pay a fee of $0.50 directly taken out of your WETH deposit.

If that wasn't already an amazing opportunity, the Mai Finance team introduced in September 2021 Vault incentives paid in Qi, the native token of Mai Finance. In other words, by depositing your assets on Mai Finance in a vault to borrow MAI, you will also get paid to do it. This articles presents in details how this functionality works.

## Vaults - What they are and how they work

### Vault creation

On Mai Finance, vaults are special storages where one can deposit their assets. Currently, there are 10 types of vaults:

![The different vault types you can create on Mai Finance](../.gitbook/assets/image%20%281%29.png)

There are 2 different types of vaults:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

and

* camWETH
* camWBTC
* camWMATIC
* camAAVE

The first 6 vaults in the list are for simple assets while the 4 last ones are for camTokens. camTokens are compounding AAVE market tokens, a representation of a deposit that you could have done on AAVE and then deposited on the yield pools of Mai Finance. While you assets is generating yields on AAVE \(and while the rewards are automatically compounded by the yield pool\), you can still borrow MAI stable coins against these tokens.

As a side note, you can see on the screenshot above that the creation page shows some very important informations:

* MAI available: this corresponds to the maximum debt ceiling, the maximum number of MAI that can be minted from vault deposits.
* Min Coll. ratio: this is the minimum Collateral to Debt ratio \(CDR\) for that vault
* Vault incentives APR

### Understanding Debt Ceiling

The maximum number of MAI that one can mint on a specific vault depends on how much assets is deposited on that vault. Debt ceiling are implemented in order to make sure that the market isn't flooded with MAI in a very short time, which may affect the price of the stable coin.

As an example, if a big institution would deposit 5,000 WBTC at once and was able to borrow $100,000,000 worth of MAI, swapping the totality for more WBTC, this could drive the price of MAI down so much that the price would deviate too much from its peg, putting the whole platform at risk. Debt ceiling is the mechanism that prevents this from happening: there's a maximum amount of MAI that can be minted for a given vault type.

When the debt ceiling is reached, the time at which there aren't any more available MAI to mint is recorded, and the system automatically increases the debt ceiling after 48 hours. This is considered enough time for the MAI price to stabilize \(in case of high sell pressure following a big sell off of MAI\).

This means that for 48h, nobody will be able to borrow more MAI from a vault that reached its debt ceiling, unless a debt is repaid.

As a side note, the more MAI on the market, the more stable the price is. Indeed, a massive sell of MAI is less invasive if there are more MAI in circulation.

* If someone sells 1,000 MAI while there are only 10,000 MAI in circulation, the sell corresponds to 10%
* If someone sells 1,000 MAI while there are 10,000,000 MAI in circulation, the sell corresponds to 0.01%

Hence, the debt ceiling isn't increased incrementally, but exponentially: the more MAI in circulation, the less impact a big sell would have, so the debt ceiling can be increased by a lot more.

{% hint style="info" %}
When you borrow MAI, it can happen that the maximum amount of MAI that you can borrow is capped by the debt ceiling, regardless of the current value of your collateral and the current amount of MAI you already borrowed. When that's the case, you may wait up for 48h before you can actually borrow more MAI.
{% endhint %}

### Understanding Collateral to Debt Ratio

The CDR, or **C**ollateral to **D**ebt **R**atio is the ratio between the value of the deposited assets in your vault compared to the amount of MAI you borrowed.

As an example, if you deposited $200 worth of WETH to borrow $100 worth of MAI, your CDR would be

$$
CDR=\frac{CollateralValue}{DebtValue}=\frac{200}{100}=200\%
$$

Maintaining a CDR above 100% means that, at any point, there are more collateral than debt. This is mandatory to ensure that the MAI stable coin is over-collateralized, and is one of the foundations of the Mai Finance tokenomics. You can get more details from the official [Mai Finance documentation](https://docs.mai.finance/stablecoin-economics).

Each vault type has a minimum CDR ratio accepted, a threshold under which the vault is considered at risk because the borrowed amount may not be backed by enough collateral. At this point, anyone can liquidate the vault, meaning a part of the debt is repaid by the liquidator that can then get a portion of the deposited collateral in repayment. Once again, you can find more details about liquidation process in the official documentation.

When you borrow MAI against a given collateral, you will get some hints on what's the maximum amount of MAI you can borrow, and what would be the impact on your health ratio depending on the amount borrowed, as you can see in the screenshot bellow:

![Health mitigation depending on borrowed amount](../.gitbook/assets/image%20%284%29.png)

It's very important to keep an eye on your CDR and keep a healthy ratio to

* prevent liquidation
* increase the health of the whole Mai Finance platform by ensuring the MAI volume in circulation is properly backed

The "healthy" CDR, as defined by the Mai Finance team, is between 25% and 270% above the minimum CDR value. As a side note, you can also check our strategy guides to see how you can use conservative/aggressive CDRs to [invest](../investment-tutorials/leverage-aave-tokens.md#examples-with-numbers) in other projects, or [repay your debt](../debt-management-tutorials/debt-repayment-how.md#repayment-using-your-collateral) using your debt.

## Vault incentives

{% hint style="info" %}
**ATTENTION**: Vaults incentives are not out yet. This section is a guess game while we are waiting for the official documentation. The estimations calculated in this section are "napkin maths" based on leaked info from the official team, and voted emission rate. Hence, this section will certainly be rewritten when Vaults incentives are out on Sunday September 19th 2021. There is absolutely no guarantee that these estimations are correct.
{% endhint %}

### Understanding Vaults incentives APRs

In September 2021, Mai Finance introduced vault incentives. This is a reward allocated by the Mai Finance platform to anyone borrowing MAI and participating in the growth of the platform.

Each Vault type \(among the 10 different types\) receives 0.05 Qi per block, that is then distributed between all the users who have a healthy Collateral to Debt Ratio. The APR of the vault is defined by the current amount of MAI borrowed.

As an example, Ben and Kila are 2 friends who deposited their ETH in the WETH vaults on Mai Finance.

* Ben deposited the equivalent of $2,000 worth of ETH and borrowed 1,000 MAI
* Kila deposited the equivalent of $10,000 worth of ETH and borrowed 6,000 MAI

The current amount of MAI borrowed by users who deposited WETH in the vault is 1,000,000 MAI.

Both Ben and Kila qualify for the vault incentives because Ben has a CDR of 200% and Kila a CDR of 166.67%. Ben, with his loan, owns 0.1% of the total amount borrowed, while Kila owns 0.6%.

The total amount of Qi allocated to the WETH vault \(or any vault\) is

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86,400 is the number of seconds in a day, and on Polygon, the block time is 2 seconds, meaning that the expected number of blocks every day is 86,400 / 2 = 43,200. Hence, the emission for each Vault is 2,160 Qi / day.

**Note:** Block time has increased lately and is around 2.6 seconds. However, all APRs and APYs displayed on all apps are assuming a block time of 2 seconds. Please DYOR and check the current [block time on PolygonScan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Hence, if the state of the Vault remains the same, Ben will get 0.1% of the 2,160 Qi distributed, while Kila will get 0.6% of the granted reward.

* Ben will get 2.16 Qi every day, which is a daily reward of 0.216%, or an APR of 78.84%
* Kila will get 12.96 Qi every day, which is also a daily reward of 0.216%, or an APR of 78.84%

On a side note, 2,160 Qi for 1,000,000 MAI is a daily reward of 0.216%, or 78.84%, which is the Vault's APR.

{% hint style="info" %}
It's easy to see that the Vault's APR is directly linked to the amount of MAI borrowed. The more MAI is borrowed, the lower the APR. As a side note, the amount of MAI that can be borrowed is also capped by the debt ceiling, which is increased with the demand for MAI.
{% endhint %}

As a verification, we can calculate the theoretical APR for the MATIC vault based on numbers published on the [analytics page](https://app.mai.finance/analytics) on Mai Finance. The amount of MAI borrowed from the MATIC vault is 799,328. The reward is 216 Qi per day for that vault. That corresponds to a APR of

$$
APR=\frac{QiReward*Qi_{Price}}{MAI_{borrowed}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

This corresponds more or less to the APR of the MATIC Vault, as displayed in the following screenshot:

![APR of a MATIC vault on Mai Finance after the launch of Vault rewards](../.gitbook/assets/image%20%2821%29.png)

### Calculating starting vaults' APRs

With the same data as the example above, it's possible to calculate the starting APRs for all vaults

| Vault type | Starting APR |
| :--- | :--- |
| MATIC | 44.29% |
| WETH | 24.03% |
| LINK | 27.41% |
| AAVE | 164.14% |
| CRV | 159.96% |
| WBTC | 36.92% |
| camWETH | 25.46% |
| camWMATIC | 44.33% |
| camAAVE | 167.23% |
| camWBTC | 47.38% |

{% hint style="info" %}
As you can see, some vaults will generate more rewards than others. Also, you can see that it's super important to deposit your assets as soon as possible to benefit from high APRs before the debt ceiling is increased and more loan is taken \(lowering the APR\).

You can also see that if you keep your loan for one year of more, the 0.5% repayment fee will easily be compensated by the reward program.
{% endhint %}

### Incentives distribution

Rewards allocated by the vault incentives will be distributed the same way as for staked Qi. Every Wednesday, the Qi allocated by the Vaults incentives program will be airdropped / claimed for the week prior to the pay day.

## Vaults incentives FAQs

If you want to know more about the way Vault incentives are working, here's an official FAQ from the Discord server.

* **What vaults are receiving rewards?**

Right now all the vault types have been allocated Qi rewards

* **How much rewards are given out for the borrowing incentives?**

0.05 Qi/block for each vault type

* **How much MAI do I need to borrow to earn rewards?**

  For Vault Borrow Incentives, stay between 25% and 270% above the liquidation ratio to receive QI token airdrop. This means:

* _Matic_ - Liquidation ratio 150% - Eligible for Incentives between 175% and 420%
* _Tokens_: - Liquidation ratio 130% - Eligible for Incentives between 155% and 400% 
* _CamTokens_: - Liquidation ratio 135% - Eligible for Incentives between 160% and 405%
* **How can I see if my vault is earning rewards?**

  If you see the fire emoji on your vault overview page that means that vault is earning rewards

* **How much will I earn?**

Your percent of the reward pool is based on the percentage of MAI you borrowed compared to the total amount of MAI borrowed from that vault type.

* **How long will the incentives program last?**

The scheduled length of the borrowing incentives program is to last 3 months. The DAO can vote to stop incentives before the 3 months is over or vote to extend the program.

* **How will we receive rewards?**

Qi will be airdropped to eligible vault holders.

* **How is eligibility for rewards gathered?**

Eligibility for rewards is calculated per block. You will earn rewards for the blocks you were eligible during the week.

* **When do tracking rewards for the week start?**

We will follow the same schedule as eQi. You can find the block numbers on the boost page.

## Disclaimer

This guide has been written **prior** to the launch of Vault incentives, meaning that the APRs promoted in this document \(as well as this document\) are subject to modifications, and/or may not be accurate. The amount of MAI borrowed, the debt ceiling and the value of the Qi token will highly impact the final APR of each vault type. Please, make sure that you invest responsibly.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly \(or make you lose money\) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

