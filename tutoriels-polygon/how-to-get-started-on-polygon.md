---
description: >-
  Dans ce guide nous allons présenter tout ce dont vous aurez besoin pour
  commencer à utiliser les différentes applications que Polygon propose sur sa
  blockchain.
---

# Comment bien démarrer sur Polygon

## Qu'est-ce que Polygon?

Polygon est un réseau construit par dessus la chaîne principale Ethereum, mais il a été conçu pour adresser les problèmes d'échelle (taille du réseau, nombre d'utilisateurs, temps de transaction) dont souffre la chaîne Ehtereum. En moyenne, une transaction sur Polygon est validée en 3 a 5 secondes, et coûte une fraction de centime, ce qui permet d'opérer des dizaines de transactions chaque jour, même avec un portefeuille modeste.

Polygon est également l'une des toutes premières chaînes annexes mise en production, et cette petite avance de quelques mois sur les autres chaînes disponibles aujourd'hui lui a permit d'obtenir

* Un nombre toujours croissant d'utilisateurs, surpassant le nombre d'utilisateurs du réseau Ethereum pour la première fois en Septembre 2021
* Un nombre croissant d'applications dans de multiples domaines
* Une valeur en dollars qui se stabilise aux alentours de 4 milliards de dollars US (répartis dans toutes les application de l'écosystème)

Polygon a également réussit à construire une certaine réputation de confiance en prouvant que le réseau était robuste et capable de soutenir une utilisation intense, faisant de la chaîne une alternative compétitive à l'Ethereum Mainnet. Ses performances ouvrent la porte au monde de la DeFi (**De**centralized **Fi**nance, ou Finance Décentralisée) aux petits investisseurs souhaitant tester les crypto-monnaies sans avoir à débourser des centaines de dollars et sacrifier des journées entières à effectuer quelques transactions. Avec cette confiance et cette facilité d'utilisation, les grandes entreprises se tournent également vers Polygon, permettant d'accroître l'anonymat et la sécurité, permettant de ce fait de rendre le réseau encore plus robuste.

## Créez simplement votre Portefeuille

Avant de pouvoir utiliser la blockchain Polygon, vous aurez besoin d'un portefeuille, identifié par une adresse unique. Il existe plusieurs types de portefeuilles, sous forme **digitale** (Metamask, TrustWallet, ...) ou sous format **physique** (Trezor, Ledger, ...). Dans le cadre de ce guide, nous allons nous concentrer sur _Metamask_, l'option la plus simple pour débuter votre voyage sur la blockchain.

### Téléchargez Metamask

La première étape est de télécharger Metamask, une extension pour votre navigateur web, depuis [le site officiel](https://metamask.io). Veuillez vérifier que l'URL est bien correcte (metamask.io), plusieurs sites ont tenté de hacker des utilisateurs en leur faisant télécharger des versions piratées de Metamask. A noter qu'il est également possible de télécharger des versions mobiles iOS ou Android de Metamask. Ce guide ne présentera que la version pour navigateur.

Une fois l'extension téléchargée et installée dans votre navigateur, vous devriez voir le logo parmi les différentes extensions. Lorsque vous ouvrez Metamask pour la première fois, vous aurez la possibilité de renseigner un compte existant (nécessitant la **seed phrase**, une combinaison de plusieurs mots uniques identifiant un compte spécifique), ou vous pourrez vous créer un nouveau compte si vous le souhaitez. Si vous avez besoin de créer un nouveau compte, veuillez suivre les étapes suivantes:

* Commencez par renseigner un mot de passe pour accéder à votre compte Metamask
* Regardez la vidéo explicative à propos de la sécurisation de votre portefeuille, et sur l'importance de la **seed phrase**.
* Votre **seed phrase** vous sera montrée. Il est impératif de sécuriser cette combinaison de mots car c'est la protection la plus importante pour votre portefeuille. Si vous perdez cette phrase, il vous sera alors impossible de restaurer votre portefeuille sur un quelconque appareil, et vous risquez de perdre l'intégralité de votre portefeuille ainsi que l'accès à votre compte Metamask. Veillez donc à conserver votre seed phrase dans un endroit sécurisé, et ne la communiquez sous aucun prétexte.

Lorsque vous avez terminé de configurer votre compte, vous devriez voir ceci dans votre navigateur:

![Interface de Metamask](<../.gitbook/assets/image (18).png>)

### Configurez l'accès à Polygon

Comme vous pouvez le voir dans la capture d'écran ci-dessus, Metamask vous crée un compte sur le réseau Ethereum Mainnet. Si vous cliquez sur le menu déroulant se trouvant dans le coin supérieur droit de la fenêtre, vous pourrez changer de chaîne, cependant Polygon ne fait pas (encore) partie des réseaux pré-définis. Nous allons donc vous montrer comment ajouter manuellement l'accès à Polygon. Veuillez noter que comme Polygon est une couche construite à partir de la chaîne Ethereum principale, vous allez conserver la même adresse de portefeuille.

Pour configurer l'accès à Polygon, commencez par cliquer sur la bulle colorée représentant votre compte, cliquez sur Settings, puis Networks afin d'accéder à la liste des réseaux pré-configurés. Cliquez sur "Add Network" et renseignez les champs comme suit:

![](<../.gitbook/assets/image (20).png>)

Une fois le réseau configuré et sauvegardé, vous êtes pratiquement prêt à utiliser Metamask sur Polygon, il ne vous reste plus qu'à changer de réseau via le menu déroulant, et vous pourrez passer à l'étape suivante.

## Obtenez vos premiers $MATIC

Maintenant que votre navigateur est configuré pour naviguer sur la chaîne Polygon, il ne vous manque plus qu'une chose: quelques MATIC. En effet, Polygon vous permet de réaliser des **transactions**, des opérations entre votre portefeuille et une applications, effectuer un échange entre 2 portefeuilles, ou toute autre interaction entre 2 protocoles sur la blockchain. Pour sécuriser et valider la transaction (opération effectuée par les validateurs), il vous faudra cependant payer des frais (aussi appelé **gas fee**, ou carburant) versés aux validateurs, et ces frais sont payés avec le jeton natif de l'écosystème, le MATIC.

Afin de pouvoir réaliser vos premières transactions, vous pourrez utiliser [cette page](https://matic.supply) qui enverra vos premiers MATICs (ou fractions de MATIC) directement dans votre portefeuille.Ces pages sont appelées des faucets (traduit littéralement par _Lavabo_), et sont des petites réserves de MATIC permettant aux nouveaux venus de commencer à utiliser Polygon. Il vous faudra connecter votre portefeuille au faucet, puis compléter le captcha afin de recevoir 0,002 MATIC (\~0,00223$), ce qui vous permettra d'effectuer quelques transactions sur Polygon.

![Getting FREE MATIC](<../.gitbook/assets/image (23).png>)

Il se peut que la page ne fonctionne pas correctement lors de certaines périodes de forte utilisation du réseau, ou lorsque de nombreux utilisateurs (y compris des robots) tentent de retirer des MATIC sur cette page. Il vous suffit alors d'attendre un peu et d'essayer à nouveau un peu plus tard. Il existe également d'autres faucets que vous pourrez utiliser (incluant [celui-ci](https://macncheese.finance/matic-polygon-mainnet-faucet.php)). Veuillez cependant effectuer vos propres recherches avant de vous connecter à n'importe quelle application. Ce guide ne vous présente que 2 solutions vérifiées, faites donc attention si vous souhaitez utiliser une autre page non-listée dans ce guide.

{% hint style="info" %}
Les faucets ne sont pas faits pour être vidés de leur contenu, ils sont là afin d'aider les débutant sur Polygon en leur offrant leurs premiers MATIC. Aucun transfert ne sera effectué si votre portefeuille possède déjà assez de MATIC, ou si vous utilisez la page plus de quelques fois en 24h. Veuillez agir de façon responsable et ne pas abuser de cette aide.
{% endhint %}

## Ajoutez vos tokens préférés à Metamask

Avec votre portefeuille configuré et vos premiers MATIC, vous voici prêt à utiliser toutes les applications et jetons que Polygon vous propose. Vous pourrez par exemple ajouter les tokens que vous allez utiliser fréquemment an ajoutant l'adresse électronique permettant de les identifier. Pour cela, vous pouvez utiliser [PolygonScan](https://polygonscan.com). Veuillez simplement entrer le nom de la crypto-monnaie que vous souhaitez ajouter à Metamask afin d'obtenir les informations qui lui sont spécifiques. Par exemple, si vous cherchez QiDAO sur PolygonScan, vous obtiendrez ce résultat:

![Résultat de la recherche de QiDAO sur PolygonScan](<../.gitbook/assets/image (24).png>)

Il vous suffit de copier l'adresse du contrat, puis de cliquer sur "Add token" dans Metamask pour renseigner l'adresse du jeton que vous souhaitez ajouter.

![Adding Qi on Metamask](<../.gitbook/assets/image (25).png>)

## Comment acheter des crypto-monnaies sur Polygon

Seuls quelques MATIC ne vous permettront pas de faire beaucoup de transactions. Vous aurez cependant la possibilité d'acheter des jetons sur Polygon, ou d'échanger les monnaies que vous aurez acheté contre d'autres. Vous pourrez le faire sur une plateforme d'échange décentralisée (**DEX**, ou **D**ecentralized **Ex**change), et sur Polygon, vous aurez le choix parmi, entre autre, [QuickSwap](https://quickswap.exchange/#/swap), [SlingShot](https://app.slingshot.finance/trade/m/MATIC/USDC), [DexGuru](https://dex.guru), [SushiSwap](https://app.sushi.com/swap) et bien d'autres.

À titre d'exemple, voici comment effectuer un échange de MATIC pour des Qi sur QuickSwap:

![Achat de Qi à partir de MATIC sur QuickSwap](<../.gitbook/assets/image (26).png>)

{% hint style="info" %}
Une autre application particulièrement intéressante pour faire des échanges est [Zapper](https://zapper.fi/es/exchange). Zapper est un optimisateur d'échange qui simulera votre échange (swap) sur plusieurs plateformes DEXes, et opèrera l'échange sur la plateforme offrant le meilleur taux de change.
{% endhint %}

## Consultez l'historique de vos transactions

Il est très important de savoir comment consulter l'historique de vos transactions. C'est un peu comme consulter un relevé de carte de crédit. Sur Polygon (et d'autres chaînes), vous pourrez utiliser [DeBank](https://debank.com). DeBank va utiliser l'adresse de votre portefeuille Metamask et lister toutes les transactions liées à cette adresse qui se trouvent sur la blockchain. DeBank propose d'autres fonctionnalités intéressantes, comme la présentation de vos différents investissements sur les applications les plus populaires. Vous pourrez aussi y consulter vos collections de NFT, comparer les applications etc ... DeBank est un outil très utile, et il vous permettra de vous assurer de l'état d'une transaction, comme la récupération de certains jetons envoyés directement dans votre portefeuille.

![Liste de toutes les transactions sur notre nouveau portefeuille](<../.gitbook/assets/image (27).png>)

{% hint style="danger" %}
Vous pouvez noter que notre portefeuille a reçu 800 000 DxDex.io sans que n'aillons fait quoi que ce soit. Veuillez faire très attention à ces tokens parachutés dans votre portefeuille, il s'agit pour la grande majorité d'arnaque vous dirigeant vers certains sites. Si vous faites une transaction sur ces sites, vous exposez l'intégralité du contenu de votre portefeuille. Vous pourrez utiliser DeBank pour bloque l'accès à ces applications. Le mieux reste de ne pas prêter attention à ces jetons.
{% endhint %}

## Autres liens utiles

Ci-dessous vous pourrez trouver d'autres applications utiles qui pourront vous aider dans votre navigation sur Polygon:

* [Mai Finance](https://app.mai.finance): La meilleure plateforme de prêt sur Polygon
* [QuickSwap](https://quickswap.exchange/#/swap): La plus grosse plateforme d'échange sur Polygon
* [AAVE](https://app.aave.com): La plus grosse plateforme de prêt/emprunt sur laquelle vous pourrez faire des gains
* [PolygonScan](https://polygonscan.com/gastracker/): Cette page vous permet de connaître le prix moyen d'une transaction sur Polygon

## Avertissement <a href="disclaimer" id="disclaimer"></a>

Ce guide, comme tous les autres sur ce site, ne propose pas de solution miracle est n'est pas à suivre de façon aveugle, il n'est écrit que dans un but éducatif en vue de vous faciliter vos premiers pas sur Polygon.

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
