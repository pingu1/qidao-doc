---
description: >-
  Ce guide vous présente un aperçu des différentes chaînes sur lesquelles la
  monnaie stable MAI peut être utilisée, et comment vous pourrez la transférer
  vers d'autres réseau.
---

# MAI dans le metaverse

![](../.gitbook/assets/screen-shot-2021-09-13-at-1.06.42-pm.png)

## Intro

MAI, que vous pourrez parfois retrouver sous le nom de miMATIC, est la première monnaie stable native au réseau Polygon. Elle est maintenue à un prix de 1,00$ et sa valeur peut fluctuer entre 0,99$ et 1,01$. Vous pouvez retrouver plus d'informations relatives au maintien de sa valeur dans [la documentation officielle](https://docs.mai.finance/stablecoin-economics). Mais ce n'est pas parce que MAI est native de Polygon qu'elle se retrouve uniquement sur cette chaîne. En effet, de la même façon que son homologue DAI est présente sur plusieurs réseaux, DAI étant une autre monnaie stable ayant vu le jour sur le réseau Ethereum Mainnet, MAI commence lentement mais certainement son expansion vers d'autres réseaux. Cet article va mettre en évidence les différentes chaînes où vous pourrez la retrouver, ainsi que la façon de transférer vos MAI d'un réseau à un autre.

## Polygon

### Obtenez des MAI sur Polygon

Comme expliqué dans l'introduction, MAI est une monnaie native de Polygon, et c'est également la seule chaîne (lors de la rédaction de cet articles en Septembre 2021) où vous pourrez en "générer". Vous pouvez au choix:

* emprunter des MAI en utilisant d'autres crypto-monnaies comme valeur collatérale en les déposant dans les coffres spécialisés sur Mai Finance
* utiliser l'[ancre](https://app.mai.finance/anchor) permettant de l'échange de monnaie stable (USDC, USDT ou DAI) pour des MAI
* vendre d'autres crytos et acheter des MAI sur n'importe quelle plateforme d'échange décentralisée sur Polygon, les plus efficaces étant [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) ou [1Inch](https://app.1inch.io/#/137/classic/swap).

### Utilisez vos MAI sur Polygon

La monnaie stable MAI est de plus en plus adoptée par tous les grands projets sur Polygon, plus précisément depuis qu'elle a été introduite auprès des autres monnaies stables sur QuickSwap. En Septembre 2021, il y a 3 fermes de rendements sur QuickSwap composées de monnaies stables uniquement, accumulant un grand total de 18 327 604$:

* MAI-DAI avec 6 553 255 $
* MAI-USDT avec 6 316 026 $
* MAI-USDC avec 5 458 323 $

Vous pourrez trouver d'autres pools sur bien d'autres projets / fermes de rendements / optimisateurs de gains. Veuillez vous référer aux différents articles de ce guide, et plus particulièrement à celui dédié à l'[Utilisation de MAI sur Polygon](../tutoriels-polygon/que-faire-avec-vos-mai-sur-polygon.md).

## Solana

### Obtenez des MAI sur Solana

Solana est une plateforme de blockchain pour les applications décentralisées. Le but sous-jacent du réseau est de proposer une solution ayant des frais de transactions bas (moins de 0,01 $) et rapide (moins de 400ms par transaction). L'idée avouée est de créer une alternative au réseau Ethereum Mainnet et à ses chaînes auxiliaires. Cependant, ce n'est pas parce que Solana est un chaine concurrente au réseau Ethereum qu'elle ne supporte pas les mêmes crypto-monnaies. En effet, Solana supporte maintenant la monnaie stable MAI qui peut être transférée depuis Polygon.

Afin d'envoyer vos tokens MAI sur Solana, vous pourrez utiliser [AllBridge](https://allbridge.io), une plateforme de transfert qui vous permettra d'envoyer vos tokens d'une chaîne à une autre. AllBridge supporte les réseaux suivants:

* Ethereum Mainnet
* Polygon
* Solana
* Huobi
* Binance Smart Chain

{% hint style="info" %}
Veuillez noter que le transfert d'une chaîne à l'autre n'assure pas le transfert de n'importe quelle crypto. Ainsi, MAI n'est pour le moment transférable que de Polygon à Solana et réciproquement.
{% endhint %}

L'interface est très intuitive dans le sens où vous n'avez qu'à sélectionner les deux réseaux et la monnaie que vous voulez transférer entre les deux.

![Transfert de MAI depuis Polygon vers Solana](../.gitbook/assets/screen-shot-2021-09-13-at-1.52.23-pm.png)

L'étape suivante vous permet de renseigner l'adresse de votre portefeuille sur Solana, ainsi que le montant que vous souhaitez faire transiter. Veuillez noter que Metamask ne supporte pas (encore) les portefeuilles de Solana, et vous aurez donc besoin de créer un portefeuille séparé sur ce réseau. Il peut s'agir un portefeuille web ou une application. Veuillez vous renseigner en lisant les [recommandations officielles de Solana](https://docs.solana.com/wallet-guide) avant d'en choisir un.

{% hint style="info" %}
Faites attention que sur Solana, il n'existe pas de faucet (site permettant d'obtenir vos premiers SOL de façon gratuite pour effectuer vos premières transactions). Vous aurez besoin d'acheter quelques SOL au préalable et de les ajouter à votre portefeuille afin de pouvoir effectuer le transfert de vos MAI.
{% endhint %}

### Utilisez vos MAI sur Solana

De la même façon que vous pouvez utiliser des MAI sur Polygon en déposant des token LP (**L**iquidity **P**rovider) dans des réserves de liquidité afin de récolter des frais de transaction et des récompenses en crypto-monnaies, vous pouvez faire la même chose sur Solana. Pour le moment, la seule plateforme supportant officiellement MAI est [Saber](https://app.saber.so) où vous trouverez une réserve MAI-USDC.

![Etat de la réserve MAI-USDC sur Saber en Septembre 2021](../.gitbook/assets/screen-shot-2021-09-13-at-2.11.10-pm.png)

Un des points forts de cette réserve sur Saber (et de la plateforme en général) est qu'il est possible de déposer des jetons uniques sans avoir à combiner une pair de tokens avec un ratio 1:1. Vous pourrez donc directement déposer des MAI (ou des USDC) sans vous soucier de balancer avec l'autre moitié de la paire stable.

![MAI et USDC sont débalancés sur la réserve MAI-USDC sur Saber](../.gitbook/assets/screen-shot-2021-09-13-at-2.13.51-pm.png)

De ce fait, vous n'avez qu'à envoyer des MAI à 100% depuis Polygon sur Solana sans avoir à convertir la moitié en USDC, en réalisant une possible perte lors de la conversion. Cela permet également de s'affranchir de la possible différence de prix (négligeable) entre les deux monnaies stables. Veuillez noter que vous recevrez des récompenses en jeton natif de la ferme Saber, de la même façon que vous recevez des QUICK lorsque vous fournissez de la liquidité sur QuickSwap. Vous pouvez ensuite vendre vos jetons pour augmenter votre position dan la réserve de liquidité MAI-USDC.

{% hint style="info" %}
Sur Solana, vous pourrez également utiliser [Sunny](https://app.sunny.ag), un optimisateur de profits qui va composer vos intérêts provenant de Saber. Veuillez noter que Sunny n'est pas une plateforme approuvée par l'équipe de Mai Finance. AllBridge et Saber sont les seuls partenaires officiels en relation avec la chaîne Solana, mais les résultats ne peuvent être garantis. Veillez, comme toujours, à effectuer vos propres recherches avant d'investir dans un quelconque projet trouvé sur internet, y compris ceux cités dans ce guide.
{% endhint %}

## Avalanche

### Obtenez des MAI sur Avax

Avalanche est une blockchain conçue pour offrir une plateforme open-source ainsi qu'un protocole de couche de niveau 1 (layer 1 protocol) où lancer des applications décentralisées et des solutions de blockchain pour les entreprises. C'est une autre alternative au réseau Ethereum Mainnet qui supporte les mêmes monnaies globales que celles que vous pourrez trouver sur Mainnet, Polygon ou Solana. À ce titre, vous avez maintenant la possibilité de transférer vos MAI depuis Polygon (la seule chaîne où il est possible de générer la monnaie stable MAI) vers Avax en utilisant [Relay Chain](https://app.relaychain.com/#/transfer).

D'une façon générale, l'interface de Relay Chain est très semblable à celle de toutes les autres plateformes de transfert. Vous avez simplement à choisir le réseau d'origine, celui de destination, ainsi que la crypto-monnaie à transférer.

![Transfert de MAI depuis Polygon vers Avalanche](../.gitbook/assets/screen-shot-2021-09-13-at-2.52.31-pm.png)

Metamask supporte les [portefeuilles Avax](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche), vous n'aurez donc pas besoin d'une autre application pour gérer vos cryptos sur Avalanche.

### Utilisez vos MAI sur Avax

Vous pourrez utiliser MAI de la même façon que sur Polygon, dans une ferme de rendements adéquate. L'application officiellement approuvée par Mai Finance est [Trader Joe](https://www.traderjoexyz.com/#/farm), où il vous sera possible de déposer des jetons de liquidité MAI-USDC.

![État de la réserve de liquidité MAI-USDC sur Trader Joe en Septembre 2021](../.gitbook/assets/screen-shot-2021-09-13-at-3.07.19-pm.png)

Les fermes sur Avalanche fonctionnent de façon très similaire à celles de Polygon. Vous pouvez ainsi effectuer les mêmes opérations sur Trader Joe que ce que vous pourriez faire sur QuickSwap. Vous devrez commencer par créer une paire stable MAI-USDC avec un ratio 1:1, puis déposer ces jetons dans la réserve. Tout comme vous êtes rétribués avec des QUICK sur QuickSwap, vous obtiendrez des tokens JOE sur Trader Joe. Vous pourrez ensuite placer des jetons JOE ailleurs, ou les vendre pour accroître vos jetons MAI-USDC.

## Fantom

### Obtenez des MAI sur Fantom

Fantom est une blockchain / plateforme de contrats intelligents dont le but est de résoudre les problèmes de croissance d'échelle que rencontrent les autres réseaux, principalement Ethereum Mainnet. Les développeurs peuvent y créer des DApps (**D**ecentralized **App**lications, ou applications décentralisées) et utiliser les mêmes crypto-monnaies que sur les autres réseaux. De ce fait, vous pouvez dès maintenant transférer la monnaie stable MAI depuis Polygon vers Fantom en utilisant [AnySwap](https://anyswap.exchange/#/bridge).

Encore une fois, on retrouve une interface graphique très similaire à celles des autres plateformes de transfert comme AllBridge ou Relay Chain. En étant connecté sur Polygon via Metamask, vous pourrez sélectionner le réseau de départ, celui d'arrivée (Fantom), ainsi que la crypto à transférer (MAI).

![Transfert de MAI depuis Polygon vers Fantom](../.gitbook/assets/image.png)

Metamask supporte les [portefeuilles Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask), il est donc très facile de configurer votre propre portefeuille pour y transférer vos MAI.

### Utilisez vos MAI sur Fantom

Au moment d'écrire ce guide, aucun partenariat officiel n'a été mis en place entre Mai Finance et les fermes de rendements sur Fantom. Nous ne pouvons donc pas renseigner une plateforme en particulier. L'intégration de MAI sur Fantom étant très récente, il se peut que ce guide soit mis à jour dans les prochaines semaines.

## Avertissement

Les détails présentés dans ce guide sont purement à titre informatif et n'ont pas été testés par l'équipe rédigeant les tutoriels. Quelques utilisateurs de la communauté sur Discord ont déjà tenté de transférer leurs crypto-monnaies d'une chaîne à une autre, vous pouvez donc rejoindre la communauté sur le serveur Discord pour poser vos questions si vous en avez. Veuillez s'il vous plaît vous renseigner sur les différents réseaux, sur leurs frais de transaction et temps d'execution, frais de transferts, temps de transfert etc ... Si vous envoyez vos crypto-monnaies sur d'autres chaînes veillez toujours à être capable de les renvoyer sur Polygon en cas de besoin.

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
