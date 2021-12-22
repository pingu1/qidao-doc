---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the Fantom chain.
---

# Como começar na Fantom

## O que é Fantom

Fantom é uma alternativa a Ethereum para desenvolvedores de blockchain. Como uma blockchain open-source com suporte para contratos inteligentes, ela permite que os desenvolvedores construam Dapps (**D**ecentralized **App**lications) seguros, compreensivos e modulares.

A rede foi projetada para vencer todas as limitaçōes da geração anterior das plataformas blockchains, as vezes referenciado como o trilema das blockchains: decentralização, segurança e escalabilidade. Para melhorar um destes aspectos, precisamos sacrificar um dos outros dois. A Fantom tenta resolver isso graças ao seu mecanismo de consenso Lachesis aBFT (Asynchronous Byzantine Fault Tolerant) baseado em DAG (Directed Acyclic Graphs), permitindo alta performance,  escalabilidade e segurança. Testes iniciais mostraram que a Fantom pode facilmente aguentar mais de 20,000 transaçōes por segundo..

Por último, a Fantom é 100% compativel a EVM (**E**thereum **V**irtual **M**achine), o que significa que DApps que foram desenvolvidos em redes compativeis a EVM podem rodar na Fantom também. Isso traz outra vantagem aos usuários, já que a MetaMask e outras aplicaçōes web3 também são compativeis com a Fantom. Você será capaz de alternar entrar a Polygon ou a Avalanche à Fantom pela mesma carteira.

## Começando na Fantom

Como a Fantom é compativel a EVM, se você já possuir uma carteira para outras redes EVM (Ethereum Mainnet, Polygon ou Avalanche), você será capaz de usá-la. Se não, é hora de criar uma nova carteira. Há muitos tipos diferentes de carteiras que podem ser usadas: **carteiras de software** como a Metamask ou a [fWallet](https://pwawallet.fantom.network/#/), e **carteiras de hardware** como a [Trezor](https://trezor.io/coins/) ou a [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/).

Aqui, como ela é a nossa escolha nos outros guias, usaremos a Metamask, mas sinta-se livre para utilizar qualquer carteira que preferir, seja de software ou hardware. Se precisar de ajuda para instalar a Metamask, você pode visitar este [guia da rede polygon](../../polygon-tutorials/how-to-get-started-on-polygon.md#downloading-metamask).

### Adicionando a rede Fantom à Metamask

Para usar a rede Fantom, você precisará configurá-la manualmente na Metamask. Para fazer isto, clique no menu "Network" na parte superior da janela (onde é exibida a rede que está sendo utilizada, Ethereum Mainnet originalmente), então selecione `Custom RPC`. As informaçōes seguintes são as que te permitirão conectar-se a rede Fantom:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Após salvar as mudanças, a Metamask irá automaticamente trocar para a rede Fantom.

![Bom trabalho! Você está na Fantom!](../../.gitbook/assets/ftm-mm0.png)

Se precisar de mais detalhes para configurar a Metamask, você pode encontrar mais informação no [guia oficial da Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask).

### FTM faucet

Now that you are on FTM, you will need some FTM (native token used to cover gas costs). You can either bridge some FTM tokens from other chains, or use a faucet that will deposit enough FTM tokens in your wallet to perform a few transactions. The [main faucet on Fantom](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas) can be found on SpookySwap, one of the main DEXes there (**D**ecentralized **Ex**change). Note that it's a service offered by SpookySwap that relies on Discord, and that will require a valid Discord Account active for more than 30 days (it's not required to be on the SpookySwap Discord server for 30 days though).

* Once you joined the [SpookySwap Discord](http://discord.gg/AqbsWsWDgn) server, and verified your account, head to the #faucet section.

![](<../../.gitbook/assets/image (42).png>)

* In the #faucet channel, simply type the `!faucet` command and the bot will send you some $FTM. Note that you'll be limited to 1 interaction every 30 days.
* If you want to verify that you properly received your FTM token, you can click the Fantom Tip Bot name to interact directly with it and type `!balance`

![Thank you Fantom Tip Bot and SpookySwap](<../../.gitbook/assets/image (45).png>)

* All you need to do now is to send your FTM tokens to your wallet address using the command `!withdraw <your_wallet_address>`. You will find your wallet address at the top of Metamask window.

![Withdrawing from Discord account](../../.gitbook/assets/ftm-faucet.png)

![Fresh deposit in my Metamask wallet](../../.gitbook/assets/ftm-mm.png)

## Bridging to Fantom

### Bridging stable coins / ETH / BTC

If you want to bridge stable coins to Fantom, you can use the following list of bridges:

* [AnySwap](https://anyswap.exchange/#/bridge): This is the officially supported bridge to send the MAI you minted on Polygon to Fantom (see the [MAI metaverse](../../mai-university/mai-metaverse.md#fantom) guide for details). This solution supports many assets and many chains so that it will be easy for you to send your crypto currencies to Fantom. Please check the Reminder notes at the bottom of the bridging UI for transaction fees and expected execution time.

![Bridging some MAI from Polygon to Fantom](<../../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): offers bridging services for many chains for most stable coins, with fees ranging from 0.04% to 0.19% to bridge to Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): low fees, and ensures that there's enough liquidity on the target chain for the token you want to bridge. The lower the liquidity (or the large the amount to bridge), the longer the transfer.

### Bridging other assets

* Binance CEX: You will be able to buy the FTM token on Binance and bridge it directly to Fantom, but this is the only token you will be able to transfer.
* [SpookySwap](https://spookyswap.finance/bridge): supports many networks and many tokens that you will be able to send to Fantom.
* AnySwap: see description made in the stable coin section.

## DeFi on Fantom

Fantom has seen a pretty impressive expansion at the end of the summer 2021, especially with reward programs that helped attracting investors and developers on the chain. The growth has also been supported by blue chip projects that deployed their DApps on Fantom in September 2021, including Curve and SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): This application is very similar to Balancer. You will be able to trade some tokens for others, and also enter balanced pools composed of multiple tokens. This is also the first official partner of Mai Finance on Fantom, and the only place where you will be able to swap your MAI, or use them in a MAI-USDC pool.

![Swapping MAI for a little more FTM](<../../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): This is the biggest DEX (**D**ecentralized **Ex**change) on Fantom where you will be able to swap your tokens for others, deposit liquidity and farm yields, pretty much the same way you would do it on QuickSwap on Polygon. SpookySwap will reward you using the BOO token, the native token of the platform. As a side note, when you stake your BOO tokens, you will get xBOO, a yield baring token, in exchange, and you can use them to earn extra rewards (same principle as the dragon syrup on QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): Traditional AMM and yield farming platform where you'll be able to swap tokens, create LP tokens and farm yields in liquidity pools. SpiritSwap will pay you with SPIRIT tokens that you can stake on the platform and get inSPIRIT tokens (SPIRIT will be locked for a certain period of time), the pendent of veCRV tokens. You can also use SpiritSwap for lending and borrowing while waiting for Mai Finance on Fantom.
* [Tarot](https://www.tarot.to): Tarot is the Fantom version of Impermax, where you will be able to use your LP tokens from SpookySwap (or other DEXs/AMM) and use them to farm on the platform. You can also deposit single tokens and lend them on the specific pools where people will be able to borrow them to generate new LP tokens and leverage their farming amount. Be aware of liquidations if you leverage your LPs in a pool where the utilization is high.
* [Scream](https://scream.sh): This is a clone of Compound where you will be able to lend your tokens and borrow against them. Lending your tokens will make you earn rewards in the token you lend, as well as SCREAM tokens that you will be able to use on other platforms.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve is the blue chip project everyone knows well, where you will be able to deposit your tokens in specific pools (no need to deposit a balanced amount) and you will be rewarded in the tokens you lend, as well as CRV and wFTM tokens.

![DAI+USDC dual pool on Curve on Fantom](../../.gitbook/assets/ftm-crv.png)

There are plenty of other opportunities on Fantom that will be described in other guides.

## Other useful links

* [Fantom explorer](https://explorer.fantom.network)
* [Fantom gas checker](https://ftmscan.com/gastracker)
* Official [Fantom Discord](how-to-get-started-on-fantom.md#ftm-faucet) server
* [DeBank](https://debank.com) portfolio managed

## Disclaimer

This guide is NOT financial advice, and should simply be regarded as an educational tool. Always do your own research. Projects presented in this guide or just showcasing the possibilities on the network, and you should not be taken as an endorsement of the project.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
