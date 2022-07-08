---
description: >-
  Este guia apresentará uma visão geral das diferentes redes em que a stablecoin
  MAI pode ser usada e como você pode enviar a moeda nativa a outras redes.
---

# Metaverso e MAI

![](../.gitbook/assets/MAI.png)

## Introdução

MAI, às vezes chamado de miMATIC, é a primeira stablecoin nativa da rede Polygon. Está atrelada a US$ 1,00 e seu valor pode flutuar entre US$ 0,99 e US$ 1,01. Você pode obter mais detalhes sobre como o peg é mantido na [documentação oficial.](https://docs.mai.finance/stablecoin-economics) Mas não é porque o MAI é nativo na Polygon que ele só é encontrado nessa rede. De fato, da mesma forma que você pode encontrar DAI em diferentes redes (DAI é na verdade outra stablecoin vinda da Ethereum Mainnet), a MAI está se expandindo lenta mas seguramente para outras redes também. Este artigo irá destacar as diferentes redes onde você pode encontrá-lo e como você pode transferir seu MAI de uma rede para outra..

## Polygon

### Obtendo MAI na Polygon

Conforme explicado, o MAI é nativo da Polygon, e esse é o único lugar (em setembro de 2021) onde você poderá cunhar MAI. Isso é feito:

* tomando emprestado MAI com garantias que você depositou anteriormente em um vault na Mai Finance
* trocando USDC por MAI na [Mai Finance](https://app.mai.finance/anchor)
* vendendo outro ativo e comprando MAI em qualquer DEX (Decentralized EXchange) na Polygon, sendo as mais eficientes a [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) or [1Inch](https://app.1inch.io/#/137/classic/swap).

### Usando MAI na Polygon

A stablecoin MAI está sendo usada, a cada dia, em mais projetos na Polygon, especialmente agora que é usada como outras stablecoins em grandes projetos como a QuickSwap. Em setembro de 2021, existem 3 farms de stablecoins na QuickSwap com um total de US$ 18.327.604:

* MAI-DAI com $6,553,255
* MAI-USDT com $6,316,026
* MAI-USDC com $5,458,323

Pools adicionais podem ser encontrados em outros projetos / farms de rendimento / otimizadores de rendimento. Você pode ler mais sobre o que fazer com seu MAI neste [artigo dedicado](../tutoriais/polygon/what-to-do-with-mai-on-polygon.md).

## Solana

### Obtendo MAI na Solana

Solana é uma plataforma blockchain para aplicativos descentralizados. O objetivo da rede é propor transações baixas (menos de US$ 0,01) e rápidas (menos de 400ms). A ideia por trás disso é criar uma alternativa à Ethereum Mainnet e suas side chains. No entanto, não é porque a Solana é uma concorrente da rede Ethereum que ela não suportaria os mesmos ativos. De fato, a Solana agora suporta a stablecoin MAI que pode ser enviada a partir da Polygon (onde pode ser cunhada).

Para enviar seus tokens MAI para a Solana, você pode usar a [AllBridge](https://allbridge.io/), uma plataforma de ponte que permite transferir tokens de uma rede para outra. AllBridge suporta as seguintes redes::

* Ethereum Mainnet
* Polygon
* Solana
* Huobi
* Binance Smart Chain

A interface é realmente intuitiva no sentido de que basta selecionar as duas redes e o ativo que deseja transferir entre as 2.

![Enviando MAI da Polygon à Solana](../.gitbook/assets/screen-shot-2021-09-13-at-1.52.23-pm.png)

O próximo passo é indicar o endereço da sua carteira Solana e o valor que deseja transferir. Esteja ciente de que a MetaMask não suporta carteiras Solana (ainda?), e você terá que criar uma carteira separada para essa rede. Pode ser uma carteira da web como a MetaMask ou uma carteira de aplicativo. Por favor, leia as [recomendaçōes oficiais da Solana ](https://docs.solana.com/wallet-guide)antes de escolher uma.

{% hint style="info" %}
Esteja ciente de que a Solana não oferece nenhuma faucet onde você obterá seu primeiro SOL (token nativo usado para pagar transações). Você precisa comprar um pouco de SOL primeiro e tê-lo em sua carteira para poder transferir o MAI para sua carteira.
{% endhint %}

### Usando MAI na Solana

Da mesma forma que você pode usar o MAI na Polygon para fornecer liquidez e obter rendimentos em farming, você pode fazer o mesmo no Solana. O principal local onde você pode usar o MAI é a [Saber](https://app.saber.so/), na pool de MAI/USDC.

![Estado do pool MAI/USDC na Saber, Setembro de 2021](../.gitbook/assets/screen-shot-2021-09-13-at-2.11.10-pm.png)

Uma das coisas boas da pool MAI/USDC na Saber é que, diferentemente das pools LP (**L**iquidity **P**roviding, ou Provedor de Liquidez) na QuickSwap, você não precisa fornecer pares LP com uma proporção de 1:1. Você pode simplesmente depositar um único ativo (MAI ou USDC) ou uma proporção (des)balanceada de ambas stablecoins.

![MAI e USDC ficam desequilibrados na pool da Saber](../.gitbook/assets/screen-shot-2021-09-13-at-2.13.51-pm.png)

Isso significa que você pode fazer depósitos com apenas MAI da Mai Finance sem precisar trocar nada por USDC. É particularmente conveniente e evita ser afetado por pequenas diferenças de preço entre as 2 stablecoins. Observe que você receberá recompensas pagas no token de farm nativo, da mesma forma que receberia QUICK realizando farming na QuickSwap (na Polygon), por exemplo. Você pode então vender seus tokens SABER para aumentar sua posição de MAI/USDC.

{% hint style="info" %}
No Solana, você também pode usar o [Sunny](https://app.sunny.ag/), um agregador que comporá automaticamente as recompensas da Saber. Observe que o agregador Sunny não é validado pela equipe Mai Finance. AllBridge e Saber são parceiros oficiais da Mai Finance, mas os resultados não são garantidos. Por favor, como de costume, faça suas próprias pesquisas.
{% endhint %}

## Avalanche

### Obtendo MAI na Avax

Avalanche é uma rede blockchain, projetada para fornecer uma plataforma de código aberto e um protocolo de camada 1 para lançar aplicativos DeFi e soluções blockchain corporativas. É outra solução alternativa a Ethereum Mainnet que também suporta os mesmos ativos que a Ethereum Mainnet, Polygon e Solana. Como tal, agora você pode enviar seu MAI da Polygon (o único lugar, em setembro de 2021, onde você pode cunhar MAI) para a Avax usando [Relay Chain](https://app.relaychain.com/#/transfer).

Quanto ao AllBridge, a interface é bastante simples. Você simplesmente seleciona a rede da qual o ativo será enviado, seu destino e o ativo a ser transferido.

![Bridging MAI from Polygon to Avalanche](../.gitbook/assets/screen-shot-2021-09-13-at-2.52.31-pm.png)

A Metamask **oferece** [carteiras para Avax](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche), ou seja, você não precisará de uma nova, diferentemente da Solana.

### Usando MAI na Avax

Da mesma forma que você pode usar MAI para farming na Polygon, você pode usar MAI na Avalanche. O principal local para isso são as [farms da Trader Joe](https://www.traderjoexyz.com/#/farm) onde você encontrará uma pool MAI/USDC.

![Estado do pool MAI/USDC na Trader Joe, Setembro de 2021](../.gitbook/assets/screen-shot-2021-09-13-at-3.07.19-pm.png)

As fazendas na Avalanche funcionam muito de perto com o que você pode encontrar em Polygon. Portanto, você pode usar o aplicativo do Trader Joe da mesma maneira que usaria o QuickSwap. Primeiro você precisa criar um par de LPs no site usando a mesma proporção de MAI e USDC e, em seguida, depositar o par LP na farm. Da mesma forma que você seria pago em QUICK ao realizar farming na QuickSwap, você será recompensado em tokens JOE na Trader Joe. Você pode usar esses tokens em outros pools ou vendê-los para aumentar seu par MAI/USDC.

## Fantom

### Obtendo MAI na Fantom

A Fantom é uma blockchain com suporte a contratos inteligentes cujo objetivo é resolver os problemas de escalabilidade de outras redes, nomeadamente a blockchain Ethereum. Os desenvolvedores podem criar seus DApps (**D**ecentralized **App**lications, ou Aplicativos Descentralizados) nessa rede e usar os mesmos ativos de outra rede. Como tal, você já pode fazer a ponte MAI da Polygon para a Fantom usando a ponte da [AnySwap](https://anyswap.exchange/#/bridge).

Se a AnySwap é outra solução de ponte, sua interface é muito semelhante à da AllBridge e Relay Chain. Quando estiver na Polygon, você terá que conectar sua carteira MetaMask primeiro, depois selecionar o ativo que deseja conectar (MAI) e a rede de destino (Fantom).

![Enviando MAI da Polygon a Fantom](../.gitbook/assets/image.png)

A Metamask **oferece** [carteiras para Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask), então é muito fácil configurá-la para receber seu MAI na Fantom e começar a usá-lo imediatamente.

### Usando MAI na Fantom

Atualmente, a equipe da Mai Finance não possui nenhuma parceria com nenhuma farm na Fantom. Assim que a equipe estiver ciente de projetos que estão usando MAI, esta documentação será atualizada. Fique ligado.

## Aviso legal

Os detalhes apresentados neste guia são puramente educacionais e não foram testados diretamente pela equipe que mantém este guia. Alguns usuários no servidor do Discord já tentaram fazer a ponte de seus ativos para Solana e/ou Avalanche, então você pode se juntar à comunidade do Discord para fazer suas perguntas. Por favor, não se esqueça de fazer suas próprias pesquisas, redes diferentes terão taxas de transação e tempos de execução diferentes, programas de recompensa diferentes, taxas de ponte, etc. Se você enviar seu MAI para outras redes, certifique-se de que você pode trazê-lo de volta caso precise dele na Polygon.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
