---
description: >-
  Cet article présente une explication détaillée de la façon dont vous pourrez
  utiliser Mai Finance pour emprunter à 0% tout en étant payé pour le faire, ce
  qui transforme votre emprunt à 0% en un empru
---

# Les emprunts de MAI et leurs récompenses

## Introduction

Le coeur de métier de Mai Finance est d'être une plateforme de prêts. Au lieu de vendre vos crypto monnaies pour en acheter d'autres, il vous suffit simplement de les déposer dans un coffre sur Mai Finance et emprunter de la monnaie stable. Ceci présente l'opportunité de conserver vos actifs de valeur (WBTC, WETH ...) tout en étant capable d'utiliser d'autres actifs et d'obtenir des gains de liquidité. Dans ce cas particulier, c'est l'emprunt qui génère du revenu et l'actif utilisé comme collatéral gagne de la valeur.

Un des autres gros avantages de Mai Finance est qu'il n'y a pas d'échéance de remboursement. En d'autres termes, vous empruntez des MAI en fonction de votre dépôt de crypto, vous ne payez pas d'intérêts, et vous avez la possibilité de rembourser uniquement lorsque vous le souhaitez. Veuillez vous référer aux articles liés aux [remboursement de vos dettes](debt-repayment-why-and-when.md) pour plus de détails. Les seuls frais que vous aurez à payer sont des frais fixes de 0,5% du montant de votre emprunt, et ils vous seront prélevés uniquement au moment du remboursement de votre dette et payés avec une partie de votre collatéral.

Par exemple, si vous déposez l'équivalent de 200$ de WETH et empruntez pour 100$ de MAI, lorsque vous rembourserez votre dette, vous devrez payer 0,50$ qui seront prélevés de votre dépôt de WETH.

Si cette opportunité n'était déjà pas suffisament avantageuse, l'équipe de Mai Finance a introduit en septembre 2021 des récompenses d'emprunts payées en Qi, le jeton natif de Mai Finance. En d'autres termes, vous serez payés en fonction du montant de votre emprunt sur Mai Finance. Cet article présente en détails le fonctionnement de css récompenses.

## Les coffres - Que sont-ils et comment fonctionnent-ils

### Création d'un coffre

Sur Mai Finance, les coffres sont des contenants spécifiques ou un utilisateur va pouvoir déposer un certain type d'actif. Il y a pour le moment 10 types de coffres disponibles sur Polygon:

![Les différents types de coffre disponibles à la création sur Mai Finance](<../.gitbook/assets/image (1).png>)

Il existe 2 types de coffres:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

et

* camWETH
* camWBTC
* camWMATIC
* camAAVE

Les 6 premiers coffres de la liste sont reéservés à des actifs simples alors que les 4 derniers sont pour les "camTokens". Les camTokens sont des jetons qui vont composer les récompenses offertes par AAVE, et sont des représentations de votre dépôt sur AAVE. Alors que vos actifs génèrent des intérêts sur AAVE (et que ces intérêts sont composés pour augmenter ces actifs), vous pouvez tout de même emprunter des MAI en utilisant les camTokens comme collatéral.

Il est bon de noter que dans la capture d'écran ci-dessus, la page de création de coffre contient quelques informations très importantes:

* MAI available: c'est ce qui correspond aux MAI qui sont disponibles comparativement au plafond de sécurité d'emprunt, ou le nombre maximum de MAI qu'il reste à emprunter pour ce type de coffre.
* Min. Coll. ratio: c'est le seuil de liquidation, ou la valeur minumal que le ratio entre la valeur de votre collatéral et la valeur de votre dette peut avoir
* Vault incentives APR: les intérêts que rapporteront votre emprunt

### Comprendre le plafonnement des emprunts

Le nombre maximum de MAI qu'un utilisateur pourra emprunter pour un coffre donné dépend principalement de la valeur des actifs déposés dans ce coffre. Le plafonnement de la dette est mis en place pour prévenir la situation dans laquelle le marché serait innondé d'une très grosse quantité de MAI dans un laps de temps très court, ce qui aurait un impact négatif sur son prix.

Par exemple, si une très grosse institution dépose 5 000 WBTC d'un coup et emprunte l'équivalent de 100 000 000$ de MAI, échanger la totalité des MAI pour acheter plus de WBTC pourrait tirer le prix du MAI vers le bas à tel point que l'ancrage au dollar US serait mis en question, et mettrait toute la plateforme en danger. Le plafonnement des emprunts est le mécanisme qui permet justement à cette situation de ne jamais être rencontrée: il y a un maximum de MAI empruntable à la fois qui correspond plus ou moins à ce que le marché est capable d'absorber dans impacter le prix du MAI.

Lorsque le plafond de la dette est atteint, ou pour faire simple, le moment ou il ne reste plus de MAI à créer, la date est enregistrée dans le système et le plafond est augmenté automatiquement après 48h. C'est le temps jugé suffisant pour que le prix du MAI se soit stabilisé (en cas d'une très grosse vente de MAI).

Ceci veut dire que pendant 48h, personne ne pourra emprunter des MAI supplémentaires pour un type de coffre donné, à mois que quelqu'un ne repaye partiellement ou entièrement sa dette.

Veuillez noter que plus il y a de MAI sur le marché, plus le MAI devient stable. En effet, une vente massive de MAI a moins d'impact s'il y a plus de MAI en circulation.

* Si quelqu'un vend 1 000 MAI alors qu'il y a seulement 10 000 MAI en circulation, la vente correspond à 10% du volume et peut avoir un impact important
* Si quelqu'un vend 1 000 MAI alors qu'il y a 10 000 000 MAI en cricluation, la vente correspond à 0.01% du volume et aura moins d'impact

Ainsi, le plafond n'est pas augmenté de façon incrémentale, mais exponentielle: plus il y a de MAI sur le marché, moins l'impact est important, et donc le plafond peut être augmenter de façon beaucoup plus importante.

{% hint style="info" %}
Quand vous empruntez des MAI, il se peut que le montant maximum de MAI que vous souhaitiez emprunter soit limité par le plafond d'emprunt global, quelque soit la valeur courrante de votre collatéral ou le montant de votre dette. Lorsque c'est le cas, il suffit simplement d'attendre jusqu'à 48h pour que le plafond soit revu à la hausse.
{% endhint %}

### Comprendre la ratio Collatéral / Dette

Le CDR, ou **C**ollateral to **D**ebt **R**atio est le ratio entre la valeur des actifs déposés qui vous servent de collatéral dans votre coffre, et la valeur de votre dette correspondant aux MAI que vous avez empruntés.

Par exemple, si vous déposez l'équivalent de 200$ d'ETH et que vous empruntez 100$ de MAI, votre CDR sera de

$$
CDR=\frac{ValeurDeCollatéral}{ValeurDeDette}=\frac{200}{100}=200\%
$$

Maintenir un CDR au dessus de 100% vous permet d'avoir à tout moment plus de collatéral que de dette. C'est un point essentiel pour assurer que la valeur de la monnaie stable MAI ne s'effondre pas. On parle de monnaie stable sur-collatéralisée, et c'est l'un des fondements du MAI. Vous pourrez retrouver plus de détails dans la [documentation officielle de Mai Finance](https://docs.mai.finance/stablecoin-economics).

Chaque type de coffre accepte un CDR minimum (aussi appelé seuil de liquidation). Il s'agit du taux en dessous duquel votre coffre est considéré comme étant à risque puisque le montant emprunté ne sera plus assuré par suffisament de collatéral. A partir de là, n'importe quel utilisateur pourra liquider votre coffre, c'est-à-dire rembourser une partie de votre dette et prendre en compensation une partie de votre collatéral. Une fois encore, vous trouverez toutes les informations importantes dans la documentation officielle.

Lorsque vous empruntez des MAI à partir d'actifs en collatéral, vous aurez également quelques informations relatives au montant maximal de MAI que vous pourrez emprunter, ainsi que l'impact qu'aura votre emprunt sur votre CDR comme vous pouvez le voir sur la capture d'écran ci-dessous:

![Mitigation du risque en fonction du montant emprunté](<../.gitbook/assets/image (2).png>)

C'est très important de garder un oeil sur votre CDR et de conserver un ratio sain afin de

* prévenir les évènements de liquidation
* accroître la santé de l'intégralité de la plateforme Mai Finance en assurant que le volume de MAI en circulation reste correctement assurée par assez d'actifs

Un "CDR" sain, si on se base sur la définition proposée par l'équipe derrière la plateforme Mai Finance, se trouve entre 25% et 270% au dessus du seuil de liquidation. A noter que vous pouvez également vous reporter à nos autre tutoriels pour comprendre comment un [CDR aggrésif/conservateur](../tutoriels/polygon/tirez-parti-aave-tokens.md#exemples-chiffres) peut impacter votre stratégie d'investissement, ou comment [repayer votre dette](debt-repayment-how.md) en fonction de votre CDR.

## Les récompenses d'emprunt

### Comprendre les intérêts sur les récompenses d'emprunt

En septembre 2021, Mai Finance a introduit les récompenses d'emprunt. Il s'agit d'intérêts alloués par la plateforme Mai Finance aux utilisateurs qui empruntent des MAI et participent ainsi à la croissance du projet.

Chaque type de coffre (parmi les 10 coffres différents) reçoivent chacun 0,05 Qi par bloc, qui sont ensuite redistribués à chaque utilisateur ayant un CDR sain. Le rendement du coffre est basé sur le montant emprunté.

Par exemple, Ben et Kila sont 2 amis ayant déposé leurs ETH dans le coffre WETH sur Mai Finance.

* Ben a déposé l'équivalent de 2 000$ d'Ehtereum et a emprunté 1 000 MAI.
* Kila a déposé l'équivalent de 10 000$ d'ETH et a emprunté 6 000MAI.

Le montant actuel de MAI empruntés par tous les utilisateurs de coffre WETH s'élève a 1 000 000MAI.

Ben et Kila sont tous les deux qualifiés pour recevoir des intérêts sur leur dette puisque Ben a un CDR de 200% et Kila un CDR de 166.67%. Ben, avec son emprunt, possède 0.1% du montant total emprunté, et Kila en possède 0.6%.

Le montant total de Qi alloué pour l'intégralité des coffres WETH (ou n'importe quel type de coffre) est de

$$
Qi=0,05*\frac{86 400}{2}=2 160
$$

{% hint style="info" %}
86 400 est le nombre de secondes dans une journée, et sur Polygon, il y a un nouveau bloc toutes les 2 secondes, ce qui veut dire que le nombre théorique de blocs quotidien est de 86 400 / 2 = 43 200. D'ouù une émission de 2 160 Qi / jour.

**Note:** Le temps séparant chaque bloc a augmenté, et est d'environ 2,6 secondes. Cependant, tous les APRs (**A**nnual **P**ercentage **R**evenue) affichés sur Polygon partent du principe de 2 secondes par bloc. Veuillez faire vos propres recherches à ce sujet, et vérifier le [temps moyen sur Polygonscan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Ainsi, si l'état des coffres WETH se maintient, Ben recevra 0,1% des 2 160 Qi distribués quotidiennement, et Kila en recevra 0,6%.

* Ben recevra 2,16 Qi chaque jour, ce qui représente 0,216% de son emprunt, ou un APR de 78,84%
* Kila recevra 12,96 Qi chaque jour, ce qui représente 0,216% de sa dette, ou un APR de 78,84%

A noter que 2 160 Qi pour 1 000 000 MAI correspond à un rendement de 0,216% quotidien, ou 78,84% total, ce que recevra chaque utilisateur ayant emprunté.

{% hint style="info" %}
Il est facile de se rendre compte que le rendement d'un coffre est directement impacté par le volume total de MAI emprunté. Plus il y aura de MAI empruntés et plus l'APR va diminuer. Il est bon de noter que le volume de dette est également limité par le plafond de la dette globale.
{% endhint %}

Dans le but de vérifier nos calculs, il est possible d'obtenir la valeur théorique de l'APR pour le coffre MATIC en fonction des chiffres publiés sur [la page d'analytics](https://app.mai.finance/analytics) de Mai Finance. Le montant total de MAI empruntés pour le coffre MATIC s'élève à 799 328. La récompense étant de 2 160 Qi par jour nous donne un APR de

$$
APR=\frac{RecompenseQi*Qi_{prix}}{MAI_{empruntés}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

Ceci correspond plus ou moins à l'APR affiché pour un coffre MATIC, comme le confirme la capture d'écran ci-dessous:

![APR d'un coffre MATIC sur Mai Finance après le lancement des récompenses d'emprunts](<../.gitbook/assets/image (23) (2) (3).png>)

### Calcul des rendements de départ de chaque coffre

Avec le même exemple que ci-dessus, il est possible de calculer chaque rendement de coffre en fonction du volume total emprunté

| Type de coffre | APR initial |
| -------------- | ----------- |
| MATIC          | 44.29%      |
| WETH           | 24.03%      |
| LINK           | 27.41%      |
| AAVE           | 164.14%     |
| CRV            | 159.96%     |
| WBTC           | 36.92%      |
| camWETH        | 25.46%      |
| camWMATIC      | 44.33%      |
| camAAVE        | 167.23%     |
| camWBTC        | 47.38%      |

{% hint style="info" %}
Comme vous pouvez le constater, certains coffres vont générer beaucoup plus de rendement que d'autres. Vous remarquerez également qu'il est très important de déposer vos actifs le plus tôt possible afin de bénéficier d'intérêts élevés avant que le plafond d'emprunt ne soit augmenté et que plus de dette ne soit contractée (diminuant ainsi le rendement).

Vous pouvez enfin voir que si vous conservez votre emprunt pour une année complète, les frais de remboursement de 0.5% seront largement compensés par le programme de récompenses.
{% endhint %}

### Distribution des intérêts

Les récompenses allouées à chaque type de coffre seront distribuées de la même façon que celles données aux utilisateurs ayant bloqués leurs Qi sur la plateforme (staking). Chaque mercredi, les Qi alloués aux coffres seront envoyés directement dans le portefeuille des détenteurs de dette pour la période correspondant à la semaine précédant la distribution.

## FAQ sur les récompenses d'emprunts

Si vous souhaitez en apprendre plus sur la façon dont les récompenses d'emprunts fonctionnent, voici la FAQ officielle présente sur le serveur Discord.

* **Quels coffres reçoivent des récompenses?**

Pour le moment, tous les types de coffre reçoivent des récompenses sous forme de Qi

* **À combien s'élèvent les récompenses d'emprunt?**

0,05 Qi/bloc pour chaque type de coffre

* **Combien de MAI dois-je emprunter afin de me qualifier pour les récompenses?**

Pour les récompenses d'emprunt, il suffit de conserver un CRD compris entre 25% et 270% au dessus du seuil de liquidation pour recevoir les récompenses en Qi. Cela correspon à:

* _MATIC_: - seuil de liquidation de 150% - CDR qualifiés entre 175% et 450%
* _Tokens_: - seuil de liquidation de 130% - CDR qualifiés entre 155% et 400%
* _CamTokens_: - seuil de liquidation de 135% - CDR qualifiés entre 160% et 405%
* **Comment puis-je savoir si mon coffre se qualifie?**

Si vous voyez une petite emoji flamme sur votre coffre dans la page listant vos coffres, c'est qu'il se qualifie pour les récompenses.

* **Combien vais-je gagner?**

Votre pourcentage de récompenses correspond au ratio entre le montant de votre dette en MAI et le montant total de la dette pour le type de coffre.

* **Combien de temps vont durer les récompenses d'emprunt?**

Pour le moment, la planification des récompenses d'emprunts est pour une durée de 3 mois. La DAO peut voter d'arrêter ces récompenses avant la fin des 3 mois, ou voter pour une extension à la fin de la période.

* **Comment allons-nous recevoir les récompenses?**

Les Qi seront distribués directement dans les portefeuilles des détenteurs de dette éligible.

* **Comment est-ce que l'éligibilité est prise en compte?**

L'éligibilité d'un coffre est calculée à chaque bloc. Vous recevrez des récompenses pour chaque bloc pendant lequel votre niveau de dette est éligible au long de la semaine.

* **Quand est-ce que la période d'éligibilité démarre-t-elle?**

Le même calendrier que les récompenses de staking sera respecté. Vous pouvez vous baser sur les numéros de blocs affichés sur la page de boost.

## Avertissement

Ce guide a été écrite **avant** que les récompenses d'emprunts ne soient démarrées, ce qui veut dire que certains des APRs affichés dans ce document (ainsi que le document au complet) peut être sujet à des modifications, et pourraient ne pas être justes. Le montant de MAI empruntés, le plafond de dette globale et la valeur du jeton Qi impactera grandement le rendement final pour chaque coffre. Veuillez s'il vous plaît investir de façon responsable.

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
