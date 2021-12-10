---
description: >-
  Este guia irá explicar em detalhes como voce pode usar QI, o token nativo da
  Mai Finance, na Polygon. Nós também iremos analisar se Qi é uma boa
  oportunidade de investimento, e o que guia o seu preço.
---

# O que fazer com Qi na Polygon

## Introdução

Qi (\[tʃ Í] ou _chee_), é o token nativo da Mai Finance. Alguns o utilizam para votar e participar das QIP (**Q**iDAO **I**mprovement **P**roposals, ou Propostas de Melhoria QiDAO), alguns fazem stake com ele para conseguir ainda mais tokens, e alguns simplesmente fazem farming. Você pode encontrar excelentes informaçōes sobre como utilizar seu Qi na plataforma Mai Finance neste [tutorial dedicado a renda passiva](../Universidade-do-MAI/earning-passive-income-with-qidao.md).

Este guia, como a maioria dos tutoriais de investimento, irá focar principalmente em farming e rendimentos de harvesting, esta vez utilizando o token Qi. Nós mostraremos como você pode gerar bastante Qi, e como usá-los nas diferentes plataformas da rede Polygon.

Fazendeiros humildes irão, às vezes, te dizer que você precisa se manter humilde, vender o que você colheu e realizar lucros. Mas pessoalmente, eu prefiro:

> Dê ao homem um peixe e ele se alimentará por um dia. Ensine um homem a pescar e ele se alimentará por toda a vida.

Então pegue sua vara de pescar, e siga o guia.

## O que fazer com seu Qi na Polygon

### Staking

Eu não irei gastar muito tempo aqui, pois já há um guia completo sobre assunto. Mas tenha em mente que a Mai Finance coleta os rendimentos, e redistribui uma grande porção aos stakers de Qi. Staking de Qi na Mai Finance é um dos melhores usos para o token, e no momento, em Setembro de 2021, 23% de todo o Qi em circulação fica travado em média por 2 anos.

### Farming com par LP

Mais uma vez, já há algumas outras páginas explicando como você pode incluir o token Qi na sua estrategia de farming para gerar rendimentos e nunca vender qualquer um de seus tokens de farm. Por exemplo, temos os guias [Empilhe DApps como peças de Lego ](../investment-tutorials/stack-dapps-like-lego-bricks.md)e [Farming ou Staking?](../investment-tutorials/farming-or-staking-or-both.md) para maiores detalhes.

Um lembrete rápido, Qi é pareado a diferentes tokens para formar pares LP (**L**iquidity **P**rovider, ou Provedor de Liquidez) na [QuickSwap](https://quickswap.exchange/#/quick) para que você possa fazer o farm de:

* Qi-WMATIC na Mai Finance e receber recompensas em tokens Qi
* Qi-WETH na QuickSwap e receber recompensas em tokens QUICK
* Qi-QUICK na QuickSwap e receber recompensas em tokens QUICK

![LP Pool na QuickSwap para o par Qi-WETH](<../.gitbook/assets/image (19) (2).png>)

### Farming apenas com Qi

Qi também pode ser usado sozinho na [Impermax](https://polygon.impermax.finance). Impermax é uma platforma onde você pode alavancar um par LP varias vezes no intuito de aumentar seus ganhos da QuickSwap.

Ela funciona da seguinte maneira: você deve tomar emprestado os 2 tokens que compōem o par que você pretende utilizar na farm, então combiná-los em mais LP tokens, e fazer o farming com uma posição muito maior. Na maioria dos casos, as taxas de emprestimo são compensados pelo APR do farming, entregando a você um bom lucro líquido.&#x20;

![Posição em Qi-WETH alavancada na Impermax](<../.gitbook/assets/image (20).png>)

Nós podemos ver aqui que o APR final na Impermax é de 393.88% após alavancarmos 5 vezes, baseado no APY de 239.68% da QuickSwap.

{% hint style="info" %}
Note que a Impermax te fornece as taxas APRs (**A**nnual **P**ercentage **R**ewards, ou Taxa de Percentual Anual) enquanto a QuickSwap te mostra os APYs (**A**nnual **P**ercentage **Y**ields, ou Rendimento Percentual Anual), o que significa que a QuickSwap assume que você reacumulará suas recompensas diariamente. O APY de 239.68% na QuickSwap corresponde a um APR 122.49%.
{% endhint %}

De qualquer forma, na Impermax, para você tomar Qi e WETH emprestados para alavancar sua posição, você precisa obtê-los de algum algum. Isso é possível apenas porque alguns outros usuários (ou você mesmo) também fornecem ambos os tokens separadamente. Quanto mais tomarmos emprestado, maior a taxa de juros, e com isso menor o APR final, que pode se tornar até mesmo negativo.&#x20;

![Estatísticas de Qi e WETH para o mercado de Qi-WETH na Impermax](<../.gitbook/assets/image (11).png>)

For our example, we will focus on Qi. You can see that the total supply of Qi is $427.21 and the total amount used in leveraged position is $321.44, giving the utilization rate of 75.24%. Impermax has some internal mechanism that automatically calculates the supply APR (APR that people lending Qi will get) and the borrowing APR (percentage of the farmed reward that will be deduced to pay the loan).

This means that you can provide Qi solely on Impermax and get, in our example, 43.73% APR, at the moment of writing. As supply and demand varies, the supply APR will also increase / decrease. When you supply single tokens on Impermax, you will get rewarded with the token you provide, meaning that this strategy will make you accumulate more Qi over time.

While you are on Impermax, you can also use the leverage option to get IMX rewards. Please read the [Stacking guide](../investment-tutorials/stack-dapps-like-lego-bricks.md) to get more details on how you can include Impermax in your farming strategy.

### Balancer

Balancer is a really nice toolbox for any strategy, especially the ones that include Qi and/or MAI. Balancer proposes an equivalent of LP pair mining, but with more than 2 tokens provided in a 1:1 ratio. The pool can have 3, 4 or 5 tokens (sometimes even more) with different weight, and the algorithm in charge of the pool makes sure that the ratio for each token is always respected, selling some and buying others to keep it balanced.

The pool that we want to use here is a pool that contains Qi, WMATIC, BAL, USDC and MAI. This pool will reward you with both Qi and BAL tokens, and you can already see that you will be able to compound both into the pool. Because another amazing advantage of pools on Balancer is that you don't need to provide all tokens forming the pool in the proper ratio, the algorithm will do it for you. This means that you can indeed only deposit Qi in the pool and let the algorithm do the rest to rebalance everything.

![Details of the pool as of September 2021](<../.gitbook/assets/image (17).png>)

As a side note, BAL tokens can (or will soon be) usable as collateral on Mai Finance, which mean that you will have the option to store your BAL tokens on the BAL vault on Mai Finance, and borrow MAI against then. In addition to that, borrowing MAI against your BAL tokens will make you eligible for Qi rewards that will feed the pool on Balancer.

![Closed loop using Mai Finance and Balancer](<../.gitbook/assets/image (18).png>)

The APR of BAL vaults will highly dictates how interesting it is to have the vault in the loop, or if compounding your Qi into the Balancer's pool will be better.

## Understanding the price of Qi

Getting a lot of Qi is one thing, however if the token loses value over time, is it really a good strategy to keep it? In this section, we will try to understand the different factors that impact directly the price of Qi so that, when you start investing your Qis, you will get a better idea of how its price may vary, and what impact you will get on the Qi ecosystem.

### Qi emission

One of the main factor that will affect the price of Qi is the rate at which they are created. Indeed, price is always driven by demand and supply. If there's a lot of supply and very low demande, the price will naturally collapse. Hence understanding how Qi is generated is crucial to estimate its value over time.

There are currently 2 sources of Qi emission: farming rewards and vault rewards.

![LP farms on Mai Finance in September 2021](<../.gitbook/assets/image (12).png>)

If you are farming yields on MAI finance, you have the choice between the MAI/USDC pair and the Qi/WMATIC pair (as of September 2021).

* The MAI/USDC pair is rewarded with 0.5 Qi / block
* The Qi/WMATIC pair is rewarded with 1 Qi / block

On Polygon, the expected block time is 2 seconds, and since there are 86,400 seconds in a day, this means that the MAI/USDC pool is rewarded with 21,600 Qi every day, and the Qi/WMATIC with 43,200 Qi.

The pools of Mai Finance alone are responsible for 64,800 new Qi daily.

As for Vaults, each vault gets an emission of 0.05 Qi / block, or a daily emission of 2,160 Qi, and there are currently 10 Vaults, for a total of 21,600 Qi allocated as Vault rewards.

This means that each day, the equivalent of 86,400 new Qi are minted and distributed to users.

### Yield optimizers

Yield optimizers are platforms that will automatically compound the rewards with some pre-defined strategies, and allocate additional rewards for you to choose their site. However, a big part of the reward harvested is sold directly, and re-used in another way on these platforms.

As an example, Adamant offers you to farm the Qi/WMATIC LP pair on their platform, with the following reward distribution

![Qi-WMATIC pool on Adamant](<../.gitbook/assets/image (15).png>)

![Details of the 179.23% APR granted by Adamant](<../.gitbook/assets/image (14).png>)

You will notice that if the overall APR is higher than on Mai Finance, it's solely because Adamant is allocating additional ADDY rewards to the farmers. The amount of Qi that is actually redistributed to the farmer is 98.45% compared to the 134.42% you can get on Mai Finance.

From these 98.45% Qi reward, half of it is directly sold to buy WMATIC and form additional LP tokens that is then given to the farmer.

With 100$ worth of LP token, assuming the APR and the token prices remain the same for a complete year, and assuming there's no compounding, you would get after one year of farming

* $134.42 worth of new Qi on Mai Finance
* $98.45 worth of new Qi/WMATIC token, or $49.23 worth of new Qi on Adamant

This means that, in the process, $85.20 worth of Qi is simply sold directly on the market, which is more than 60% of the total emission allocated to the pool on Adamant.

And Adamant isn't the only platform proposing the same type of service. Some other examples are Beefy Finance and Kogecoin. From the $4.9M TVL in the Qi/WMATIC farm on Mai Finance, $2.3M are coming directly from Adamant, $41k from Beefy and $12k from Kogecoin, representing for these 3 platforms more than 50% of the value locked on Mai Finance. A raw estimation is that more than 30% of the total daily Qi emission is dumped by these platforms, putting some very negative sell pressure on the token, decreasing its price, which partially explains why Qi has difficulties keeping a high price.

### Understanding LP pairs

When you farm yields by providing LP pairs, the LP token is actually used to provide liquidity to users who are swapping one token for another. In our example of Qi/WETH, when someone is buying WETH, some of the token can be taken off the LP pool and sold to the user requiring it.

At that point, because some WETH has been taken off the pool, there is a balance mismatch: less WETH for the same amount of Qi. The algorithm in charge of maintaining the pool ratio to 1:1 will then sell some Qi from this pool to buy back some more WETH and recreate a perfect 1:1 ratio. The opposite things also happen when someone buys Qi, i.e. WETH is sold to buy back some Qi.

The same phenomenon occurs when one of the 2 tokens composing the pair gains or loses value. As an example, we will assume that Qi price is $1 and ETH price is $1,000, and that we have a pool that has $100 worth of Qi and $100 worth of WETH. It means that the pools contains 100 Qi and 0.1 WETH.

Now, if the price of ETH goes up to $2,000, if the pool keeps the same amount of token, we would have $100 worth of Qi but $200 worth of WETH, and we would have lost the balance. Hence, the algorithm in charge of the pool will sell a little bit of ETH to buy some Qi. In our easy example, $50 worth of ETH will be sold to buy $50 worth of Qi, and the final state would be

* 150 Qi with a value of $150$
* 0.075 ETH with a value of $150

This also means that when the price of one of the 2 token goes up, the pool creates some demande for the other, also driving its price up. The opposite is also true: if one token loses value, the other one will be sold to maintain a 1:1 ratio, driving the price down. This also partially explains the price fluctuation of Qi when compared to the price fluctuation of WEHT and WMATIC (the 2 main tokens to which Qi is paired).

![Price of Qi (left) VS Price of WMATIC (right)](<../.gitbook/assets/image (13).png>)

### Lack of use case

Finally, the lack of use for Qi, or the lack of known use cases, can explain why the price of the token is going down. People collecting Qi from Vault rewards and/or farming on Mai Finance will just sell it while it still has "some" value in order to realize a profit, with no long-term vision, which is actually a pretty reasonable strategy. This guide tries actually to promote different ways to use your Qi tokens without selling them, but if the price doesn't go up, or if you can't generate benefits in other tokens (a.k.a profit leak), there's very little advantages stacking them.

### How can we help price to go up?

If we want the price of Qi to go up (and who wouldn't want to), there are a few options.

* Reduce emission: with 86,400 new Qi minted daily, the supply is very high. If we cut down this emission, the supply may be lower, and with less supply, price should in theory go up. However, the current emission for the farms need to remain the same because they're part of a current partnership with QuickSwap. Vault incentives have been launched, and are an amazing way to promote the lending platform, pushing people to take loans, so cutting these emissions is probably another bad idea.
* Farm responsibly: I'm not saying that Adamant is the main culprit or is a bad product. Indeed, I include this platform in most of my strategies and use it on a daily basis. However, I try to farm in pools for which I have less concerns that the token will be dumped. If you want to farm yields on Adamant in a pool that is using the Mai Finance farm, keep in mind that you participate in the Qi depreciation. If you are ok with that, that's totally fine.
* Understand how things work: prices of ALL crypto-currencies are highly volatile, and most of the time, the price of BTC and ETH dictate the price of all other tokens. This is not done magically. Also, please understand that when some people earn money, it's because some other are loosing some. There's no free money, and magical internet money is actually not that magical.
* Find new ways to use your Qi tokens. This guide will always provide ideas that will help you increase the volume of your portfolio, and sell as few tokens as possible. Closed loops are the best because the output of one product feeds the input of the next one, creating a nice bubble that will only grow over time.

Keep also in mind that

$$
Value = Quantity * Price
$$

When the price go down but your quantity goes up, your value may increase, or at least it won't decrease as fast.

## Disclaimer

This guide is actually a result of many discussion about Qi price on the Discord channel. I realized that some people complaining about the price depreciation didn't fully understand the reasons about why the price of Qi was on a consistant down trend. This leads to frustration and delusion, which is very negative for Qi, the Mai Finance product, and the whole DeFi ecosystem in general. However, there's absolutely no guarantee that the price will ever go up, so if you want to keep your Qis and invest them, please do your own research and do it at your own risk. Plan your strategy properly and stick to it.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
