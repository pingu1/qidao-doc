---
description: >-
  Neste guia, explicaremos tudo o que você precisa saber para começar a usar os
  diferentes DApps que Arbitrum tem a oferecer.
---

# Como começar na Arbitrum

## O que é Arbitrum?

Arbitrum é uma solução de escalabilidade cumulativa que permite aos usuários enviar transações na rede Ethereum e executá-las mais rapidamente por um custo de gas muito menor. Por esta razão, a Arbitrum é conhecida como uma layer 2, ou segunda camada, da Ethereum (L2 para abreviar). Como a sua rede irmã, Optimism, a Arbitrum usa a tecnologia de rollup otimista, que se refere ao tipo de provas que a rede usa para trabalhar em conjunto com a rede principal do Ethereum (camada 1 ou L1). Para ler mais sobre rollups otimistas e outras soluções de rollup como ZK (conhecimento zero), visite [este link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Por ser uma tecnologia de rollup, a Arbitrum não produz seus próprios blocos e, portanto, não é uma verdadeira blockchain. Offchain Labs, os desenvolvedores por trás da Arbitrum, pretendem tornar a rede compatível com EVM (Ethereum Virtual Machine) equivalente com futuras atualizações.

Observe que, por causa disso, a Arbitrum não usa seu próprio token de gas, mas usa Ether como gas para pagar as transações.

## Começando na Arbitrum

Antes de usar a Arbitrum, você precisará de um endereço de carteira. Como a Arbitrum é uma rede EVM, ela aceitará as mesmas carteiras que em outras cadeias EVM, incluindo carteiras web como a Metamask ou a Nifty, e você poderá usar sua carteira de hardware, como Trezor ou Ledger, mas talvez seja necessário seguir mais passos para poder conectá-las à rede.

Para este tutorial, vamos nos ater à Metamask, assim como fazemos em todos os outros guias deste site. Se você não tiver a Metamask instalado, poderá encontrar instruções em [Como começar a sua jornada na Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Adicionando a Arbitrum à Metamask

Abra o pop-up Metamask, clique no ícone da sua carteira, navegue até`Settings` então escolha `Networks` e encontre `Add Network`. Você usará as seguintes informações nos campos de texto relevantes:

* **Network Name:** Arbitrum
* **New RPC URL:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **Chain ID:** 4216
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://arbiscan.io/](https://arbiscan.io/)

Salve as alterações e a Metamask o mudará automaticamente para a Arbitrum:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## Pontes à Arbitrum

### Faucets

Não há faucets para gas na Arbitrum, mas se você usar um DApp como a [ElkNet](https://app.elk.finance/#/elknet), você pode optar por usar alguns de seus tokens Elk como gas ao fazer a ponte para qualquer uma das redes suportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### Pontes

* [Multi Chain](https://app.multichain.org/#/router) é o parceiro oficial da Mai Finance se você deseja transferir seu MAI ou QI para a Arbitrum de qualquer outra rede. A partir de sua rede selecionada, você pode simplesmente escolher a rede de destino (Arbitrum) e o ativo que deseja enviar (MAI ou ETH com o valor correto, e clicar no botão `Transfer`. Preste atenção às taxas de transferência cobradas diretamente no ativo que você está transferindo.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) é uma ponte popular e permite transferir tokens de cerca de quinze redes diferentes para a Arbitrum.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) é outra ponte popular. Há apenas um pequeno número de tokens suportados, incluindo ETH e várias stablecoins como USDC, DAI e USDT, mas oferece taxas de ponte mais baixas do que a maioria das outras soluções.
* [Hashflow](https://app.hashflow.com/) é uma tecnologia de ponte mais recente que funciona essencialmente como uma DEX (corretora descentralizada) crosschain para qualquer token com liquidez suficiente. Além disso, os usuários do Hashflow atualmente podem ganhar HFTs (tokens Hashflow) por trocar ou fornecer liquidez. Atualmente, as redes estão limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon e BNB..

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) atuará como uma ponte e como uma faucet quando você transferir o token ELK entre 2 redes. Você poderá conectar seu ELK e, na extremidade receptora, poderá ter uma pequena parte do seu ELK diretamente disponível como token de gás, ETH no nosso caso, conforme explicado na seção acima.

## DeFi na Arbitrum

* A [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) é atualmente a única plataforma com pool de liquidez em MAI na rede Arbitrum. Ao depositar seu MAI no pool MAI/USDC/USDT, os usuários podem ganhar cerca de 13% de rendimentos em suas stablecoins. Observe que este pool será migrado em breve, o que corrige um bug de liquidez existente.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## Mai Finance na Arbitrum

A plataforma de empréstimos já está disponível na Arbitrum, onde você poderá depositar seus tokens WETH (Wrapped Ether) ou WBTC (Wrapped Bitcoin) em um cofre e tomar emprestado MAI contra eles. Você poderá então depositar o seu MAI na Balancer para gerar rendimentos.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## Aviso legal

Este guia NÃO é um conselho financeiro e deve ser simplesmente considerado uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
