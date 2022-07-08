---
description: >-
  Este guia irá explicar em detalhes como voce pode usar QI, o token nativo da
  Mai Finance, na Polygon. Nós também iremos analisar se Qi é uma boa
  oportunidade de investimento, e o que guia o seu preço.
---

# O que fazer com Qi na Polygon

## Introdução

Qi (\[tʃ Í] ou _chee_), é o token nativo da Mai Finance. Alguns o utilizam para votar e participar das QIP (**Q**iDAO **I**mprovement **P**roposals, ou Propostas de Melhoria QiDAO), alguns fazem stake com ele para conseguir ainda mais tokens, e alguns simplesmente fazem farming. Você pode encontrar excelentes informaçōes sobre como utilizar seu Qi na plataforma Mai Finance neste [tutorial dedicado a renda passiva](../../Universidade-do-MAI/earning-passive-income-with-qidao.md).

Este guia, como a maioria dos tutoriais de investimento, irá focar principalmente em farming e rendimentos de harvesting, esta vez utilizando o token Qi. Nós mostraremos como você pode gerar bastante Qi, e como usá-los nas diferentes plataformas da rede Polygon.

Fazendeiros humildes irão, às vezes, te dizer que você precisa se manter humilde, vender o que você colheu e realizar lucros. Mas pessoalmente, eu prefiro:

> Dê ao homem um peixe e ele se alimentará por um dia. Ensine um homem a pescar e ele se alimentará por toda a vida.

Então pegue sua vara de pescar, e siga o guia.

## O que fazer com seu Qi na Polygon

### Staking

Eu não irei gastar muito tempo aqui, pois já há um guia completo sobre assunto. Mas tenha em mente que a Mai Finance coleta os rendimentos, e redistribui uma grande porção aos stakers de Qi. Staking de Qi na Mai Finance é um dos melhores usos para o token, e no momento, em Setembro de 2021, 23% de todo o Qi em circulação fica travado em média por 2 anos.

### Farming com pares LP

Mais uma vez, já há algumas outras páginas explicando como você pode incluir o token Qi na sua estrategia de farming para gerar rendimentos e nunca vender qualquer um de seus tokens de farm. Por exemplo, temos os guias [Montando DApps como peças de Lego ](stack-dapps-like-lego-bricks.md)e [Farming ou Staking?](farming-or-staking-or-both.md) para maiores detalhes.

Um lembrete rápido, Qi é pareado a diferentes tokens para formar pares LP (**L**iquidity **P**rovider, ou Provedor de Liquidez) na [QuickSwap](https://quickswap.exchange/#/quick) para que você possa fazer o farm de:

* Qi-WMATIC na Mai Finance e receber recompensas em tokens Qi
* Qi-WETH na QuickSwap e receber recompensas em tokens QUICK
* Qi-QUICK na QuickSwap e receber recompensas em tokens QUICK

![LP Pool na QuickSwap para o par Qi-WETH](<../../.gitbook/assets/image (19) (2) (1) (1) (1).png>)

### Farming apenas com Qi

Qi também pode ser usado sozinho na [Impermax](https://polygon.impermax.finance). Impermax é uma platforma onde você pode alavancar um par LP varias vezes no intuito de aumentar seus ganhos da QuickSwap.

Ela funciona da seguinte maneira: você deve tomar emprestado os 2 tokens que compōem o par que você pretende utilizar na farm, então combiná-los em mais LP tokens, e fazer o farming com uma posição muito maior. Na maioria dos casos, as taxas de emprestimo são compensados pelo APR do farming, entregando a você um bom lucro líquido.&#x20;

![Posição em Qi-WETH alavancada na Impermax](<../../.gitbook/assets/image (20).png>)

Nós podemos ver aqui que o APR final na Impermax é de 393.88% após alavancarmos 5 vezes, baseado no APY de 239.68% da QuickSwap.

{% hint style="info" %}
Note que a Impermax te fornece as taxas APRs (**A**nnual **P**ercentage **R**ewards, ou Taxa de Percentual Anual) enquanto a QuickSwap te mostra os APYs (**A**nnual **P**ercentage **Y**ields, ou Rendimento Percentual Anual), o que significa que a QuickSwap assume que você reacumulará suas recompensas diariamente. O APY de 239.68% na QuickSwap corresponde a um APR 122.49%.
{% endhint %}

De qualquer forma, na Impermax, para você tomar Qi e WETH emprestados para alavancar sua posição, você precisa obtê-los de algum algum. Isso é possível apenas porque alguns outros usuários (ou você mesmo) também fornecem ambos os tokens separadamente. Quanto mais tomarmos emprestado, maior a taxa de juros, e com isso menor o APR final, que pode se tornar até mesmo negativo.&#x20;

![Estatísticas de Qi e WETH para o mercado de Qi-WETH na Impermax](<../../.gitbook/assets/image (11).png>)

Para o nosso exemplo, nós iremos nos concentrar em Qi. Você também pode ver que o fornecimento total de Qi é de $427.21 e a quantidade total usada em posiçōes alavancadas é de $321.44, que nos dá uma taxa de utilização de 75.24%. A Impermax possui um mecanismo interno que automaticamente calcula o APR de fornecimento (APR para as pessoas quem emprestam QI) e o APR de empréstimo (porcentagem da recompensa deduzida para pagar a dívida).

Isso significa que você pode prover apenas Qi na Impermax e obter, no nosso exemplo, um APR de 43.73%, no momento em que escrevo. Conforme a oferta e demanda variam, o APR de fornecimento também irá aumentar ou diminuir. Quando você fornece tokens na Impermax, você é recompensado com o token que você forneceu, o que significa que essa estratégia fará você acumular mais e mais Qi ao longo do tempo.&#x20;

Na Impermax, você também pode utilizar a opção de alavancagem e receber recompensas IMX. Por favor, leia o [guia sobre como montar DApps](stack-dapps-like-lego-bricks.md) para obter mais detalhes sobre como você pode incluir Impermax na sua estratégia de farming.

### Balancer

Balancer é uma caixa de ferramentas muito boa para qualquer estratégia, especialmente para aquelas que incluem Qi e/ou MAI. A balancer propōe algo aquivalente à mineração de um par LP, mas com mais de 2 tokens sendo providos em uma proporção 1:1. A pool pode ter 3, 4 ou 5 tokens (às vezes até mais) com pesos diferentes, e o algoritmo que controla a pool garante que a proporção para cada token é sempre respeitada, vendendo algums e comprando outros para mantê-la equilibrada.

A pool que nós queremos usar aqui é a pool que contém Qi, WMATIC, BAL, USDC a MAI. Esta pool irá te recompensar com ambos Qi e BAL, e você já pode ver que será capaz de reacumular ambos na pool. E devido à outra incrivel vantagem das pools na Balancer, você não irá precisar prover os tokens que formam a pool na proporção correta, o algoritmo já faz isso para você. Isso significa que você pode depositar apenas QI na pool e deixar o algoritmo fazer o resto, equilibrando tudo.

![Details of the pool as of September 2021](<../../.gitbook/assets/image (17).png>)

Uma observação é que tokens BAL podem (ou logo poderão) ser usados como garantia na Mai Finance, o que significa que você tem a opçao de guardar o seus tokens BAL na _vault_, ou cofre, BAL da Mai Finance, utilizá-los como garantia, e tomar emprestado MAI. Somado a isso, tomar emprestado MAI, com BAL como garantia, te fará elegível para receber recompensas em Qi que irão alimentar a pool na Balancer.

![Loop fechado usando a Mai Finance e a Balancer](<../../.gitbook/assets/image (18).png>)

O APR das vaults BAL irá responder se vale mais a pena ter a vault no loop, ou se é melhor reacumular seu Qi na pool da Balancer.

## Entendendo o preço do Qi

Ter bastante Qi é uma coisa, porém se o token perde valor ao longo do tempo, será mesmo uma boa estratégia mantê-lo? Nessa seção, nós iremos tentar entender como diferentes fatores impactam o preço do Qi, para que, ao investir os seus Qis, você possa ter uma ideia mais clara de como o preço pode variar, e que impacto você terá no ecosistema Qi.

### Emissão de Qi

Um dos principais fatores que afetarão o preço de Qi é o ritmo no qual eles sãos criados. De fato, o preço é sempre o resultado de oferta e demanda. Se há muita oferta e pouca demanda, o preço irá naturalmente colapsar. Por isso é crucial entender como o Qi é produzido para estimar o seu valor ao longo do tempo.

Há atualmente 2 fontes de emissão de Qi: recompensas de farming e recompensas da vault.

![LP farms na Mai Finance em Setembro de 2021](<../../.gitbook/assets/image (12).png>)

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

![Pool Qi-WMATIC na Adamant](<../../.gitbook/assets/image (15).png>)

![Detalhes do APR de 179.23% APR garantido pela Adamant](<../../.gitbook/assets/image (14).png>)

Você irá perceber que o APR total é maior do que na Mai Finance, somente porque a Adamant aloca recompensas ADDY adicionais aos farmers, ou fazendeiro. A quantidade de Qi é redistribuída é de 98.45% comparada aos 134.42% que você pode obter na Mai Finance.

Dessa recompensa em Qi de 98.45%, metade dela é vendida diretamente para comprar WMATIC e formar LP tokens adicionais, que são então dados aos farmer.

Com 100$ de LP token, assumindo que APR e o preço dos tokens permanecem os mesmo durante o ano todo, e assumindo que não haja reacumulação, você teria apos um ano de farming:&#x20;

* $134.42 de novos Qi na Finance
* $98.45 de novos tokens Qi/WMATIC, ou $49.23 de novos Qi na Adamant

Isto significa que, no processo, $85.20 de Qi são simplesmente vendidos no mercado, que é mais de 60% da emissão total alocada na pool da Adamant.

E a Adamant não é a unica plataforma disponibilzando este tipo de serviço. Outros exemplos são a Beefy Finance e Kogecoin. Dos $4.9M em TVL (Total Value Locked, ou Valor Total Bloqueado) na farm de Qi/WMATIC na Mai Finance, $2.3M estão vindo diretamente da Adamant, $41k da Beefy e $12k da Kogecoin, representado para essas 3 plataformas mais de 50% do valor bloqueado na Mai Finance. Uma estimativa bruta é que mais de 30% da emissão total diario de Qi é despejada por essas plataformas, causando uma grande pressão vendedora no token, diminuindo o seu preço, o que explica parcialmente o porque Qi tem dificuldade em manter um preço elevado.

### Entendendo os pares LP

Quando você obtém rendimentos por meio de farms por providenciar pares LP, o token LP é na verdade usado para prover liquidez aos usarios que estão trocando um token pelo outro. No nosso exemplo de Qi/WETH, quando alguém compra WETH, parte do token pode ser obtido da LP pool e vendido ao usuário que requeriu.

Neste momento, porque um pouco de WETH foi tirado da pool, há uma incompatibilidade no balanço: menos WETH para a mesma quantidade de Qi. O algoritmo encarregado de manter a razão em 1:1 irá então vender um pouco de  Qi dessa pool para comprar de volta mais WETH e restaurar a razão 1:1. O oposto também ocorre quando alguém compra Qi, ou seja, WETH é vendido para comprar mais Qi.

O mesmo fenomeno ocorre quando um dos 2 tokens compondo o par ganha ou perde valor. Como um exemplo, nós iremos assumir que o preço de Qi é de $1 e o preço de ETH é de $1,000, e que nós temos uma pool que contém $100 de Qi e $100 de WETH. Isso significa que a pool contém 100 Qi e 0.1 WETH.

Agora, se o preço de ETH for a $2,000, se a pool manter a mesma quantidade de tokens, nós teriamos $100 de Qi mas $200 de WETH, e nós teriamos perdido o balanço. Dai, o algoritmo no controle da pool irá vender um pouco de ETH e comprar mais Qi. No nosso simples exemplo, $50 de ETH serão vendidos para comprar $50 de Qi, e o estado final será de:

* 150 Qi com um valor de $150$
* 0.075 ETH com um valor de $150

Isto também significa que quando o preço de um dos dois tokens sobre, a pool cria demanda para o outro, também levantando o seu preço. O oposto também é verdade: se um token perde valor, o o outro será vendido para manter uma proporção de 1:1, jogando o preço para baixo. Isso também explica parcialmente a flutuação de preço de Qi quando comparada à flutuação de preço de WEHT e WMATIC (os 2 principais tokens aos quais Qi é pareado).

![Preço de Qi (à esquerda) vs preço de WMATIC (à direita)](<../../.gitbook/assets/image (13).png>)

### A questão da falta de uso

Por ultimo, a falta de uso de Qi, ou a falta de usos conhecidos, pode explicar porque o preço do token está caindo. Pessoas coletando Qi das recompensas da vault e/ou farm na Mai Finance irão simplesmente vendê-lo enquanto possuem valor para realizar seu lucro, sem visão de longo-prazo, o que na verdade é uma estratégia bem sensata. Este guia, na verdade, tenta promover diferentes maneiras de utilizar seus tokens Qi sem vendê-los, mas se o preço não sobe, ou se você não consegue gerar benefícios por outros tokens (conhecido como vazamento de lucro), há pouca vantagem em acumulá-los.

### Como podemos ajudar o preço a subir?

Se nós queremos que o preço de Qi suba (e quem não quer isso?), há algumas opçōes:

* Reduzir a emissão: com novos 86,400 Qi sendo cunhados diariamente, a oferta é muito grande. Se nós cortarmos esta emissão, a oferta pode diminuir, e com menor oferta, o preço deve, em teoria, subir. Entretanto, emissão atual para as farms precisa permanecer a mesma porque elas  são parte de uma atual parceria com a QuickSwap. Incentivos de vault já foram lançados, e são uma maneira incrível de promover a plataforma de empréstimos, levando as pessoas a tomarem emprestado, então cortar essas emissōes é provavelmente outra má ideia.
* Responsabilidade com a farm: Eu não estou dizendo que a Adamant é o principal culpado ou que é um mau produto. De fato, eu incluo essa plataforma na maioria das minhas estratégias e a uso diariamente. Entretanto, eu tento fazer farm em pools que eu tenho menor preocupação em saber que o token será despejado. Se você quer rendimentos de farm na Adamant em uma pool que usa a farm da Mai Finance, tenha em mente que você contribuiu para a depreciação de Qi. Se você não tem problema com isso, não há problema algum.
* Entenda como as coisas funcionam: os preços de todas as criptomoedas são altamente voláteis, e na maioria das vezes, os preços do BTC e ETH determinam os preços de todos os outros tokens. Isso não é feito magicamente. Também, entenda que quando alguém faz dinheiro é porque outra pessoa esta perdendo. Não há dinheiro grátis, e dinheiro mágico da internet não é tão mágico assim.
* Encontre novos usos para os tokens Qi. Este guia irá sempre prover ideias que irão te ajudar a aumentar o volume do seu portfólio. E raramente venda os seus tokens. Loops fechados são os melhores porque a saída de um produto alimenta a entrada do próximo, criando uma bela bolha que apenas crescerá ao longo do tempo.

Também tenha em mente que:

$$
Valor = Quantidade * Preço
$$

Quando o preço diminuí mas a quantidade sobe, seu valor pode aumentar, ou pelo menos não irá diminuir tão rapidamente.

## Aviso legal

Este guia é, na verdade, um resultado de muitas discussōes sobre o preço de Qi no servidor do Discord. Eu entendi que algumas pessoas reclamando sobre a depreciação do preço não entendiam completamente as razōes por trás da constante tendencia de baixa de Qi. Isso causa frustração e delírio, o que é muito negativo para Qi, o produto da Mai Finance, e todo o ecosistema DeFi no geral. Entretanto, não há garantia se quer que o preço irá subir algum dia, então se você quer manter seus Qis e investí-los, por favor, faça a sua própria pesquisa e corra os seus próprios riscos. Planeje a sua estratégia corretamente e cumpra com ela.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um periodo de tempo pode performar mal (ou te fazer perder dinheiro) em outro período. Por favor, se informe, monitore os mercados, mantenha um olho em seus investimentos, e como sempre, faça a sua propria pesquisa.
{% endhint %}
