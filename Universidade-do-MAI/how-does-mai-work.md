---
description: >-
  Entender bem como o MAI funciona é crucial para qualquer investidor que
  realmente queira entender a Mai Finance, e neste artigo você entenderá isso.
---

# Como a MAI funciona?

## O que é uma stablecoin?

Antes de falarmos sobre MAI, temos que entender o que é uma stablecoin. Uma stablecoin é um tipo de criptomoeda projetada para manter um preço de mercado estável. A maioria das stablecoins são atreladas (uma moeda em que o preço é projetado para permanecer o mesmo que um ativo designado) ao dólar americano, mas você pode encontrar outras stablecoins atreladas a outras commodities, como ouro (como EGold) ou prata (SilverCoin).

No entanto, existem 2 categorias principais em que todas as stablecoins podem se encaixar, **com** ou **sem garantia**. As stablecoins **com garantia** são aquelas que detêm os ativos contra os quais sua moeda está atrelada, enquanto as **sem garantia** fazem uso de algoritmos para controlar a oferta de tokens a fim de manter o preço fixado em um nível predeterminado.

## O desastre da IRON Finance

Se você já trabalha com criptomoedas há algum tempo, pode se lembrar do desastre do token **TITAN** e **IRON**, mas para aqueles que não conhecem, aqui está uma rápida recapitulação. O IRON Finance era um projeto que tinha 2 tokens, a moeda estável IRON e o token TITAN, no entanto, a moeda estável IRON **não era totalmente lastreada** em moedas estáveis, a proporção para a moeda IRON era de **75% em USDC** e **25% em TITAN**. Então foi basicamente uma receita para o desastre.

In June of 2021 the TITAN token reached an ATH of $65, which caused that a bunch of investors, who invested heavily in the coin, decided to sell. This caused a problem because TITAN is priced based on supply and demand. So as the available supply of TITAN increased, the price began to decrease. This caused a huge sell pressure so the price of TITAN fell even faster, so when TITAN began to fall rapidly, IRON lost its backing and eventually its peg.

![Price chart of the TITAN token](../.gitbook/assets/iron.jpg)

![Price chart of the IRON stablecoin](../.gitbook/assets/titan.jpg)

People started buying the IRON stable coin to sell it for USDC and earn some quick bucks, in a huge arbitrage opportunity (this means profiting in the price variations of tokens) Long story short, it's been calculated that almost $1.75 billion were lost in this incident. Now, is there a difference between the IRON stable coin and the MAI stable coin?

## What is MAI?

MAI is a stable coin that is backed by locked collateral tokens, the minting of MAI can be done either through depositing **approved collateral** in vaults or through using **Anchor.**

When minting MAI depositing approved collateral, the **CDR** (Collateral to Debt Ratio) needs to be between 150%, this means that if you deposit $100 worth of collateral, the newly minted MAI can be at most worth $66.6667. We'll get to the reason behind this later in this article.

Another way to mint MAI is through the [Anchor](https://app.mai.finance/anchor), this means that when you swap a stable coin (as of September 2021 you can mint MAI using **DAI**, **USDC** and **USDT**) for MAI, new MAI is minted by the treasury and the deposited stablecoin is held in the treasury as collateral. Meanwhile, when you swap back your stablecoins, the MAI that you provide will be burned.

![Stablecoins that can be swaped to mint MAI](<../.gitbook/assets/image (9).png>)

As you can see on the picture below, the price of the MAI stable coin it's almost always close to $1, this is because as the [official documentation](https://docs.mai.finance/stablecoin-economics) says, the MAI stable coin allows users to engage in risk-free arbitrage through Anchor when the price of MAI falls below $0.99 or rises above $1.01.

![Price chart of the MAI token in the last 90 days](<../.gitbook/assets/image (7) (1) (1).png>)

## Why is it always close to $1?

The peg to $1 is maintained by 2 mechanisms, via **Anchor** or by **depositing collatera**l in the vaults, in this section of the article, you'll understand why

### Anchor

Anchor allows users to mint MAI with stable coins and redeem stable coins from MAI. Also, as you can see on the picture below, there's a 1% fee when swapping your stable coins for MAI or vice versa, there are two main reasons for these fee:

* The 1% minting fee to create MAI sets a price ceiling of $1.01.
* The 1% fee to redeem stable coins from MAI sets a price floor of $0.99

![](<../.gitbook/assets/image (8).png>)

Having a price ceiling and a price floor helps MAI to not diverge from its peg too much, however as you've seen on the picture of the MAI chart, you can participate on low- risk arbitrage opportunities (meaning that you can sell your stable coins when MAI is under $1 or sell MAI when is above $1 to earn some quick bucks).

About what causes the fluctuation of the price of MAI, there could be two main reasons for this:

* If the **market is in a bearish trend**: people will sell their volatile assets and buy more stable coins to avoid losing value of volatile assets. This means that people want to buy MAI, increasing its price.
* If the **market is in a bullish trend**: people buy more volatile assets when their price is low, using their stable coins. This means that people sell their MAI, driving its price down.

### Depositing collaterals in vaults

In order to mint MAI using the vaults in Mai Finance, you need to deposit some collateral in there and have a **CDR** (Collateral to Debt Ratio) above a certain threshold, in this case is 150% (however this percentage can change in the future if the community decides so). This means that the vaults will always be over-collateralized (by 150%) to ensure that there is always collateral value to back the stable coins minted. Remember that if a vault has less than a 150% CDR it could be partially liquidated by the community, so somebody could loose some of their collateral if a liquitador pays some of their debt.

As the value of the collateral rises, more stable coins can be issued as a rise in collateral price will increase your collateral to debt ratio. Conversely, as the value of the collateral falls, fewer stable coins can be issued, this is done to prevent that the CDR falls below the 150% mark.

## Afterword

As you've seen throughout this article, the MAI stable coin is a type of stable coin that is **over-collateralized,** meaning that there will always be enough collateral to back the price of the MAI token. This should give enough relief to those investors who hesitate about investing in projects that mint stable coins. Also, keep in mind that as MAI is expanding to other blockchains, there'll be more MAI in the market, resulting in less volatily in MAI's price.

Recently, the vaults incentives have been introduced to Mai Finance, if you want to understand what that is, stay tuned because there'll be an article about this topic. This will help even more to the stability of the MAI price.

## Disclaimer

You can find[ ](https://docs.mai.finance/stablecoin-economics)the original article of the Mai Finance team about MAI [here](https://docs.mai.finance/stablecoin-economics).

This guide is definitely not financial advice, it was made with an educational goal in mind.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
