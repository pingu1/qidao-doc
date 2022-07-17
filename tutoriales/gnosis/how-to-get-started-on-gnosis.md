---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the different DApps that Gnosis has on its blockchain.
---

# How to get started on Gnosis Chain

## What is Gnosis Chain?

The Gnosis Chain is a EVM-compatible blockchain, meaning that it's compatible with the code deployed on the Ethereum network (EVM = **E**thereum **V**irtual **M**achine). As most chains are trying to achieve the Security/Scalability/Decentralization Trifecta, Gnosis Chain focuses on speed (5s transaction finality) and low costs for transactions. It uses xDAI (gnosis chain wrapped DAI) as its main gas token for regular transactions, but also uses the GNO token for governance and staking. The Gnosis Chain has been originally designed for prediction markets built on Ethereum. Prediction markets are like exchanges where outcome of events are traded. As events unfold, the gnosis tokens gain or lose value depending on what was predicted.

To support the goal of the Gnosis Chain, an application layer has been added, on which you will find specialized decentralized applications such as 

* RealT: a Tokenized Real Estate application 
* Kleros: a Justice-as-a-Service platform that aims at resolving conflicts using blockchain technology

You can check additinonal details about Gnosis Chain like its TVL and other applications on [DeFi Llama](https://defillama.com/chain/Gnosis).

## Getting started on Gnosis Chain

Before usign the Gnosis Chain, you will need a wallet address. Because Gnosis is an EVM network, it will accept the same wallets as on other EVM chains, including web wallet like Metamask or Nifty, and you will be able to use your hardware wallet such as Trezor or Ledger, but you may have to follow extra steps to be able to connect your cold wallet to the network.

For this tutorial, we will stick to Metamask like for all the other guides on this site. If you don't have Metamask installed, you can find instructions on [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Adding Gnosis Chain to Metamask

In theory, Gnosis comes pre-installed with MetaMask, meaning that you should not have to add the chain information for Metamask to work. However, it may be a good idea to verify that your setup is correct by double checking the values saved into your local wallet. Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Gnosis Chain`. The data you should get are as follows:

* **Network Name:** Gnosis Chain
* **New RPC URL:** https://rpc.gnosischain.com/
* **Chain ID:** 100
* **Currency Symbol:** xDAI
* **Block Explorer URL:** https://blockscout.com/xdai/mainnet

Save the changes, and Metamask will automatically switch you over to the Gnosis chain:

![Success!! You're now on Gnosis!](../../.gitbook/assets/gnosis-0.png)

## Bridging to Gnosis Chain

### Faucets

You can use Google to find a few faucets on Gnosis Chain where you will be able to request your first few xDAI to start transacting. I don't recommend anything in particular, but found [this community-ran faucet](https://www.gimlu.com/faucet) that delivers 0.002 xDAI on every requests. Beware that the number of request you can do is limited, and it's absolutely not a way to make free money.

![I received a few xDAI from the faucet, let's do some transactions now.](../../.gitbook/assets/gnosis-1.png)

### Bridges

* [Multi Chain](https://app.multichain.org/#/router) is the official partner of Mai Finance if you want to transfer your MAI to Gnosis Chain from Polygon or other networks. When you're connected to Polygon, you can simply chose the destination chain (Gnosis Chain) and the asset you want to send (MAI or miMATIC) with the correct amount, and click on the `Transfer` button. Pay attention to the transfer fees taken directly on the asset you're transferring.

![Bridging MAI from Polygon to Gnosis using Multi Chain](../../.gitbook/assets/gnosis-2.png)

* [Elknet](https://app.elk.finance/#/elknet) will act both as a bridge and as a faucet when you transfer the ELK token between 2 networks. You will be able to bridge your ELK and on the receiving end, you can have a small portion of your ELK directly available as the gas token, xDAI in our case.

## DeFi on Gnosis

Gnosis will propose a few DeFi options on its chain, including:

* [SushiSwap](https://app.sushi.com/farm?chainId=100): This is one of the main DEX and AMM on Gnosis/xDAI. You will be able to swap your assets, or participate in liquidity mining by providing LP (**L**iquidity **P**roviding) pairs in farms.
* [Curve](https://xdai.curve.fi/): This is where the majority of the liquidity is provided on the Gnosis Chain. This is also where you will be able to provide the MAI stablecoin in the [MAI Stablecoin](https://xdai.curve.fi/factory/4) pool and receive rewards in GNO tokens.

![LP pools that include MAI on Curve as of June 2022](../../.gitbook/assets/gnosis-3.png)

* [Honeyswap](https://app.honeyswap.org/#/pool), [Honeycomb](https://1hive.io/#/wallet) and [Agave](https://app.agave.finance/#/dashboard): Respecively a DEX (Uniswap fork) that allows you to swap tokens and create Liquidity Providing tokens, an AMM (Goose fork) that lets you stake your LP tokens created on Honeyswap and get yields for providing liquidity, and a lending protocol (AAVE fork) that lets you lend certain assets and borrow others. These 3 dApps are forming a complete ecosystem managed by the same team.
* [Elk Finance](https://app.elk.finance/#/farms): Elk is a Uniswap V2 fork that will let you operate swaps, deposit liquidity and farm their $ELK token using different assets of the Gnosis Chain, including $MAI. You will also be able to stake your ELK tokens for more rewards, or transfer them from one chain to another using the ElkNet bridge.

![Farming ELK using MAI on Elk Finance as of June 2022](../../.gitbook/assets/gnosis-5.png)

## Mai Finance on Gnosis Chain

The lending platform is already available on Gnosis Chain where you will be able to put your GNO tokens in a vault and borrow MAI against it. This will allow you to use your GNO tokens as collateral, and use your MAI on Curve to farm more GNO tokens. The loop would consist of

* Create a vault on [Mai Finance](https://app.mai.finance)
* Deposit your $GNO tokens in the vault
* Borrow $MAI against your collateral at 0% interest
* Deposit the $MAI on Curve Finance and get GNO rewards

![Farming yields on Gnosis Chain](../../.gitbook/assets/gnosis-4.png)

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
