---
description: >-
  Neste guia vamos te explicar tudo o que precisas de saber para começares a
  utilizar a rede Avalanche.
---

# Como começar na rede Avalanche

## O que é a rede Avalanche?

A rede Avalanche é uma blockchain "layer-one" que funciona como uma plataforma para aplicações descentralizadas e redes de blockchains personalizadas. A rede Avalanche consiste em 3 redes individuais: rede-X, rede-C e rede-P. Cada rede serve um propósito distinto, o que é radicalmente diferente de outras blockchains, em que todos os nodos validam todas as transações. As várias redes da rede Avalanche utilizam diferentes mecanismos de consenso baseado na sua utilidade.

A rede Avalanche é 100% EVM compativel com as ferramentas existentes na rede Ethereum e a rede-C oferece as mesmas funcionalidades que a rede Ethereum mas com maior rendimento, finalização abaixo de 1 segundo e transações com baixo custo. O token utilizado para gás é o token AVAX.

## Aceder à rede Avalanche

Antes de utilizar a rede Avalanche precisas de criar um endereço para uma carteira. Existem diferentes carteiras disponíveis, tanto de software (Metamask ou a carteira nativa [Avalanche Wallet](https://wallet.avax.network)) ou hardware ( [Trezor](https://trezor.io/coins/) ou [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true).)

Para o propósito deste tutorial, vamos usar a carteira Metamask. Se ainda não tens uma carteira instalada, podes encontrar as instruções no guia [Como começar a tua jornada na rede Polygon.](../tutoriais-para-polygon/how-to-get-started-on-polygon.md)

### Adicionar a rede Avalanche na carteira Metamask

Para conseguires aceder à rede Avalanche, precisas de a adicionar à carteira Metamask. Para fazer isso, tens que clicar no menu suspenso _"Network" _(irá aparecer como Rede Ethereum se for a primeira vez que adicionas uma rede) e de seguida selecionar _"custom RPC"_. Podes depois adicionar os seguintes parâmetros:

* **Network Name**: Avalanche Network
* **New RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Symbol**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Guarda as mudanças e a carteira Metamask mudará automaticamente para a rede Avalanche.

![Successo! Tens acesso à rede Avalanche!](../.gitbook/assets/avax_MM.png)

## Transferindo fundos para a rede Avalanche

### Torneiras (Faucets)

De momento não existem torneiras disponiveis na rede Avalanche. Se precisas de tokens AVAX para pagar as transações, tens que enviar AVAX diretamente da tua carteira de uma CEX (plataforma centralizda de criptomoedas) ou transferir tokens através de pontes.

### Pontes (Bridges)

* [Ponte oficial Avalanche](https://bridge.avax.network):  A rede Avalanche fornece uma ponte para transferir os teus tokens da rede Ethereum. As taxas de transação são pagas com o token a ser transferido, podendo ser elevadas tendo em conta que estás a transferir da rede Ethereum.
* [Anyswap](https://anyswap.exchange/#/bridge): Ponte que permite a transferência de tokens para várias redes.  Existe um número minimo de tokens a ser transferidos que varia consoante o token, mas o custo de transação é geralmente baixo.
* [Celer Bridge](https://cbridge.celer.network/#/transfer): Ponte que oferece transferência de tokens entre várias redes. A taxa de transação é de 3% para a rede Avalanche.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer): Ponte que oferece uma interface intuitiva com baixos custos de transação. Adicionalmente, esta ponte é a solução oficialmente suportada para transferir tokens MAI para a rede avalanche. 
* [Elknet](https://app.elk.finance/#/elknet): Serviço de transferência oferecido pela plataforma ElK Finance, uma plataforma descentralizada disponivel em várias redes como Avalanche, Binance, Fantom, Polygon e xDai. O que diferencia esta plataforma das outras pontes é que não precisas de AVAX para fazer a transferência, existindo no entanto pormenores  técnicos que vamos descrever a seguir:
  * De forma a transferires os teus tokens através da ponte Elknet, primeiro tens que converter os  teus tokens para o token **Elk**, o token nativo da plataforma Elk Finance.
  * Podes depois utilizar a ponte para transferior os teus tokens Elk para outras redes como a  rede Avalanche. Se clicares na caixa "Swap $ELK 1 for gas" uma porção da tua transferência é convertida em AVAX para pagar os custos da transação na rede Avalanche.
  * Após a transferência estar concluída (geralmente leva menos de 10 minutos) podes trocar a tua carteira para rede Avalanche e poderás ver os teus tokens ELK e tokens AVAX prontos a serem utilizados. Podes agora trocar os tokens ELK para os tokens da tua escolha.
  * O mesmo pode ser feito no sentido inverso em qualquer rede suportada.

![Interface Elknet](../.gitbook/assets/AVAX_elkswap.png)

## DeFI na rede Avalanche

A rede Avalanche viu um grande crescimento nos últimos meses o que resultou no desenvolvimento de vários projetos nativos e na migração de projectos DeFi estabelecidos noutros cadeias, como o protolo Curve e Aave.

* [Aave](https://app.aave.com/dashboard) lançou recentemente na rede Avalanche tendo já acumulado 4 biliões de doláres em TVL. Os tokens que podem ser utilizados como colateral são AVAX, Aave, Dai, Tether, USDC, WBTC, and WETH. Tokens camAVAX são aceitados como colateral nas vaults da plataforma Mai Finance.
* [Beefy Finance](https://app.beefy.finance/#/avax) é conhecido pela maior parte dos utilizadores DeFi e está disponível em várias cadeias como Binance, Fantom, Harmony, Polygon e muitas mais. Esta app é conhecida como um "autocompounder" que fornece valores de APY elevados tanto para "farms" de token único ou duplo. De momento podes utilizar a plataforma Beefy para fazer "autocompounding" dos tokens [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) e [MAI/USDC.e ](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e)encontradas na plataforma Trader Joe.
* [Benqi](https://app.benqi.fi/markets) é um protocolo semelhante à plataforma Aave e foi o primeiro a depor na rede. Os tokens aceites como colateral são Avalanche, Dai, Link, Tether, USDC, WBTC, e WETH.

![Interface BenQI](../.gitbook/assets/AVAX_benqi.png)

* [TraderJoe](https://www.traderjoexyz.com/#/home) é uma plataforma descentralizada que se tornou um dos projetos mais conceituados da rede Avalanche com uma interface de usuário intuitiva e um recurso de troca de tokens que permite a sua conversão diretamente para "liquidity pools". A plataforma TraderJoe é também um dos parceiros oficiais da plataforma Mai Finance com um LP de MAI-USDC.

![](../.gitbook/assets/AVAX_joe.png)

* [YieldYak](https://yieldyak.com/farms) é outro "autocompounder" que oferece APYs elevados. As "farms" de tokens únicos trabalham em conjunto com a app BenQI par aumentar os retornos sendo assim considerado uma jogada de risco elevado.

![Interface YieldYak](../.gitbook/assets/avax_yak.png)

## Outros links úteis

* [Avalanche Network](htts://avax)
* [Avalanche community links](https://www.avax.network/community) (Discord, Medium, Reddit, Twitter, etc)
* [Debank](https://debank.com), portfolio manager

## Aviso

Este guia não tem como intuito oferecer conselhos financeiros e deve ser apenas considerado como uma ferramenta educativa. Faz sempre a tua própria pesquisa. Projetos discutidos neste guia não devem ser considerados como se estivessem a ser promovidos.
