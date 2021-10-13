---
description: >-
  Cette page présente le moyen de tirer le meilleur parti de vos crypto en
  utilisant Mai Finance et AAVE sans investir d'argent supplémentaire, grâce aux
  prêts à taux 0%.
---

# Appliquez un effet de levier sur vos tokens AAVE

## Quand un dessin vaut mille mots

![](<../.gitbook/assets/Screen Shot 2021-08-07 at 10.29.50 AM.png>)

## Mais une bonne explication est parfois nécessaire

L'idée derrière ce schéma est de présenter comment utiliser Mai Finance afin d'accroître vos investissements et vos rendements.

Pour cela, nous partirons d'un exemple dans lequel vous aimez vraiment la crypto MATIC, et vous pensez qu'elle a un fort potentiel de croissance. MATIC pourrait très prochainement atteindre 2$, 5$ ou même 10$. Et peut-être que vous avez raison sur ce point. Cependant, étant un petit investisseur, vous n'avez que l'équivalent de 100$ de MATIC dans votre portefeuille sur Polygon. Nous allons voir comment vous allez pouvoir générer plus de MATIC à partir de vos tokens. HODL c'est bien, investir c'est mieux.

### Utiliser AAVE pour augmenter son capital

[AAVE](https://app.aave.com) est une plateforme sur laquelle vous allez pouvoir prêter et emprunter vos MATIC (parmi d'autres tokens). En prêtant vos cryptos sur AAVE, vous allez accumuler des gains. Par exemple, actuellement vos MATIC vont pouvoir vous rapporter 1.2% de rendement annuel (**A**nnual **P**ercentage **Y**ield, ou gain annuel en pourcentage). Il se peut que AAVE ait un partenariat avec un autre système qui vous rapportera également des récompenses supplémentaires. Pour le moment, Polygon offre 3.69% de rendement annuel supplémentaire sous forme de MATIC.

Tant que vos MATIC sont dans le pot commun sur AAVE, les intérêts s'accumulent automatiquement, ce qui veut dire que votre montant de MATIC grossit avec le temps.

![Sur cet exemple, j'ai déposé 0.2 MATIC sur AAVE](<../.gitbook/assets/Screen Shot 2021-08-06 at 5.29.53 PM.png>)

En déposant vos tokens MATIC sur AAVE, vous recevez en échange un montant équivalent en amWMATIC (aave market wrapped MATIC). Il se peut que vous ne les trouviez pas dans votre portefeuille, mais vous les possédez bien.

![I can see the 0.20 MATIC I lended on DeBank](<../.gitbook/assets/Screen Shot 2021-08-06 at 5.31.01 PM.png>)

### Utiliser Mai Finance pour accroître ses tokens AAVE

Mai Finance accepte vos tokens amWMATIC sur leur page de yield. En déposant vos amWMATIC sur Mai Finance, vos fonds sont "transférés" depuis AAVE vers Mai Finance. Vous pourrez remarquer que le rendement proposé sur Mai Finance est pratiquement le même que celui proposé sur AAVE.

La différence est que Mai Finance va combiner les gains générés par le pot commun sur AAVE avec les récompenses potentielles offertes par les programmes auxiliaires (pour un pool ETH, les MATIC offerts par Polygon sont échangés en ETH et rajoutés au pot commun). Dans notre exemple ci-dessus, AAVE offre 1.16% de rendement sur les MATIC, ainsi que 3.69% supplémentaires en récompenses payées sous forme de MATIC. Cependant, sur AAVE les récompenses ne génèrent pas de profit. En déposant vos amWMATIC sur Mai Finance, les récompenses sont récoltées régulièrement et remises dans le pot commun afin de leur appliquer le taux d'intérêt de 1.16%.

![Mes 0.2 MATIC sont maintenant déposés sur Mai Finance et vont me rapporter 4.93% par an](<../.gitbook/assets/Screen Shot 2021-08-06 at 5.45.00 PM.png>)

Lorsque vous déposez vos amWMATIC sur Mai Finance, vous recevrez en échange des tokens camWMATIC. Leur valeur n'est pas exactement à ratio 1:1 car les camWMATIC représentent une part du pot commun de amWMATIC sur Mai Finance, dans lequel les intérêts et les récompenses sont accrus. Vous noterez également que lorsque vos amWMATIC sont déposés sur Mai Finance, ils sont automatiquement retirés de AAVE. Cependant, si vous retirez vos camWMATIC de la page de yield sur Mai Finance, vous pourrez retrouver vos MATIC sur AAVE.

{% hint style="info" %}
Simplement en déposant vos amWMATIC (ou n'importe quel amToken) sur Mai Finance, vous allez générer plus de revenu que si vous aviez simplement déposé vos MATIC sur AAVE. En effet, comme les intérêts de base sont ré-appliqués aux récompenses collectées régulièrement, le taux d'intérêt composite est plus élevé.
{% endhint %}

### amTokens VS camToken

Beaucoup de personnes ont du mal à comprendre la différence entre les amTokens et les camTokens. Les amTokens sont une représentation de votre dépôt sur AAVE. Leur nombre est exactement indexé sur le montant de Tokens que vous avez déposé. De leur côté, les camTokens représentent une part du pot de amTokens sur Mai Finance.

Partant du principe que lors de la création du pot de amToken sur Mai Finance il y avait 1 000 amTokens, dont 100 vous appartenant. Puisque le pot vient juste d'être créé, le ratio entre les amTokens et les camTokens est de 1:1, et vous possédez 10% du pot. Après un an, en assumant que personne n'a ajouté ni retiré de amTokens du pot, les intérêts de 4.93% générés font que le pot contient maintenant 1 049.3 amTokens. Cependant, votre part n'a pas changé, vous avez toujours 10% du pot représenté par 100 camTokens. Le ratio est maintenant de 1:1.0493, ou autrement dit, chaque camToken vaut 1.0493 amToken.

### Emprunter des MAI (stable coin)

Mai Finance vous permet d'emprunter le stable coin MAI lorsque vous déposez des fonds en tant que collatéral. Et l'un des avantages principaux est que les tokens camWMATIC (et autres camTokens) peuvent être utilisés comme collatéral. Sur Mai Finance, vos camWMATIC vont continuer à générer des intérêts tout en vous servant de collatéral, ce qui se traduit simplement par un CDR (**C**ollateral to **D**ebt **R**atio en anglais, ou Ratio Dette/Collatéral) croissant. Et plus vous conserverez longtemps votre emprunts, plus facilement vous pourrez rembourser les 0.5% de frais de remboursements chargés par la plateforme.

{% hint style="info" %}
Lorsque vous déposez vos camWMATIC dans votre coffre de collatéral, la valeur de ces tokens sur la page de yield tombe à 0. Cependant, cela ne veut pas dire qu'ils ne continuent pas à accroître des intérêts.
{% endhint %}

Lorsque vous ouvrez la page des coffres (Vaults) et sélectionnez le coffre de camWMATIC, vous avez alors la possibilité d'y déposer vos tokens (il faudra commencer par créer un coffre si vous n'en avez pas déjà un). Gardez à l'esprit que vous aurez à conserver un ratio Dépôt/Emprunt d'au moins 155% lorsque vous allez emprunter contre vos camWMATIC.

![Mes 0.2 MATIC sont maintenant utilisés comme collatéral](<../.gitbook/assets/Screen Shot 2021-08-06 at 5.57.55 PM.png>)

**Note: **sur cette page, vous pourrez voir la valeur de votre dépôt en Dollars US, et sa valeur peut fluctuer en fonction du type de collatéral, de la valeur sous-jacente du token utilisé, et des bénéfices réalisés par le pot commun de camWMATIC.

**Bon plan:** Lorsque je dépose des tokens pour emprunter des MAI, j'essaye toujours de n'emprunter que 50% de ce que je dépose. Dans l'idéal, j'essaye de rester au dessus de 200% de CDR. Si ma valeur de collatéral augmente (le token ne perd pas de valeur, et les intérêts s'accumulent), cette stratégie reste très peu risquée. Si jamais j'ajoute plus de collatéral à un coffre existant, je ne retire jamais plus que 50% de ce que je dépose, et n'essaye pas de redescendre le plus proche possible de 200% de CDR. Je peux par contre emprunter moins si lors de mon dépôt le CDR est passé en dessous de 200%.

{% hint style="info" %}
Il est de votre responsabilité de vous rendre sur la page des coffres et de vérifier que votre niveau de liquidation reste toujours aux alentours de votre objectif, et d'augmenter la valeur de votre collatéral au besoin.
{% endhint %}

![J'ai maintenant 0.10$ de MAI pour un CDR de 214.56%](<../.gitbook/assets/Screen Shot 2021-08-06 at 6.07.34 PM.png>)

Il est maintenant tant d'utiliser notre emprunt.

### Acheter plus de MATIC

Je peux maintenant me rendre sur mon DEX préféré (QuickSwap ou SushiSwap sont d'excellents exemples) et échanger mes MAI contre de nouveaux MATIC.

![](<../.gitbook/assets/Screen Shot 2021-08-06 at 6.10.35 PM.png>)

Après l'échange, j'ai des MATIC en plus dans mon portefeuille.

### Répéter la boucle

Initialement, j'avais 0.20 MATIC dans mon portefeuille. Ils sont pour le moment déposé sur Mai Finance et génèrent 4.93% d'intérêt par an. J'ai également en ma possession 0.09MATIC. Je peux maintenant me rendre sur AAVE pour les y déposer, et reprendre la procédure depuis le début.

### À quel moment arrêter la boucle?

Pour ce qui est des étapes, il est plus avantageux de s'arrêter après le dépôt de vos camWMATIC dans le coffre à collatéral. En effet, en faisant ceci vous augmentez votre ratio collatéral/dette, ce qui réduit un tout petit peu le risque de se faire liquider. En fonction du dernier montant déposé, il se peut que cette augmentation soit négligeable.

En ce qui concerne le nombre d'itérations, j'arrête en général lorsqu'une boucle supplémentaire n'augmenterait mon capital investi que de moins de 1%, soit dans notre cas présent, 0.002 camWMATIC. Dans notre exemple, les montants sont par ailleurs tellement faible que le prix des transactions influe également sur le moment où je vais sortir de la boucle.

## Exemples chiffrés

Les exemples qui suivent sont basés sur un investissement initial de 1 000$ de MATIC, avec différent CDR cibles afin d'illustrer comment l'effet de levier peut être appliqué grâce à Mai Finance.

### 200% Ratio Collatéral / Dette

| Nombre d'itération | investissement |    dette | revenu estimé | APY équivalent |
| :----------------: | -------------: | -------: | ------------: | -------------: |
|          1         |      1 000,00$ |  500,00$ |        49,30$ |         4,930% |
|          2         |      1 500,00$ |  750,00$ |        73,95$ |         7,395% |
|          3         |      1 750,00$ | 875,00$  |        86,75$ |         8,628% |
|          4         |      1 875,00$ |  937,50$ |        92,44$ |         9,244% |
|          5         |      1 937,50$ |  968,75$ |        95,52$ |         9,552% |
|          6         |      1 968,75$ |  984,38$ |        97,06$ |         9,706% |
|          7         |      1 984,38$ |  992,19$ |        97,83$ |         9,783% |
|          8         |      1 992,19$ |        - |        98,21$ |         9,821% |

Après la 7ème boucle, ajouter plus de dette ne permettrait pas d'augmenter mon investissement de plus que 10$ (1% de mon investissement initial), et c'est donc le moment de sortir de la boucle. L'augmentation de mon pourcentage de revenu annuel ne changerait pas de façon significative de toutes façons. Et dans cet exemple, je conserve un CDR relativement raisonnable de 200,79%.

Il est facile de se rendre compte qu'utiliser AAVE en combinaison avec Mai Finance permet de pratiquement doubler mon profit, tout en bénéficiant des fluctuations de valeur de ma crypto.

### 175% Ratio Collatéral / Dette

| Nombre d'itération | investissement |     dette | revenu estimé | APY équivalent |
| :----------------: | -------------: | --------: | ------------: | -------------: |
|          1         |      1 000,00$ |   571,43$ |        49,30$ |         4,930% |
|          2         |      1 571,43$ |   897,96$ |        77,47$ |         7,747% |
|          3         |      1 897,96$ | 1 084,55$ |        93,57$ |         9,357% |
|          4         |      2 084,55$ | 1 191,17$ |       102,77$ |        10,277% |
|          5         |      2 191,17$ | 1 252,10$ |       108,02$ |        10,802% |
|          6         |      2 252,10$ | 1 286,91$ |       111,03$ |        11,103% |
|          7         |      2 286,91$ | 1 306,81$ |       112,74$ |        11,274% |
|          8         |      2 306,81$ | 1 318,18$ |       113,73$ |        11,373% |
|          9         |      2 318,18$ | 1 324,67$ |       114,29$ |        11,429% |
|         10         |      2 324,67$ |         - |       114,61$ |        11,461% |

Cette fois-ci, passé la 9ème itération il n'est plus intéressant de continuer, je peux donc arrêter la boucle et avoir un CDR final de quasiment 175,49%.

Ici, avec une approche un peu plus agressive, le revenu annuel moyen est également un peu plus intéressant, comme à chaque fois lorsqu'on s'expose à plus de risques.

### Plus de chiffres

Si vous êtes intéressé par les mathématiques derrière la théorie, vous pouvez calculer votre investissement final en fonction de votre investissement initial et du taux de CDR que vous vous fixez. La formule est la suivante:

$$
InvestissementFinal = InvestissementInitial *\sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

Dans cette formule, _n_ représente le nombre de boucles que vous souhaitez opérer, et _CDR_ est le ratio collatéral/dette que vous vous fixez, en pourcentage.

Dans notre exemple précédant, avec un CDR cible de 200% et 7 boucles, on obtient

$$
InvestissementFinal = 1000 *\sum_{i=0}^{7}{\frac{100}{200}}^i
$$

$$
InvestissementFinal = 1000 * (\frac{1}{2}^0 + \frac{1}{2}^1 + \frac{1}{2}^2 + \frac{1}{2}^3 + \frac{1}{2}^4 + \frac{1}{2}^5 + \frac{1}{2}^6 + \frac{1}{2}^7)
$$

$$
InvestissementFinal = 1000 * (1 + 0.5 + 0.25 + 0.125 + 0.0625 + 0.03125 + 0.015625 + 0.0078125)
$$

$$
InvestissementFinal = 1000 * 1.9921875 = 1992.1875
$$

Avec la même méthode, il est facile d'obtenir la formule permettant de calculer le rendement annuel final après plusieurs boucles:

$$
APY equivalent = APY initial * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

Et ici encore, avec notre CDR cible de 200%, un rendement initial de 4.93% et 7 boucles, nous obtenons un APY équivalent final à

$$
APY equivalent = 4.93 * 1.9921875 = 9.821484375
$$

##  Avertissement <a href="disclaimer" id="disclaimer"></a>

Tout ce qui est présenté dans ce tutoriel assume que

* Les rendements proposés par AAVE restent les même sur une année (ce qui n'est pas exactement vrai)
* Le programme offert par Polygon reste le même sur une année (ce qui est faux)
* Le prix du MATIC reste relativement stable sur une année (ce qui n'est clairement pas le cas)

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
