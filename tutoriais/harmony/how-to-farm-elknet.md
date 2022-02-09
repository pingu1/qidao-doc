---
description: >-
  Este guia apresenta diferentes formas de fazer farming com um único par LP
  para ilustrar as diferenças entre staking e reacumular tokens.
---

# Um par LP, diferentes formas de farming

## Introdução

Fornecer liquidez em uma DEX (**D**ecentralized **EX**change, ou Corretora Decentralizada) e farming é uma das maneiras mais comuns de gerar rendimentos por DeFi (**De**centralized **Fi**nance, ou Finanças Descentralizadas). No entanto, muitos usuários apenas prestam atenção nas taxas da LP pool (**L**iquidity **P**roviding, ou Fornecimento de Liquidez) que entram, sem realmente verificar se a taxa é dada em APR (**A**nnual **P**ercentage **R**eward) ou APY (**A**nnual **P**ercentage **Y**ield). Existem muitas maneiras de participar de uma pool e gerenciar os tokens de recompensa. Veremos neste guia algumas das maneiras diferentes de fazer farming em um das pools mais recentes na Harmony, MAI-ELK, e veremos o que você pode fazer com os tokens ELK que receberá como recompensa.

{% hint style="info" %}
Este guia definitivamente não é um conselho financeiro, foi feito com um objetivo educacional em mente. Você precisa ficar atento às variações de preços, oferta e demanda, programas de recompensas, datas de término dos programas, perdas impermanentes, etc. O objetivo não é propor receitas que possam ser seguidas às cegas, então faça sua lição de casa e sua própria simulação, e só invista o que você está disposto a perder.
{% endhint %}

![](../../.gitbook/assets/elk-farming-1.png)

## Elk Finance

[Elk Finance](https://app.elk.finance/#/) é um DEX bifurcado da Uniswap v2, bem como uma AMM (Automoated Market Maker). Você encontrará todos os recursos usuais dos forks Uniswap: negociar seus ativos, combinar suas diferentes moedas criptográficas em tokens LP, cultivar alguns pares LP e apostar seu token nativo, o ELK.

O que torna a Elk Finance um projeto totalmente diferente é sua presença em muitas blockchains, e não apenas nas redes compatíveis com EVM (Ethereum Virtual Machine). De fato, a Elk Finance está presente em 16 redes e planeja expandir para muitas outras. Eles conseguiram construir uma ponte entre todas essas cadeias para permitir que os usuários transferissem o token ELK: O ELKNET.

![Enviando alguns ELK da Harmony para a Moonriver usando a ElkNet](../../.gitbook/assets/elk-farming-2.png)

Além disso, um recurso interessante proposto pela ElkNet é a possibilidade de trocar uma parte do ativo transferido por tokens de gas do destino. Isso é útil se você estiver acessando pela primeira vez uma blockchain que não tenha faucets disponíveis.

{% hint style="success" %}
Exceto por redes onde o gas é alto (apenas Avalanche e Cronos no momento da escrita), usar a ElkNet para enviar seus tokens ELK de uma rede para outra é feito sem despesas. Você leu isso direito, você não paga taxas de envio!
{% endhint %}

Por último, a Elk Finance fornece proteção contra perda impermanente. Você pode ler todos os detalhes sobre o programa de perda impermanente em [sua documentação oficial](https://docs.elk.finance/features/impermanent-loss-protection), mas basicamente, tudo que você precisa saber é que, se o preço de ELK alterar entre o momento em que você depositar e o momento que você retirar, você receberá ELK extra a fim de cobrir a perda impermanente. Como a MAI é atrelado a 1 USD, a perda impermanente só está ligada ao movimento de preços de ELK, então você fica sempre ganhando ao entrar nas LP pools na DEX Elk Finance.

## Farming com o Par LP MAI-ELK

O ELK Finance fez uma parceria com a Mai Finance em janeiro de 2022 para propor o farming de tokens usando o par LP MAI-ELK em sua DEX. O par MAI-ELK pode ser usado em 3 redes diferentes por enquanto: Harmony, Moonriver e Gnosis. Algumas pools adicionais podem ser lançadas mais tarde na Polygon, Cronos e Fantom. Vamos ver as diferentes estratégias que você pode aplicar nesta nova pool.

{% hint style="info" %}
Estamos propondo este guia para a Harmony porque as taxas de gas são muito baratas, o que permite que você reacumule suas recompensas manualmente diariamente. Isso a torna uma blockchain muito boa para iniciantes que têm apenas alguns dólares para investir. No entanto, tudo apresentado aui também pode ser aplicado em qualquer rede.
{% endhint %}

### Farming e Staking

A primeira estratégia é bastante simples:

* Combine seu par LP&#x20;
* Deposite o LP na pool MAI-ELK para obter um APR de 200%&#x20;
* Colha suas recompensas diariamente&#x20;
* Faça staking para obter um APR de 32,53%

Se você começar com $100, aqui estão os resultados que você pode obter mensalmente em um ano completo de farming, supondo que as taxas fornecidas acima permaneçam as mesmas durante o período inteiro.

| Dia | MAI-ELK ($) | ELK em Staking ($) |
| --- | ----------- | ------------------ |
| 30  | 100.000     | 16.653             |
| 60  | 100.000     | 33.756             |
| 90  | 100.000     | 51.323             |
| 120 | 100.000     | 69.366             |
| 150 | 100.000     | 87.897             |
| 180 | 100.000     | 106.930            |
| 210 | 100.000     | 126.479            |
| 240 | 100.000     | 146.557            |
| 270 | 100.000     | 167.180            |
| 300 | 100.000     | 188.360            |
| 330 | 100.000     | 210.115            |
| 360 | 100.000     | 232.458            |

No final do ano, você teria:

* $100.00 de LP tokens MAI-ELK na pool
* $236.24 de tokens ELK em staking

O que corresponde a um APY médio de 236,24%. Não é exatamente um APR porque parte da recompensa é reacumulada (ELK em staking).

{% hint style="info" %}
Você pode encontrar todos os resultados e a fórmula usada para construir esta tabela nesta [planilha da Google Sheets](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) na primeira aba. Você pode copiar esse arquivo para o seu próprio disco e ajustar as taxas e o investimento inicial para ver a alteração do APY causada pelos valores inseridos.
{% endhint %}

### Farming e reacumulando diretamente

Reacumular significa colher suas recompensas e as usar para criar tokens LP adicionais. No nosso caso, você iria:

* colher recompensas ELK
* vender 50% por MAI
* combinar em tokens LP MAI-ELK adicionais
* depositar na pool

Se você começar com o mesmo investimento inicial de $100, os resultados que você pode esperar para um ano completo de farming, supondo que as taxas fornecidas permaneçam as mesmas para todo o período, são os seguintes:

| Dia | MAI-ELK ($) |
| --- | ----------- |
| 30  | 117.172     |
| 60  | 138.044     |
| 90  | 162.635     |
| 120 | 191.607     |
| 150 | 225.739     |
| 180 | 265.952     |
| 210 | 313.328     |
| 240 | 369.143     |
| 270 | 434.901     |
| 300 | 512.374     |
| 330 | 603.647     |
| 360 | 711.179     |

E no final do ano, você teria:

* $730.878 em LP tokens MAI-ELK na pool

O que corresponde, para um investimento inicial de $100, a um APY de 630,88%. Como estamos reacumulando a recompensa, este é o APY exato que você obteria com um APR de 200%.

Como observação, as fórmulas para calcular o APY de um APR com reacumulação diária (ou um APR a partir de um APY) são as seguintes:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

$$
APR = N * (( 1 + APY)^\frac{1}{N} - 1)
$$

Sendo `N`  o número de vezes que você reacumula suas recompensas. No nosso caso, as fórmulas nos dariam:

$$
APY = ( 1 + \frac{2}{365})^{365}-1 = 634.88\%
$$

$$
APR = 365 * (( 1 + 6.3488)^\frac{1}{365} - 1) = 199.99\%
$$

É fácil perceber que, se você aplicar um APR de 200% (APR da LP pool) à sua recompensa, obterá melhores rendimentos do que se aplicar um APR de 32,53% (APR de staking). Aqui, o reinvestimento é muito melhor do que o staking enquanto a APR de farming for maior do que APR de staking. Obviamente, isso pode mudar com a quantidade de liquidez no pool.

{% hint style="info" %}
Como na seção anterior, a simulação pode ser encontrada na mesma [planilha do Google](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) na segunda aba.
{% endhint %}

### Farming e reacumulando usando a Mai Finance

Se o staking e o reinvestimento estão dando bons resultados, ambos os métodos estão diretamente ligados ao preço do token ELK, portanto, o valor do seu investimento variará com o preço do ELK. Já vimos que a reacumulação oferece melhores opções em comparação com o staking. Agora veremos como você pode capturar certo valor de suas recompensas de farming e continuar investindo na mesma pool usando a Mai Finance. A rotina diária seria a seguinte:

* Colha as recompensas ELK.
* Venda 66% da recompensa para comprar algum token blue chip aceito como garantia na Mai Finance. Para nosso exemplo, usaremos o token ONE.
* Deposite os tokens ONE em seu vault na Mai Finance.
* Tome MAI emprestado adicional a uma CDR de 200% (Colateral to Debt Ratio, ou Proporção de Garantia para Dívida), cujo valor corresponderá aos seus tokens ELK restantes
* Combine-os em tokens LP MAI-ELK adicionais
* Deposite-os na pool

{% hint style="info" %}
Converter seus tokens de recompensa em ONE pode não ser a maneira mais segura de proteger seus ativos, uma das melhores maneiras de fazer isso é os converter em stablecoins. No entanto, as opções da Mai Finance na Harmony (ao escrever este artigo) são bastante limitadas. Você pode obter melhores opções no futuro (após janeiro de 2021), como fazer staking com tokens LP da Stake DAO como garantia (consulte nosso[ artigo dedicado à Polygon](../polygon/the-elephant-and-the-otter.md) para ver como você pode usar os tokens da Stake DAO na Mai Finance).
{% endhint %}

Se você começar com o mesmo investimento inicial de $100, os resultados que você pode esperar para um ano completo de farming, supondo que as taxas fornecidas permaneçam as mesmas para todo o período e que seu vault não seja liquidado, são os seguintes:

| Dia | MAI-ELK ($) | ONE ($) | Dívida na Mai ($) |
| --- | ----------- | ------- | ----------------- |
| 30  | 111.154     | 11.560  | 5.780             |
| 60  | 124.003     | 24.456  | 12.228            |
| 90  | 138.337     | 38.842  | 19.421            |
| 120 | 154.328     | 54.892  | 27.446            |
| 150 | 172.168     | 72.797  | 36.398            |
| 180 | 192.070     | 92.772  | 46.386            |
| 210 | 214.273     | 115.055 | 57.528            |
| 240 | 239.042     | 139.915 | 69.958            |
| 270 | 266.674     | 167.648 | 83.824            |
| 300 | 297.501     | 198.588 | 99.294            |
| 330 | 331.891     | 233.106 | 116.552           |
| 360 | 370.257     | 271.609 | 135.805           |

E no final do ano, você teria:

* $377.069 em tokens LP MAI-ELK na pool
* $278.446 em tokens ONE em seu vault
* $139.223 em dívidas na Mai Finance
* Uma CDR de 200%, como esperado

A partir de uma posição original de $100 em MAI-ELK, isso representaria um APY de 416,29%. Aqui estamos obtendo um pouco menos de ganhos em comparação com a reacumulação pura, porém também extraímos boa parte de nossos ganhos para ONE, que pode ser menos volátil que ELK, portanto, pode apresentar menos risco.

{% hint style="info" %}
Mais uma vez, a simulação pode ser encontrada na mesma [planilha da Google](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) na terceira guia.
{% endhint %}

Alternativamente, você também pode vender todas as suas recompensas ELK por tokens aceitos na Mai Finance, tomar emprestado MAI e vender parte dele para comprar ELK adicional para aumentar sua posição no pool MAI-ELK. Ao fazer isso, você aumenta sua exposição a ONE, mas também aumenta sua dívida. Você terminaria com $270.715 em MAI-ELK, $352.913 em ONE e $171.457 em dívidas para um APY total de 342,17%.

## Influência da frequência com que você reacumula

Whether you decide to stake your rewards or compound, it's important to understand that your reward will change depending on the frequency at which you perform your harvest + invest routine. As a reminder, the formula that links APY and APR is as follows:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

In this equation, `N` represents the number of times you compound your rewards in a year. So, and APR of 200% as above would give you the following APY depending on the frequency you compound:

| Compounding frequency | equivalent APY |
| --------------------- | -------------- |
| daily                 | 634.88 %       |
| twice in a week       | 625.01 %       |
| weekly                | 611.71 %       |
| twice in a month      | 609.55 %       |
| monthly               | 535.86 %       |
| quarterly             | 406.25 %       |
| twice in a year       | 300.00 %       |

Manually compounding more than once a day can be expensive depending on the chain you're on. But basically, it's clear that the more often you compound, the better the reward. This is also explaining why yield optimizer / auto-compounder are popular. Keep in mind that by compounding, you add sell pressure to the token you farm, which will have a negative impact on the price of that token. If that's also the token you are using to farm (in our exemple ELK), you may be impacted by impermanent losses, unless you're using Elk Finance DEX, which protects you from impermanent losses.

## Choosing the right pool

The MAI-ELK pair has been deployed to several chains, so it's possible for you to deploy your capital to the chain that offers the best rates.

![MAI-ELK pools on Gnosis (top), Moonriver (middle) and Harmony (bottom) as of January 2021](../../.gitbook/assets/elk-farming-3.png)

{% hint style="info" %}
The MAI-ELK pool may also be deployed to other chains in a near future, possibly on Polygon, Cronos and Fantom. This is not guaranteed and there's no ETA for that, so stay updated by checking the difference Discord servers of both projects, of following them on twitter.
{% endhint %}

Besides the reward rate on each chain, you may also have to consider the price of the ELK token on each chain. Indeed, if the price is almost the same on all chains, the tiny difference may also be a factor for you to choose the chain where you want to farm the ELK token.

![Price of the ELK tokens on all the chains where it's present](../../.gitbook/assets/elk-farming-4.png)

As you can see, the MAI-ELK pool on Moonriver gives a better reward rate, and the ELK token also has a higher price on that chain. This means that, at time of writing, it may be better to farm the MAI-ELK pool on Moonriver than on Harmony or Gnosis, especially if you plan to sell a part of the farmed tokens. Note that this may not be true all the time, so make sure you choose your chain properly and that you do your own researches before joining a LP pool. Finally, it is strongly recommended to read the [documentation about IL protection](https://docs.elk.finance/features/impermanent-loss-protection) because the insurance is highly dependant on the number of days your LP tokens are deposited in the pool.

As a side note, because bridging ELK is free, you can possibly move from one chain to another in order to always benefit from the best rates. Make sure that you understand that by doing so, you will also influence the reward rates of the pool you exit and the one you join (less liquidity will increase the APR, more liquidity will lower it).

## Disclaimer

This guide has been written in order to illustrate the different ways to farm yields using liquidity providing tokens. You will highly influence your gains with the strategy that you pick, as well as your exposure to risk. Of course, all the notions pointed in this document are also applicable to any LP pair, and it's highly recommended to run your own simulations before picking a strategy, a LP pair, a pool or even a DEX.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
