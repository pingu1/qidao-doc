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

Se você decidir fazer staking com suas recompensas ou reacumular, é importante entender que sua recompensa mudará dependendo da frequência com que você realiza sua rotina de colheita + investimento. Como lembrete, a fórmula que vincula APY e APR é a seguinte:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Nesta equação, `N` representa o número de vezes que você reacumula suas recompensas em um ano. Portanto, e APR de 200%, conforme acima, forneceria o seguinte APY, dependendo da frequência que você reacumula:

| Frequência de reacumulação | APY equivalente |
| -------------------------- | --------------- |
| Diariamente                | 634.88 %        |
| Duas vezes por semana      | 625.01 %        |
| Semanalmente               | 611.71 %        |
| Duas vezes por mês         | 609.55 %        |
| Mensalmente                | 535.86 %        |
| A cada trimestre           | 406.25 %        |
| A cada semestre            | 300.00 %        |

Reacumular manualmente mais de uma vez por dia pode ser caro, dependendo da rede em que você está. Mas, basicamente, é claro que quanto mais você reinveste, melhor a recompensa. Isso também explica por que o otimizadores de rendimento / reacumuladores automáticos são populares. Lembre-se de que, ao reacumular, você adiciona pressão de venda ao token que cultiva, o que terá um impacto negativo no preço desse token. Se esse também for o token que você está usando para farm (no nosso exemplo ELK), você pode ser afetado por perdas impermanentes, a menos que esteja usando a DEX da Elk Finance, que te protege de perdas impermanentes.

## Escolhendo a pool correta

O par MAI-ELK foi implantado em várias redes, portanto, é possível que você invista seu capital na rede que oferece as melhores taxas.

![Pools MAI-ELK na Gnosis (topo), Moonriver (meio) e Harmony (abaixo) em janeiro de 2021](../../.gitbook/assets/elk-farming-3.png)

{% hint style="info" %}
A pool MAI-ELK também pode ser implantado em outras redes em um futuro próximo, possivelmente na Polygon, Cronos e Fantom. Isso não é garantido e não há previsōes, então fique atualizado verificando os diferentes servidores Discord de ambos os projetos e seguindo-os no twitter.
{% endhint %}

Além da taxa de recompensa em cada rede, você também pode considerar o preço do token ELK. De fato, se o preço for quase o mesmo em todas as redes, a pequena diferença também pode ser um fator para você escolher a rede em que deseja cultivar o token ELK.

![Preço dos tokens ELK em todas as redes onde está presente.](../../.gitbook/assets/elk-farming-4.png)

Como você pode ver, a pool MAI-ELK na Moonriver oferece uma melhor taxa de recompensa, e o token ELK também tem um preço mais alto nessa rede. Isso significa que, no momento em que escrevo, pode ser melhor cultivar a pool MAI-ELK na Moonriver do que na Harmony ou na Gnosis, especialmente se você planeja vender uma parte dos tokens cultivados. Observe que isso pode não ser o caso o tempo todo, portanto, certifique-se de escolher sua rede corretamente e de fazer suas próprias pesquisas antes de ingressar em um pool LP. Por fim, é altamente recomendável ler a [documentação sobre proteção de perda impermanente](https://docs.elk.finance/features/impermanent-loss-protection) porque o seguro depende muito do número de dias em que seus tokens LP são depositados na pool.

Como observação, como a ponte de ELK é gratuita, você pode mudar de uma rede para outra para sempre se beneficiar das melhores taxas. Certifique-se de entender que, ao fazê-lo, você também influenciará as taxas de recompensa da pool que você sair e da que você ingressar (menos liquidez aumentará o APR, mais liquidez o diminuirá).

## Aviso legal

Este guia foi escrito para ilustrar as diferentes maneiras de produzir rendimentos usando tokens de fornecimento de liquidez. Você influenciará muito seus ganhos com a estratégia que escolher, bem como sua exposição ao risco. Claro, todas as noções apontadas neste documento também se aplicam a qualquer par de LPs, e é altamente recomendável executar suas próprias simulações antes de escolher uma estratégia, um par de LPs, um pool ou mesmo um DEX.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
