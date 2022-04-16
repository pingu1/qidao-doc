---
description: >-
  Contracter un prêt n'est pas exactement contracter une dette lorsque vous utilisez ce prêt comme
  le point de départ d'une stratégie d'investissement. Il s'agit d'un véritable investissement.
---

# La Spooky Symphonie

## Introduction

Contracter un prêt contre vos actifs est toujours une arme à double tranchant : cela peut vous aider à lancer une stratégie d'investissement ou à tirer parti de vos actifs, mais vous aurez une dette que vous devrez rembourser à un moment donné. Dans ce guide, nous utiliserons un prêt contracté sur Market.XYZ, un protocole de prêt sur lequel vous pourrez emprunter des MAI avec un faible taux d'emprunt, et utiliserons ce prêt pour farmer la plupart des protocoles éprouvés sur Fantom. Nous utiliserons la stratégie de remboursement du prêt et verrons à quelle vitesse cela peut être fait afin de débloquer les actifs déposés en collateral.

{% hint style="info" %}
Ce guide n'est absolument pas un conseil financier, il a été réalisé dans un but éducatif. Vous devez faire attention aux variations de prix, à l'offre et à la demande, aux programmes de récompense, aux dates de fin, aux pertes impermanentes, etc... Le but n'était pas de proposer des recettes à suivre aveuglément, alors faites vos devoirs et votre propre simulation, et n'investissez que ce que vous êtes prêt à perdre éventuellement.

## Avertissement

Ce guide a été principalement conçu pour montrer comment vous pouvez rembourser une dette en utilisant les rendements agricoles. La vitesse à laquelle vous remboursez votre dette influence fortement le taux de récompense global, mais présente également des aspects très positifs, le principal étant la réduction du risque de liquidation.

Bien sûr, vous pouvez très facilement faire des économies avec cette stratégie, changer des éléments de la boucle pour d'autres, remplacer des protocoles par quelque chose que vous préférez etc ... Cependant, assurez-vous de lire toute la documentation disponible pour les protocoles que vous voulez utiliser, et assurez-vous de comprendre tous les différents risques.

{% hint style="info" %}
Ce guide n'est absolument pas un conseil financier, il a été réalisé dans un but éducatif. Vous devez faire attention aux variations de prix, à l'offre et à la demande, aux programmes de récompense, aux dates de fin, aux pertes impermanentes, etc ... Le but n'était pas de proposer des recettes à suivre aveuglément, alors faites vos devoirs et votre propre simulation, et n'investissez que ce que vous êtes prêt à perdre éventuellement.
{% endhint %}

{% endhint %}

![](<../../.gitbook/assets/spooky-symfony-1.png>)

## Fantom Protocols: Gotta use 'em all

In this strategy, we will use the a lot of different LP (**L**iquidity **P**roviding) pairs on a lot of different protocols, so we thought it would be a good idea to give you a brief recap of what each protocol is doing.

### Market.XYZ

[Market.XYZ](https://fantom.market.xyz/) est un protocole de prêt qui construit plusieurs coffres pour ses partenaires. Vous pourrez déposer des actifs uniques ou des tokens LP comme collateral, et emprunter d'autres actifs contre vos dépôts. Comme vous empruntez contre un collateral, il est important de s'assurer que vous ne serez pas liquidé. Une liquidation se produit lorsque la valeur de l'actif que vous avez déposé en collateral devient inférieure à la valeur de l'emprunt que vous avez contracté. C'est pourquoi il est important de veiller à ce que le rapport entre les deux valeurs reste relativement élevé, et que votre collateral ne perde pas trop de valeur lorsque le marché baisse.

Afin d'atténuer le risque de liquidation, nous utiliserons le token FTM-USDC LP comme collateral.

* La perte impermanente (IL) sur cette paire est relativement faible.
* L'USDC est un stable coin liée au dollar américain.
* FTM est le token de gaz natif de Fantom, il a une grande liquidité et est utilisé partout.
* Les taux de récompense sur la paire FTM-USDC sont élevés, ce qui signifie que même si le prix de FTM reste le même, la valeur de votre collateral augmentera.

Vous pourrez emprunter contre la paire FTM-USDC à partir du [Spooky LP pool] (<https://fantom.market.xyz/pool/10>) sur market.xyz. Les étapes pour déposer votre collatéral sont les suivantes :

* Créer [FTM-USDC LP tokens on SpookySwap] (<https://spookyswap.finance/add/FTM/0x04068DA6C83AFCFA0e13ba15A6696662335D5B75>) en fournissant des liquidités dans un rapport 1:1 pour les deux actifs.
* Déposez le token FTM-USDC LP sur Beefy finance pour obtenir un reçu mooBooFTM-USDC (recherchez la plateforme SpookySwap et l'actif USDC dans les filtres de recherche).
* Déposer le token de reçu mooBooFTM-USDC sur Market.xyz

![Marché de prêt de Spooky sur MarketXYZ à partir de février 2022](<../../.gitbook/assets/spooky-symfony-2.png>)

Lorsque vos tokens de reçu LP beefy sont sur Market.XYZ, vous obtenez toujours la récompense APY fournie par Beefy. Cela signifie que vos actifs continuent à générer des rendements pour vous pendant que vous empruntez . C'est un outil très puissant, surtout quand vous voyez que le mSPLP-FTM-USDC (**m**oo **S**pookyswa**p** FTM-USDC = mooBooFTM-USDC) rapporte 51,4% d'APY et que vous pouvez emprunter MAI à 2,56% APR. En d'autres termes, votre garantie croît plus vite que votre dette, donc en théorie vous pouvez très bien rembourser votre prêt avec les intérêts de votre garantie.

{% hint style="info" %}
Accessoirement, vous pouvez voir que le vault Spooky LP Pool offre également la possibilité d'emprunter contre d'autres tokens LP : ETH-FMT, DAI-FTM, BTC-FTM et fUSDT-FTM. En fonction des actifs que vous avez dans votre portefeuille, de vos convictions et de votre tolérance au risque, vous pouvez tout à fait utiliser n'importe quel LP de Spookyswap comme garantie.
{% endhint %}

Pour ce tutoriel, nous allons également limiter le risque en empruntant avec un CDR (**C**collatéral à **D**dette **R**atio) de 200%. Cela signifie que nous emprunterons 50 % de la valeur de notre garantie. Plus d'informations dans la section sur la stratégie agricole. Les ratios de liquidation sont exprimés en LTV (**L**oan **t**o **V**alue) qui est l'opposé d'un CDR. Vous pouvez voir que le LTV pour le token mooBooFTM-USDC est de 60%, au-delà duquel vous serez liquidé. Cela équivaut à un CDR de 166,67%. Avec un objectif de 200% de CDR, nous sommes 33% au-dessus du ratio de liquidation, ce qui peut être risqué ou non, en fonction de votre tolérance au risque.

{% hint style="danger" %}
Market.XYZ n'autorise que les prêts d'une valeur minimale de 0,05 ETH (~$170.00 au moment de la rédaction). Assurez-vous de déposer suffisamment de garanties si vous souhaitez emprunter dans les différents coffre.
{% endhint %}

### BeethovenX

[BeethovenX](https://beets.fi/#/) est une **D**ecentralized **Ex**change et **A**utomated **M**arket **M**aker fork de Balancer. Vous serez en mesure de déposer vos actifs dans des pools de liquidité, ainsi que d'échanger différents actifs sur leur application. Ils ont été de solides partenaires du protocole QiDAO, fournissant des tokens LP pour les positions de farming que vous pouvez trouver sur Mai Finance. Nous allons utiliser deux pools différents sur BeethovenX pour cette stratégie

* Le Monolithe : un pool inventif qui a été ouvert pour Exodia, un fork Ohm que [nous avons présenté dans ce tutorial] (investing-in-discounted-assets-using-bonds.md). Vous pourrez déposer vos tokens MAI directement dans ce pool et collecter des rendements
* Pirate Party : un pool incentivé dédié aux tokens LQDR, le token natif de Liquid Driver, un autre gros protocole que nous utiliserons dans ce guide

![Le pool Monolith sur BeethovenX avec 20% de MAI en février 2022](<../../.gitbook/assets/spooky-symfony-3.png>)

![Pool Pirate Party sur BeethovenX avec 80% de LQDR en février 2022](<../../.gitbook/assets/spooky-symfony-4.png>)

Comme toujours, le plus grand avantage d'utiliser BeethovenX (ou Balancer) est que vous pouvez déposer des actifs uniques dans les pools au lieu de devoir fournir des tokens dans un ratio équilibré.

### SpookySwap

[Spookyswap](https://spookyswap.finance/) est le plus grand fork Uniswap V2 sur Fantom, une plateforme où vous pourrez échanger des actifs et fournir de la liquidité pour de nombreuses paires. Spookyswap a également été un partenaire solide de Mai Finance et propose un pool MAI-USDC. Le partenariat s'est étendu via Market.XYZ où vous pourrez emprunter du MAI contre certaines paires LP spécifiques (voir la section sur Market.xyz) ainsi que vos tokens BOO et BOO staked, le token natif de Spookswap.

Pour ce guide, nous allons utiliser deux tokens LP différents de SpookySwap :

* FTM-USDC qui sera utilisé comme point de départ de la stratégie. Ce token LP est utilisé comme garantie sur market.xyz.
* FTM-BOO car c'est l'un des pools de SpookySwap accepté sur Liquid Driver avec le plus haut APR. Nous échangerons les récompenses BEETS du Monolithe contre cette paire (plus d'informations dans la section Stratégie).

### Liquid Driver

[Liquid Driver](https://www.liquiddriver.finance/) est un optimiseur de rendement sur lequel vous pourrez déposer des tokens LP de différentes fermes et gagner des rendements sur ceux-ci. Le fonctionnement de l'optimiseur de rendement consiste à récolter les tokens de récompense de la plateforme cible et à les composer pour vous. Ceci est utile car l'essence sur Fantom peut être chère. Une commission de performance est prélevée, mais une partie des revenus du protocole est redistribuée aux stakers LQDR. LQDR est le token natif de Liquid Driver.

Pour cette stratégie, nous utiliserons la paire de LP FTM-BOO car c'est un pool avec l'un des plus hauts APR en LQDR pour Spookyswap.

![Paires de LP FTM-BOO et FTM-USDC sur LiquidDriver en février 2022](<../../.gitbook/assets/spooky-symfony-5.png>)

## Stratégie d'exploitation

Pour cette stratégie, nous utiliserons Market.XYZ comme point de départ pour emprunter des MAI contre des tokens mooBooFTM-USDC LP. Les MAI empruntés seront déposés sur BeethovenX dans le pool The Monolith. Comme il s'agit du pool avec le taux de récompense le plus élevé dans notre stratégie, nous l'utiliserons comme moteur pour rembourser notre dette : 50% des BEETS seront vendus pour rembourser la dette sur Market.xyz, et 50% seront convertis en tokens FTM-BOO LP. Les tokens FTM-BOO seront déposés sur LiquidDriver pour collecter des tokens LQDR qui seront ensuite mis en jeu dans le pool Pirate Party sur BeethovenX. Une fois la dette entièrement remboursée, les récompenses BEETS seront entièrement converties en tokens FTM-BOO. Les récompenses BEETS fournies par le pool du Parti Pirate seront également composées en plus de FTM-BOO.

Pour cette simulation, nous allons utiliser les chiffres suivants

* Nous commençons avec une valeur de 1000 $ de tokens mooBooFTM-USDC.
* L'APR pour le token mooBooFTM-USDC fourni par SpookySwap via Beefy est de 41,5%.
* Le taux d'emprunt pour MAI est de 2,56%.
* BeethovenX donne un taux d'intérêt annuel de 304,17 % pour le Monolithe et de 175,77 % pour le Parti Pirate.
* LiquidDriver donne un APR de 82% pour la paire de LP FTM-BOO.

Comme d'habitude pour nos simulations, nous supposons que tous les prix restent les mêmes pendant toute la période d'un an, que les taux restent les mêmes, et nous utilisons également les APR fournis tels quels. En réalité, les prix et les taux varieront, et les APR sont composés de frais de transaction et de tokens de récompense, ce qui peut affecter le résultat final. Il est également important de noter que **aucun frais de transaction** n'est pris en compte pour cette simulation. Enfin, nous utilisons un grand nombre de protocoles, et chaque protocole peut présenter des risques liés aux contrats intelligents. Assurez-vous de faire vos propres recherches avant d'utiliser une plateforme, et n'investissez que ce que vous êtes prêt à perdre.

Vous pouvez trouver notre simulation Spooky Symfony [dans cette feuille de calcul] (<https://docs.google.com/spreadsheets/d/19s6kBnT5w0b9GKuTkDiiD1u_ZoeNUZtI9XYxEmk_WM0/edit?usp=sharing>). N'hésitez pas à la copier et à jouer avec elle pour voir comment la boucle fonctionne, et comment les différents taux peuvent affecter votre APY final.

![](<../../.gitbook/assets/spooky-symfony-6.png>)

### Jour 1

Le jour 1, vous devez créer votre collatéral pour Market.xyz.
 Obtenez une portion égale de FTM et d'USDC et fournissez la liquidité sur SpookySwap pour créer des tokens FTM-USDC LP.
 Ces tokens seront déposés sur Beefy, ce qui vous permettra d'obtenir la preuve de dépôt mooBooFTM-USDC.
 C'est ce token qui sera utilisé comme garantie sur Market.xyz et contre lequel vous emprunterez le MAI. Comme nous voulons garder un CDR de 200%, nous emprunterons 500$ de MAI. Enfin, les tokens MAI seront placés sur BeethovenX dans le pool The Monolith.

A la fin du premier jour, vous aurez

|     positon    |  value ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,000.000 |
| the monolith   |    500.000 |
| pirate party   |      0.000 |
| BEETS rewards  |      4.167 |
| FTM-BOO        |      0.000 |
| LQDR rewards   |      0.000 |
| MAI debt       |    500.000 |

### Day 2

Le deuxième jour, vous devrez

* vendre 50 % de vos BEETS contre des MAI pour rembourser une petite fraction de votre prêt
* échanger vos récompenses BEETS contre une paire de LP FTM-BOO. Vous pouvez soit échanger sur BeethovenX et créer la paire de LP sur SpookySwap, soit tout faire sur SpookySwap.
* Les LP FTM-BOO sont mis en jeu sur Liquid Driver pour commencer à collecter des token LQDR.

A la fin du deuxième jour, vous aurez

|     positon    |  value ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,001.137 |
| the monolith   |    500.000 |
| pirate party   |      0.000 |
| BEETS rewards  |      4.167 |
| FTM-BOO        |      2.083 |
| LQDR rewards   |      0.005 |
| MAI debt       |    497.952 |

### Day 3

Répétez l'opération du Jour 2, puis récoltez vos premiers tokens LQDR. Ceux-ci seront déposés sur BeethovenX dans le pool de la Pirate Party pour obtenir des récompenses BEETS supplémentaires, et à la fin du Jour 3 vous aurez

|     positon    |  value ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,002.275 |
| the monolith   |    500.000 |
| pirate party   |      0.005 |
| BEETS rewards  |      4.167 |
| FTM-BOO        |      4.167 |
| LQDR rewards   |      0.000 |
| MAI debt       |    495.903 |

{% hint style="info" %}
les gains de pirate party sont trop petit pour être notable à ce point, il faudra être patient pour les voir grandir de façon notable
{% endhint %}

### Routine quotidienne

À ce stade, le système est complètement amorcé. Votre routine quotidienne consistera à

* Récolter les récompenses BEETS du Monolithe.
* Récolter les BEETS du Parti Pirate.
* échanger 50 % des BEETS contre des MAI si vous avez encore une dette à rembourser
* rembourser une partie de ta dette si tu en as encore une
* Échangez le reste des BEETS contre des tokens LP FTM-BOO.
* déposer les FTM-BOO sur LiquidDriver
* récolter les LQDR
* déposer dans le Parti Pirate

Cette stratégie n'est pas très économe en gaz, vous pouvez donc envisager de ne composer vos gains qu'une fois par semaine, ou même moins fréquemment.

### Résultats bruts mois après mois

Voici les résultats bruts mois après mois, tels que vous pouvez les obtenir dans la feuille de calcul Google liée ci-dessus.

| day |  FTM-USDC  | The Monolith | Pirate Party |  FTM-BOO  | MAI debt |
|-----|------------|--------------|--------------|-----------|----------|
|  30 |  1,033.503 |      500.000 |        1.901 |    60.500 |  440.541 |
|  60 |  1,069.343 |      500.000 |        8.031 |   123.652 |  378.905 |
|  90 |  1,106.425 |      500.000 |       18.452 |   187.988 |  317.139 |
| 120 |  1,144.794 |      500.000 |       33.265 |   254.136 |  255.242 |
| 150 |  1,184.493 |      500.000 |       52.612 |   322.738 |  193.216 |
| 180 |  1,225.569 |      500.000 |       76.681 |   394.462 |  131.058 |
| 210 |  1,268.069 |      500.000 |      105.704 |   470.006 |   68.770 |
| 240 |  1,312.043 |      500.000 |      139.963 |   550.105 |    6.351 |
| 270 |  1,357.542 |      500.000 |      181.427 |   691.752 |    0.000 |
| 300 |  1,404.619 |      500.000 |      233.046 |   846.443 |    0.000 |
| 330 |  1,453.328 |      500.000 |      295.350 | 1,009.331 |    0.000 |
| 360 |  1,503.726 |      500.000 |      368.942 | 1,182.000 |    0.000 |

### 365 jours

A la fin d'une année complète d'exploitation de ce système, vous aurez

* 1 512,294 $ de jetons FTM-USDC sur Market.xyz.
* 500 000 $ de MAI dans le pool de The Monolith.
* 382,353 $ de LQDR stockés dans le pool du Parti Pirate.
* 1 211 845 $ de jetons FTM-BOO sur Market.xyz.
* une dette finale qui sera entièrement remboursée après le jour #243.

Cela équivaut à un rendement annuel total de 260,65%.

### Effet du remboursement de la dette sur le résultat global

Dans la plupart de nos guides, nous ne remboursons aucune dette dans le cadre de la stratégie. Cela est dû, dans la plupart des cas, au fait que nous utilisons un prêt à 0% d'intérêt contracté sur Mai Finance. Ici, nous empruntons sur Market.XYZ avec un taux d'emprunt de 2,56% et nous remboursons la dette avec 50% des BEETS récoltées au Monolithe.

Si vous allouez plus de 50% au remboursement de la dette, vous paierez moins d'intérêts, mais vous ferez croître vos positions beaucoup plus lentement sur Liquid Driver. Si vous allouez moins de 50% au remboursement de la dette, vous obtiendrez plus de récompenses des autres plateformes, mais vous paierez aussi plus d'intérêts sur Market.xyz.

Voici un petit tableau qui indique l'effet des BEETS alloués à votre remboursement de dette sur votre APY global :

| BEETS % | Overall APY | debt repaid after |
|---------|-------------|-------------------|
|     100 |      242.85 |          122 days |
|      90 |      245.06 |          135 days |
|      80 |      247.75 |          152 days |
|      70 |      251.05 |          174 days |
|      60 |      255.23 |          203 days |
|      50 |      260.65 |          244 days |
|      40 |      267.92 |          305 days |
|    33.5 |      274.09 |          364 days |

Si vous utilisez moins de 33,5 % de vos récompenses BEETS pour rembourser votre dette, vous aurez encore des MAI à rembourser après une année complète.

Il est également bon de comprendre que si vous remboursez plus rapidement, vous augmentez également votre CDR de manière plus significative, ce qui vous permet de vous éloigner plus rapidement du ratio de liquidation.

## Variations à considérer

Cette stratégie présente de nombreuses variantes qui présentent des avantages différents.

### Mai Finance VS Market.xyz

Vous pouvez totalement emprunter MAI à [Mai Finance] (<https://app.mai.finance>) à 0% d'intérêt. Par exemple, si vous utilisez mooScreamFTM au lieu de mooBooFTM-USDC comme garantie, cela présente les avantages suivants :

* Vous n'avez pas de pertes impermanentes sur votre collatéral.
* Vous empruntez à 0% avec une seule commission de remboursement de 0,5%, ce qui sera dans la plupart des cas, bien inférieur aux intérêts que vous paierez sur Market.xyz (s'il y a des MAI à emprunter pour ce coffre)
* Vous pouvez obtenir des récompenses en Qi pour emprunter sur la plateforme, ce qui vous permettra de participer à la gouvernance du protocole, ainsi que d'obtenir des dividendes si vous mettez en jeu vos jetons Qi. Cela augmentera vos gains annuels
* Vous êtes protégé des taux d'emprunt très fluctuants sur Market.xyz. Mai Finance prêtera régulièrement de nouveaux MAI pour maintenir les taux d'emprunt aussi bas que possible, mais ce n'est pas une garantie qu'ils n'augmenteront pas. Vous pouvez vérifier les métriques du marché des prêts [ici] (<https://metrics.market.xyz/d/HChNahwGk/fuse-pool-details?orgId=1&refresh=10s&var-poolID=10&var-chain=250>).

Cependant, les tokens mooScreamFTM ont un taux annuel beaucoup plus bas que les tokens mooBooFTM-USDC, donc vous pouvez ne pas en profiter.

### Misez sur votre LQDR

Si vous mettez en jeu vos LQDR au lieu de les utiliser dans le pool de la Pirate Party, vous gagnerez des dividendes de Liquid Driver qui sont payés en différents actifs (LQDR, WFTM, LINSPIRIT, BOO, SPELL et BEETS). Vous obtiendrez également des xLQDR qui vous permettront de participer à la gouvernance de Liquid Driver, et éventuellement LINSPIRIT pour voter sur l'allocation des récompenses sur Spirit Swap. Veuillez consulter attentivement la page [xLQDR](https://www.liquiddriver.finance/xlqdr) pour plus de détails.

### Misez sur vos BEETS

Si les BEETS du Monolithe jouent un rôle important dans cette stratégie, vous pouvez tout à fait utiliser ceux du Parti Pirate comme suit :

* Déposez les BEETS dans le pool Fidelio Duetto (BEETS-FTM).
* miser le jeton LP sur BeethovenX pour recevoir des fBEETS
* mettez en jeu vos fBEETS pour obtenir des dividendes protocolaires.

Cela vous permettra également de voter sur les améliorations du protocole BeethovenX, ainsi que sur l'allocation des récompenses pour les différents pools de la plateforme. Ceci est particulièrement utile pour garder un APR élevé sur le Monolithe.

### Utiliser le pool FTM-BEETS sur Spookyswap

Dans notre stratégie, nous vendons toutes les récompenses BEETS du Monolithe. Cependant, vous pouvez également intégrer le pool FTM-BEETS de Spookyswap dans votre boucle. Vous devriez vendre 50% de vos BEETS pour FTM et combiner les deux jetons dans une nouvelle paire de LP qui vous rapportera des BOO. Vous pouvez alors décider de créer le FTM-BOO et de le déposer sur Liquid Driver, ou vous pouvez miser vos BOO sur SpookySwap. Notez que si vous mettez en jeu votre BOO, vous aurez la possibilité de déposer les jetons de réception xBOO et de gagner directement des jetons LQDR, et vous pouvez même utiliser les jetons xBOO comme garantie sur Market.xyz. Cette brique de lego supplémentaire ouvre de nombreuses possibilités.

{% hint style="info" %}
Gardez un œil sur cette paire particulière au cas où elle deviendrait disponible sur Liquid Driver. C'est peut-être une meilleure option que celle de FMT-BOO.
{% endhint %}

### Utilisez votre FTM-USDC sur Liquid Driver

Une fois votre prêt entièrement remboursé, vous pouvez conserver les jetons mooBooFTM-USDC sur Market.xyz ou sur Beefy, ils continueront à accumuler des récompenses. Cependant, vous pouvez également retirer la paire de LP de Beefy et la déposer sur Liquid Driver pour obtenir plus de LQDR.

Par ailleurs, pendant que vous remboursez votre prêt, la valeur de votre rapport garantie/dette augmente (la garantie accumule les récompenses et prend de la valeur tandis que la dette diminue après chaque remboursement partiel). Cela signifie que vous pouvez retirer les garanties morceaux par morceaux afin de garder un CDR sûr, et les déposer sur Liquid Driver pour plus de jetons LQDR.

### Gardez une petite fuite de bénéfices

Ce système est une boucle fermée qui s'auto-alimente. Cependant, vous pouvez très bien continuer à vendre des parties de vos BEETS pour d'autres actifs après avoir fini de rembourser votre prêt sur Market.xyz. A titre d'exemple, vous pouvez convertir vos récompenses BEETS en USDC ou une autre stable, ou augmenter une de vos positions qui rapporte plus de récompenses que celles accordées pour la paire FTM-USDC.
