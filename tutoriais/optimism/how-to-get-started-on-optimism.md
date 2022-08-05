---
description: >-
  Neste guia, explicaremos tudo o que você precisa saber para começar a usar os
  diferentes DApps que o Optimism tem a oferecer.
---

# Como começar na Optimism

## O que é Optimism?

Optimism, ou Optimistic Ethereum como às vezes é chamado, é uma solução de escalabilidade de rollup que permite aos usuários enviar transações na rede Ethereum e executá-las mais rapidamente por um custo de gas muito menor. Por esse motivo, a Optimism é conhecida como uma segunda camada, ou layer 2, da Ethereum (L2 para abreviar). O nome Optimism vem do uso da tecnologia de rollup otimista, que se refere ao tipo de prova que a rede usa para trabalhar em conjunto com a rede principal da Ethereum (camada 1 ou L1). Para ler mais sobre rollups otimistas e outras soluções de rollup como ZK (conhecimento zero), visite [este link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Por ser uma tecnologia de rollup, a Optimism não produz seus próprios blocos e, portanto, não é um blockchain. Além disso, a API da rede Optimism usa amplamente a mesma especificação JSON-RPC da Ethereum e, portanto, é essencialmente equivalente ao EVM (Ethereum Virtual Machine), permitindo que aplicativos criados para a rede principal do Ethereum sejam executados na Optimism sem alterações em sua base de código.

Observe que, por causa disso, a Optimism não possui um próprio token de gas, mas Ether para pagar as transações..

## Começando na Optimism

Antes de usar o Optimism, você precisará de um endereço de carteira. Como a Optimism é uma rede EVM, ele aceitará as mesmas carteiras que em outras cadeias EVM, incluindo carteiras web como Metamask ou Nifty. Você também poderá usar sua cold wallet, como a Trezor ou Ledger, mas talvez seja necessário seguir mais passos para poder conectá-la à rede.

Para este tutorial, vamos nos ater ao Metamask, assim como fazemos em todos os outros guias deste site. Se você não tiver a Metamask instalado, poderá encontrar instruções em [Como começar a sua jornada na Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Adicionando a Optimism na Metamask

Abra o pop-up da Metamask, clique no ícone da sua carteira, navegue até `Settings` então selecione `Networks` e encontre `Add Network`. Você usará as seguintes informações nos campos de texto relevantes::

* **Network Name:** Optimism
* **New RPC URL:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

Salve as alterações e a Metamask irá automaticamente mudar para a Optimism:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## Pontes à Optimism

### Faucets

Não há faucets para gas, ou torneiras, na Optimism, mas se você usar um DApp como a [ElkNet](https://app.elk.finance/#/elknet), você pode optar por trocar alguns de seus tokens Elk por gas ao fazer a ponte para qualquer uma das redes suportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Pontes

* [Multi Chain](https://app.multichain.org/#/router) é o parceiro oficial da Mai Finance se você deseja transferir seu MAI ou QI para a Optimism, de qualquer outra rede. Após selecionar a sua rede, você pode simplesmente escolher a rede de destino (Optimism) e o ativo que deseja enviar (MAI ou ETH com o valor correto, e clicar no botão`Transfer`. Mas preste atenção às taxas de transferência cobradas diretamente no ativo que você está transferindo.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) é uma ponte popular e um dos parceiros oficiais da rede Optimism.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) é outra ponte popular que também é parceira oficial da rede Optimism. Há apenas um pequeno número de tokens suportados, incluindo ETH e várias stablecoins como USDC, DAI e USDT, mas oferece taxas mais baixas do que a maioria das outras soluções.
* [Hashflow](https://app.hashflow.com/) é uma tecnologia de ponte mais recente que funciona essencialmente como uma DEX (corretora descentralizada) crosschain para qualquer token com liquidez suficiente. Além disso, os usuários do Hashflow atualmente podem ganhar HFTs (tokens Hashflow) por trocar ou fornecer liquidez. Atualmente, as redes estão limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon e BNB..

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) atuará como uma ponte e como uma faucet quando você transferir o token ELK entre 2 redes. Você poderá conectar seu ELK e, na extremidade receptora, poderá ter uma pequena parte do seu ELK diretamente disponível como token de gas, ETH no nosso caso, conforme explicado na seção acima.

## DeFi na Optimism

Para começar na Optimism, aqui estão alguns DApps que você pode achar úteis para usar seu MAI e QI, incluindo:

* [Curve](https://optimism.curve.fi/factory/4/deposit): É aqui que a maior parte da liquidez do MAI existe atualmente na Optimism, pois a Curve é extremamente eficiente na realização de swaps de stablecoin.\
  \
  Ao depositar MAI na Curve LP, você receberá tokens LP que podem ser depositados na farm da Curve na [página de Farm](https://app.mai.finance/farm) da Mai Finance para ganhar rendimento em tokens QI.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) foi lançada recentemente na Optimism, e é aqui que você encontrará o pool de liquidez QI/WETH. Atualmente, é ainda não disponível no protocolo, mas deve fornecer um caso de uso adicional para o QI até que o staking de QI seja lançado na rede. Observe que a Arrakis usa pools da Uniswap, portanto, você terá que depositar QI e WETH nas proporções especificadas para entrar no LP.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019), um fork da Balancer oficialmente sancionado e lançado na Optimism em junho de 2022, oferece um nova pool de stablecoins de alta liquidez apelidado de "Come Together", composto por FRAX, USDC e MAI. Devido às suas grandes recompensas, incluindo tokens QI, BEETS e BAL, certamente se tornará o pool de stablecoins "oficial" para a MAI na Optimism.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Mai Finance na Optimism

A plataforma de empréstimo já está disponível na Optimism, onde você poderá depositar seus tokens WETH (Wrapped Ether) ou WBTC (Wrapped Bitcoin) em um cofre e tomar emprestado MAI contra eles. MAI pode ser depositado na farm da Curve para rendimentos em QI, ou no novo pool de stablecoins FRAX/USDC/MAI no recém-lançado BeethovenX, que produz recompensas em tokens QI, BEETS e BAL.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## Aviso legal

Este guia NÃO é um conselho financeiro e deve ser simplesmente considerado uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
