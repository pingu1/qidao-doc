---
description: >-
  This page will present different options to repay your debt on Mai Finance.
  Keep in mind that repaying a debt is never mandatory as long as you want to
  keep your loan, and don't need your collateral.
---

# Rimborso del debito - Come?

The market is on a bull run and your crypto, locked in the Vault, is gaining more and more value, so much that you decided to sell it. However, because it's in the Vault on Mai Finance, you can't totally unlock it unless you repay your loan.

The market is bearish, and your crypto is losing value very quickly. You don't generate yield fast enough to cover up the damages and keep an healthy Collateral to Debt Ratio \(CDR\), and liquidation is near. It's time to repay your debt to make sure you're not losing too much, and prevent liquidation.

If you are not in any of the above situation, it's probably not worth repaying your debt. Please see the chapter on [Debt Repayment](https://qidao-qimps.gitbook.io/mai-finance-tutorials/debt-management-tutorials/debt-repayment-why-and-when) for more details.

## Partial or Full repayment using fiat

The most direct way to repay your debt is to use some fiat, especially if you want to keep your collateral and other investments untouched.

Mai Finance is partnering with [Transak](https://transak.com/) to easily bridge money bought by Credit / Debit Cards, or bank transfers, directly to the Polygon network. Simply head to Mai Finance and click the transak icon in the menu bar to open a modal that will let you purchase some MATIC and send them directly to your Polygon wallet.

![Buying some USDC from fiat and bridging to Polygon directly](../.gitbook/assets/screen-shot-2021-08-18-at-9.43.07-am.png)

The main issue is the time taken to process the transaction. However, doing so will let you swap USDC for MAI and then partially or fully repay your debt.

## Repayment using the benefits of your loan

### Partial Repayment

Most people will want to borrow MAI on Mai Finance in order to invest into specific projects. Yield farmers that are using MAI will most probably be successful generating additional resources and will hopefully not lose money on degen farms. If you're in that case, you have 2 options

* repay your loan with the generated revenue
* re-invest your gains into the same \(or another\) project

In most cases, it's probably better to re-invest your gains. Indeed, by compounding your rewards, APR \(**A**nnual **P**ercentage **R**evenue\) is applied on a bigger amount, which in turns generates more revenue. See our investment guides to get ideas on how you can maximize your investments.

However, some people simply don't like the idea of having a debt, and will want to repay it as quickly as possible. If that's your case, you can simply swap your gains into MAI, and repay your debt.

* Open your Vault info
* Select the `Manage` option
* Select the Repay tab at the bottom of your Vault
* Enter any amount you want to repay
* Click `Repay MAI` and you're done

![Partially repaying a portion of my debt](../.gitbook/assets/screen-shot-2021-08-17-at-1.02.23-pm.png)

As an example

* You have $1,000.00 worth of camWMATIC in your vault, with a debt of $400.00
* You swapped $10.00 worth of ADDY tokens for MAI
* You repay $10.00 today
  * Your debt is now $390.00
  * Your camWMATIC value is $999.95 \(you add to pay 0.5% of $10.00 in repayment fees\)

At some point, you will be able to totally repay your debt using this technique, as long as you can generate enough revenue via your loan.

Is this strategy efficient? Not really. Repaying your debt this way doesn't change anything except for your CDR. Indeed, your collateral remains partially locked until you totally repay your debt, and if you're using amTokens as collateral, whether you have a debt or not will not change the fact that your collateral is generating yield. The only advantage is that you can possibly withdraw a portion of your collateral and re-use it somewhere else / sell it.

### Full Repayment

Another approach, very similar to the above strategy, is to repay everything at once. In the example above, instead of repaying $10.00 every few days, I could instead compound the $10.00 earned into my investment to generate yield faster. I can also invest these gains into another project that would also generate revenue. Once I received the equivalent of $400.00 that corresponds to my loan, I can repay everything at once.

## Repayment using your collateral

### Main idea

On Mai Finance, you can borrow MAI stable coins by depositing a certain amount of collateral in a vault. The collateral to debt ratio needs to always be above a certain threshold, 150% for most vaults. This means, for a 150% CDR, that for any $100 worth of collateral, you can only borrow $66.6667 of MAI.

However, this would directly put you in a liquidation position. This means that the health of your vault is considered too risky, and anyone can repay a portion of your debt using their funds and get paid back by getting a portion of your collateral. For more details about liquidation, please read [the official documentation](https://docs.mai.finance/liquidation).

It's usually considered best practice to keep a high collateral to debt ratio to prevent liquidation, but even with a CDR close to 150%, it's easy to see that the value of the collateral is ALWAYS bigger than the value of the debt. This means that you can, in theory, repay your debt by selling some of your collateral asset.

### How to use collateral

Let's consider a vault with $1,000.00 worth of MATIC and a $500.00 debt. The CDR is 200%. The minimum CDR is 150%. In this example, we want to repay the debt completely, but we want to avoid liquidation, and we will try to never go bellow a 160% CDR when withdrawing our collaterals. We will be using the following formulas:

$$
CDR=\frac{Collateral}{Debt}
$$

$$
AvailableCollateral = InitialCollateral - TargetCDR*Debt
$$

In this situation, if we want to keep a CDR of 160%, the amount of collateral we can withdraw "safely" is

$$
AvailableCollateral=$1000-1.60*$500=$200
$$

Hence, we will have to proceed in multiple steps:

* Withdraw $200 from the collateral
  * the vault now has $800 worth of MATIC and $500 of debt, CDR is 160%
* Sell the $200 worth of collateral to buy MAI
* Repay $200 of the debt with a 0.5% repayment fee
  * the vault now has $799 worth of MATIC and $300 of debt, CDR is 266.33%
* Calculate the new amount of collateral we can withdraw: $319
* Withdraw $319 from the collateral
  * the vault now has $480 of MATIC and $300 of debt, CDR is 160%
* Sell the $319 worth of collateral to buy MAI
* Repay $300 of the debt with a 0.5% repayment fee
  * the vault has $478.50 worth of MATIC and $0 of debt, and you still have $19 of MAI

You can see that keeping a healthy CDR can greatly help you repay your debt with very little number of loops. Of course, if your CDR is closer to the 150% limit, you may have to operate more loops since you cannot withdraw as much at once.

{% hint style="info" %}
A collateral to debt ratio of 260% is enough to be able to withdraw the total amount of your debt and stay above 160% CDR. This way, you only need one loop to fully repay your debt.
{% endhint %}

Note that fully repaying your debt by selling your collateral is never necessary if you don't need to sell your underlying assets, or to modify your CDR and keep your vault from being liquidated.

## Repayment using a robot

This paragraph is pure theory and is there only for advanced programmers. The idea is to use flash loans that will help you repay your debt and unlock the collateral so that it can be paid. Flash loans are an option proposed by some applications on different networks, including Polygon, that allow you to borrow funds and repay the loan in the same transaction block. If the loan cannot be fully repaid within the same block, the transaction is simply reverted. On Polygon, AAVE is proposing flash loans.

If we take the example above with $1,000.00 worth of MATIC and a debt of $500.00. The flow would be as follows:

* Borrow $600.00 of USDC on AAVE in a flash loan
* Swap the USDC for MAI
* Repay your debt completely
* Withdraw your MATIC collateral
* Sell your MATIC for USDC
* Repay the AAVE flash loan

When submitted, this list of transactions will all happen in the same block, and you will end up with whatever is left from your MATIC as USDC in your wallet \(more or less $500.00, with some slight variations due to flash loan interest rate, swap fees, and repayment fees\).

Right now, you would have to interact directly with the smart contracts, which requires some good understanding of how they work. If you need help, you can find some on our Discord server where there's a programming channel. Maybe in a near future, [FuruCombo](https://furucombo.app/combo) will propose Mai Finance bricks that would allow you to operate this directly using their graphic tool, but for now it's not possible. Finally, the idea of a button to "repay debt using collateral" has been proposed to the team of devs of Mai Finance, and the option may be implemented in the future.

## Short term VS Long term Debt Repayments

Depending on your strategy and the way you feel regarding your debt, it may be a good idea to compare different lending platforms. However, keep in mind that Mai Finance with its 0% interest and 0.5% repayment fee is one of the top product on the Polygon market. The real competitor is AAVE, but only if you want to borrow MAI or USDC for a short period of time.

* Mais is 0% interest + 0.5% repayment fee
* AAVE has no repayment fees, but a variable APR for interests you need to pay back

![Supplying and Borrowing APY on AAVE as of August 2021](../.gitbook/assets/screen-shot-2021-08-18-at-6.52.08-am.png)

As an example for USDC, you can see that the borrowing rate is 3.79% with a current reward of 2.08% paid back in MATIC. This gives, at the moment of writing, the equivalent of 1.71% you need to pay back if you keep your loan for a complete year. With AAVE, since you can repay your debt very quickly, the variable APY is equivalent to 0.005% daily. Hence, it would take 100 days \(a bit more than 3 months\) to reach 0.5% of your debt.

If you plan to keep your loan longer than that, it's definitely better to use Mai Finance. Also, it's important to understand that AAVE borrowing APRs are variable, they will fluctuate with the amounts that are deposited and required \(the more people want to borrow from AAVE, the higher the borrowing APR\). Keep also in mind that the MATIC reward program will end at some point, and the 1.71% interest will soon become a 3.79% interest rate. At least with Mai Finance, you don't have to keep a close eye on your loan to see when it becomes dangerous to keep it.

Finally, the team of Mai Finance is working on Vaults incentives that would work the same way as the MATIC reward, meaning that you would still get a 0% interest loan and a bonus paid in Qi that may very well reduce the repayment fee to 0% of your debt. And the longer you keep your loan, the more reward you will collect, making it a true negative interest loan.

## Disclaimer

The views, thoughts, and opinions expressed in the text belong solely to the author, and not necessarily to the rest of the community, nor the development team behind Mai Finance. It should not be taken as a financial advice or guidance of any kind.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly \(or make you lose money\) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

