---
description: >-
  Neste guia, usaremos o conceito de títulos para obter ativos a um preço
  inferior ao preço de mercado e usaremos protocolos de alta recompensa para
  aumentar os ganhos.
---

# Combo do Exodia na Fantom

## Introdução

Uma das coisas mais importantes a ter em mente ao investir em criptomoedas é garantir que sua posição inicial esteja protegida. Se você mantiver esse fundamento em mente, poderá apenas colocar seus ganhos em risco. No entanto, há outra opção se você quiser investir em um token que represente incertezas: comprá-lo com desconto e garantir que as recompensas sejam altas o suficiente para cobrir seu investimento inicial o mais rápido possível.

Há alguns meses, isso se tornou possível com a introdução de títulos e taxas de recompensa muito altas propostas por alguns projetos. Então, hoje, exploramos dois projetos no Fantom que estão usando o conceito de bonding para atingir 2 objetivos muito diferentes.

![](../../.gitbook/assets/exodia-tomb-0.png)

## Exodia

### Apresentação do projeto

[Exodia](https://app.exodia.fi/dashboard) é um pequeno projeto na Fantom que tem um potencial gigantesco. É um Ohm-fork baseado no token EXOD, uma moeda de reserva apoiada por diferentes ativos. Os ativos de rerva iniciais adicionados ao tesouro da Exodia foram DAI e FTM, mas a equipe e a DAO encarregados do protocolo decidiram desenvolver laços com a comunidade Olympus e alocar 33% de suas reservas excedentes para comprar ativos denominados em OHM. Como tal, uma pequena parte da tesouraria é denominada em tokens gOHM.

![Detalhamento do Tesouro da Exodia em janeiro de 2022](../../.gitbook/assets/exodia-tomb-1.png)

### Novo LP Token para Bonding

Para fortalecer laços, a Exodia votou recentemente para aumentar a quantidade de tokens relacionados ao OHM em seu tesouro e em breve aceitará um novo token como parte de seu programa de bonding. O novo token é um token LP (Liquidity Provider) que pode ser criado no BeethovenX. Uma das melhores coisas sobre os tokens BeethovenX é que eles podem ser criados mesmo se você possuir apenas um único ativo da seleção no pool, o que o torna facilmente acessível. O token LP é composto por:

* 20% em wFTM
* 20% em EXOD
* 20% em wsEXOD
* 20% em gOHM
* 20% em MAI

![A LP pool Monolith na BeethovenX em janeiro de 2022](../../.gitbook/assets/exodia-tomb-2.png)

Este é provavelmente o primeiro fork da Ohm usando um token LP de um fork da Balancer para bonding. Isso é interessante porque agora você pode comprar novos títulos usando apenas seus tokens EXOD. As etapas seriam:

* deposite seu token EXOD no pool `The Monolith` da BeethovenX para obter o token LP
* venda seu token LP no aplicativo da Exodia para comprar um novo EXOD com desconto
* aguarde o período de vesting e colete seus tokens EXOD
* repita

Isso reduz drasticamente a pressão de venda dos tokens EXOD, o que beneficia o protocolo. Anteriormente, os flippers de títulos teriam que vender seu EXOD para obter DAI e comprar títulos adicionais, o que é prejudicial por reduzir o preço do token e causar um efeito em cascata ao tesouro e ao projeto.

{% hint style="info" %}
Se você não está familiarizado com os projetos Ohm, recomendo fortemente mais algumas leituras sobre o assunto. Você pode consultar nosso guia sobre Klima (veja a seção Polígono) ou ir diretamente para a [official documentation of Exodia](https://docs.exodia.finance/). Além disso, você pode se juntar à discórdia e se inscrever no esquema de educação..
{% endhint %}

Você também vê que o LP token aceita MAI, a stablecoin que você pode cunhar na Mai Finance. Esta será, na verdade, nossa fonte principal para o LP (veremos a seguir). Depois de comprar seus bonds com um desconto decente, você receberá seus tokens EXOD no final do período de vesting. Você também pode fazer staking com esse token, rendendo um APY (**A**nnual **P**ercentage **Y**ield, ou Rendimento Percentual Anual) de 38.787%, o que equivale a um APR (**A**nnual **P**ercentage **R**ate, ou Taxa Percentual Anual) de 601% e um ganho diário de 1,65%.

Usaremos o sistema de bonding para comprar tokens EXOD com desconto e lucrar com o enorme APY para coletar ganhos das recompensas de rebase.

## Tomb Finance

[Tomb Finance](https://tomb.finance/) é um projeto muito particular, original em muitos aspectos. O token TOMB é uma stablecoin algorítmica atrelada ao token FTM, projetada para ser um meio de troca e para adicionar liquidez adicional ao FTM, o token de gas da rede Fantom.

O ecossistema Tomb Finance propõe mais 2 tokens:

* TSHARE: este é o token de governança para o Tomb Finance. Os detentores de TSHARE têm poder de voto. Os participantes do TSHARE também receberão TOMBs adicionais. A emissão de tokens TOMB adicionais para os detentores de TSHARE segue a mesma mecânica dos forks Ohm, com novos tokens sendo cunhados no final de cada época com um APY muito alto.
* TBOND: este é um token especial que é usado principalmente para manter o peg em 1 FTM. Quando o preço do TOMB cai abaixo de 1 FTM, os usuários podem comprar TBOND ao preço atual dos tokens TOMB. Eles podem fazer isso vendendo tokens TOMB para o protocolo e esses tokens são queimados, o que aumenta o valor do TOMB de volta para 1 FTM. Comprar TBOND com desconto e poder resgatar tokens TOMB deu o nome ao token TBOND. Quando o token TOMB está acima do peg, as pessoas podem trocar seu TBOND por TOMB. Novos TOMB são cunhados, reduzindo o valor do token. Em outras palavras, este é um token de arbitragem!

![Valor de TOMB, TBOND e TSHARE em janeiro de 2022](../../.gitbook/assets/exodia-tomb-3.png)

A Tomb Finance também oferece 2 LP pools que lhe darão tokens TSHARE. Isso é particularmente importante, pois a Tomb Finance deve ter profundidade de liquidez. No entanto, para atingir o objetivo de ter o TOMB como uma solução alternativa ao FTM, é importante que o protocolo tenha usuários utilizando o TOMB, detendo assim a liquidez. Quando você faz farming nas pools TOMB-FTM e TSHARE-FTM, você é recompensado com tokens TSHARE que permitirão que você ganhe mais tokens TOMB, o que é um belo loop fechado em um único aplicativo.

## Peças adicionais para fechar loops

Agora que apresentamos as 2 grandes peças da nossa estratégia, vamos ver rapidamente as outras peças do quebra-cabeça.

### Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) é um otimizador de rendimento que aceitará tokens LP de determinadas DEX (Decentralized Exchanges), tokens de recompensa de farm e deixará seus algoritmos venderem a recompensa por LP adicional. Dessa forma, você pode obter uma posição de investimento crescente que comporá apenas os tokens do LP e capturará o valor do token de recompensa no momento em que o token for colhido.

Para nossa estratégia, usaremos o token LP TOMB-FTM. Os motivos são vários:

* TOMB sendo atrelado ao token FTM, não há IL (**I**mpermanent **L**oss, ou Perda Impermanente) neste par, então a única variação será vinculada à variação de preço do FTM
* TOMB-FTM é recompensado com TSHARE, então vender TSHARE não afetará os 2 tokens do par
* TOMB-FTM tem um APY bastante alto que para um token LP sem IL
* usar o token LP na Beefy permitirá a você obter o token de comprovante `mooTombTOMB-FTM`

![Pares LP deTomb na Beefy Finance em janeiro de 2022](../../.gitbook/assets/exodia-tomb-4.png)

{% hint style="info" %}
Para os propósitos deste guia, estamos usando o token TOMB-FTM porque apresenta menos risco devido à ausência de impermanent loss no par. No entanto, você pode usar totalmente o par TSHARE-FTM para obter recompensas mais altas. Certifique-se de entender os riscos e faça a sua própria pesquisa.
{% endhint %}

### Plataforma de empréstimo Market.XYZ

[Market.XYZ](https://fantom.market.xyz/pool/3) é um protocolo de empréstimo no qual você poderá depositar alguns ativos específicos e, por eles, tomar emprestado outros ativos. Quando você empresta seu ativo, pode receber alguns incentivos de empréstimo pagos no ativo emprestado. Ao fazer um empréstimo, você terá que pagar alguns juros no momento do reembolso no mesmo ativo que tomou emprestado.

Market.XYZ iniciou uma parceria com a Mai Finance em 2021 para permitir que classes adicionais de ativos sejam usadas como garantia para tomar emprestado a stablecoin MAI. Esses ativos são considerados mais arriscados do que os atualmente aceitos diretamente no Mai Finance, ou estão apenas aguardando um Oráculo ChainLink oficial e não são aceitos diretamente no aplicativo principal. Isso traz benefícios adicionais: o protocolo QiDAO está ganhando taxas do MAI emprestado, os mutuários estão recebendo MAI a baixas taxas de juros (Mai Finance está adicionando mais MAI do tesouro regularmente com base na demanda) e é um caso de uso muito interessante para a stablecoin, aumentando seu uso. Por outro lado, os mercados de empréstimos são uma ótima maneira de iniciar relações fortes com diferentes parceiros enquanto esperam que seus ativos sejam aceitos diretamente na Mai Finance.

![TOMB Beefy Locker na Market XYZ em janeiro de 2022](../../.gitbook/assets/exodia-tomb-5.png)

O mercado de empréstimos que nos interessa para esta estratégia é o TOMB Beefy Locker. Depois de depositarmos nossos tokens TOMB-FTM na Beefy, recebemos o token comprovante mooTombTOMB-FTM que é uma "prova de propriedade" para o token que está acumulando recompensas na Beefy. Este token comprovante pode ser usado como garantia na Market.XYZ para tomar emprestado MAI adicional.

{% hint style="danger" %}
Market.XYZ só permite empréstimos com um valor mínimo de 0.05 ETH (\~$170,00 no momento da escrita). Certifique-se de depositar garantia suficientes se quiser tomar emprestado dos diferentes lockers.
{% endhint %}

Na captura de tela acima, você pode ver que podemos:

* depositar o token mooTombTOMB-FTM como garantia e obter um APY de 355,4% sobre ele, fornecido pela Beefy
* tomar emprestado MAI com uma taxa de juros de 15,02% (APR)

É fácil ver que os ganhos que obtemos com o farming LP superam de longe os juros de empréstimos, o que torna essa estratégia viável. No entanto, certifique-se de monitorar adequadamente o preço do FTM e TOMB para evitar a liquidação e certifique-se de tomar emprestado a uma CDR (Colateral to Debt Ratio, ou Proporção de Garantia para Dívida) muito alta, o que lhe dará tempo suficiente para reembolsar seu empréstimo em caso de uma grande queda de preço.

{% hint style="info" %}
Se você não está interessado nessa estratégia, mas é usuário do Mai Finance, o Market XYZ é um aplicativo incrível para emprestar seu MAI. Você será pago em MAI adicional que será reacumulado em sua posição.
{% endhint %}

## Estratégia de farming

Para completar nosso loop de investimento, começaremos com a compra de bonds EXOD usando MAI. As recompensas de rebase EXOD serão usadas para comprar tokens LP TOMB-FTM. Os tokens serão usados na Beefy para acumular as recompensas TSHARE. Além disso, o token LP comprovante será usado como garantia na Market.XYZ para tomar emprestado mais MAI, o que nos envia de volta à nossa etapa inicial.

Vamos simular com algumas suposições:

* todas as taxas e preços de recompensa permanecem os mesmos ao longo de um ano&#x20;
* O APY da Exodia é de 38.787%&#x20;
* O APY de TOMB-FTM pela Beefy é de 318,51%&#x20;
* As taxas de juros do empréstimo da Market.XYZ geram um APR de 15,02% (os juros não são compostos, então usaremos APR quando nos referimos a taxas de empréstimo)

Além disso, assumiremos que você está colhendo seus bonds e tokens EXOD diariamente e realizando staking de 50% para se beneficiar dos rebases o mais rápido possível. Os títulos serão comprados com um desconto médio de 0% para simplificar, mas esperamos obtê-los com um desconto melhor, e assumiremos que podemos comprar novos títulos a cada 5 dias.

![](../../.gitbook/assets/exodia-tomb-6.png)

### 1º dia

Precisamos primeiro descobrir qual ponto de entrada apresenta o menor risco. O LP TOMB-FTM parece se encaixar exatamente nisso (veja os motivos detalhados na descrição do par de LPs), portanto, iniciaremos o loop neste ponto com US$ 1.000 em tokens TOMB-FTM. Depois que o token LP for criado no SpookySwap, você poderá depositá-lo na Beefy Finance e começar a pedir empréstimos imediatamente. \
\
Para esta estratégia, tentaremos manter uma CDR de 300%. Isso significa que poderemos tomar emprestado $333 em MAI do locker com uma taxa de juros de 15,02%. O MAI emprestado será usado no BeethovenX para obter um token LP wFTM-EXOD-gOHM-wsEXOD-MAI. Por fim, compraremos um bond EXOD com o LP. Observe que toda a configuração pode ser no primeiro dia. No final do dia (assumindo 3 rebases) obteremos:

| Posição             | Valor ($) |
| ------------------- | --------- |
| TOMB-FTM            | 1,000.000 |
| Empréstimo de MAI   | 333.333   |
| EXOD                | 66.667    |
| TOMB-FTM adicionais | 3.930     |
| EXOD adicionais     | 1.098     |

### 2º, 3º, 4º e 5º dia

Nos próximos dias, é inútil fazer colher e acumular as recompensas de EXOD, já que o bond que compramos no primeiro dia ainda está passando por vesting. Assim, podemos deixar o token LP TOMB-FTM aumentar de preço sem pedir mais empréstimos e focar nas recompensas EXOD. 50% da recompensa será acumulada em mais EXOD, e os outros 50% serão adicionados ao LP TOMB-FTM. No final do quinto dia, quando o bond já tiver passado pelo vesting, teríamos:

| Posição             | Valor ($) |
| ------------------- | --------- |
| TOMB-FTM            | 1,021.369 |
| Empréstimo de MAI   | 333.333   |
| EXOD                | 338.869   |
| TOMB-FTM adicionais | 4.014     |
| EXOD adicionais     | 5.582     |

{% hint style="info" %}
O TOMB-FTM e EXOD adicionais são apenas o que é produzido no dia 5 e acumulado no início do dia 6.
{% endhint %}

### 6º dia

O TOMB-FTM acumulado no quinto dia, bem como os 50% de EXOD colhidos, dão a você um total de $1.028,173 em TOMB-FTM no início do sexto dia. Isso significa que seu possível empréstimo é de $342.724, permitindo que você tome emprestado mais $9.391 em MAI que serão usados para adquirir um novo bond na Exodia. A partir deste momento, o sistema está montado e você pode simplesmente gerenciar seu investimento por meio de uma rotina diária leve.

### Rotina diária

A rotina é dividida em 2 partes: a rotina diária real que você terá que operar diariamente e uma que você terá que operar a cada 5 dias. \
\
Diariamente, você terá que:

* Reivindicar tokens EXOD do vesting da Exodia
* Fazer staking com 50% dos tokens EXOD na Exodia
* Vender 25% dos tokens EXOD para FTM na SpookySwap
* Vender 25% dos tokens EXOD para TOMB na SpookySwap
* Criar um LP token TOMB-FTM na SpookySwap
* Depositar o LP token TOMB-FTM na Beefy Finance
* Depositar o token comprovante mooTombTOMB-FTM na Market.xyz

A cada 5 dias, você terá que:

* Tomar emprestado mais MAI da Market.xyz para manter uma CDR de 300%
* Depositar o MAI emprestado na BeethovenX na pool The Monolith
* Trocar seu LP token Beethoven por bond de EXOD na Exodia

### Resultados brutos mensais

Aqui estão os resultados brutos mês após mês:

| Dia | TOMB-FTM   | EXOD       | Dívida em MAI |
| --- | ---------- | ---------- | ------------- |
| 30  | 1,222.088  | 488.438    | 407.363       |
| 60  | 1,531.135  | 735.586    | 510.378       |
| 90  | 1,956.250  | 1,093.089  | 652.083       |
| 120 | 2,546.404  | 1,609.179  | 848.801       |
| 150 | 3,371.740  | 2,353.088  | 1,123.913     |
| 180 | 4,532.773  | 3,424.178  | 1,510.924     |
| 210 | 6,173.591  | 4,965.049  | 2,057.864     |
| 240 | 8,500.790  | 7,180.350  | 2,833.597     |
| 270 | 11,810.653 | 10,363.762 | 3,936.884     |
| 300 | 16,528.139 | 14,936.728 | 5,509.380     |
| 330 | 23,262.834 | 21,504.023 | 7,754.278     |
| 360 | 32,889.239 | 30,933.491 | 10,963.080    |

### 365º dia

Depois de um ano completo cultivando esse sistema, e assumindo que tudo permanece constante desde o primeiro dia (preços, taxas, etc), você teria:&#x20;

* $34,855.954 em LP tokens TOMB-FTM na Beefy
* $32,863.908 em tokens EXOD
* uma dívida de $11.618,651 em MAI na Market.xyz, com alguns juros adicionais a pagar (correspondendo a uma dívida total de $13.363,772)

É muito importante notar que a sua CDR permanece próxima ou acima de 300% em qualquer momento durante a simulação, então é totalmente possível você vender uma parte do seu TOMB-FTM ou EXOD para pagá-lo e diminuir os juros. Também é possível ajustar a parte do EXOD que você vende diariamente para simplesmente pagar seu empréstimo inicial e comprar novos bonds EXOD vendendo TOMB-FTM. As variações são infinitas, então sinta-se à vontade para ajustar de acordo com o que você mais gosta.

No final, com um investimento inicial de $1.000, você terminaria com um ganho de $67.719,862 e uma dívida de $13.363,772, o que corresponde a um APY total de 5.335,56%.

## Aviso legal

Este é um guia experimental que destaca como você pode aumentar seus ganhos adicionando forks-Ohm em seus loops de investimento. A simulação foi feita em um momento em que a Exodia tinha um APY muito alto em tokens EXOD em staking. O mesmo pode ser dito sobre o TOMB-FTM. Esses índices muito altos geralmente variam muito, então você pode esperar um resultado bem inferior ao longo de um ano completo. De fato, a maioria dos forks-Ohm não são projetados para sustentar esses altos rendimentos por mais de alguns meses e geralmente reduzem drasticamente sua emissão para continuar funcionando.

Mantenha-se informado sobre os projetos que está usando, não hesite em fazer perguntas e, como sempre, faça suas próprias pesquisas.

{% hint style="info" %}
Este guia definitivamente não é um conselho financeiro, foi feito com um objetivo educacional em mente. Você precisa ficar atento às variações de preços, oferta e demanda, datas de término dos programas de recompensas, perdas impermanentes, etc. O objetivo não era propor receitas que possam ser seguidas às cegas, então faça sua lição de casa e sua própria simulação, e apenas investir o que você está pronto para perder.
{% endhint %}
