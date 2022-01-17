---
description: >-
  This guide will propose a new way to maximize your stable investments
  by adding an Ohm fork as a reward multiplier.
---
# The Elephant, the Chimp and the Otter
 
## Introduction
 
This could be a good title for some poetry, however, it appears that these are the 3 totem animals of the protocols we will be discussing in this guide. Today, we will take a close look at one of the latest (as of January 2022) additions to the collateral tokens collection backing the MAI stable coin on Mai Finance: the sdam3CRV token. We will explain in detail what it is and how you can get it. We will then propose a little strategy to use it and get high returns using the stable receipt token from Stake DAO, Mai Finance, and the OtterClam protocol as a reward multiplier.
 
![](<../../.gitbook/assets/stakedao-otter-1.png>)
 
## Stake DAO
 
### Presentation of Stake DAO
 
[Stake DAO](https://app.stakedao.org/) is a yield optimization platform where users are able to deposit their assets and let the platform use the most curated strategies to maximize yields. The investments are proposed with a risk score, and investments are properly displayed on a nice dashboard that makes it easy to follow the results of chosen strategies. Primarily launched on Ethereum Mainnet, Stake DAO is rapidly expanding to other chains like Polygon and Avalanche. You can of course read more about Stake DAO on their [official documentation](https://stakedao.gitbook.io/stakedaohq/).
 
### The am3CRV strategy
 
For our guide, we will be using the `Passive Aave USD Strategy` for Polygon. This is a strategy that is using the am3CRV pool from [Curve Finance](https://polygon.curve.fi/): you deposit your stable assets (USDC, USDT, or DAI) in the aave pool from Curve and you will receive an am3CRV receipt token. This is the token that you can stake on Curve directly to receive CRV and WMATIC rewards, but you can also deposit this token on Stake DAO and the CRV and WMATIC rewards will be sold and compounded into your stable position.
 
![aave pool on Curve as of January 2022](<../../.gitbook/assets/stakedao-otter-2.png>)
 
As you can see above, staking your am3CRV tokens on Curve would give you an overall APR of 8.35% (**A**nnual **P**ercentage **R**eward). If you go to Stake DAO, you will find in the `Strategies` tab for Polygon the strategy that is using the am3CRV tokens where you will be to deposit your receipt token and earn 11.11% APY (**A**nnual **P**ercentage **Y**ield, that assumes you compound your rewards at least daily).
 
![Passive AAVE USD Strategy on Stake DAO as of January 2022](<../../.gitbook/assets/stakedao-otter-3.png>)
 
When you deposit your am3CRV tokens on Stake DAO, you will receive a new receipt token: sdam3CRV (**s**take **d**ao am3CRV).
 
{% hint style="info" %}
Please note that Stake DAO is taking fees on your gains for each strategy that you are using. In our case, and as of January 2022, the performance fee is 15%, and there will also be a 0.5% withdrawal fee. Make sure that you understand this before you enter the pool.
{% endhint %}
 
This strategy can be considered a very safe one (DYOR) since it's using only stable coins. The Impermanent Loss risk is close to none because the am3CRV LP token is composed of only stable coins pegged to the US dollar. If you want to use Stake DAO, make sure that you however take into account the smart contract risks since your asset will be lent on AAVE via Curve, and the LP token is on Stake DAO, so you have 3 layers of protocols that are exposed to risks.
 
You can use the farming instrument on Stake DAO to deposit your sdam3CRV tokens and get an extra ~9% paid in SDT token, the native token of Stake DAO. For our guide, we will however use the sdam3CRV token differently.
 
## Mai Finance
 
[Mai Finance](https://app.mai.finance) is a lending protocol where you can deposit your assets as collateral, and borrow against them. This is not the average lending platform where you will find people lending assets to borrowers. On Mai Finance, you only lend to yourself, and you only borrow against the assets you own. Find more details about Mai Finance on this site, or on [the official documentation](https://docs.mai.finance/).
 
In January 2022, the sdam3CRV token was approved as a collateral option on Mai Finance. This means that the token that has been created by depositing your am3CRV receipt on Stake DAO can now be used to borrow the MAI stable coin. This is particularly great for a few reasons:
 
* the sdam3CRV token is composed of stable coins only, so it should not be affected by Impermanent Loss and should keep a steady price
* because the price is not changing much, it's fairly easy to avoid liquidations, even if you borrow close to the liquidation level
* your collateral is growing in value because it's a yield-bearing asset. At the time of writing this guide, you'd get 11% APR on your collateral
 
![Example of a sdam3CRV vault on Mai Finance](<../../.gitbook/assets/stakedao-otter-4.png>)
 
This vault is using a high CDR (**C**ollateral to **D**ebt **R**atio) because we always try to promote safety in the guides presented on this website. A high CDR presents a few benefits:
 
* It keeps you away from liquidation in case of major negative price actions of your collateral
* It allows you to withdraw a good chunk of your collateral and sell it to repay your debt (see our [guide on debt repayment](../../mai-university/debt-repayment-how.md))
 
However, feel free to get a CDR that suits your tolerance to risk.
 
{% hint style="info" %}
The sdam3CRV vault is using stable coins as collateral. Like the camDAI vault, it will **NOT** get any borrowing incentives. Its liquidation ratio may also be decreased to 110%, like for the camDAI vault.
{% endhint %}
 
With the MAI you can borrow against your collateral, you can leverage your position. If you need details, please read our specific [guide on leveraging camDAI](camdai-beginner-strategy.md) and apply it to your sdam3CRV tokens. You can indeed get a much bigger exposure to the rates provided by Stake DAO just by applying some levering loops. However, this applies some strong sell pressure on the MAI token, so we will propose another approach.
 
## OtterClam DAO
 
[OtterClam Finance](https://app.otterclam.finance/) is a very unique Ohm Fork on Polygon that is very innovative, integrating cool NFTs on their platform. Launched in November 2021, OtterClam has seen a lot of growth since its inception and is now moving toward GameFi.
 
One of the most interesting things about OtterClam is its partnership with the QiDao protocol behind Mai Finance. The biggest portion of the stable coins backing their CLAM token is in MAI, the stable coin minted on Mai Finance. This means that you can purchase CLAM bonds using MAI directly, and this is exactly what we will be doing in our strategy. Indeed, Ohm forks are known to provide very high reward rates, and OtterClam isn't an exception. Another unique thing about the bonds on OtterClam is that you purchase sCLAM (staked CLAM tokens), so the tokens are getting rebase rewards during the entire vesting period, which makes bonds even more attractive.
 
![Purchasing sCLAM bonds on OtterClam finance as of January 2022](<../../.gitbook/assets/stakedao-otter-5.png>)
 
On this screenshot, you can see that we will indeed purchase sCLAM with a discount of 3.66% (purchase price is 9.20 MAI while the market price is $9.54), but during the entire vesting period of 5 days, the sCLAM purchased will also grow by 6.95%. Because of the very high reward rates (13,400% APY at time of writing), it will be important to keep the sCLAM tokens staked, but we will be selling the staking rewards for stable coins, and deposit them on Curve to increase our am3CRV position.
 
![Congratulations, you have some CLAM staked](<../../.gitbook/assets/stakedao-otter-6.png>)
 
If you check the price of CLAMs, you will see that this token has a lot of volatility, however, and like for most Ohm forks, the price of the token is irrelevant, we're only using OtterClam as a multiplier for the gains. Ohm forks are designed to lower the token price to $1 (or whatever asset is backing the token), and the token is a "reserve currency" meaning that it's designed to be used and bought/sold.
 
{% hint style="info" %}
Staking rewards are accrued into the vesting sCLAM tokens, but cannot be accessed during the vesting period. We will have to wait for the vesting tokens to be fully vested before we can collect and sell the staking rewards.
{% endhint %}
 
## Farming Strategy
 
As in most cases, the best starting point for strategies is to start with stable coins. This way, you reduce the risk of impermanent losses, and you only work with benefits from your farming (or the borrowed amount in our case).  So the loop starts by depositing stables on Curve to get an am3CRV token. This receipt token is deposited on Stake DAO so that you can get a sdam3CRV receipt. This token will be deposited on Mai Finance as collateral to borrow MAI. The loan is used to purchase MAI bonds on OtterClam. The rebase rewards are swapped for more stable coins. As a side note, you can sell whatever amount of the rebase reward. For our guide, we'll be selling 100% of it, but you can keep some to increase your CLAM position faster and collect bigger rewards faster.
 
As always for simulations, we will fix all numbers as follows:
 
* APY for the sdam3CRV strategy on Stake DAO is 11.11%
* APR for staked CLAMs on OtterClam is 13,400%
 
We will also not deal with the debt repayment and will assume all prices remain the same. We will run the simulation with $100 worth of USDC as a starting point, and we will also try to stick to a 235% CDR when more MAI is borrowed. Finally, we will assume, for the simplicity of this simulation, that at the end of each vesting period, there's an available MAI bond with a 0% discount (you will hunt for discounts greater than 0% obviously).
 
![](<../../.gitbook/assets/stakedao-otter-7.png>)
 
### Day 1
 
On day 1, you can prepare pretty much everything:
 
* Deposit your $100 worth of USDC (or USDT or DAI, up to you) on Curve finance
* Deposit your am3CRV receipt token on Stake DAO
* Deposit your sdam3CRV receipt token on Mai Finance
* Borrow at a CDR of 200%, or $50 worth of MAI for a first loan
* Purchase a MAI bond on OtterClam Finance
 
At this point, you're set and will have to wait for the entire vesting period to start collecting rebase rewards. At the end of Day 1, you would have
 
| Position            | value ($) |
|---------------------|-----------|
| sdam3CRV            |   100.000 |
| MAI loan            |    50.000 |
| sCLAM               |    50.000 |
| additional sdam3CRV |     0.030 |
| additional sCLAM    |     0.000 |
 
### Day 2, 3 and 4
 
Nothing to say, your sdam3CRV is collecting yields, but that's pretty much it, nothing to harvest while the bond is vesting
 
### Day 5
 
At the end of Day 5, the bond is fully vested, and because rebase rewards have been compounded during the entire vesting period, you would have at the end of the day
 
| Position            | value ($) |
|---------------------|-----------|
| sdam3CRV            |   100.122 |
| MAI loan            |    50.000 |
| sCLAM               |    53.382 |
| additional sdam3CRV |     0.030 |
| additional sCLAM    |     0.722 |
 
### Day 6
 
You have some additional sdam3CRV tokens against which you can borrow to purchase a new bond. This will be a very small bond (just a few cents for now) but with time, you will be able to purchase more and more sCLAM with your new MAI. At the end of Day 6, you will then have
 
| Position            | value ($) |
|---------------------|-----------|
| sdam3CRV            |   100.875 |
| MAI loan            |    50.437 |
| sCLAM               |    53.820 |
| additional sdam3CRV |     0.031 |
| additional sCLAM    |     0.728 |
 
At this point, your staked CLAMs will produce rewards every day that you can compound in your sdam3CRV vault, or you can simply compound every 5 days when the bond is vested.
 
### Daily Routine
 
Assuming you compound every day, the daily routine will be
 
* unstake the equivalent of 3 rebases from your staked CLAMs
* sell them for whatever stable coin you would get the most based on the market status
* deposit the additional stable into the aave pool on Curve Finance
* deposit the am3CRV token on Stake DAO
* deposit the sdam3CRV token on Mai Finance
 
Then, every 5 days you will be able to perform the following additional steps:
 
* borrow additional MAI to keep a CDR of 200%
* purchase additional MAI bond on OtterClam
 
### Raw results month after month
 
Here are raw results month after month
| day |  sdam3CRV  |    CLAM    |   MAI debt |
|-----|------------|------------|------------|
|  30 |    121.249 |     64.007 |     60.625 |
|  60 |    150.866 |     78.815 |     75.433 |
|  90 |    187.350 |     97.057 |     93.675 |
| 120 |    232.294 |    119.529 |    116.147 |
| 150 |    287.659 |    147.212 |    143.830 |
| 180 |    355.863 |    181.314 |    177.931 |
| 210 |    439.882 |    223.323 |    219.941 |
| 240 |    543.383 |    275.074 |    271.691 |
| 270 |    670.884 |    338.825 |    335.442 |
| 300 |    827.950 |    417.358 |    413.975 |
| 330 |  1,021.437 |    514.101 |    510.719 |
| 360 |  1,259.790 |    633.277 |    629.894 |
 
### Day 365
 
After a complete year of farming this system, and assuming everything are the same as on Day 1 (prices, rates, and everything else ...), you would have:
 
* $1,304.575 worth of sdam3CRV tokens in your vault on Mai Finance
* $655.670 worth of CLAM on OtterClam finance
* a debt of $652.288 worth of MAI
 
You can see that at the end of the year, you still have a CDR of 200%. You could withdraw your collateral to repay your debt and unlock the rest of your collateral. You can also repay your debt by selling your CLAMs and unlocking 100% of your collateral.
 
In the end, from an initial investment of $100 you would end up with $1,307.958 and a debt of $652.288, which corresponds to an overall APY of 1,207.958%.
 
{% hint style="success" }
If you extract only 50% of your rebase reward from OtterClam Finance and keep the rest staked, the high APY will be applied to a position that grows much faster. This presents more risks, but assuming everything stays the same, and if you sell only 50% of your reward, you would possibly end up with $3,608.447 split between your vault and OtterClam, and a debt of $750.828 for an equivalent APY of 2,757.619%.
{% endhint %}
 
## Disclaimer
 
This strategy is pretty interesting, because it presents very little risk on the initial side. Indeed, your money is working off stables, and the initial is "protected", so the probability of losing it is very small. The liquidation risk is also very small due to the very high CDR used for a very small price variation between the collateral and the borrowed asset. Without additional tools, you would probably get ~12% APY but it's clear that using other protocols to maximize the rewards can lead to very high returns.
 
However, make sure that you understand this investment strategy in its finest details. Make sure you accept the smart contract risks because we're using a lot of different protocols. Also, you need to understand how Ohm forks work and don't pay attention to the price of CLAMs, which may vary a lot. Finally, if rates _may_ remain the same on Stake DAO, the reward rate on OtterClam will most certainly decrease over time since ohm forks can't sustain such high APYs for long periods of time. As always, read the documentation of the different projects you will use, and make sure you understand all the risks.
 
{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs, end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}
 