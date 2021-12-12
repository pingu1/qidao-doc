---
description: >-
  Este guia mostra em detahles como você pode usar diferentes DApps na rede
  Polygon para aumentar seus ganhos ao fazer farming de stablecoins.
---

# Montando DApps como peças de Lego

## Introdução

Ao buscar rendimentos em alguma farm, você geralmente recebe as suas recompensas na forma do token nativo da farm. Você então pode escolher entre vendê-los, ou mantê-los com a esperança de que irão valorizar ao longo do tempo. Este guia apresenta alguns diferentes DApps (**D**ecentralized **App**lications, ou Aplicaçōes Decentralizadas) para maximizar seus rendimentos sem que você precise vender qualquer coisa, enquanto ainda recebe juros compostos. Este artigo também irá começar com stablecoins, pois essa é considerada uma estratégia relativamente segura. Porém, você precisa ter em mente que isto não é conselheiro financeiro, e que este guia deve ser seguido com caução já que os resultados não são garantidos. Como sempre, faça a sua própria pesquisa.

![](../.gitbook/assets/screen-shot-2021-08-30-at-10.52.20-am.png)

## QuickSwap

A QuickSwap é uma das maiores AMM (**A**utomated **M**arket **M**aker, Agente Automatizado de Mercado) na rede Polygon. Pessoas depositam pares de tokens em pools de liquidez e recebem taxas das transaçōes dos outros usários que usam a plataforma para trocar seus tokens. Durante uma troca, a QuickSwap automaticamente escolhe a melhor rota utilizando diferentes pools de liquidez, e cada pulo de uma pool a outra é sujeito às taxas das transaçōes, que são redistribuídas aos fornecedores de liquidez.

### Farming com Stablecoins

Para este exemplo, iremos utilizar o par MAI/USDC na QuickSwap. Esta pool de liquidez, uma stable pool, entrega um APY (**A**nnual **P**ercentage **Y**ield, Rendimento Percentual Anual) que varia entre 20% e 25%. O rendimento é composto de taxas de transaçōes (que são acumuladas na pool de liquidez) e recompensas em QUICK.

![Pool de liquidez MAI/USDC na QuickSwap em Agosto de 2021](../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

A pool recebe uma quantidade fixa de tokens QUICK todos os dias, então, eles são distribuídos aos fornecedores de liquidez de acordo com sua fatia da pool. Por exemplo, se a pool tem o equivalente a $1,000,000 de liquidez, e você já depositou $1,000 de LP tokens (**L**iquidity **P**rovider, fornecedor de liquidez), você possui 0.1% da pool, o que te entitula a 0.1% das recompensas diárias de QUICK. Sua recompensa será então exigível quando você gerenciar a pool que você entrou.

![Reivindicando minhas recompensas em QUICK por um depósito de $20](../.gitbook/assets/screen-shot-2021-08-30-at-6.39.44-am.png)

Você pode reinvidicá-las frequentemente para fazê-las trabalhar. Vamos ver como fazer isso.

### Dragon's Lair

A Dragon's Lair é uma maneira de otimizar seus ganhos na QuickSwap. Você pode depositar os tokens QUICK que você recebe das pools de liquidez na Lair, e eles então irão te render recompensas QUICK adicionais. Esta é uma ótima ideia se você prefere guardar os tokens QUCIK ao invés de vendê-los. Ao fazer staking de seus tokens QUICK na Dragon's Lair, as recompensas que eles geram são automaticamente reacumuladas, e o APY da Lair é de cerca de 12%.

![APY da Dragon's Lair em Agosto de 2021](../.gitbook/assets/screen-shot-2021-08-30-at-6.42.39-am.png)

Após depositar seus tokens QUICK, você irá receber em sua carteira tokens dQUICK que representam a sua fatia da pool de QUICK. Note que a razão QUICK:dQUICK não é de 1:1 já que o token dQUICK representa a sua fatia na pool, enquanto a quantidade de QUICK que você possui aumenta ao longo do tempo com mais recompensas sendo adicionadas a pool.&#x20;

Agora você tem suas stablecoins depositadas na pool de liquidez, e elas geram recompensas QUICK. As recompensas geram mais recompensas graças a Dragon's Lair. Mas espera, tem mais...

### Dragon's Syrup

A Dragon's Syrup é uma maneira adicional que a QuickSwap oferece para recompensar ainda mais usuários que estão segurando tokens QUICK. O time da QuickSwap criou um programa onde parceiros podem promover seus produtos ao garantir seus tokens aos usuários da plataforma QuickSwap. Você pode então depositar seus tokens dQUICK em uma das farms para receber esses tokens exóticos somados a suas recompensas da Dragon's Lair. A que nos temos interesse está na farm de ADDY.

![Dragon's Syrup, uma farm para coletar tokens ADDY através de depositos de dQUICK](../.gitbook/assets/screen-shot-2021-08-30-at-6.49.25-am.png)

Quando você deposita seus tokens dQUICK na farm, eles desaparecem da Dragon's Lair (da mesma maneira como seus camTokens desaparecem da página de rendimentos na Mai Finance quando você os deposita na Vault). Mas você pode ver claramente que o APY dQUICK da Lair ainda é aplicado, e que você também recebe recompensas ADDY adicionais. Aqui, o APR (**A**nnual **P**ercentage **R**eward, Taxa de Percentual Anual) é de 21.36% atualmente.

{% hint style="info" %}
Você irá notar que as farms da Syrup possuem data de validade. Aqui, a farm ADDY irá expirar em 50 dias e 11 horas. Algumas novas farms irão ser exibidas conforme outras vão desaparecendo.
{% endhint %}

No nosso caso, as recompensas em ADDY que nós recebemos podem ser reinvidicadas manualmente. Você pode notar que a taxa pela qual colhemos as recompensas ADDY pode apenas acelerar se nós reacumulamos manualmente as nossas recompensas QUICK em dQUICK que então depositamos na farm de ADDY na QuickSwap.

### Recapitulando

Nós temos tokens LP MAI/USDC depositados na pool de liquidez, e nós ganhamos:

* Taxas das trocas
* Recompensas em QUICK da pool, que precisamos reinvidicar manualmente e adicionar à Dragon's Lair
* Recompensas em QUICK da Dragon's Lair que são automaticamente reacumuladas com as nossas recompensas existentes
* Recompensas ADDY da Dragon's Syrup que nós podemos reivindicar

## Impermax

Impermax is an application that allows their user to leverage automatically their assets in order to amplify their positions in liquidity pools. This is done by borrowing additional assets supplied on the Impermax platform.

### Stable coin farmin

For this exercise, we will also use the MAI/USDC pool in Impermax. By depositing some LP tokens into the MAI/USDC pool, we now have the option to leverage this deposit a certain number of times in order to increase our exposed capital, and gain more rewards. You need to pay attention to a few things when you're using Impermax though

* You can only borrow what other users supply
* The more assets are borrowed, the higher the borrowing rate
* If the borrowing rate becomes too high, your final APR can become negative, and then you will lose some of your LP
* The more you leverage, the higher the APR, but the higher the borrowing rate

### Levered position

On QuickSwap, I deposited $20 worth of MAI/USDC pair. On Impermax, I will deposit only $10 worth of MAI/USDC and will apply a x2 lever on it to get a $20 exposure.

![Leverage window on Impermax at a given time](../.gitbook/assets/screen-shot-2021-08-30-at-7.11.10-am.png)

You can see on the screenshot above that, if I increase my leverage to x2.1, I would borrow

* 0.481269 USDC
* 0.487593 MAI

We can also see by how much the trading fees I collect would increase (+3.45%), as well as the increase in QUICK rewards (+36.83%), IMX rewards (+23.05%) and the borrowing rate (-37.20%) for a final estimated APR of 26.13%.

Note in this example that the Borrowing fees are paid using the QUICK rewards and the trading fees in case the QUICK rewards aren't enough. Then the IMX reward goes to the supplier if the borrowing fee isn't yet paid, and finally the deposit is used to pay the supplier if there's still something to pay.

Our goal here is to match the deposit we have on QuickSwap, so we'll stick to a x2 leverage. This also ensures that we don't get the risk of going into negative APRs. Our goal is not to collect as much reward as possible, but to increase our position over time, and collect IMX tokens.

### Quick recap

We have MAI/USDC tokens deposited in the appropriate pool

* Our position is levered two times in order to match the amount deposited in QuickSwap
* We collect IMX tokens

## Adamant

Adamant is a yield optimizer platform that automates harvesting into liquidity pools and auto-compound rewards into additional LP tokens. Most of the pools present on Adamant are popular pools from big liquidity providers like QuickSwap, SushiSwap and others. Let's see how we can use Adamant to optimize our yields.

### QUICK/IMX farming

We earn QUICK tokens on QuickSwap, and we earn IMX tokens on Impermax. Let's use Adamant to farm the QUICK/IMX pool from QuickSwap. Why do that? Because the farm is actually very profitable, as you can see here:

![IMX/QUICK pool from QuickSwap on Adamant](../.gitbook/assets/screen-shot-2021-08-30-at-7.27.26-am.png)

As this article is being written, the current APY of the IMX/QUICK pool on Adamant is 417.25%. The reward is composed of

* 168.49% auto-compounded QUICK (QUICK rewards from QuickSwap are sold to buy additional IMX/QUICK LP tokens that are added to your position)
* 212.85% ADDY tokens that you can claim on Adamant (they are vested for 90 days so you can't access them right away)
* 35.91% fee dividends paid in WMATIC if you claim your ADDY daily

This means that your IMX/QUICK position will grow over time, and that you will collect ADDY rewards. The more ADDY you hold, the more dividend (WMATIC) you will collect.

You can also see that the APY on Adamant is _Boostable_. This means that if you stake additional ADDY tokens (not the vested ones), you will apply an additional multiplier to the reward you get. And that's actually a good thing, because we DO get additional ADDY tokens from the Dragon's Syrup on QuickSwap!

### Harvesting ADDY and WMATIC

When you harvest the ADDY earned from your LP position in the IMX/QUICK pool, they will be locked for 90 days, but will allow you to get some dividends in the form of WMATIC. The current APR for dividends is 34% based on your vested ADDY tokens.

After the 90 days vest period, you will have the possibility to lock them for at least an additional 90 days in order to boost the ADDY tokens earned from vaults and earn additional ADDY tokens.

WMATIC dividends are the actual output of the QuickSwap + Impermax + Adamant trio we're after, because we'll be able to use them to re-inject additional LP tokens into both QuickSwap and Impermax.

### Quick recap

We deposit IMX and QUICK tokens earned from Impermax and QuickSwap under the form of IMX/QUICK LP tokens. Adamant is earning

* more LP tokens by auto-compounding a part of the QUICK tokens granted by QuickSwap for the IMX/QUICK pool
* ADDY tokens that are used to boost the IMX/QUICK rewards, and makes us eligible to dividends
* WMATIC dividends

## AAVE

With the WMATIC tokens earned on Adamant, we now can deposit them on AAVE in order to get some yield. This is the regular AAVE token leverage mentioned in [the dedicated article](leverage-aave-tokens.md).

## Mai Finance

Following the AAVE deposit, we get amWMATIC in our wallet. We can use the yield page on Mai Finance to auto-compound the reward provided by AAVE with the rewards from the Matic incentive and get an additional 4% on our MATIC earned on Adamant.

The camWMATIC can then be used as collateral on Mai Finance by depositing them in the camWMATIC vault, which allows us to borrow MAI, and swap a part of the minted MAI into USDC. Once we have more MAI and USDC in our wallet, we can combine the 2 stable coins into additional LP tokens that will be deposited on QuickSwap and Impermax. Once again, if you need details on how you can do that, please read [the dedicated article](leverage-aave-tokens.md).

## Bootstrapping the system

What follows is a simulation made with an initial investment of $1,000 worth of MAI/USDC LP tokens, and the current APRs / APYs given by the different platforms on August 30th 2021. This is not a real application of what we described above. Rates will vary, token prices will vary, some programs will come to an end etc ... so the final results are just an estimation of what you could get if everything remained stable, which will never be the case.

### Day 1

Since we have $1,000 worth of MAI/USDC, we want to split the LP tokens between QuickSwap and Impermax. Because Impermax allows us to leverage our deposit, we can actually put more tokens on QuickSwap and use the leverage option on Impermax to match what we get on QuickSwap.

In order to lower the risk of negative interests on Impermax, the split will be as follows:

* $900 worth of MAI/USDC on QuickSwap
* $100 worth of MAI/USDC on Impermax with a x9 lever to expose $900 in the MAI/USDC pool

For the rest of the simulation, we will consider that QuickSwap grants a 25.56% APR on MAI/USDC paid in QUICK tokens, and Impermax gives a 20% average APR on MAI/USDC at x9, only paid in IMX tokens. This corresponds to a daily rate of

* \+0.07% on QuickSwap
* \+0.05% on Impermax

This means that at the end of Day 1, we already collected

* $0.63 worth of QUICK
* $0.49 worth of IMX

From there, we can combine all the IMX we get with a portion of the QUICK reward into IMX/QUICK LP pair that will be deposited on Adamant. The LP pair has a value of $0.98 and we still have $0.14 worth of QUICK that we deposit on the Dragons's Lair for dQUICK. dQUICK are then used on Dragon's Syrup to start collecting ADDY on Day 2.

| Reward type              | Value in dollars |
| ------------------------ | ---------------- |
| dQUICK on QuickSwap      | 0.14             |
| ADDY on QuickSwap        | 0                |
| IMX/QUICK on Adamant     | 0.98             |
| ADDY on Adamant          | 0                |
| WMATIC on Adamant        | 0                |
| camWMATIC on Mai Finance | 0                |
| debt on Mai Finance      | 0                |

### Day 2

We still have the same position on QuickSwap and Impermax, nothing changes and we once again get $0.63 worth of QUICK and $0.49 worth of IMX that are used to get $0.98 worth of IMX/QUICK and $0.14 of dQUICK deposited in the ADDY farm on QuickSwap.

However, the IMX/QUICK position on Adamant is earning 151.96% APR in IMX/QUICK (or +0.42% daily). This means that our original $0.98 deposit is now at $0.984, and we're adding $0.98 from farming on QuickSwap and Impermax. It also generated 177.43% APR (or +0.49% daily) ADDY, corresponding to $0.005.

On QuickSwap, the dQUICK we deposited in Dragon's Syrup is generating additional QUICK tokens at 12.26% APR (+0.03% daily) and ADDY tokens at 17.08% APR (+0.05% daily). This is applied to the $0.18 worth of QUICK, meaning that at the end of Day 2 we already generated $0.00006 worth of ADDY and $0.000054 worth of QUICK. The ADDY reward can be claimed and added into Adamant to start boosting the ADDY APR of the IMX/QUICK position.

| Reward type              | Value in dollars |
| ------------------------ | ---------------- |
| dQUICK on QuickSwap      | 0.274            |
| ADDY on QuickSwap        | 0.00006          |
| IMX/QUICK on Adamant     | 1.98             |
| ADDY on Adamant          | 0.005            |
| WMATIC on Adamant        | 0                |
| camWMATIC on Mai Finance | 0                |
| debt on Mai Finance      | 0                |

### Day 3

Moving on, the ADDY reward claimed on Adamant are now generating some WMATIC reward. The first $0.005 worth of ADDY collected earn 56% APR (0.15% daily) or WMATIC dividends, which corresponds to $0.000007 worth of WMATIC. Keep in mind we're only starting the engine here.

| Reward type              | Value in dollars |
| ------------------------ | ---------------- |
| dQUICK on QuickSwap      | 0.411            |
| ADDY on QuickSwap        | 0.00019          |
| IMX/QUICK on Adamant     | 2.971            |
| ADDY on Adamant          | 0.014            |
| WMATIC on Adamant        | 0.000007         |
| camWMATIC on Mai Finance | 0                |
| debt on Mai Finance      | 0                |

### Day 4

We can now add the WMATIC in the loop. This dividend will be deposited on AAVE, then used on Mai Finance to borrow new MAI.

| Reward type              | Value in dollars |
| ------------------------ | ---------------- |
| dQUICK on QuickSwap      | 0.548            |
| ADDY on QuickSwap        | 0.00038          |
| IMX/QUICK on Adamant     | 3.969            |
| ADDY on Adamant          | 0.029            |
| WMATIC on Adamant        | 0.000029         |
| camWMATIC on Mai Finance | 0.000007         |
| debt on Mai Finance      | 0.0000035        |

At this point, the "debt" on Mai Finance will be used to increase the MAI/USDC LP positions on both QuickSwap and Impermax, and the system is completely primed.

## Farming results

![](../.gitbook/assets/screen-shot-2021-08-30-at-11.33.34-am.png)

### Daily routine

The daily routine is composed by the following transactions

* Harvest IMX on Impermax
* Harvest QUICK on QuickSwap
* Create new IMX/QUICK LP pair on QuickSwap
* Deposit the remaining QUICK on Dragon's Lair to get dQUICK
* Deposit dQUICK on Dragon's Syrup to get additional ADDY
* Harvest ADDY on Dragon's Syrup
* Deposit harvested ADDY on Adamant vault
* Deposit IMX/QUICK LP tokens on Adamant
* Harvest ADDY on Adamant from LP pair
* Harvest WMATIC dividends on Adamant
* Deposit WMATIC on AAVE and get amWMATIC
* Deposit amWMATIC on Mai Finance and get camWMATIC
* Deposit camWMATIC on Mai Finance's vault
* Borrow 50% of the deposit as MAI stable coin on Mai Finance
* Swap 50% of the minted MAI for USDC on Mai Finance
* Create new MAI/USDC LP pair on QuickSwap
* Deposit 90% of the new LP tokens on QuickSwap liquidity pool
* Deposit 10% of the new LP tokens on Impermax liquidity pool
* Leverage the new position on Impermax to match the position on QuickSwap

### Raw results month after month

| Month | dQUICK | IMX/QUICK | ADDY    | WMATIC | Debt   |
| ----- | ------ | --------- | ------- | ------ | ------ |
| 1     | $4.25  | $32.56    | $2.32   | $0.03  | $0.02  |
| 2     | $8.36  | $68.34    | $9.65   | $0.28  | $0.15  |
| 3     | $12.48 | $108.86   | $22.30  | $0.98  | $0.49  |
| 4     | $16.59 | $154.78   | $41.34  | $2.41  | $1.20  |
| 5     | $20.71 | $206.83   | $67.50  | $4.86  | $2.42  |
| 6     | $24.84 | $265.83   | $101.73 | $8.70  | $4.34  |
| 7     | $28.97 | $332.74   | $145.11 | $14.31 | $7.15  |
| 8     | $33.12 | $408.63   | $198.87 | $22.14 | $11.06 |
| 9     | $37.29 | $494.73   | $264.40 | $32.70 | $16.34 |
| 10    | $41.48 | $592.45   | $343.28 | $46.57 | $23.26 |
| 11    | $45.71 | $703.39   | $437.33 | $64.40 | $32.19 |
| 12    | $49.97 | $829.37   | $548.59 | $86.94 | $43.46 |

### Day 365

After a complete year, the final state of our investment would be

| Reward type              | Value in dollars |
| ------------------------ | ---------------- |
| dQUICK on QuickSwap      | 50.689           |
| ADDY on QuickSwap        | 4.325            |
| IMX/QUICK on Adamant     | 851.968          |
| ADDY on Adamant          | 568.972          |
| WMATIC on Adamant        | 91.209           |
| camWMATIC on Mai Finance | 91.220           |
| debt on Mai Finance      | 44.30            |

Note that the WMATIC in Adamant and collected daily so they're not part of the final revenue generated via this process. Also, the ADDY that have been generated via the QuickSwap farm haven't been harvested daily and added to boost the ADDY rewards on Adamant in this simulation (it is already complex enough).

Finally, after one year, the generated revenue is worth $1,567.174. If we consider the initial investment was $1,000 worth of MAI/USDC, this leads to a final APY of 156.71% on our stable pair.

## Conclusion

This Lego game allowed us to generate an impressive APY from stable coin farming, with very little risk exposure. Of course, this simulation makes a few assumptions that are 100% incorrect, but it illustrates how we can combine different DApps to maximize yield farming. It also showcases that it's not a necessity to sell tokens that we farm, and that there's certainly a was to use them efficiently if you take the time to research possibilities.

## Disclaimer

This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
