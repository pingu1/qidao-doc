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

Para o nosso exemplo, nós iremos nos concentrar em Qi. Você também pode ver que o fornecimento total de Qi é de $427.21 e a quantidade total usada em posiçōes alavancadas é de $321.44, que nos dá uma taxa de utilização de 75.24%. A Impermax possui um mecanismo interno que automaticamente calcula o APR de fornecimento (APR para as pessoas quem emprestam QI) e o APR de empréstimo (porcentagem da recompensa deduzida para pagar a dívida).

Isso significa que você pode prover apenas Qi na Impermax e obter, no nosso exemplo, um APR de 43.73%, no momento em que escrevo. Conforme a oferta e demanda variam, o APR de fornecimento também irá aumentar ou diminuir. Quando você fornece tokens na Impermax, você é recompensado com o token que você forneceu, o que significa que essa estratégia fará você acumular mais e mais Qi ao longo do tempo.&#x20;

Na Impermax, você também pode utilizar a opção de alavancagem e receber recompensas IMX. Por favor, leia o [guia sobre como empilhar DApps](../investment-tutorials/stack-dapps-like-lego-bricks.md) para obter mais detalhes sobre como você pode incluir Impermax na sua estratégia de farming.

### Balancer

Balancer é uma caixa de ferramentas muito boa para qualquer estratégia, especialmente para aquelas que incluem Qi e/ou MAI. A balancer propōe algo aquivalente à mineração de um par LP, mas com mais de 2 tokens sendo providos em uma proporção 1:1. A pool pode ter 3, 4 ou 5 tokens (às vezes até mais) com pesos diferentes, e o algoritmo que controla a pool garante que a proporção para cada token é sempre respeitada, vendendo algums e comprando outros para mantê-la equilibrada.

A pool que nós queremos usar aqui é a pool que contém Qi, WMATIC, BAL, USDC a MAI. Esta pool irá te recompensar com ambos Qi e BAL, e você já pode ver que será capaz de reacumular ambos na pool. E devido à outra incrivel vantagem das pools na Balancer, você não irá precisar prover os tokens que formam a pool na proporção correta, o algoritmo já faz isso para você. Isso significa que você pode depositar apenas QI na pool e deixar o algoritmo fazer o resto, equilibrando tudo.

![Details of the pool as of September 2021](<../.gitbook/assets/image (17).png>)

Uma observação é que tokens BAL podem (ou logo poderão) ser usados como garantia na Mai Finance, o que significa que você tem a opçao de guardar o seus tokens BAL na _vault_, ou cofre, BAL da Mai Finance, utilizá-los como garantia, e tomar emprestado MAI. Somado a isso, tomar emprestado MAI, com BAL como garantia, te fará elegível para receber recompensas em Qi que irão alimentar a pool na Balancer.

![Loop fechado usando a Mai Finance e a Balancer](<../.gitbook/assets/image (18).png>)

O APR das vaults BAL irá responder se vale mais a pena ter a vault no loop, ou se é melhor reacumular seu Qi na pool da Balancer.

## Entendendo o preço do Qi

Ter bastante Qi é uma coisa, porém se o token perde valor ao longo do tempo, será mesmo uma boa estratégia mantê-lo? Nessa seção, nós iremos tentar entender como diferentes fatores impactam o preço do Qi, para que, ao investir os seus Qis, você possa ter uma ideia mais clara de como o preço pode variar, e que impacto você terá no ecosistema Qi.

### Emissão de Qi

Um dos principais fatores que afetarão o preço de Qi é o ritmo no qual eles sãos criados. De fato, o preço é sempre o resultado de oferta e demanda. Se há muita oferta e pouca demanda, o preço irá naturalmente colapsar. Por isso é crucial entender como o Qi é produzido para estimar o seu valor ao longo do tempo.

Há atualmente 2 fontes de emissão de Qi: recompensas de farming e recompensas da vault.

![LP farms na Mai Finance em Setembro de 2021](<../.gitbook/assets/image (12).png>)

Se você busca obter rendimentos de farms na Mai finance, você pode escolher entre o par MAI/USDC e o par Qi/WMATIC (em Setembro de 2021).

* O par MAI/USDC é recompensado com 0.5 Qi / bloco
* O par Qi/WMATIC é recompensado com 1 Qi / bloco

Na Polygon, o tempo esperado para um bloco é de 2 segundos, e como há 86,400 segundos em um dia, isso significa que a pool MAI/USDC é recompensada com 21,600 Qi todos os dias, e a pool Qi/WMATIC com 43,200 Qi.

As pools na Mai Finance, sozinhas, são responsaveis por 64,800 de Qi diariamente.

Já as vaults, possuem uma emissão de 0.05 Qi / bloco cada, ou uma emissão diario de 2,160 Qi, e há atualmente 10 vaults, que resultam em um total de 21,600 Qi alocados como recompensa.

Isso significa que, todos os dias, o equivalente a 86,400 de novos Qi são cunhados e distribuídos aos usuários.

### Otimizadores de rendimento

Otimizadores de rendimento são plataformas que automaticamente reacumulam as recompensas de acordo com algumas estratégias pré-definidas, e alocam recompensas adicionais para voce escolher em seu website. Entretanto, uma grande parte da recompensas é vendida diretamente, e reutilizada de outra forma nestas plataformas.

Como exemplo, a Adamant oferece a você o farming do par LP Qi/WMATIC em sua plataforma, com a seguinte distribuição de recompensas:&#x20;

![Pool Qi-WMATIC na Adamant](<../.gitbook/assets/image (15).png>)

![Detalhes do APR de 179.23% APR garantido pela Adamant](<../.gitbook/assets/image (14).png>)

Você irá perceber que o APR total é maior do que na Mai Finance, somente porque a Adamant aloca recompensas ADDY adicionais aos farmers, ou fazendeiro. A quantidade de Qi é redistribuída é de 98.45% comparada aos 134.42% que você pode obter na Mai Finance.

Dessa recompensa em Qi de 98.45%, metade dela é vendida diretamente para comprar WMATIC e formar LP tokens adicionais, que são então dados aos farmer.

Com 100$ de LP token, assumindo que APR e o preço dos tokens permanecem os mesmo durante o ano todo, e assumindo que não haja reacumulação, você teria apos um ano de farming:&#x20;

* $134.42 de novos Qi na Finance
* $98.45 de novos tokens Qi/WMATIC, ou $49.23 de novos Qi na Adamant

Isto significa que, no processo, $85.20 de Qi são simplesmente vendidos no mercado, que é mais de 60% da emissão total alocada na pool da Adamant.

E a Adamant não é a unica plataforma disponibilzando este tipo de serviço. Outros exemplos são a Beefy Finance e Kogecoin. Dos $4.9M em TVL (Total Value Locked, ou Valor Total Bloqueado) na farm de Qi/WMATIC na Mai Finance, $2.3M estão vindo diretamente da Adamant, $41k da Beefy e $12k da Kogecoin, representado para essas 3 plataformas mais de 50% do valor bloqueado na Mai Finance. Uma estimativa bruta é que mais de 30% da emissão total diario de Qi é despejada por essas plataformas, causando uma grande pressão vendedora no token, diminuindo o seu preço, o que explica parcialmente o porque Qi tem dificuldade em manter um preço elevado.

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
