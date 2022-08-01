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

## Getting started on Arbitrum

Before using Arbitrum, you will need a wallet address. Because Arbitrum is an EVM network, it will accept the same wallets as on other EVM chains, including web wallet like Metamask or Nifty, and you will be able to use your hardware wallet such as Trezor or Ledger, but you may have to follow extra steps to be able to connect your cold wallet to the network.

For this tutorial, we will stick to Metamask just as we have done for all the other guides on this site. If you don't have Metamask installed, you can find instructions on [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Adding Arbitrum to Metamask

Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Add Network`. You will use the following information in the relevant text fields:

* **Network Name:** Arbitrum
* **New RPC URL:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **Chain ID:** 4216
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://arbiscan.io/](https://arbiscan.io/)

Save the changes, and Metamask will automatically switch you over to Arbitrum:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## Bridging to Arbitrum

### Faucets

There are no faucets for gas on Arbitrum, but if you use a DApp like [ElkNet](https://app.elk.finance/#/elknet), you can opt to swap some of your Elk tokens as gas when bridging from any of the supported networks.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### Bridges

* [Multi Chain](https://app.multichain.org/#/router) is the official partner of Mai Finance if you want to transfer your MAI or QI to Arbitrum from any other networks. From your selected network, you can simply chose the destination chain (Arbitrum) and the asset you want to send (MAI or ETH with the correct amount, and click on the `Transfer` button. Pay attention to the transfer fees taken directly on the asset you are transferring.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) is a popular bridge and allows you to transfer tokens from about fifteen different networks to Arbitrum.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) is another popular bridge. There are only a small number of supported tokens including ETH, and various stablecoins like USDC, DAI, and USDT, but it offers lower bridging fees than most other solutions.
* [Hashflow](https://app.hashflow.com/) is a newer bridging technology that works essentially as a crosschain DEX (decentralized exchange) for any token with sufficient liquidity. Additionally, Hashflow users can currently earn HFT (Hashflow tokens) for swapping or providing token liquidity. Chains are currently limited to Ethereum, Avalanche, Arbitrum, Optimism, Polygon, and BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) will act both as a bridge and as a faucet when you transfer the ELK token between 2 networks. You will be able to bridge your ELK and on the receiving end, you can have a small portion of your ELK directly available as the gas token, ETH in our case, as explained in the section above.

## DeFi on Arbitrum

* [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) currently has the only pool on Arbitrum with MAI liquidity. By depositing your MAI into the MAI/USDC/USDT pool, users can earn roughly 13% yield on their stablecoins. Please note that this pool will be migrated shortly which fixes an existing liquidity bug.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## Mai Finance on Arbitrum

The lending platform is already available on Arbitrum where you will be able to deposit your WETH (Wrapped Ether) or WBTC (Wrapped Bitcoin) tokens in a vault and borrow MAI against them. You can then deposit your borrowed MAI on Balancer to earn yield.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
