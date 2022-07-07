---
description: In this guide, we'll explain how to get started using Moonbeam.
---

# How to get started on Moonbeam

## What is Moonbean?

Launching in January 2020, Moonbeam is an EVM (Ethereum virtual machine) compatible smart contract platform running on the Polkadot network making it what is called a Polkadot parachain. Parachains are interconnected set of chains that benefit from Polkadot's main relay chain while remaining interoperable, thereby partaking in the benefits and security of the main chain while running in parallel to it.\
\
Polkadot describes the benefits of parachains as follows, “Parachains end the era of siloed blockchains, creating a decentralized, connected internet of blockchains where before there existed only isolated networks with their own tribalistic communities.”

![Moonbeam, a Polkadot parachain](<../../.gitbook/assets/moonbeam (1).jpg>)

Because of its EVM compatibility layer, Moonbeam makes it easier for Solidity developers to be able to port their existing applications from other EVM-compatible networks to Moonbeam with few code changes. Moonbeam currently has a TVL of $130m, and a [vibrant and growing](https://defillama.com/chain/Moonbeam) ecosystem of applications.&#x20;

Moonbeat also offers Substrate compatibility. Substrate is a modular blockchain framework used by developers for building blockchains tailored to their needs using reusable components called pallets. It uses the Rust programming language and is the framework most developers use when building parachains for the Polkadot network.

As Moonbeam is a Substrate-based blockchain, apps integrated with its network benefit from interoperability between the Polkadot and Ethereum chains, as well as others like Bitcoin.

Developers can also use Substrate-compatible ecosystem tools commonly used on Ethereum, including block explorers, front-end development libraries, and wallets, as well as development tools like Truffle and Remix.\
\
The native gas token for Moonbeam is GLMR.

## Getting started on Moonbeam

Before using Moonbeam, you will need a wallet address. Because Moonbeam is an EVM network, it will accept the same wallets as on other EVM chains, including web wallet like Metamask or Nifty, and you will be able to use your hardware wallet such as Trezor or Ledger, but you may have to follow extra steps to be able to connect your cold wallet to the network.

For this tutorial, we will stick to Metamask just as we have done for all the other guides on this site. If you don't have Metamask installed, you can find instructions on [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Adding Moonbeam to Metamask

Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Add Network`. You will use the following information in the relevant text fields:

* **Network Name:** Moonbeam
* **New RPC URL:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **Chain ID:** 128
* **Currency Symbol:** GLMR
* **Block Explorer URL:** [https://moonscan.io/](https://moonscan.io/)

Save the changes, and Metamask will automatically switch you over to Moonbeam:

![Moonbeam on Metamask](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## Bridging to Moonbeam

### Faucets

GLMR is Moonbeam's native gas token so you'll need to have some in your wallet to make transactions on chain. Fortunately, the official Moonbeam Faucet will help get your started with a small amount of GLMR, though please note that the amount dispersed by the token may sometimes not be enough to complete a transaction if the network is congested. \
\
In order to receive some free GLMR, you'll need to verify you're a human via the captcha bot, and connect your Metamask wallet to the site. A small amount (0.007 GLMR) will then be sent immediately to your wallet.

![GLMR.Supply Faucet](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

Additionally, users may want to use Solarflare's "[Swap for gas](https://app.solarflare.io/bridge/gas-swap)" feature. This allows users to swap other tokens including WETH, WBTC, USDC, DAI, USDT, BUSD, FLARE, and BNB into GLMR, Moonbeam's native gas token.

![Solarflare's "Swap for Gas" feature](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### Bridges

* [Multichain](https://app.multichain.org/#/router) is the official bridge for MAI through its partnership with MAI finance, and you can easily send your MAI to Moonbeam by using it.

![Multichain on Moonbeam](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) is a full-featured AMM (automated market maker) on Moonbeam which is very similar to Uniswap. Solarflare has a built-in bridge which allows users to bridge assets from Ethereum mainnet as well as BNB chain to Moonbeam. Solarflare also has a "Swap for gas" feature as mentioned in the Faucets section above.

![Bridging with Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) is a popular bridge that also supports Moonbeam. Please note that you may not be able to bridge from every chain into Moonbeam (Polygon to Moonbeam bridging is not supported, for example).

![Bridging with Celer](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* Other bridges are available but may be chain specific such as Nomad or Axelar for the Cosmos ecosystem.

## DeFi on Moonbeam

[StellaSwap](https://app.stellaswap.com/farm) is currently the main source of liquidity for MAI on Moonbeam. The MAI-Base4Pool is comprised of MAI, FRAX, USDT, USDC, and DAI and currently has a TVL (total value locked) of $535k, yielding a solid 26% APR (annual percentage rate) on your stablecoins.

![MAI-Base4Pool on StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam has a vibrant DeFi ecosystem with dozens of DApps (decentralized applications) available to use including DeFi staples found on other chains such as [Curve](https://moonbeam.curve.fi/) and [Beefy Finance](https://app.beefy.com/). For a full list of available DApps, check out [DefiLlama's Moonbeam page](https://defillama.com/chain/Moonbeam).

## Mai Finance on Moonbeam

While Mai Finance is not available on Moonbeam, you can create vaults and borrow MAI against xStella and wGLMR on StellaSwap. Please note that borrowing MAI on StellaSwap will incur interests - 12% on xStella vaults, and 8% on wGLMR vaults. You can find out more on how to use StellaSwap's MAI vaults in the next section titled, [Playing with MAI legos on StellaSwap](playing-with-mai-legos-on-stellaswap.md).

![Vaults on StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
