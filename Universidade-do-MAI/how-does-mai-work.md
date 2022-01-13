---
description: >-
  Entender bem como o MAI funciona é crucial para qualquer investidor que
  realmente queira entender a Mai Finance, e neste artigo você entenderá isso.
---

# Como a MAI funciona?

## O que é uma stablecoin?

Antes de falarmos sobre MAI, temos que entender o que é uma stablecoin. Uma stablecoin é um tipo de criptomoeda projetada para manter um preço de mercado estável. A maioria das stablecoins são atreladas (uma moeda em que o preço é projetado para permanecer o mesmo que um ativo designado) ao dólar americano, mas você pode encontrar= outras stablecoins atreladas a outras commodities, como ouro (como EGold) ou prata (SilverCoin).

No entanto, existem 2 categorias principais em que todas as stablecoins podem se encaixar, **com** ou **sem garantia**. As stablecoins **com garantia** são aquelas que detêm os ativos contra os quais sua moeda está atrelada, enquanto as **sem garantia** fazem uso de algoritmos para controlar a oferta de tokens a fim de manter o preço fixado em um nível predeterminado.

## O desastre da IRON Finance

Se você já trabalha com criptomoedas há algum tempo, pode se lembrar do desastre do token **TITAN** e **IRON**, mas para aqueles que não conhecem, aqui está uma rápida recapitulação. O IRON Finance era um projeto que tinha 2 tokens, a stablecoin IRON e o token TITAN, no entanto, a stablecoin IRON **não era totalmente lastreada** em stablecoins, a proporção para a moeda IRON era de **75% em USDC** e **25% em TITAN**. Basicamente, uma receita para o desastre.

Em junho de 2021, o token TITAN atingiu um ATH de US$ 65, o que fez com que vários investidores, que investiram pesadamente na moeda, decidissem vendê-la. Isso causou um problema porque o preço do TITAN é baseado na oferta e na demanda. Assim, à medida que a oferta disponível de TITAN aumentou, o preço começou a diminuir. Isso causou uma enorme pressão de venda, de modo que o preço do TITAN caiu ainda mais rápido, então, quando o TITAN começou a cair rapidamente, o IRON perdeu seu apoio e, eventualmente, seu pareamento.

![Gráfico de preço do token TITAN](../.gitbook/assets/iron.jpg)

![Gráfico de preço da stablecoin IRON](../.gitbook/assets/titan.jpg)

As pessoas começaram a comprar a moeda estável IRON para vendê-la por USDC e ganhar dinheiro rápido, em uma enorme oportunidade de arbitragem (lucrando com as variações de preço dos tokens). Resumindo, foi calculado que quase US$1,75 bilhão foram perdidos neste incidente. Portanto, existe uma diferença entre a stablecoin IRON e a MAI?

## O que é MAI?

MAI é uma stablecoin apoiada por tokens de garantia bloqueados, a cunhagem do MAI pode ser feita através do depósito de **garantias aprovadas** em cofres ou usando o **Anchor**.

Ao cunhar MAI, depositando garantias aprovadas, o **CDR** (Collateral to Debt Ratio, ou Taxa de Garantia para Dívida) precisa estar entre 150%, isso significa que, se você depositar $100 em garantia, o MAI recém-cunhado pode valer no máximo $66,6667. Chegaremos à razão por trás disso mais adiante neste artigo.

Outra forma de cunhar MAI é através da [Anchor](https://app.mai.finance/anchor), isso significa que, quando você troca uma stablecoin (a partir de setembro de 2021, você pode cunhar MAI usando **DAI**, **USDC** e **USDT**) por MAI, o novo MAI é cunhado pelo tesouro e a stablecoin depositada é mantida no tesouro como garantia. Enquanto isso, quando você troca suas stablecoins, a MAI que você fornece será queimada.

![Stablecoins que podem ser trocadas para cunhar MAI](<../.gitbook/assets/image (9).png>)

Como você pode ver na imagem abaixo, o preço da stablecoin MAI está quase sempre próximo a $1, isso porque, como a [documentação oficial](https://docs.mai.finance/stablecoin-economics) diz, a stablecoin MAI permite que os usuários se envolvam em arbitragem sem risco por meio da Anchor quando o preço do MAI cair abaixo de US$ 0,99 ou subir acima de US$ 1,01.

![Gráfico de preço do token MAI nos ultimos 90 dias](<../.gitbook/assets/image (7) (1) (1).png>)

## Porque está sempre proximo a $1?

O pareamento em $1 é mantido por 2 mecanismos, pela Anchor ou depositando garantias nos vaults, nesta seção do artigo, você entenderá o porque.

### Anchor

A Anchor permite aos seus usuários cunharem MAI com stablecoins e resgatarem stablecoins moedas de MAI. Além disso, como você pode ver na imagem abaixo, há uma taxa de 1% ao trocar suas stablecoins por MAI ou vice-versa. Existem dois motivos principais para essa taxa:

* A taxa de cunhagem de 1% para criar MAI estabelece um teto de preço de US$ 1,01
* A taxa de 1% para resgatar moedas estáveis do MAI estabelece um preço mínimo de US$ 0,99

![](<../.gitbook/assets/image (8).png>)

Ter um teto e um piso de preço ajuda o MAI a não divergir muito em seu pareamento, no entanto, como você viu na imagem do gráfico do MAI, você pode participar de oportunidades de arbitragem de baixo risco (o que significa que você pode vender suas stablecoins quando o MAI estiver abaixo de $1 ou vender o MAI acima de $1 para ganhar algum dinheiro rápido).

Sobre o que causa a flutuação do preço do MAI, pode haver duas razões principais para isso:

* Se o mercado estiver em **tendência de baixa**: as pessoas venderão seus ativos voláteis e comprarão stablecoins para evitar a perda de valor de ativos voláteis. Isso significa que as pessoas querem comprar MAI, aumentando seu preço.
* Se o mercado estiver em **tendência de alta**: as pessoas compram ativos mais voláteis quando o preço está baixo, usando suas stablecoins. Isso significa que as pessoas vendem seu MAI, reduzindo seu preço.

### Depositando garantias em vaults

Para cunhar MAI usando os vaults da Mai Finance, você precisa depositar alguma garantia lá e ter um **CDR** acima de um determinado limite, neste caso é 150% (no entanto, esse percentual pode mudar no futuro se a comunidade assim o decidir). Isso significa que os cofres serão sempre supercolateralizados (em 150%) para garantir que sempre haja garantia para lastrear as moedas estáveis cunhadas. Lembre-se de que, se um cofre tiver menos de 150% de CDR, ele poderá ser parcialmente liquidado pela comunidade, de modo que alguém poderá perder parte de sua garantia se um liquidante pagar parte de sua dívida.

À medida que o valor da garantia aumenta, mais stablecoins podem ser emitidas, pois um aumento no preço da garantia aumentará sua relação garantia/dívida. Por outro lado, à medida que o valor da garantia cai, menos stablecoins podem ser emitidas, isso é feito para evitar que o CDR caia abaixo da marca de 150%.

## Palavra final

Como você viu ao longo deste artigo, a stablecoin MAI é um tipo de stablecoin supercolateralizada, o que significa que sempre haverá garantia suficiente para apoiar o preço do token MAI. Isso deve dar alívio suficiente para os investidores que hesitam em investir em projetos que cunham stablecoins. Além disso, lembre-se de que, à medida que o MAI está se expandindo para outras blockchains, haverá mais MAI no mercado, resultando em menos volatilidade no preço do MAI.

Recentemente, os incentivos de vaults foram introduzidos na Mai Finance, se você quiser entender o que é isso, fique atento porque haverá um artigo sobre esse tema. Isso ajudará ainda mais na estabilidade do preço do MAI.

## Aviso legal

Você pode encontrar o artigo original da equipe Mai Finance sobre MAI [aqui](https://docs.mai.finance/stablecoin-economics).

Este guia definitivamente não é um conselho financeiro, e foi feito com um objetivo educacional em mente.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
