---
description: >-
  Mai Finance proposes loans with 0% interest rates and a single 0.5% repayment
  fee. This is particularly useful to leverage investments on DeFi on Polygon,
  but you can use it in the real world too.
---

# How to use MAI in the real life

## Case study for MAI

DogeOfWallStreet is very bullish on Ethereum. With all the craze revolving around the crypto, partially driven by the NFT hype and bullish case for Eth2.0, he wants to make sure he can get as much ETH as possible before the price really goes to the moon.

In order to do so, our friend already invested in a small mining rig with 6 GPUs. He is mining ETH 24/7/365 and makes on average $40.00 a day with his 6 RTX 3080.

Today is THE day! His initial investment on GPUs is finally fully repaid, and now the rig is only generating profits. However, DogeOfWallStreet did his homework, and noticed a few things

* after EIP1559, his profit decreased, but only by 15% which isn't too bad
* a lot of ETH miners are selling their cards because they think mining is no longer profitable
* price of GPUs slightly dropped, and it's now possible to buy some on specialized websites and even in store
* "The Merge" that would move Ethereum from P-o-W \(Proof of Work\) to P-o-S \(Proof of Stake\) will not occur before Q1 2022 and the Ethereum developers are famous for adding delays to what they are supposed to deliver
* GPU and ASIC manufacturers are adding more ETH miners to the market, betting on the fact that ETH2.0 will be delayed by months, maybe years

So instead of sitting on his profits waiting for the price to sky rocket, DogeOfWallStreet decides that it's time to buy more graphic cards, and possibly increase his mining profits. In terms of costs, the _RTX 1660 super_ seems to be the most profitable card right now, and it only costs $500.00.

![](../.gitbook/assets/screen-shot-2021-08-13-at-12.07.41-pm.png)

After 1 month of mining, the clever miner checks his portfolio on the ETH mainnet after the pool paid him. He has the equivalent of $1,340.00 worth of ETH \(mining profit and ETH gained almost 12% in 4 weeks\) , which should be way enough to buy the card ... but then, dilemma:

* should he keep his ETH because the price is on the rise?
* should he sell his ETH because the sooner he buys his GPU, the sooner he will mine more ETH?

That's about when he discovered Mai Finance and the power of 0% interest loans.

## Getting the 0% interest / 0.5% repayment fee loan

After reading the different docs for Mai Finance, and getting some help from the [Discord](https://discord.gg/mQq55j65xJ) server and the amazing Qi community, DogeOfWallStreet sees a possibility to keep his Ethereum while still buying his graphic card.

The first step is to bridge the ETH to the Polygon network. This is easy using the [PoS bridge](https://wallet.matic.network/bridge), and bridging the assets when the network is cool is done at a "reasonable price" of $20,00 paid in ETH.

DogeOfWallStreet deposits his ETH on AAVE and receives amWETH. He goes now to Mai Finance and deposits the amWETH to get camWETH tokens that will be used as collateral in the vaults. At that stage, he still owns all his ETH, and Mai Finance allows him to gain 1.39% APY on his asset. Not much, but still appreciated.

After depositing $1,320.00 worth of camWETH in the vault, our friend can now borrow MAI against his collateral. DogeOfWallStreet decides to stay above a 200% collateral to debt ratio, and only borrows 600 MAI. He then uses the swap page to get 594 USDC \(1% swap fee\) that he bridges back to the mainnet, paying once again a $20.00 fee. He doesn't really care about paying fees because a part of it is redistributed to miners, and he is one of them, and plans to make money from these fees.

In order to get some USD out of his 574 USDC, DogeOfWallStreet moves the USDC to his Coinbase wallet where he can now sell them and transfer $562.00 USD \(coinbase fee of 2%\) to his paypal account, and finally to his bank account!

At this point, DogeOfWallStreet kept almost 100% of his ETH that is now generating 1.39% annually, AND he has 562.00 USD in his bank account. It's time to move to the next step!

## Investing in the real world

DogeOfWallStreet buys the 1660 super he wanted, paid some taxes and shipping fees for a grand total of $554.35. After a few days, he receives his GPU and installs it in his rig.

The extra GPU is increasing his mining revenue by $2.14 daily. It will take him 270 days to fully repay the card, which is an acceptable ROI according to him. Indeed, his $554.35 new investment will possibly generate a revenue of $781.10 \($2.14 \* 365\) annually, which is an APR of 140.90%. This needs to be added to the $18.34 worth of camToken that the vault on Mai Finance is generating annually.

Seeing those numbers, DogeOfWallStreet will certainly transfer all the ETH he is mining to Polygon and repeat the loop every month to acquire more cards, and mine more ETH.

At some point, if mining ETH becomes unprofitable, he can always switch to another coin \(ETC, RVN, ERG...\), but his mining rig is currently an amazing investment.

## Initial investment and real life debt repayment strategies

Thinking about it, DogeOfWallStreet is now sad that he didn't know Mai Finance existed before he bought his rig. Indeed, this is what he could have done

* Get a bank loan of $20,000.00 at 5% rate and a 2 years amortization \($877.43 repayment / mo\)
* Convert the USD to ETH, bridge it to Polygon, use AAVE and Mai Finance to borrow 10,000 MAI
* Convert the MAI to USD and buy his rig + initial GPUs
* Generate an average of $1,300.00 every month to repay his bank loan and keep the rest as ETH that can be used to repay his debt on Mai Finance, or increase his debt on Mai and invest into something else

Alternatively, he could also split the $1,300.00 worth of ETH into

* A portion of ETH sold directly, but less than the amount owed every month to the bank
* A portion of ETH bridged to Polygon and Mai Finance where he can borrow MAI and repay the rest of the bank loan

Assuming you get _Earnings_ and need to repay a _Debt_ with _Earnings_ &gt; _Debt_. Assuming that _Debt_ is also bigger than half of your _Earnings_. Let's assume _Fiat_ to be the portion of your _Earnings_ you need to use to repay your _Debt_, and _Crypto_ the portion that will be sent to Mai Finance to borrow MAI. We get the following equations

$$
Earnings = Fiat + Crypto
$$

$$
Debt = Fiat+\frac{Crypto}{CDR}
$$

Which leads to the following results

$$
Crypto=Earnings - \frac{Debt*CDR-Earnings}{CDR-1}
$$

$$
Fiat = \frac{Debt*CDR-Earnings}{CDR-1}
$$

In our example with $1,300.00 earned that need to pay a $878.00 debt, the math is

$$
Fiat=\frac{878*2-1300}{2-1}=\$456.00
$$

$$
Crypto=1300-\frac{878*2-1300}{2-1}=\$844.00
$$

Hence we need to sell $456.00 worth of ETH and use Mai Finance to borrow $422.00 of MAI from $844.00 worth of ETH deposited in the vault \(assuming a collateral to debt ratio of 200%\). It's clear that, by doing so, we're keeping more of our earnings and have to sell less crypto. It's a way to increase your savings while still repaying your debt outside of the crypto world.

Of course, this is moving the debt that you need to repay to the bank to a debt you need to repay to Mai Finance. However, the fact that the bank has a high interest fee model, and that you need to repay monthly explains why it's better to move it to Mai Finance \(0% interest, no time limit to repay\).

{% hint style="info" %}
If you want to use a more agressive Collateral to Debt ratio, you would be able to sell less crypto to fiat, and deposit/borrow more from Mai vaults. As an example, with a CDR of 175%, you would sell the equivalent of $316.00 of EHT and keep $984.00 in Mai Finance to borrow $562.00 of MAI, still repaying your $878.00 debt to the bank every month.
{% endhint %}

**Note**: All the math here is not including transaction fees.

## Disclaimer

This tutorial is absolutely not financial advice and should absolutely not be taken for granted. Mining Ethereum is a risky business. Hardware is still pretty expensive and there's no guarantee that mining will still be profitable in the near future. Investing in mining should be done at your own risk, please understand how mining works, and make sure the ROI is acceptable for you. Mining revenues are highly depending on the demand for transactions, and may become unprofitable before you could fully repay your initial investment.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly \(or make you lose money\) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

