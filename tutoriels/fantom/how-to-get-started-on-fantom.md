---
description: >-
  Dans cet article, nous vous expliquerons tout ce que vous devez savoir pour
  commencer à utiliser la chaîne Fantom.
---

# Comment démarrer sur Fantom

## Qu'est-ce que Fantom ?

Fantom est une alternative à Ethereum pour les concepteurs de blockchain. En tant que blockchain à base de smart contracts open-source, elle permet aux concepteurs de développer des DApps (applications décentralisées) sûres, complètes et modulaires.

La chaîne a été conçue pour surmonter toutes les limites de la génération précédente de plates-formes blockchain, parfois désignées comme le trilemme de la blockchain : décentralisation, sécurité et évolutivité. Pour améliorer l'un de ces aspects, il faut le faire au détriment de l'un des deux autres. Fantom a tenté de résoudre ce problème grâce à son mécanisme de consensus Lachesis aBFT (Asynchronous Byzantine Fault Tolerant) basé sur les DAG (Directed Acyclic Graphs), ce qui lui permet d'être performant, évolutif et sécurisé. Les premiers benchmarks ont montré que Fantom peut facilement gérer plus de 20 000 transactions par seconde.

Enfin, Fantom est compatible à 100% avec l'EVM (Ethereum Virtual Machine), ce qui signifie que les DApps qui ont été développées sur des réseaux compatibles EVM pourront également être déployées sur Fantom. Ceci apporte également un autre avantage pour les utilisateurs puisque MetaMask et d'autres applications web3 sont également compatibles avec Fantom. Vous pourrez passer sans problème de Polygon ou Avalanche à Fantom au sein d'un même portefeuille.

## Aller sur Fantom

Fantom étant compatible EVM, si vous avez déjà un portefeuille pour d'autres chaînes EVM (Ethereum Mainnet, Polygon ou Avalanche), vous pourrez l'utiliser. Sinon, il est temps de créer un portefeuille. Il existe différents types de portefeuille qui peuvent être utilisés:

* Portefeuille logiciel: MetaMask, [fWallet](https://pwawallet.fantom.network/#/)
* Portefeuille "physique": [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/), [Trezor](https://trezor.io/coins/)

Pour cet article, et parce que nous utilisons Metamask dans tous nos autres articles, nous utiliserons Metamask, mais n'hésitez pas à utiliser tout autre logiciel/matériel que vous souhaitez. Si vous avez besoin d'instructions sur la façon d'installer Metamask, vous pouvez trouver des instructions dans [l'article sur Polygon](../../polygon-tutorials/how-to-get-started-on-polygon.md#downloading-metamask).

### Ajouter Fantom à Metamask

Afin d'utiliser le réseau Fantom, vous devrez l'ajouter manuellement à Metamask. Pour ce faire, cliquez sur le menu déroulant `Network` en haut de la fenêtre Metamask (où il indique le réseau que vous utilisez actuellement, Ethereum Mainnet par défaut), puis sélectionnez `Custom RPC`. Les informations suivantes sont celles qui vous permettront de vous connecter à Fantom:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Après avoir enregistré vos modifications, Metamask passera automatiquement au réseau Fantom.

![Good job! You're on Fantom!](<../../.gitbook/assets/image (41).png>)

Si vous avez besoin de plus de détails pour configurer Metamask, vous trouverez des informations supplémentaires dans le [guide officiel de Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask).

### FTM faucet

Maintenant que vous êtes sur FTM, vous aurez besoin de quelques FTM (jeton natif utilisé pour couvrir les frais de transaction). Vous pouvez soit faire un pont avec des jetons FTM d'autres chaînes, soit utiliser un faucet qui déposera suffisamment de jetons FTM dans votre portefeuille pour effectuer quelques transactions. Le principal faucet sur Fantom se trouve sur SpookySwap, l'un des principaux DEX (Échange Décentralisé). Notez qu'il s'agit d'un service offert par SpookySwap qui repose sur Discord et qui nécessite un compte Discord valide et actif depuis plus de 30 jours (il n'est pas nécessaire d'être sur le serveur Discord de SpookySwap depuis 30 jours).

* Après avoir rejoins le serveur [Discord de SpookySwap](http://discord.gg/AqbsWsWDgn), et vérifié votre compte, allez dans la section `#faucet`.

![](<../../.gitbook/assets/image (42).png>)

* Dans le canal #faucet, tapez simplement la commande `!faucet` et le bot vous enverra des $FTM. Notez que vous serez limité à une interaction tous les 30 jours.
* Si vous voulez vérifier que vous avez bien reçu votre jeton FTM, vous pouvez cliquer sur le nom du Fantom Tip Bot pour interagir directement avec lui et taper `!balance`

![Merci Fantom Tip Bot et SpookySwap](<../../.gitbook/assets/image (45).png>)

* Tout ce que vous devez faire maintenant est d'envoyer vos jetons FTM à l'adresse de votre portefeuille en utilisant la commande `!withdraw <votre_adresse_de_portefeuille>`. Vous trouverez l'adresse de votre portefeuille en haut de la fenêtre Metamask.

![Retirer depuis un compte Discord](../../.gitbook/assets/ftm-faucet.png)

![Nouveau dépot dans mon portefeuille Metamask](../../.gitbook/assets/ftm-mm.png)

## Ponter vers Fantom

### Pontage des pièces stables / ETH / BTC

Si vous souhaitez établir un pont entre des pièces stables et Fantom, vous pouvez utiliser la liste suivante de ponts:

* [AnySwap](https://anyswap.exchange/#/bridge): Il s'agit du pont officiellement supporté pour envoyer les MAI que vous avez obtenus sur Polygon vers Fantom (voir l'article [MAI dans le Metaverse](../../universite-MAI/mai-dans-le-metaverse.md) pour plus de détails). Cette solution prend en charge de nombreux actifs et de nombreuses chaînes afin qu'il soit facile pour vous d'envoyer vos crypto-monnaies à Fantom. Veuillez consulter les notes de rappel au bas de l'interface utilisateur de la passerelle pour connaître les frais de transaction et le temps d'exécution prévu.

![Bridging some MAI from Polygon to Fantom](<../../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): offre des services de pontage pour de nombreuses chaînes pour la plus part des pièces stables, avec des frais allant de 0,04% à 0,19% pour le pontage vers Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): Les frais de transfert sont faibles et permettent de s'assurer qu'il y a suffisamment de liquidités sur la chaîne cible pour le jeton que vous souhaitez transférer. Plus la liquidité est faible (ou plus le montant à ponter est important), plus le transfert est long.

### Pontage d'autres actifs

* Binance CEX: Vous pourrez acheter le jeton FTM sur Binance et le transférer directement à Fantom, mais c'est le seul jeton que vous pourrez transférer.
* [SpookySwap](https://spookyswap.finance/bridge): supporte plusieurs réseaux et plusieurs jetons que vous pourrez envoyer à Fantom.
* AnySwap: voir la description faite dans la section des pièces stables ci-dessus.

## La DeFi sur Fantom

Fantom a connu une expansion assez impressionnante à la fin de l'été 2021, notamment grâce aux programmes de récompense qui ont permis d'attirer les investisseurs et les développeurs sur la chaîne. La croissance a également été soutenue par des projets de premier ordre qui ont déployé leurs DApps sur Fantom en septembre 2021, notamment Curve et SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Cette application est très similaire à Balancer. Vous pourrez échanger certains jetons contre d'autres, et aussi entrer dans des pools équilibrés composés de plusieurs jetons. C'est aussi le premier partenaire officiel de Mai Finance sur Fantom, et le seul endroit où vous pourrez échanger vos MAI, ou les utiliser dans la pool MAI-USDC.

![Swapping MAI for a little more FTM](<../../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): Il s'agit du plus grand DEX (Échange décentralisé) sur Fantom où vous pourrez échanger vos jetons contre d'autres, déposer des liquidités et récolter des rendements, à peu près de la même façon que vous le feriez sur QuickSwap sur Polygon. SpookySwap vous récompensera en utilisant le jeton BOO, le jeton natif de la plateforme. Par ailleurs, lorsque vous stakez vos jetons BOO, vous obtenez en échange du xBOO, un jeton de rendement, que vous pouvez utiliser pour obtenir des récompenses supplémentaires (même principe que le sirop de dragon sur QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): Plateforme traditionnelle d'AMM et de yield farming où vous pourrez échanger des jetons, créer des jetons LP et farmer des rendements dans des pools de liquidité. SpiritSwap vous paiera avec des jetons SPIRIT que vous pourrez stakez sur la plateforme et obtenir des jetons inSPIRIT (SPIRIT sera bloqué pendant un certain temps), le pendentif des jetons veCRV.
* [Tarot](https://www.tarot.to): Tarot est la version Fantom d'Impermax, où vous pourrez utiliser vos jetons LP de SpookySwap (ou d'autres DEX/AMM) et les utiliser pour farmer sur la plateforme. Vous pouvez également déposer des jetons seuls et les prêter sur les pools spécifiques où les gens pourront les emprunter pour générer de nouveaux jetons LP et augmenter le montant de leur farming. Faites attention aux liquidations si vous utilisez vos LP dans un pool où l'utilisation est élevée.
* [Scream](https://scream.sh): Il s'agit d'un clone de Compound où vous pourrez prêter vos jetons et emprunter contre eux. En prêtant vos jetons, vous gagnerez des récompenses en jetons que vous prêtez, ainsi que des jetons SCREAM que vous pourrez utiliser sur d'autres plateformes.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve est le projet de premier ordre que tout le monde connaît bien, où vous pourrez déposer vos jetons dans des pools spécifiques (pas besoin de déposer un montant équilibré) et vous serez récompensé en jetons que vous prêtez, ainsi qu'en jetons CRV et wFTM.

![DAI+USDC dual pool on Curve on Fantom](../../.gitbook/assets/ftm-crv.png)

Il y a beaucoup d'autres possibilités sur Fantom qui seront décrites dans d'autres articles.

## Autres liens utiles

* [Explorateur de Fantom](https://explorer.fantom.network)
* [Prix du gas sur Fantom](https://ftmscan.com/gastracker)
* [Serveur Discord officiel de Fantom](how-to-get-started-on-fantom.md#ftm-faucet)
* [DeBank](https://debank.com): gestionnaire de portfolio

## Avertissements

Cet article n'est PAS un conseil financier et doit simplement être considéré comme un outil éducatif. Faites toujours vos propres recherches. Les projets présentés dans cet article ne sont que des exemples des possibilités offertes par le réseau et ne doivent pas être considérés comme une approbation du projet.

{% hint style="info" %}
N'oubliez pas qu'une stratégie qui fonctionne bien à un moment donné peut donner de mauvais résultats (ou vous faire perdre de l'argent) à un autre moment. Restez informé, surveillez les marchés, gardez un œil sur vos investissements et, comme toujours, faites vos propres recherches.
{% endhint %}
