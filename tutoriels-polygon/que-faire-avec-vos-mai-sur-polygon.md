---
description: >-
  Ce tutoriel présente les différentes options qui vous laisseront utiliser vos
  MAI fraîchement générés sur le réseau Polygon.
---

# Que faire avec vos MAI sur Polygon

## But de ce tutoriel

Le but de ce tutoriel n'est pas de présenter en détails ce que vous pourrez faire avec vos MAI, mais d'avoir une liste de sites et d'applications DeFi (**De**centralized **Fi**nance, ou Finance Décentralisée) sur lesquels vous pourrez utiliser vos MAI directement, ou en combinaison avec une autre monnaie stable. Pour plus de détails spécifiques sur les façons d'utiliser la monnaie stable MAI, vous pouvez vous référer aux autres tutoriels de ce site, ou venir chercher de l'aide sur Discord ou Telegram.

Veuillez noter que la liste n'est pas complète, et ne le sera certainement jamais, puisque de nouvelles applications sont lancées chaque semaine sur le réseau. Je ne peux pas les tester toutes, donc je vais présenter les applications principales, ou tout du moins les plus connues / les moins risquées.

Si vous souhaitez qu'un projet en particulier soit listé dans ce tutoriel, venez en discuter en rejoignant la communauté Qi sur [Discord](https://discord.gg/mQq55j65xJ).

{% hint style="info" %}
Veuillez prendre en compte que je ne présenterai pas Mai Finance comme ferme à rendement. Ce sujet nécessite son propre article, car le token Qi est bien plus qu'un token de ferme ne servant qu'à être revendu pour accroître vos position dans d'autres cryptos.
{% endhint %}

## Cultivez en toute sécurité sur des projets de premier plan

Les projets de premier plan sont des application DeFi qui ont prouvé leur solidité sur le long terme, et présentent relativement peu de risques. Ils ont pour la plupart fait l'objet de plusieurs audits, et les équipes supportant ces projets le font déjà depuis plusieurs années. S'ils ne proposent pas des rendements importants, au moins vous pouvez leur faire confiance.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) est une plateforme de gestion de portefeuille automatisée, ainsi qu'un fournisseur de liquidité. Sur cette plateforme, vous pourrez déposer votre crypto-monnaie et collecter des frais de change sur les transactions permettant de re-balancer les portefeuilles en suivant les meilleures opportunités du marché.

Balancer est présent sur le réseau Ethereum, ainsi que sur Polygon où vous pourrez par exemple déposer vos fonds dans la réserve de liquidité composée des 4 monnaies stables: DAI, USDC, USDT et MAI (miMATIC). Cette réserve propose pour le moment un rendement relativement stable (**A**nnual **P**ercentage **R**ate, ou Taux de pourcentage annuel) de \~20%.

![Etat de la réserve de liquidité "stable" en août 2021](../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)

Il est bon de noter que sur Balancer, vous n'avez pas besoin de fournir les 4 monnaies stables pour pouvoir rejoindre la réserve de liquidité (Liquidity Pool). Balancer va générer un dépôt balancé composé de la meilleure combinaison à partir du dépôt que vous ferez. En d'autres termes, si vous possédez l'équivalent de 100$ de MAI, vous pouvez simplement les déposer sur Balancer et laisser l'algorithme décomposer ce dépôt correctement pour qu'il y ait 25% de chaque monnaie stable, et ce en fonction de leur prix réel au moment du dépôt. Par exemple, vos 10 MAI seront décomposés en 2.31 USDC, 2.18 DAI, 3.29 MAI et 2.22 USDT, qui pourrait correspondre à la meilleure balance au moment du dépôt.

Les récompenses des réserves sur Balancer sont payées avec le token BAL et sont distribuées une fois par semaine. En plus des récompenses BAL, des récompenses spécifiques à chaque réserve sont également distribuées. Vous pouvez voir les différents [programmes de récompenses ici](https://balancer-incentives.web.app). Dans le cas qui nous intéresse. en participant à la reserve stable, nous recevront également des récompenses sous forme de MATIC et de Qi.

Le flot complet pourrait ressembler au suivant:

![](../.gitbook/assets/screen-shot-2021-08-12-at-11.10.40-am.png)

Si vous avez besoin de plus de détails sur la façon d'utiliser Mai Finance pour déposer vos crypto-monnaies et emprunter des MAI (au lieu de vendre vos cryptos pour acheter des MAI), veuillez vous référer aux autres guides sur ce site. Afin de maximiser vos gains, vous pouvez également [inclure AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/fr-tutorials/tirez-parti-aave-tokens) dans votre stratégie.

### Curve Finance

[Curve](https://polygon.curve.fi) est une autre plateforme réputée sur laquelle vous pourrez déposer vos crypto-monnaies dans une réserve de liquidité et récupérer des intérêts. Les programme intéressants sont:

* La réserve AAVE qui génère entre 5% et 15% d'intérêts par an (l'APR varie en fonction des programmes de récompense) sur un trio de monnaies stables (DAI/USDC/USDT). La réserve fonctionne exactement comme celle de Balancer dans le sens où vous pouvez déposer une seule crypto que le protocole déposera ensuite sur AAVE.
* La réserve atricrypto, composée des trois monnaies stables ainsi que de wBTC et wETH. Cette réserve propose un APR qui varie entre 25% et 30%. L'équipe de Mai Finance travaille actuellement avec les équipes de Curve afin d'intégrer la monnaie stable MAI dans leur réserve, ce qui permettrait aux détenteurs de MAI de faire un dépôt direct plutôt que de passer par un swap (échange) pour du USDC.

En attendant que l'application accepte la monnaie stable MAI dans leurs réserves, il est toujours possible d'utiliser vos cryptos en utilisant Mai Finance et Curve en suivant ces étapes (exemple avec du MATIC)

* Déposez vos MATIC sur AAVE et collectez des amWMATIC
* Déposez vos amWMATIC sur Mai Finance et collectez des camWMATIC (les récompenses de AAVE s'appliquent directement sur les tokens camWMATIC)
* Utilisez vos camWMATIC comme collatéral afin d'emprunter des MAI
* Utilisez la [page de swap](https://app.mai.finance/anchor) sur Mai Finance afin d'échanger vos MAI contre des USDC
* Ensuite, vous pouvez au choix
  * Utiliser la réserve atricrypto sur Curve et déposer vos USDC pour gagner 25% a 30% par an
  * Utiliser la réserve AAVE sur Curve en y déposant vos USDC et gagner entre 5% et 15% par an

Les récompenses sur Curve sont distribuées de la façon suivante:

* Une partie est ré-injectée dans la réserve, augmentant votre capital investi (auto-compounding)
* Une partie est distribuée en WMATIC que vous pouvez utiliser pour recommencer la boucle décrite ci-dessus et augmenter votre investissement dans Curve sans revendre vos gains
* Une partie est distribuée en CRV (monnaie propre à Curve). Ces tokens peuvent également être utilisés comme collatéral sur Mai Finance pour emprunter des MAI et augmenter vos investissements

![](../.gitbook/assets/screen-shot-2021-08-12-at-11.41.07-am.png)

### AAVE

Il existe un guide complet sur la façon d'utiliser vos MAI afin d'[optimiser vos crypto sur AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/fr-tutorials/tirez-parti-aave-tokens). Cette option n'utilise pas la monnaie stable MAI directement. Il se pourrait que AAVE accepte MAI et propose une réserve stable dédiée où vous pourrez déposer vos MAI.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) est probablement une des plateformes d'échange les plus connues sur Polygon (aussi nommées DEX pour **D**ecentralized **EX**change), avec SushiSwap. C'est également un AMM (**A**utomated **M**arket **M**aker) qui permet d'échanger des cryptos efficacement sur le réseau par le biais de réserves de liquidité. Chaque échange sur le site est sujet à des frais qui sont partiellement redistribués aux utilisateurs qui déposent leurs cryptos sur la plateforme.

La façon d'utiliser votre monnaie stable MAI sur QuickSwap est très similaire à de la récolte sur une ferme à rendement. Si vous avez besoin de détails sur la façon exacte de procéder et de mettre à disposition des tokens LP (**L**iquidity **P**rovider tokens) sur QuickSwap, un guide entier est dédié au sujet (en anglais seulement pour le moment).

Actuellement, si vous rejoignez la réserve MAI/USDC sur QuickSwap, vous pourrez gagner

* des frais de transactions
* des tokens QUICK (natifs à QuickSwap)

![Détails de la réserve MAI/USDC sur QuickSwap en Août 2021](../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

## Fermes dégénérées et Agrégateurs

### Adamant

[Adamant](https://adamant.finance/home) est un agrégateur qui liste toutes les "meilleures" fermes sur Polygon et vous permet de vous positionner dans leurs réserves de liquidité directement depuis Adamant. En déposant vos LP tokens sur une réserve spécifique sur Adamant, les algorithmes vont récolter les intérêts générés de façon automatique et les composer directement pour vous afin d'augmenter le montant de vos tokens de liquidité. En réalité, seulement une partie des récompenses moissonnées est rajoutée à votre position, le reste est converti en WMATIC qui seront ensuite redistribués aux utilisateurs ayant des tokens ADDY (natifs à Adamant) bloqués sur le site. Enfin, vous recevrez une récompense sous forme de tokens ADDY (bloqués pendant 90 jours suite à leur collecte) qui vous permettront de prétendre aux dividendes sous forme de WMATIC.

De manière générale, Adamant est une plateforme intéressante pour les utilisateurs qui ne soucient pas des tokens générés par les fermes de rendement, ou ceux qui ne souhaitent pas avoir à composer les intérêts manuellement chaque jour (ou plusieurs fois par jour). Adamant génère également plus de revenus que les fermes qu'ils exploitent puisque vous obtenez en plus des récompenses en ADDY et WMATIC.

Actuellement (Août 2021), Adamant supporte quelques réserves acceptant les LP tokens MAI/USDC. Ces réserves sont celles de

* QuickSwap (voir paragraphe ci-dessus): les QUICK sont convertis en MAI/USDC et WMATIC
* DinoSwap: les Dinos sont convertis en MAI/USDC et WMATIC
* Mai Finance: les Qi sont convertis en MAI/USDC et WMATIC

![Réserve MAI/USDC de QuickSwap accessible sur Adamant](../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)

{% hint style="info" %}
Les captures d'écran ci-dessus présentant les rendements sur QuickSwap et sur Adamant ont été prises le même jour afin d'illustrer la différence d'APY (**A**nnual **P**ercentage **Y**ield, ou pourcentage d'intérêts composés) entre les 2 plateformes.
{% endhint %}

Il est facile de voir que le rendement sur Adamant est un peu plus élevé que sur QuickSwap. La composition des intérêts sur Adamant est la suivante

* 12.88% des QUICK sont composés (revendus pour fabriquer de nouveaux LP tokens)
* 9.16% sont alloués sous la forme de tokens ADDY (non composés)
* 3.40% sont alloués sous forme de dividendes en WMATIC (si vous récoltez vos ADDY quotidiennement)

Cela veut dire qu'à partir des 20.92% de rendement de QuickSwap, seulement 12.88% vous sont redistribués directement afin d'accroître le nombre de vos LP tokens, et le reste est converti en WMATIC. Vous aurez la possibilité de récolter les récompenses en ADDY quotidiennement (où dès qu'elles sont récoltables) et les bloquer afin de prétendre aux dividendes. En d'autres termes, Adamant _semble_ être une solution plus intéressante grâce à des rendements plus importants et des intérêts directement composés, mais afin de maximiser vos positions, la plateforme nécessite aussi beaucoup d'opérations manuelles.

{% hint style="info" %}
L'utilisation d'Adamant a également un fort impact the le prix des tokens natifs des fermes exploitées. En effet, puisque les tokens sont revendus régulièrement quelque soit leur prix, Adamant inonde le marché avec ces tokens de ferme, diminuant ainsi leur prix.
{% endhint %}

### Autres fermes à rendement acceptant la paire MAI/USDC

La monnaie stable MAI gagnant de la popularité sur Polygon, principalement grâce à son intégration par les grandes plateformes comme QuickSwap, de plus en plus de fermes à rendement proposent la paire MAI/USDC comme moyen de générer du rendement. La liste suivante est non exhaustive et présente les fermes les plus réputées:

* DinoSwap
* Augury
* Polypup
* ...

Il existe de nombreuses autres fermes. Si vous souhaitez suivre le lancement des nouvelles fermes ainsi que leur date de lancement, je vous recommande fortement le [calendrier de RugDoc.io](https://rugdoc.io/calendar/), ainsi que le reste de leur site qui présente une analyse de chaque ferme et des risques possiblement encourus par les utilisateurs souhaitant les rejoindre.

## Impermax

### Quelques explications

[Impermax](https://polygon.impermax.finance) est une plateforme permettant aux utilisateurs d'appliquer un effet de levier sur leurs investissements en utilisant plusieurs boucles de prêt/emprunt afin de maximiser les rendements. Le but est vraiment simple: en déposant une paire de liquidité et en l'utilisant comme collatéral, vous pouvez emprunter les tokens composant la paire afin de créer plus de tokens de liquidité, et recommencer la boucle.

![La boucle Impermax expliquée schématiquement](../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)

En utilisant des boucles de levier, les utilisateurs s'exposent a des pertes impermanentes liées aux fluctuations de prix des tokens composant la paire de liquidité, et ces pertes potentielles sont amplifiées par le nombre de boucles. Le risque de liquidation est également amplifié. Cependant, si les risques sont augmentés, les gains sont également largement impactés par l'effet de levier.

Il est cependant bon de noter qu'en utilisant des paires composées de monnaies stables, les risques de liquidation et de pertes impermanentes sont relativement minimisés puisque chaque token va varier très peu en termes de prix l'un par rapport à l'autre. Cela veut également dire que le ratio dette/collatéral peut être très bas (très proche de 100%), permettant d'opérer un très grand nombre de boucles, et augmentant le rendement de façon importante.

Il est important de noter qu'Impermax prélève des frais lorsque vous empruntez des cryptos pour appliquer des boucles de levier. Les frais correspondent à 0.1% de votre emprunt final. Ainsi, si vous commencez avec 100$ de paire MAI/USDC et que vous appliquez 50 boucles, votre position finale sera de 5 000$. Vous aurez alors emprunté 4 900$, et payé $4.90 de frais.

En bouclant les prêts/emprunts, vous allez multiplier votre APR final. Ainsi, avec un rendement initial de 20% pour la paire MAI/USDC, avec un ratio dette/collatéral de 110% (imposé par Impermax) et en bouclant 50 fois, le rendement final sera de

$$
APR_{final}=APR_{Initial} * \sum_{i=0}^{n}{\frac{100}{CDR}^i}
$$

Ce qui donne un rendement final de 228%. Bien entendu, plusieurs autres facteurs rentrent en compte dans le calcul du rendement final, notamment le taux d'emprunt (intérêts sur les montant empruntés pour fabriquer plus de tokens LP), ainsi que l'offre et la demande pour chaque crypto composant la paire de liquidité que vous empruntez (impactant directement le taux d'emprunt).

Notez également que ces facteurs sont d'autant plus amplifiés que vous effectuez un nombre de boucles important. Le rendement peut donc varier de façon drastique, et parfois même devenir négatif (vos tokens  LP seront alors utilisés pour payer les frais).

### Effet de levier sur la paire MAI/USDC

Pour simplifier, vous utilisez le rendement initial mais appliqué sur un plus gros montant investi, ce qui, rapporté à votre investissement initial, donne un rendement plus élevé.

![Exemple de tableau de bord sur Impermax avec un investissement initial de 70.52$ de MAI/USDC](../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)

On voit de façon claire le montant initial investi, le montant total équivalent, le nombre de boucles, ainsi que les valeurs de liquidation. Cette position, au moment d'écrire ce tutoriel, me donnera les rendements suivants

![Estimations des gains et dépenses à un moment donné](../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)

Le rendement est distribué sous forme de tokens IMX (natifs à Impermax) qui peuvent, au choix, être échangé pour plus de MAI/USDC (pensez à utiliser la puissance de Mai Finance et des emprunts à taux 0), ou utilisés sur Impermax afin de pourvoir de la liquidité à des paires acceptant le token IMX.

### Proposer de la liquidité aux emprunteurs

En effet, il est également possible de déposer des cryptos directement sur Impermax afin que les utilisateurs souhaitant utiliser l'effet de levier puissent les emprunter pour augmenter leurs profits. En déposant vos MAI et USDC séparément de cette façon, vous obtiendrez une partie des frais d'emprunts tout en laisser les emprunteurs prendre tous les risques de liquidation et de pertes impermanentes. Il est également bon de noter que plus le montant des emprunts est élevé (demande forte), plus les frais d'emprunts sont élevés pour un montant fixe proposé, ce qui augmente votre rendement.

![Taux pour les prêts et les emprunts pour MAI sur Impermax](../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)

Ceci est une autre façon d'optimiser vos emprunts à taux 0% sur Mai Finance.

## Avertissement <a href="disclaimer" id="disclaimer"></a>

Tout ce tutoriel est purement éducatif. Le but est simplement de mettre en lumière les projets qui, selon moi, valent la peine d'être connus par les personnes qui évoluent dans le monde des cryptos sur Polygon. Bien entendu, je n'ai pas présenté la façon de récolter du revenu sur Mai Finance car un tutoriel lui sera dédié.

En conclusion, ce guide n'est ABSOLUMENT PAS fait pour être suivi à la lettre, ce n'est pas un conseil sur une stratégie d'investissement en particulier, et vous ne devriez pas suivre mes propos aveuglément. Veuillez lire les documentations des projets présentés avant d'investir quoi que ce soit sur ces plateformes.

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
