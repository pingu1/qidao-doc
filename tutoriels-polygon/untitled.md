---
description: >-
  Cet article présente comment combiner la culture de revenus avec les
  récomponses d'emprunt de Mai Finance pour augmenter vos intérêts.
---

# Comment combiner les récompenses de fermes et d'emprunts

## Intro

En septembre 2021, Mai Finance a ajouté des récompenses à ses coffres pour promouvoir les emprunts, augmentant ainsi le nombre de MAI crée via les coffres. Ce qui veut dire que, en plus d'avoir un prêt à 0% d'intérêt, avec un petit frais de remboursement, vous êtes payé pour emprunter du MAI. Cet article propose une stratégie basée sur la culture de jetons stables avec [Augury Finance](https://augury.finance) comme source de jetons que l'on peut utiliser pour nourrir nos coffres sur Mai Finance, profitant ainsi des incitations à l'emprunt, et du MAI additionel qui sera réinjecté dans la ferme.

![](<../.gitbook/assets/image (7).png>)

## Présentation des applications et réserves

### Augury Finance

Augury Finance est un aggrégateur de revenus qui ne se concentre pas sur l'auto-capitalisation de vos jetons LP (**L**iquidity **P**rovider). À la place, Augury vend les jetons de la ferme et s'en sert pour acheter d'autres tokens dans leurs _Infusions._

Par exemple, vous pouvez cultiver la paire DFYN/WETH sur Augury.

![Exemple de la réserve DFYN-WETH sur Augury Finance](<../.gitbook/assets/image (32).png>)

Cette infusion se sert de DinoSwap comme ferme sous-jacente et un jeton LP, obtenable sur DFYN. Avec une APR de 123,43%, les utilisateurs qui déposent de la liquidité dans cette réserve seront récompensés avec:

* 30% de WETH
* 20% de LINK
* 20% de WBTC
* 15% d'USDT
* 15% de WMATIC

Si vous cultivez sur DinoSwap, vous seriez payés en jetons DINO, dont le prix est très volatile. Sur d'autres aggrégateur, comme Adamant ouBeefy, vos positions (en LP) augmenteraient avec, mais avec Augury vous "sécurisez" vos positions en recevant des jetons qui sont des valeurs sûres. L'inconvénient est que vos positions ne grandissent pas avec le temps puisque tous les DINOs récoltés sont échangés pour le set de jetons composant les récompenses d'Augury.

{% hint style="info" %}
Augury finance utilise 3 tiers differents d'Infusion qui ont est frais de dépôt et performance différents. Renseignez vous sur les tiers et soyez certains de comprendre leurs impacts sur votre stratégie pour choisir celui qui vous convient.
{% endhint %}

Dans cette stratégie, nous utiliserons l'infusion: USDT/UST Tier 2 qui récompense ses utilisateurs avec un mix de WETH/WBTC/LINK/WMATIC/USDC, parce que Mai Finance propose des coffres pour 4 des 5 jetons du set. Pour maximiser nos profits, nous ajoutons une étape entre Augury et Mai: Aave, car 3 des 5 jetons ont un coffre qui accepte la version d'Aave (camWETH/camWBTC/camWMATIC).

![Stable coin farming USDT-UST for our strategy](<../.gitbook/assets/image (31).png>)

### Curve

Curve est une valeur sûre, en terme de projet, qui récompenses les utilisateurs qui fournissent des jetons qui sont des valeurs sûres. Les récompenses sont composées de jetons auto-réinvestis (ajouter à votre investissement), jetons WMATIC et de jetons CRV, les derniers étant des collatéraux acceptés sur Mai Finance.

Un aspect très intéressant de Curve et ses réserves est qu'un utilisateur n'a pas besoin d'équilibrer les jetons déposés dans les réserves. Il est possible de déposer seulement 1 jeton de la réserve et l'algorithme qui gère la ferme va automatiquement ajuster les autres jetons (en vendant/achetant) pour maintenir un ratio correcte.

Nous utiliserons la réserve "atricrypto3" qui accepte du WBTC/WETH/USDC/USDT/DAI et nous y ajouterons l'USDC généré sur Augury.

![Détails de la réserve atricrypto3 sur Curve, en September 2021](<../.gitbook/assets/image (30).png>)

### AAVE

Aave est une autre valeur sûre, en terme de projet, et, comme mentionné dans le paragraphe sur Augury, est utilisé pour ajouter une petite APR (<5%) sur les récompenses d'Augury. Au lieu de mettre directement les WBTC, WETH & WMATIC dans un coffre de Mai Finance, nous allons déposé ces jetons sur Aave puis dans la page "[/yield](https://app.mai.finance/yield)" de Mai Finance, pour auto-réinvestir les récompenses d'Aave et faire grandir notre position, et pour finir, dans un coffre. Vous pouvez trouver plus de détails sur cette partie [ici](tirez-parti-aave-tokens.md).

![Récompenses d'AAVE sur les prêts, en septembre 2021](<../.gitbook/assets/image (29).png>)

{% hint style="info" %}
À la mi-septembre 2021,[ Aave a voté pour ajouter CRV, BAL & LINK à leur marché](https://snapshot.org/#/aave.eth/proposal/QmUjs75wxvsv4q4urC5DXZSgh8mAWK99SsRPXNu3zeuuYa). Une fois implémentés, Mai Finance pourra les utiliser pour créer des coffres camCRV, camBAL & camLINK.
{% endhint %}

### Balancer

Balancer est, encore une fois, une valeur sûre, comme Curve & Aave. Comme sur Curve, vous pouvez déposer des jetons dans les réserves sans vous souciez du ratio, la réserve s'équilibre automatiquement.

Pour notre stratégie, nous utiliserons la réserve WETH/BAL/Qi/MAI/USDC. Cette réserve accepte le Qi, que nous gagnerons via la dette de nos coffres sur Mai Finance, et nous récompenses avec plus de Qi et du BAL, que nous deposerons dans un coffre sur Mai Finance, pour pouvoir emprunter plus de MAI et augmenter notre position sur Augury.

![Balancer 5-pool as of September 2021](<../.gitbook/assets/image (23).png>)

## Préparer le système

![](<../.gitbook/assets/image (19).png>)

Ce qui suit est une simulation faite avec un investissement initial de $1000 d'ETH, qui est déposé dans un coffre camWETH et sur lequel on emprunte $500 de MAI, que l'on échange pour $500 de paire USDT/UST LP. Cette simulation est faite avec les APR suivantes:

* USDT/UST sur Augury: 22,53%
* camWBTC sur Mai: 0,39%
* camWETH sur Mai: 1,71%
* camWMATIC sur Mai: 3,80%
* atricrypto3 sur Curve:
  * 3,86% sur les jetons auto-réinvestis
  * 13,09% de WMATIC
  * 17,63% de CRV
* 5-jetons réserve sur Balancer: 43,46% avec un ratio BAL/Qi de 1 pour 6.
* Dette sur les coffre de Mai:
  * 23,28% pour camWBTC
  * 21,52% pour camWETH
  * 32,93% pour camWMATIC
  * 24,51% pour LINK
  * 116,71% pour CRV
  * 62,38% pour BAL

Toutes ces APRs vont varier avec le temps, et il n'y a aucune garantie qu'elles continuent pendant 1 an. Nous les utiliserons tout de même afin de se faire une idée de l'APR possible du système. Pour garder la simulation simple, nous ne tiendrons pas non plus compte ni de la variations des prix, ni des frais de transaction. Par ailleurs, veuillez noter que cette simulation considère que nous réinvestissons les récompenses de Mai Finance & Balancer quotidiennement plutôt que chaque semaine; ces récompenses sont envoyées chaque semaine par les protocoles directement dans le portefeuille des utilisateur. Finalement, nous partons du principe que le ratio collatéral/dette des coffres est toujours à 200%, ce qui signifie que nous empruntons seulement la moitié de ce que l'on a déposé, pour éviter d'être liquidé.

### Jour 1

Si vous avez toujours vos $1000 de WETH, déposez les dans Aave pour obtenir des amWETH, puis déposez ces derniers dans Mai Finance pour obtenir des camWETH, et finalement, déposez les dans un coffre camWETH et empruntez 500 MAI.

Vous pouvez utiliser l'Anchor de Mai pour échanger votre MAI pour de l'USDT (ou n'importe quel autre DEX, comme QuickSwap, si l'Anchor n'a plus d'USDT). Pour obtenir de l'UST vous pouvez aller sur DFYN, ou 1inch. Pour obtenir la paire USDT/UST LP, déposez vos USDT et UST dans la réserve de DFYN. Finalement, déposez vos paires USDT/UST LP sur Augury. Notez que vous aurez besoin d'un peu d'OMEN, vous pouvez en obtenir sur QuickSwap et 1inch aussi.

À la fin du premier jour, nous récoltons les récompenses suivantes:

| Récompenses                     | Valeur en dollars |
| ------------------------------- | ----------------- |
| WBTC via Augury                 | 0.123             |
| WETH via Augury                 | 0.031             |
| WMATIC via Augury               | 0.031             |
| LINK via Augury                 | 0.031             |
| USDC via Augury                 | 0.092             |
| Qi via la dette de notre coffre | 0.295             |

### Day 2

Une fois les récompenses récoltées:

* Déposez les WBTC, WETH & WMATIC sur Aave puis sur la page "yield" de Mai, puis dans les coffres correspondants
* Déposez les LINK directement dans un coffre Mai correspondant
* Déposez les USDC dans la réserve atricrypto3 de Curve.
* Déposez les Qi dans la réserve de Balancer (encore une fois, ce n'est pas une action faisable chaque jour)
* Empruntez du MAI depuis nos coffres, en gardant un ratio collatéral/dette à 200%: $0,13 MAI pour être précis.
* Créez plus de USDT/UST LP et déposez les dans Augury.

À la fin du premier jour, nous récoltons les récompenses suivantes:

| Récompenses                    | Valeur en dollars |
| ------------------------------ | ----------------- |
| WBTC via Augury                | 0.123             |
| WETH via Augury                | 0.031             |
| WMATIC via Augury + Curve      | 0.031             |
| LINK via Augury                | 0.031             |
| USDC via Augury                | 0.093             |
| CRV via Curve                  | 0.00004           |
| BAL via Balancer               | 0.00005           |
| Qi via la dette de nos coffres | 0.296             |

À partir de là, le système est prêt et les récompenses s'alimentent toutes entre elles, créant ainsi une petit boucle fort appréciable.

## Résultats

### Routine quotidienne

Elle est composée des transactions suivantes

* Récolter sur Augury
* Déposer les WBTC, WETH et WMATIC sur AAVE
* Déposer les amWBTC, amWETH et amWMATIC sur Mai Finance via la page "/yield"
* Déposer les camWBTC, camWETH et camWMATIC dans leurs coffres sur Mai Finance
* Déposer les LINK dans le coffre sur Mai Finance
* Déposer les USDC dans la réserve atricrypto3 sur Curve
* Récolter les WMATIC de Curve et les utiliser dans le coffre camWMATIC
* Récolter les CRV de Curve et les déposer dans le coffre
* Emprunter du MAI dans les différents coffres, jusqu'à 200% de ratio collat/dette
* Échanger les MAI contre de l'USDT et de l'UST
* Créer de nouvelles paires USDT/UST LP sur DFYN
* Déposer les nouveaux jetons LP sur Augury

### Routine par semaine

Chaque semaine, vous receverez, directement dans votre portefeuille, du BAL (via le Qi déposé sur Balancer) et du Qi (via le Qi déposé sur Balancer et la dette de vos coffres). Vous deverez:

* Déposer le Qi sur Balancer
* Déposer le BAL dans un coffre sur Mai Finance
* Emprunter du MAI, l'échanger pour former des pairs USDT/UST et les déposer sur Augury

### Résultats mois après mois

| Mois | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| ---- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1    | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2    | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3    | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4    | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5    | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6    | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7    | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8    | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9    | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10   | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11   | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12   | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

Quelques notes:

* La position USDT/UST grandit uniquement grace aux MAI empruntés depuis les coffres
* La réserve CRV est presque inexistante à cause du faible montant d'USDC déposés sur Curve
* Le coffre BAL n'est pas très important car 14,28% des récompenses de Balancer sont payées en BAL, le reste est en Qi.
* Le montant dans la réserve Balancer est le plus gros gain et n'est que le résultat des récompenses sur notre dette et de Balancer.

### Jour 365

Après une année complète, notre investissement serait le suivant:

| Position    | Valeur en dollars |
| ----------- | ----------------- |
| USDT-UST    | 553.24            |
| atricrypto3 | 36.20             |
| Balancer    | 137.62            |
| camWBTC     | 47.45             |
| camWETH     | 1,029.19          |
| camWMATIC   | 14.39             |
| LINK        | 11.84             |
| CRV         | 0.017             |
| BAL         | 3.93              |

La position USDT/UST est entièrement construite sur notre dette, qui vaut donc $553,24 et la valeur totale des récompenses générées est $280,63, cela nous donne une APY de 28,06%.

### Comparaison avec d'autres stratégies

Une APY de 28% en cultivant des jetons stables n'est pas mauvais, mais regardons d'autres stratégies, plus simples, que nous pourrions appliquer à nos $1000 d'ETH:

* Appliquer un effet de levier 8 fois sur de l'amWETH via AAVE: pour cela, nous suivons cet [article](tirez-parti-aave-tokens.md).
* Seulement cultiver de la stable sur Augury: pour cela, nous vendons notre WETH et cultivons avec  $1,000 de USDT-UST sur la même infusion d'Augury.
* Seulement cultiver de la stable sur QuickSwap: pour cela, nous utilisons le coffre camWETH pour bénéficier des récompenses, puis nous cultivons avec $500 de MAI sur QuickSwap (MAI/DAI avec une APY de 19,78%), et nous mettons le dQUICK récolté dans un coffre (55,72% APR) et on emprunte contre pour réinvestir dans la ferme de QuickSwap.

| Stratégie                                 | APY finale |
| ----------------------------------------- | ---------- |
| Stratégie présentée dans cet article      | 28.06%     |
| Levier x8 via Aave                        | 46.46%     |
| Seulement la culture de stable sur Augury | 22.53%     |
| culture sur Quickswap + coffre dQUICK     | 35.96%     |

## Avertissements

Cette stratégie est très intéressante et utilise la plupart des coffres de Mai Finance, et cet article a été écrit pour démontrer que, en septembre 2021, les coffres sont la partie qui génère le plus de récompense en cultivant de la stable. Cependant, cette stratégie n'est peut-être pas la plus intéressante et fait intervenir beaucoup de manipulations entre plusieurs plateformes. Finalement, Augury est une plateforme fantastique qui génère des jetons spécifiques qui peuvent être inclus dans plusieurs stratégies et probablement pas que pour la culture de stable. Une dernière remarque: aucun frais de dépôt et/ou de performances ont été pris en compte pour calculer l'APY finale.

{% hint style="info" %}
Gardez à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut moins bien fonctionner, voir vous faire perdre de l'argent, à un autre. Restez informé, surveillez les marchés et vos investissements, et, encore une fois, **faites vos recherches**.
{% endhint %}
