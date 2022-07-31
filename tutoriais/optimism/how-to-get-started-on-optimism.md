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

Não há torneiras para gas, ou faucets, na Optimism, mas se você usar um DApp como a [ElkNet](https://app.elk.finance/#/elknet), você pode optar por trocar alguns de seus tokens Elk por gas ao fazer a ponte para qualquer uma das redes suportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Pontes

* [Multi Chain](https://app.multichain.org/#/router) é o parceiro oficial da Mai Finance se você deseja transferir seu MAI ou QI para a Optimism, de qualquer outra rede. Após selecionar a sua rede, você pode simplesmente escolher a rede de destino (Optimism) e o ativo que deseja enviar (MAI ou ETH com o valor correto, e clicar no botão`Transfer`. Mas preste atenção às taxas de transferência cobradas diretamente no ativo que você está transferindo.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) é uma ponte popular e um dos parceiros oficiais da rede Optimism.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) é outra ponte popular que também é parceira oficial da rede Optimism. Há apenas um pequeno número de tokens suportados, incluindo ETH e várias stablecoins como USDC, DAI e USDT, mas oferece taxas mais baixas do que a maioria das outras soluções.
* [Hashflow](https://app.hashflow.com/) é uma tecnologia de ponte mais recente que funciona essencialmente como uma DEX crosschain (corretora descentralizada entre redes) para qualquer token com liquidez suficiente. Além disso, os usuários do Hashflow atualmente podem ganhar HFT (tokens de fluxo de hash) para trocar ou fornecer liquidez para tokens. Atualmente, as redes estão limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon e BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) will act both as a bridge and as a faucet when you transfer the ELK token between 2 networks. You will be able to bridge your ELK and on the receiving end, you can have a small portion of your ELK directly available as the gas token, ETH in our case, as explained in the section above.

## DeFi on Optimism

To get started on Optimism, here are some DApps you may find useful to put your MAI and QI to use, including:

* [Curve](https://optimism.curve.fi/factory/4/deposit): This is where the majority of the MAI liquidity currently exists on Optimism as Curve is extremely efficient at performing stablecoin swaps.\
  \
  By depositing MAI into the Curve LP, you will then receive LP tokens which can be deposited into the Curve farm on Mai Finance's [Farm page](https://app.mai.finance/farm) to earn yield in QI tokens.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) recently launched on Optimism, and this is where you will find the QI/WETH liquidity pool. It is currently unseeded by the protocol, but should provide an additional use case for QI until QI staking launches on the network. Please note that Arrakis uses Uniswap pools so you will have to deposit both QI and WETH in the specified ratios in order to enter the LP.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019), an officially sanctioned Balancer fork, launched on Optimism on June 2022 and offers a brand new high liquidity stablecoin pool dubbed "Come Together" which is composed of FRAX, USDC, and MAI. Due to its large rewards including QI, BEETS, and BAL tokens, it is certain to become the de facto stablecoin pool for MAI on Optimism.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Mai Finance on Optimism

The lending platform is already available on Optimism where you will be able to deposit your WETH (Wrapped Ether) or WBTC (Wrapped Bitcoin) tokens in a vault and borrow MAI against them. MAI can be deposit into the Curve farm to earn QI, or the new FRAX/USDC/MAI stable pool on the recently launched BeethovenX which earns rewards in QI, BEETS, and BAL tokens.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
