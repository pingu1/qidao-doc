---
description: >-
  DeFi não precisa ser complicado. Este artigo mostra como podes começar a
  aventurar-te no espaço DeFi utilizando a plataforma Mai Finance com uma
  estratégia de baixo risco e taxas de juros razoáveis.
---

# Estratégia de principiante camDAI

## Introdução

A maioria das pessoas se assusta quando pensam em DeFi. Existem sempre fatores de risco a considerar quando estamos a falar de criptomoedas, a volatilidade do mercado pode resultar na perda de dinheiro para algumas pessoas e existem tantas possibilidades disponíveis, o que dificulta a tarefa de encontrar uma estratégia adequada para a tua métrica de risco. No entanto, se você utilizar as ferramentas corretas, algumas estratégias fáceis e de baixo risco podem te garantir bons resultados, podendo até competir com estratégias mais complexas e arriscadas.

Neste guia, vamos apresentar uma estratégia de investimento com base na alavancagem de uma _stable coin_, moeda estavel em inglês, com uma pitada de risco para obter maiores taxas de juros.

## Entendendo o conceito de alavancagem



![A história de um mineiro azarado](../.gitbook/assets/canDAI-farwest.png)

Estamos no faroeste, durante a grande corrida do ouro. Os bancos querem comprar ouro para oferecerem como empréstimo aos clientes e recebem taxas de juros nesses empréstimos, enquanto que os mineiros querem ficar ricos ao vender ouro aos bancos.

Vamos considerar que você é um mineiro, mas sem grande sorte. Apenas encontra uma pepita de ouro. No entanto, como é super inteligente, em vez de minerar, tem outro plano em mente!

Você vai a um banco e diz que tem ouro. Você pode depositar o ouro no banco como colateral, o que significa que o banco pode utilizar aquele ouro para empréstimos, fornecendo-te em troca taxas de juros pelo teu depósito.

E agora, porque você depositou ouro, o banco aceita te emprestar dinheiro, e no caso de você não conseguir pagar o emprestimo, o banco pagará a si mesmo, utilizando o ouro que você depositou. Agora, você recebe juros do ouro que depositou, e também consegue dinheiro.

Com isso, você decide visitar um colega minerador e comprar o seu ouro com teu dinheiro. Assim, ele pode focar na mineração e ele ganha dinheiro pelo ouro que ele encontrou. Todos ficam felizes.&#x20;

Você volta ao banco e deposita o ouro que comprou. Isso resulta em juros maiores, e agora o banco permite você pegar emprestado mais dinheiro, pelo ouro adicional que você depositou. Você possui mais ouro exposto ao juros bancarios, e agora um pouco mais de dinheiro. Hora de voltar e visitar novamente o seu amigo para ver se ele encontrou mais ouro, então repete-se o processo várias e várias vezes.&#x20;

Isso é o que nós chamamos de alavancagem. Agora, imagine que você pode encontrar um banco que permite você tomar emprestado, a juros de 0%. Isso é uma excelente maquina de imprimir dinheiro, apenas pelos juros que você esta recebendo.

## Introducing the tools

### AAVE

[AAVE](https://app.aave.com) is a lending and borrowing platform where you can deposit your assets. By lending on AAVE, your deposited tokens will earn yield. For our strategy, we'll be lending DAI, a stable coin (pegged to the US dollar). On AAVE, $100 worth of DAI will potentially generate between 4% and 10% rate of return over the span of 1 year.

![AAVE markets on Polygon as of October 2021](../.gitbook/assets/canDAI-aave.png)

When you deposit your assets on AAVE, you will receive a proof of deposit. In our example, since we are depositing DAI, we will get amDAI tokens in our wallet (**a**ave **m**arket DAI). You absolutely need to keep this receipt because you will need it to remove your DAI from AAVE. This is the bank that will accept your gold in our far west comparison.

### Mai Finance

[Mai Finance](https://app.mai.finance) is a lending platform that will let you deposit some assets in a vault, and borrow against the value of this deposit. If we go back to the bank analogy, it would be a bank that lets you take a loan, but the loan doesn't come from what other people are lending. Instead, the bank prints money corresponding to your personal deposit, so you only borrow against yourself.

Mai finance will accept the amDAI on its [yield instrument](https://app.mai.finance/yield). The yield instrument is just an intermediate tool between AAVE and the vault on Mai Finance. As you can see in the AAVE screenshot, lending DAI will make you earn 8.75% in DAI (that is compounded), but also 2.01% reward in MATIC. The yield instrument on Mai Finance will harvest this MATIC reward and swap it for more DAI that will be added to your DAI deposit. The APY (**A**nnual **P**ercentage **Y**ield) on the Mai Finance site is hence showing the aggregated interests from AAVE.

![Yield instrument on Mai Finance](../.gitbook/assets/camDAI-yield.png)

Once you deposited your amDAI on the yield instrument, you will get some camDAI in your wallet (**c**ompounding amDAI). This is a receipt that indicates your share of the amDAI pool in the yield instrument. As a side note, because camDAI is a representation of your share of the amDAI pool, the ratio between amDAI and camDAI isn't 1:1. See [this article](../investment-tutorials/leverage-aave-tokens.md#amtokens-vs-camtoken) for more details.

You can now [deposit your camDAI](https://app.mai.finance/vaults) tokens in a vault on Mai Finance, and will then be able to borrow some MAI (a stable coin pegged to $1) against your collateral. In our far west comparison, this is a second bank that will let you take a cash loan based on the amount of gold you deposited in the first bank. This second bank accepts the receipt from the first bank as a guarantee in case you cannot repay your loan.

### Zapper

[Zapper](https://zapper.fi/dashboard) is a Swiss army knife of DeFi on Polygon. This platform will let you farm yields in liquidity pools, lend your assets on AAVE directly from their platform, presents a dashboard of your different investments, and will let you swap some currencies for other currencies. This is the last feature that we will be using in order to exchange the MAI stable coin we just borrowed for more DAI.

![Swapping MAI for DAI](../.gitbook/assets/camDAI-zapper.png)

In our far west example, Zapper is the gold miner that will accept your cash and will sell you gold.

### Balancer

As you can see in the screenshot above, Zapper is using Balancer has the protocol to operate the swap. [Balancer](https://polygon.balancer.fi/#/) is an automated portfolio manager, liquidity provider, and price sensor where you will be able to provide liquidity (and get fees from this) or swap currencies using the liquidity pools.

For our guide, we will use Balancer to expose our investments to a little more volatility and get better interests. This is 100% optional though.

## Strategy description

### Main strategy

Even if we explained what AAVE is, our strategy will use a feature from Mai Finance to automate the DAI deposit on AAVE, the amDAI deposit in the yield instrument and the camDAI deposit in the camDAI vault.

![](../.gitbook/assets/camDAI-zapDAI.png) ![](../.gitbook/assets/camDAI-zapdeposit.png)

The `Zap in using DAI` button opens a popup that lets you deposit your DAI in the vault and operates the AAVE deposit under the hood. This is saving a lot of time, and some gas.

This will be our first step. Assuming we have $100 worth of DAI, we will deposit them on Mai Finance in a camDAI vault. This will allow us to borrow MAI against this initial deposit.

The minimal CDR (**C**ollateral to **D**ebt **R**atio) for camDAI is 110%. This means that the ratio between your collateral (the $100 worth of DAI) and the loan we're about to get needs to remain above 110%.

{% hint style="danger" %}
If this CRD ratio reaches the minimal value of 110%, it means that your collateral is losing value and your debt may become bigger than the value of your collateral. At this point, your vault can be liquidated: someone can repay a part of your debt and get a part of your collateral as a compensation. However, since both DAI and MAI are stable coins pegged to the US dollar, the risk of getting a big difference between the 2 assets is very low, which makes this strategy fairly safe.
{% endhint %}

In order to maintain the liquidation risk fairly low, we will try to stick to a CDR of 115%. In order to know how much MAI we can borrow to stay at a 115% CDR, we will use this formula:

$$
MAI_{available} = \frac{Collateral_{value} - Debt_{value} * Target_{CDR}}{Target_{CDR}}
$$

With a collateral value of $100, no debt yet, and a target CDR of 115%, here's how much we can borrow:

$$
MAI_{available}=\frac{100 - 0*1.15}{1.15}=86.95
$$

​You can then swap the MAI you borrowed for DAI and repeat. Here's what your collateral and debt should look like:

| Loop # | Collateral | Debt    | Available loan | Equivalent APY | DAI liquidation price |
| ------ | ---------- | ------- | -------------- | -------------- | --------------------- |
| 1      | 100.000    | 0.000   | 86.956         | 10.42%         | 0                     |
| 2      | 189.956    | 86.956  | 75.614         | 19.48%         | 0.512                 |
| 3      | 262.571    | 162.571 | 62.751         | 27.36%         | 0.681                 |
| 4      | 328.323    | 228.323 | 57.175         | 34.21%         | 0.765                 |
| 5      | 385.498    | 285.498 | 49.718         | 40.17%         | 0.815                 |
| 6      | 435.216    | 335.216 | 43.233         | 45.35%         | 0.847                 |
| 7      | 478.449    | 278.448 | 37.593         | 49.85%         | 0.870                 |
| 8      | 516.042    | 416.042 | 32.690         | 53.77%         | 0.887                 |
| 9      | 548.732    | 448.732 | 28.426         | 57.18%         | 0.899                 |
| 10     | 577.158    | 477.158 | 24.718         | 60.14%         | 0.909                 |
| 11     | 601.877    | 501.877 | 21.494         | 62.72%         | 0.917                 |
| 12     | 623.371    | 523.371 | 18.691         | 64.96%         | 0.924                 |
| 13     | 642.062    | 542.062 | 16.253         | 66.90%         | 0.929                 |
| 14     | 658.315    | 558.315 | 14.133         | 68.60%         | 0.933                 |
| 15     | 672.448    | 572.448 | 12.289         | 70.07%         | 0.936                 |
| 16     | 684.737    | 584.737 | 10.686         | 71.35%         | 0.939                 |
| 17     | 695.423    | 595.423 | 9.293          | 72.46%         | 0.942                 |

We're stopping at 17 loops but you can operate more if you want to.

At the end of the 17 loops, you'd get $695.423 of collateral and $595.423 of debt. This corresponds to a CDR 116.79% which should be safe enough to prevent liquidation.

If we consider the 10.42% APY granted by the yield instrument, this would generate

$$
Interests = Collateral_{value}*APY=695.423*10.42\%= \$72.463
$$

If we consider that the initial investment was only $100, that's an equivalent APY of 72.463% on single staking a stable coin!

### Alternative strategy

In order to get a little exposure to high volatility assets, you can use the same loop as above but only leverage 90% of the borrowed MAI, and use the 10% to buy something else. In this example, we will use the 10% to buy Qi (the native token of Mai Finance) and use the Qi-BAL pool on Balancer that currently has an APR (**A**nnual **P**ercentage **R**evenue) of 107.12%.

![Qi-BAL pool state as of October 2021](../.gitbook/assets/camDAI-balancer.png)

Since we're re-injecting less DAI in the camDAI vault, we will also operate less loops. The setup will look like this:

| Loop # | Collateral | Debt    | Qi     | Available loan | Equivalent APY | DAI liquidation price |
| ------ | ---------- | ------- | ------ | -------------- | -------------- | --------------------- |
| 1      | 100.000    | 0.000   | 0.000  | 86.957         | 10.42%         | 0                     |
| 2      | 178.261    | 86.957  | 8.696  | 68.053         | 35.22%         | 0.537                 |
| 3      | 239.509    | 155.009 | 15.501 | 53.259         | 54.63%         | 0.712                 |
| 4      | 287.441    | 208.268 | 20.827 | 41.681         | 69.82%         | 0.797                 |
| 5      | 324.954    | 249.949 | 24.995 | 32.620         | 81.71%         | 0.846                 |
| 6      | 354.312    | 282.569 | 28.257 | 25.529         | 91.01%         | 0.877                 |
| 7      | 377.288    | 308.097 | 30.810 | 19.979         | 98.29%         | 0.898                 |
| 8      | 395.269    | 328.076 | 32.808 | 15.636         | 103.99%        | 0.913                 |
| 9      | 409.341    | 343.712 | 34.371 | 12.237         | 108.45%        | 0.924                 |
| 10     | 420.354    | 355.948 | 35.595 | 9.576          | 111.94%        | 0.931                 |

At the end of the 10 loops, you'd get

* $420.354 of DAI as collateral
* $355.948 of debt
* $35.595 of Qi

The same math as in the previous case gives the following results

* A final CDR of 118.09%, which should be considered as safe enough to prevent liquidation
* $43.800 of interests on DAI from the 10.42% APY granted by the yield instrument
* $68.139 of interests on your Qi from the Balancer pool, if you assume you will be compounding the Qi and BAL rewards in the Qi-BAL pool
* A total APY of 111.94%

This strategy presents more risks in the sense that the investment in the Qi-BAL pool isn't guaranteed. However, you will get a little bit of exposure to Qi, which will let you participate to the QiDAO protocol. If you use the BAL reward on Mai Finance as a collateral and borrow against it, you will also be able to re-invest in the camDAI vault or in the Qi-BAL pool. If you do so, you will also be entitled to borrowing rewards paid in Qi every week.

## Conclusion

With some minimal investment and low maintenance, you can get some pretty solid results simply by leveraging your DAI. Since DAI is a stable coin that has a lot of liquidity across multiple chains, the risk is relatively low for DAI to go off peg and for your vault to be liquidated. It's the kind of "set and forget" setup that can easily be a very good starting point for any DeFi beginner, and chances are this strategy will perform the same way in a bull market or in a bear market. Finally, we also explained how you can use the same strategy to grab a portion of your loan and test out the many possibilities that DeFi has on Polygon.

## Disclaimer

Everything presented in this tutorial is educational content made to illustrate the leverage option proposed by Mai Finance. We didn't talk about debt repayment because there are articles dedicated to this on this site, but you need to keep in mind that Mai Finance charges a 0.5% repayment fee on the borrowed amount. As always, make your own researches and don't hesitate to ask question on the [Discord server of the DAO](https://discord.com/invite/qidaoprotocol) community.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
