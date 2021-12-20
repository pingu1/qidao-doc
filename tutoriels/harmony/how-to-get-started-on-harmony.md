---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the Harmony chain.
---

# How to get started on Harmony

## What is Harmony

Harmony is a blockchain that tries to solve the issues that the Ethereum Mainnet faces: achieving a satisfying degree of balance between decentralization and scalability. The main focus of the chain are made on a high transaction throughput, speed and energy efficiency. This is done by highly leveraging sharding of validators that would be grouped to process transactions simultaneously. Supporting scalability is as simply as growing the number of shards, which also helps achieving faster transaction. Feel free to dig more about Harmony and its technology in their [official documentation](https://docs.harmony.one/home/general/technology).

## Getting started on Harmony

In order to use the Harmony network, you will need a wallet address. Because Harmony is an EVM-compatible network (**E**thereum **V**irtual **M**achine), it will accept the same wallets as on other EVM-compatible chains, including web wallet like Metamask or Nifty, and you will be able to use your hardware wallet such as Trezor or Ledger.

For this tutorial, we will stick to Metamask like for all the other guides on this site. If you don't have Metamask installed, you can find instructions on [How to get started on Polygon](../../polygon-tutorials/how-to-get-started-on-polygon.md).

### Adding Harmony to Metamask

If you have installed the latest version of Metamask, you should already have access to the Harmony chain and there's nothing else for you to de besides selecting `Harmony One` in the network dropdown at the top of Metamask. You can also set a new RPC yourself to access Harmony using these steps. Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Harmony One`. The data you should get are as follows:

* **Network Name:** Harmony One
* **New RPC URL:** https://api.harmony.one
* **Chain ID:** 1666600000
* **Currency Symbol:** ONE
* **Block Explorer URL:** https://explorer.harmony.one/

Save the changes, and Metamask will automatically switch you over to the Harmony network:

![Congratulations!! You're now on Harmony](../../.gitbook/assets/Harmony-onboarding-1.png)

## Bridging to Harmony One

### Faucets

There isn't any official faucet to get your first ONE tokens for your first few transactions. You will mostly have to bridge some tokens from another chain using the official [Harmony bridge](https://bridge.harmony.one/erc20) that will let you bridge some specific assets from either Ehtereum Mainnet or Binance to Harmony. You can also get a list of projects that will let you get some ONE via Fiat Gateways or Exchange Gateways from [this list](https://docs.harmony.one/home/developers/harmony-stack#bridges-fiat-gateways-exchanges) curated by the Harmony team.

As always, you can also use [ElkNet](https://app.elk.finance/#/elknet) to transfer some ELK tokens from other chains to Harmony. If you do so, make sure to check the box `Swap $ELK 1 for gas` that will swap a part of your transferred tokens to ONE, which will also let you swap the rest of your ELK tokens to more ONE, or other assets.

### Bridges

* [Multichain.org](https://app.multichain.org/#/router) (previously known as AnySwap) is the official partner of Mai Finance that will let you bridge your MAI tokens from Polygon and other chains to Harmony. As a side note, Multichain has been working hand in hand with the Mai Finance devs to make sure the MAI that you bridge to Harmony is the same as what you will be able to borrow from the lending platform. There's no need for a Hub on Harmony. Simply head to the Multichain router, select the origin network, the token you want to transfer, and the destination network, and you're done. Pay attention to minumum amounts to transfers, transfer fees, and bridging duration, but once done, you'll get your asset on Harmony.

![Bridging MAI from Polygon to Harmony One](../../.gitbook/assets/Harmony-onboarding-2.png)

* [Official Harmony Bridge](https://bridge.harmony.one/erc20), as explain in the previous paragraph, will let you transfer specific assets from Ethereum Mainnet or BSC.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) is another solution if you want to transfer something to Harmony. Check their application to see which assets are bridgeable.
* [ElkNet](https://app.elk.finance/#/elknet) is a particular case since the bridge from Elk Finance will let you bridge the ELK token from any EVM-compatible chain to any other EVM-compatible chain where they're deployed with the possibility to swap a small portion of the transferred amount into gas token (see the section dedicated to Faucets just above).

## DeFi on Harmony

Because Harmony One is a network that offers fast and secured transaction, as well as very cheap gas, a lot of EVM-compatible DApps (**D**ecentralized **App**lications) have been deployed to this network. The list that follows doesn't present all of them, feel free to explore the network and its DApps list yourself. You can find a more [exhaustive list on DefiLlama](https://defillama.com/chain/Harmony).

* [ViperSwap](https://viper.exchange/#/swap): This is the first partner of Mai Finance on Harmony One. This is a regular Uniswap v2 fork, a DEX (**D**ecentralized **Ex**change) and AMM (**A**utomated **M**arket **M**aker) where you will be able to swap your assets, create LP (**L**iquidity **P**roviding) tokens and farm rewards by providing liquidity to traders. The reward is paid using the VIPER token, that you will be able to stake on the app for more rewards. This is the DEX where you will find some MAI liquidity to swap your MAI, or to farm rewards using your MAI.

![MAI-ONE and MAI-VIPER pools on ViperSwap as of December 2021](../../.gitbook/assets/Harmony-onboarding-3.png)

You will note that the APRs (**A**nnual **P**ercentage **R**ate) on pools are very high. This is mostly due to the reward format on ViperSwap: when you claim your rewards, 5% of the VIPER tokens can be used directly, while 95% if locked until 2021-12-25. After that, the reward is vesting over a complete year, meaning that you will not be able to access your farming gains right away, and it will drip very VERY slowly. There's another twist on ViperSwap pools: you will have to pay a withdrawal fee that decreases if you stake your LP tokens for a long time. It goes from 25% fee if you withdraw within the same block as the deposit transaction (to fight flashloan operations) to 0.01% if you withdraw after 1 month. More details in their official documentation about [farming rewards](https://docs.venomdao.org/viper/tokenomics#bbd0) and [LP withdrawal fees](https://docs.venomdao.org/viper/fees).

* [DeFi Kingdom](https://game.defikingdoms.com/#/): This is a particularly interesting project that is mixing DeFi and Gamification. Its native token, the JEWEL token, is used as a farming reward for users that are providing liquidity, but it can be used in game or in the marketplace. Explaining the entire universe of DeFi Kingdom (or DFK) would take too much time for this guide, so we strongly recommend reading [the official documentation](https://docs.defikingdoms.com).

![Main map of DeFi Kingdom as of December 2021](../../.gitbook/assets/Harmony-onboarding-4.png)

* [SushiSwap](https://app.sushi.com) is the famous DEX/AMM that is also present on many other chains. Swap, provide liquidity, farm ONE and SUSHI yields.
* [Curve Finance](https://harmony.curve.fi) is another cross-chain application that will let you provide liquidity (3pool and tricrypto) and will reward you with compounded tokens, as well as ONE and CRV.
* [Beefy Finance](https://app.beefy.finance/#/harmony) is a yield optimizer that we already present in many of our guides since it's present on many chains. Currently, you will be able to deposit your LP tokens from Curve and SushiSwap, and let the Beefy compounder aggregate the rewards provided by the farming platform into more LP tokens.
* [Euphoria DAO](https://app.euphoria.money/#/dashboard) is currently the biggest Ohm-fork on Harmony, and developped by the Venom DAO also behind ViperSwap. You can bond a few different assets and get their native asset, the WAGMI token. Stake WAGMIs for more WAGMI with insane APY (**A**nnual **P**ercentage **Y**ield) as for most OHM projects.

## Mai Finance on Harmony

Mai Finance launched on Harmony One in December 2021, and this guide is pretty close to the launch date so the application may have been updated when you read it.

You will be able to deposit your WETH or your ONE tokens on Mai Finance (https://app.mai.finance/vaults/create) in order to borrow the MAI stable coin. You will then be able to swap MAI to leverage your assets, margin trade, or farm yields on ViperSwap.

![MAI Finance vaults as of December 2021](../../.gitbook/assets/Harmony-onboarding-5.png)

## Disclaimer

As usual, this guide is not financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
