---
description: >-
  Dans cet article, nous expliquerons tout ce qu'il y a à savoir sur la chaine
  Avalanche pour s'en servir.
---

# Comment démarrer sur Avalanche

## Avalanche, c'est quoi?

Avalanche est une blockchain de 1ère couche (L1, comme Ethereum, Bitcoin, Solana, ...) qui fonctionne comme une plateforme pour des applications décentralisées et des réseaux blockchain personnalisés. Le réseau Avalanche est composé de 3 blockchains individuelles: X-Chain, C-Chain, et P-Chain. Chacune a un but précis, ce qui est une approche radicalement différente d'autres réseaux. Les blockchains Avalanche utilisent même un mécanisme de consensus différent, en fonction de leurs rôles.

Avalanche est 100% compatible avec l'EVM (Ethereum Virtual Machine), ce qui signifie qu'elle est compatible avec les outils Ethereum existants. La C-Chain offre les même fonctionnalités qu'Ethereum mais avec un débit plus élevé, une finalité inférieur à la seconde, et des frais de transactions bien inférieurs. AVAX est le jeton natif d'Avalanche et est utilisé pour payer les transactions.

## Aller sur Avalanche

Avant d'utiliser Avalanche, il vous faut un portefeuille. Il y a différent types de portefeuille:

* Portefeuille **logiciel**, comme MetaMask & le [portefeuille natif à Avalanche](https://wallet.avax.network)
* Portefeuille **matériel**, comme [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true) ou [Trezor](https://trezor.io/coins/)

Pour cet article, nous utiliserons MetaMask. Si vous ne l'avez pas installé, vous pouvez trouver des instructions [ici](../polygon/how-to-get-started-on-polygon.md#telechargez-metamask).

### Ajouter Avalanche à MetaMask

Pour utiliser le réseau Avalanche, vous devez l'ajouter à votre liste de RPC sur MetaMask. Pour le faire, cliquez sur le menu déroulant des réseaux (il y a écrit Ethereum Mainnet si c'est la première fois que vous vous en servez), puis selectionnez `RPC Personnalisé`. Vous pouvez ajouter les valeurs suivantes dans le formulaire qui apparait:

* **Nom du réseau**: Avalanche Network
* **Nouvelle URL RPC**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Symbole**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Sauvegardez les changements, puis MetaMask passera automatiquement sur le réseau Avalanche.

![Success! You're on Avalanche!](<../../.gitbook/assets/image (36).png>)

## Amener des fonds sur Avalanche

### Faucets

Il n'y a pas de faucet disponible sur Avalanche. Si vous avez besoin d' AVAX pour payer les frais de transactions, vous devrez en envoyer directement à votre portefeuille, via un échange centralisé, ou un pont (tel que Elknet). Plus sur ces derniers dans la section ci-dessous.

### Ponts

* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) offre une interface intuitive et facile à utiliser avec des frais faibles. C'est la passerelle officielle du [MAI vers Avalanche](../../universite-MAI/mai-dans-le-metaverse.md#avalanche).
* [Pont Avalanche Officiel](https://bridge.avax.network) - Avalanche a son propre pont qui peut être utiliser pour faire transférer des assets depuis Ethereum. Les frais de transactions sont payés avec les jetons transférer et peuvent être élevés puisque vous venez d'Ethereum.
* [Anyswap](https://anyswap.exchange/#/bridge) permet de faire le pont entre plusieurs chaines, pour plusieurs jetons. Il y a un minimum de jetons à transferer qui varie selon le jeton, ainsi que des frais de transfert constant.
* [Celer Bridge](https://cbridge.celer.network/#/transfer) offre des ponts vers plein de chaine avec une très bonne interface utilisateur. Les frais de transfert sont de \~3% vers Avalance.
* [Elknet](https://app.elk.finance/#/elknet) est un pont déployé par Elk Finance, un échange décentralisé disponible sur plusieurs réseaux, dont Avalanche, Binance, Fantom, Polygon et xDai. Ce qui démarque Elknet des ponts ci-dessus, c'est qu'il n'y a pas besoin d'AVAX pour faire le pont mais il y a un hic que nous allons voir ci-dessous. Il n'y a que les frais de transactions pour faire le pont.
  * Pour envoyer vos jetons vers Avalanche via Elknet, vous devez les convertir en ELK, le jeton natif d'Elk Finance.
  * Vous pouvez ensuite utiliser le pont pour déplacer vos ELK, et si vous cochez "Swap $ELK for gas", une partie de votre transfert sera converti en AVAX.
  * Une fois le pont complété (en général, moins de 10 minutes), vous pouvez passer votre MetaMask sur le réseau Avalanche et vous verrez vos ELK et un peu d'AVAX prêts à l'emploi. Vous pouvez maintenant échanger vos ELK directement sur le site vers n'importe quel jeton disponible sur Avalanche.
  * La même opération peut être effectuée pour retourner sur Polygon, ou n'importe quel réseau supporté.

![Elknet interface](<../../.gitbook/assets/image (40).png>)

## La DeFi sur Avalanche

Avalanche a eu une croissance rapide dans les derniers mois ce qui mène, non seulement, à de très bons projets natifs, mais aussi, à des valeurs sûres de la DeFi qui se déploient sur le réseau.

* [Aave](https://app.aave.com/dashboard) a récemment été déployé sur Avalanche et a déjà $4b en valeur total bloquée. Les jetons acceptés en collatéraux incluent: AAVE, AVAX, DAI, USDT, USDC, WBTC, et WETH. Les jetons camAVAX seront acceptés en collatéraux dans les coffres de Mai Finance.
* [Beefy Finance](https://app.beefy.finance/#/avax) est probablement connu de la plupart des utilisateurs de la DeFi puisqu'il est disponible sur la BSC, Fantom, Harmony, Polygon et d'autres. C'est un auto-réinvestisseur, et fournis des APYs élevées pour des jetons seuls ou en paire. Il support les paires [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) et [MAI/USDC.e](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e) disponible sur Trader Joe.
* [Benqi](https://app.benqi.fi/markets) est un protocole similaire à Aave et était le premier du genre sur Avalanche. Il supporte AVAX, DAI, LINK, USDT, USDC, WBTC et WETH en collatéraux.

![BenQI interface](<../../.gitbook/assets/image (37).png>)

* [TraderJoe](https://www.traderjoexyz.com/#/home) est un échange décentralisé et est devenu l'un des top projets d'Avalanche avec son interface utilisateur intuitive, et la possibilité de convertir un jeton directement en jeton de réserve de liquidité. C'est aussi un partenaire officiel avec sa [réserve MAI-USDC](../../universite-MAI/mai-dans-le-metaverse.md#utilisez-vos-mai-sur-avax).

![](<../../.gitbook/assets/image (39).png>)

* [YieldYak](https://yieldyak.com/farms) est un autre auto-réinvestisseur qui fournit des APYs de culture élevées. Ses fermes pour jetons seul fonctionne en conjonction avec BenQi pour tirer parti de revenus plus élevés et est donc considéré plus risqué.

![](<../../.gitbook/assets/image (38).png>)

## Autres liens utiles

* [Réseau Avalanche](htts://avax)
* [Liens communautaires d'Avalanche](https://www.avax.network/community) (Discord, Medium, Reddit, Twitter, etc)
* [Debank](https://debank.com), gestionnaire de portfolio

## Avertissements

Cet article **n'est pas un conseil financier** et devrait être considéré comme un outil éducatif. Faites toujours vos propres recherches. La mention d'un projet dans cet article ne devrait pas être considérée comme une approbation.
