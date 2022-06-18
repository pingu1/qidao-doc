---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the different DApps that Optimism has to offer.
---

# How to get started on Optimism



## What is Optimism?

Optimism, or Optimistic Ethereum as it is sometimes called, is a rollup scaling solution that allows users to submit transactions on the Ethereum network and get them executed faster for a much lower gas cost. For this reason, Optimism is known as an Ethereum layer 2 (L2 for short). The name Optimism comes from its use of optimistic rollup technology which refers to the type of proofs that the network uses to work in tandem with the main Ethereum chain (layer 1, or L1). For further reading on optimistic rollups and other rollup solutions like ZK (zero knowledge), please visit [this link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Because it is a rollup technology, Optimism does not produce its own blocks and is therefore not a blockchain. Additionally, the Optimism network API largely uses the same JSON-RPC specification as Ethereum and is therefore essentially EVM (Ethereum Virtual Machine) equivalent, allowing applications created for Ethereum mainnet to run on Optimism with essentially no changes to their codebase.\
\
Please note that because of this, Optimism does not use its own gas token, but rather uses Ether as gas to pay for transactions.

## Getting started on Optimism

Before using Optimism, you will need a wallet address. Because Optimism is an EVM network, it will accept the same wallets as on other EVM chains, including web wallet like Metamask or Nifty, and you will be able to use your hardware wallet such as Trezor or Ledger, but you may have to follow extra steps to be able to connect your cold wallet to the network.

For this tutorial, we will stick to Metamask just as we have done for all the other guides on this site. If you don't have Metamask installed, you can find instructions on [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Adding Optimism to Metamask

Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Add Network`. You will use the following information in the relevant text fields:

* **Network Name:** Optimism
* **New RPC URL:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

Save the changes, and Metamask will automatically switch you over to Optimism:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## Bridging to Optimism

### Faucets

There are no faucets for gas on Optimism, but if you use a DApp like [ElkNet](https://app.elk.finance/#/elknet), you can opt to swap some of your Elk tokens as gas when bridging from any of the supported networks.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Bridges

* [Multi Chain](https://app.multichain.org/#/router) is the official partner of Mai Finance if you want to transfer your MAI or QI to Optimism from any other networks. From your selected network, you can simply chose the destination chain (Optimism) and the asset you want to send (MAI or ETH with the correct amount, and click on the `Transfer` button. Pay attention to the transfer fees taken directly on the asset you are transferring.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) is a popular bridge and one of the official bridging partners for the Optimism network.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) is another popular bridge that is also an official partner for the Optimism network. There are only a small number of supported tokens including ETH, and various stablecoins like USDC, DAI, and USDT, but it offers lower bridging fees than most other solutions.
* [Hashflow](https://app.hashflow.com/) is a newer bridging technology that works essentially as a crosschain DEX (decentralized exchange) for any token with sufficient liquidity. Additionally, Hashflow users can currently earn HFT (Hashflow tokens) for swapping or providing token liquidity. Chains are currently limited to Ethereum, Avalanche, Arbitrum, Optimism, Polygon, and BNB.

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
