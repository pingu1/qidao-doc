---
description: >-
  Neste guia, explicaremos tudo o que você precisa saber para começar a usar os
  diferentes DApps que a BNB Chain oferece.
---

# Como começar na BNB Chain

## O que é a BNB Chain?

A BNB Chain é uma rede compatível com EVM (Ethereum Virtual Machine) que é uma versão atualizada da Binance Smart Chain original que fornece baixas taxas de transação e tempos de bloco muito mais rápidos do que a Ethereum, a rede na qual se baseia.

Por isso, a BNB Chain é uma das redes mais populares do mundo, com mais de 4,5 bilhões de transações anuais e um [ecossistema de DApps](https://dappbay.bnbchain.org/) extremamente vibrante e maduro.

A BNB Chain usa o token BNB da Binance para pagar as taxas de gas, portanto, certifique-se de ter alguns em sua carteira para realizar transações. A Binance oferece [guias fáceis de serem seguidos ](https://www.binance.com/en/support/faq/85a1c394ac1d489fb0bfac0ef2fceafd)sobre como comprar ou transferir tokens para sua rede BNB.

## Começando na BNB Chain

Antes de usar a BNB Chain, você precisará de um endereço de carteira. Como o BNB Chain é uma rede EVM, ele aceitará as mesmas carteiras que em outras cadeias EVM, incluindo carteiras web como a Metamask ou a Nifty, e você poderá usar sua carteira de hardware como Trezor ou Ledger, mas pode ser necessário seguir etapas extras para poder conectá-las a rede.

Para este tutorial, vamos nos ater à Metamask, assim como fazemos em todos os outros guias deste site. Se você não tiver a Metamask instalada, poderá encontrar instruções em[ Como começar sua jornada na Polygon.](../polygon/how-to-get-started-on-polygon.md)

Além disso, você pode usar a própria Binance Wallet para começar na rede mais facilmente.

### Adding BNB Chain to Metamask

Open the Metamask popup, click the icon of your wallet, navigate to `Settings` then chose `Networks` and find `Add Network`. You will use the following information in the relevant text fields:

* **Network Name:** BNB Chain
* **New RPC URL:** [https://docs.binance.org/smart-chain/developer/rpc.html](https://docs.binance.org/smart-chain/developer/rpc.html)
* **Chain ID:** 0x38
* **Currency Symbol:** BNB
* **Block Explorer URL:** [**https://bscscan.com/**](https://bscscan.com/)\*\*\*\*

Save the changes, and Metamask will automatically switch you over to BNB:

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.28.44 AM.png>)

If you would like to search for additional RPCs with lower latency, take a look at [ChainList](https://chainlist.org/) for additional endpoints.

## Bridging to BNB Chain

### Faucets

There are freely available faucets on BNB Chain, but it is the opinion of the author that it will be safer to use something like ElkNet to get free gas tokens. If you choose to use a faucet you found online, please do so at your own risk. With [ElkNet](https://app.elk.finance/#/elknet), you can opt to swap some of your Elk tokens as gas when bridging from any of the supported networks.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.29.50 AM.png>)

### Bridges

* [Multi Chain](https://app.multichain.org/#/router) is the official partner of Mai Finance if you want to transfer your MAI or QI to BNB Chain from any other networks. From your selected network, you can simply chose the destination chain (BNB Chain) and the asset you want to send (MAI or QI for example) with the correct amount, and click on the `Transfer` button. Pay attention to the transfer fees taken directly on the asset you are transferring.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.32.07 AM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) is a popular bridge and allows you to transfer tokens from about fifteen different networks to BNB Chain.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.31.15 AM.png>)

* [Hashflow](https://app.hashflow.com/) is a newer bridging technology that works essentially as a crosschain DEX (decentralized exchange) for any token with sufficient liquidity. Additionally, Hashflow users can currently earn HFT (Hashflow tokens) for swapping or providing token liquidity. Chains are currently limited to Ethereum, Avalanche, Arbitrum, Optimism, Polygon, and BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.33.51 AM.png>)

* [Elknet](https://app.elk.finance/#/elknet) will act both as a bridge and as a faucet when you transfer the ELK token between 2 networks. You will be able to bridge your ELK and on the receiving end, you can have a small portion of your ELK directly available as the gas token, BNB in our case, as explained in the section above.

## DeFi on BNB Chain

* [Ellipsis Finance](https://ellipsis.finance/pool/0x68354c6E8Bbd020F9dE81EAf57ea5424ba9ef322) is the go to place for MAI liquidity on BNB Chain. The MAI pool on Ellipsis (MAI+val3EPS) is comprised of four stablecoins including BUSD (Binance USD), USDC, USDT (Tether), and MAI. By depositing stablecoins, and then staking the LP into Ellipsis, users can earn a variable yield between 6 and 15% paid out in Ellipsis' EPS token, Vallas' VAL token, as well as trading fees.

![MAI+val3EPS pool on Ellipsis](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.07.42 AM.png>)

## Mai Finance on BNB Chain

The lending platform is already available on BNB Chain where you will be able to deposit your WBNB (Wrapped BNB) and CAKE (PancakeSwap) tokens in a vault and borrow MAI against them. You can then deposit your borrowed MAI on Ellipsis to earn yield on your MAI.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.11.26 AM.png>)

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Discussion of a project in this guide should not be considered as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
