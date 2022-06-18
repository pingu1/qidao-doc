---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the different DApps that Arbitrum has to offer.
---

# How to get started on Arbitrum

## What is Arbitrum?

Arbitrum is a rollup scaling solution that allows users to submit transactions on the Ethereum network and get them executed faster for a much lower gas cost. For this reason, Arbitrum is known as an Ethereum layer 2 (L2 for short). Like its sibling network, Optimism, Arbitrum uses optimistic rollup technology which refers to the type of proofs that the network uses to work in tandem with the main Ethereum chain (layer 1, or L1). For further reading on optimistic rollups and other rollup solutions like ZK (zero knowledge), please visit [this link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Because it is a rollup technology, Arbitrum does not produce its own blocks and is therefore not a true blockchain. Offchain Labs, the developers behind Arbitrum, aim to make the network EVM (Ethereum Virtual Machine) equivalent with future upgrades.\
\
Please note that because of this, Arbitrum does not use its own gas token, but rather uses Ether as gas to pay for transactions.

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
