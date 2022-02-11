---
description: >-
  Ce guide propose une nouvelle façon d'optimiser vos investissements
  stables en incluant un projet de type Ohm en tant que multiplicateur
  de récompenses.
---

# L'éléphant, le singe et la loutre

## Introduction

Ce titre pourrait annoncer un excellent poème, cependant ces trois animaux représentent les protocoles qui seront utilisés dans ce guide. Aujourd'hui, nous allons nous attarder sur l'un des derniers ajouts (en Janvier 2022) à la liste des crypto-monnaies acceptées comme collatéral sur Mai Finance afin de soutenir la monnaie stable MAI: le jeton sdam3CRV. Nous allons vous expliquer de quoi il s'agit et comment vous en procurer. Nous vous proposerons ensuite une petite stratégie les mettant en œuvre afin de récolter des revenus importants en utilisant la stratégie stable de Stake DAO, Mai Finance, ainsi que le protocole OtterClam comme multiplicateur de récompenses.

![](<../../.gitbook/assets/stakedao-otter-1.png>)
 
## Stake DAO
 
### Presentation de Stake DAO

[Stake DAO](https://app.stakedao.org/) est une plateforme vous permettant d'optimiser vos gains (yield optimizer). Vous pourrez déposer vos actifs sur la plateforme et utiliser des stratégies automatisées permettant de maximiser vos revenus. Ces stratégies sont proposées avec un score de risque, et listées sur un tableau de bord clair et simple, ce qui rend aisé de les classer et choisir celle qui vous correspond le plus. Si ce protocole est principalement présent sur le réseau Ethereum Mainnet, Stake DAO est également déployé sur d'autres chaînes, y compris Polygon et Avalanche. Vous pouvez bien entendu en apprendre plus dans [leur documentation officielle](https://stakedao.gitbook.io/stakedaohq/).
 
### La stratégie am3CRV

Pour notre guide, nous allons utiliser la stratégie `Passive Aave USD Strategy` pour Polygon, une stratégie basée sur les revenus passifs donnés par Aave. Elle est avant tout basée sur la réserve de liquidité am3CRV sur [Curve Finance](https://polygon.curve.fi/): vous pouvez y déposer vos actifs stables (USDC, USDT ou DAI) dans la réserve et vous recevrez un jeton de reçu appelé am3CRV. Vous pouvez ensuite l'utiliser sur Curve afin de récolter des récompenses payées en jetons CRV et WMATIC, mais vous pouvez également les déposer sur Stake DAO. Si vous faites ainsi, les récompenses en CRV et WMATIC seront vendues pour des actifs stables additionnels qui seront composés dans votre dépôt initial.
 
![Réserve aave sur Curve en janvier 2022](<../../.gitbook/assets/stakedao-otter-2.png>)

Comme vous pouvez le voir ci-dessus, utilisez vos am3CRV sur Curve vous donnerait un APR (**A**nnual **P**ercentage **R**eward, ou pourcentage de récompenses annuel) de 8,35%. Si vous allez sur Stake DAO, vous pourrez noter que dans les stratégies sur Polygon, les jetons am3CRV vous permettront de gagner 11.11% d'APY (**A**nnuel **P**ercentage **Y**ield, ou pourcentage annuel de gains composés).
 
![Stratégie passive AAVE USD sur Stake DAO en janvier 2022](<../../.gitbook/assets/stakedao-otter-3.png>)

Lorsque vous déposez vos am3CRV sur Stake DAO, vous recevrez un nouveau jeton de reçu: le sdam3CRV (**s**take **d**ao am3CRV).

{% hint style="info" %}
Veuillez noter que Stake DAO prélève des frais sur vos gains pour chaque stratégie utilisée. Dans notre cas, au moment de l'écriture de l'article en janvier 2022, les frais de performance sont de 15%, et il y a aussi des frais de 0.5% lorsque vous ressortez vos actifs. Faites bien attention de comprendre la structure des frais avant d'entrer dans la pool.
{% endhint %}

Cette stratégie peut être considérée comme très sûre (DYOR) puisqu'elle n'utilise que des cryptos stables. Les risques de perte impermanente sont quasiment nuls puisque les tokens am3CRV sont seulement composés de cryptos stables indexés sur le prix du dollar US. Si vous voulez utiliser Stake DAO, il vous faudra tout de même prendre en compte le risque lié au smart contracts. En effet, vos actifs sont mis à disposition sur AAVE via Curve, et vos reçus sont déposés sur Stake DAO, il y a donc 3 couches de protocoles possiblement à risque.

Vous pourrez utiliser l'instrument de farming de Stake DAO afin de déposer vos sdam3CRV et gagner un 9% supplémentaire payés en tokens SDT, le token natif de Stake DAO. Pour notre guide cependant, nous allons les utiliser différemment.
 
## Mai Finance

[Mai Finance](https://app.mai.finance) est un protocole de prêt/emprunt où vous pouvez déposer vos actifs comme collatéral afin d'emprunter de la monnaie stable, ce qui vous permet d'éviter de vendre vos cryptos. Cependant, le mode de fonctionnement est différent des autres plateformes de prêt où les prêteurs mettent leurs actifs à disposition des emprunteurs. Sur Mai Finance, vous ne prêtez qu'à vous-même, et vous ne pouvez emprunter qu'en fonction de vos propres actifs. Vous pourrez trouver beaucoup plus d'informations sur Mai Finance dans [leur documentation officielle](https://docs.mai.finance/) ou dans la section sur L'Université du MAI.

En janvier 2022, les jetons sdam3CRV ont été approuvés en tant que collatéral pour les coffres Mai Finance. Celà veut dire que le jeton que vous recevez comme reçu de vos dépôts sur Stake DAO peuvent désormais être utilisés afin d'emprunter de la monnaie stable MAI. Ceci est particulièrement intéressant pour les raisons suivantes:

* les jetons sdam3CRV représentent une preuve de dépôt composé de monnaie stables uniquement, ainsi vous êtes à l'abris des pertes impermanentes et le jeton devrait conserver un prix fixe uniquement affecté par son taux de rendement
* puisque le prix ne varie pas à la baisse, il est simple d'éviter la liquidation, et ce même si vous empruntez proche du seuil de liquidation
* votre collatéral grossit en valeur avec le temps puisque les intérêts récoltés sur AAVE sont composés. Au moment d'écrire ce guide, le rendement est de 11% annuel
  
![Exemple d'un coffre sdam3CRV sur Mai Finance](<../../.gitbook/assets/stakedao-otter-4.png>)
 
Ce coffre utilise un CDR élevé (**C**ollateral to **D**ebt **R**atio, ou ratio entre la valeur du collatéral et celle de la dette). Ceci est dû au fait que nous proposons toujours des solutions jugées sûres dans les guides présents sur ce site. Un CDR élevé présente en effet plusieurs avantages:

* Il vous garde relativement à l'abris de la liquidation en cas d'événement négatif majeur sur le marché
* Il vous permet de retirer une importante partie de vos actifs en collatéral et de les vendre afin de rembourser votre dette (veuillez vous reporter à notre [guide sur le remboursement de la dette](../../mai-university/debt-repayment-how.md) pour plus de détails)

Cependant, libre à vous de réduire la valeur de CDR en fonction de votre tolérance au risque.

{% hint style="info" %}
Le coffre sdam3CRV utilise des monnaies stables comme collatéral. De la même façon que pour le coffre camDAI, vous ne recevrez **PAS** de récompenses lorsque vous empruntez avec ce coffre. Il se peut également que le seuil de liquidation soit baissé à 110%, de même que pour le coffre camDAI.
{% endhint %}
 
Avec les MAI empruntés, vous pourrez bien entendu appliquer un effet de levier sur votre position dans Stake DAO. Si vous souhaitez plus de détails sur comment appliquer un effet de levier sur vos cryptos, vous pouvez lire notre [guide dédié au camDAI](camdai-beginner-strategy.md) et appliquer la même stratégie à vos jetons sdam3CRV. Vous pourrez ainsi recevoir un rendement bien supérieur simplement en bouclant vos investissements. Cependant, pour ce guide, nous utiliserons une autre approche qui n'implique pas de vente massive de MAI.
 
## OtterClam DAO

[OtterClam Finance](https://app.otterclam.finance/) est un projet sur Polygon basé sur le protocole Ohm. Il est particulièrement innovant puisqu'il intègre des NFTs dans leur modèle économique. Démarré en novembre 2021, OtterClam a vu une croissance importante sur l'aspect DeFi (**De**centralized **Fi**nance, ou finance décentralisée), et se lance maintenant dans la GameFi.

L'un des aspects les plus intéressants de OtterClam pour notre stratégie est son partenariat avec Mai Finance. En effet, la plus grosse part de la trésorerie de OtterClam est en monnaie stable MAI, et est utilisée pour soutenir l'émission de leur jeton natif, le CLAM. Par là même, vous avez la possibilité d'acheter des bonds CLAMs directement à partir de vos MAI, et c'est exactement ce que nous allons faire dans cette stratégie. En effet, les projets de type Ohm sont réputés pour leur émission très importante, résultant en des taux de rendement élevés, et OtterClam ne fait pas exception à la règle. Un autre point particulier sur les bonds vendus sur OtterClam est que vous allez acheter des jetons sCLAM directement (**s**taked CLAMs), et vous recevrez ainsi des récompenses de staking pendant toute la durée de maturation de votre bond, ce qui les rend encore plus attractifs.
 
![Achat de bond sCLAM sur OtterClam en janvier 2021](<../../.gitbook/assets/stakedao-otter-5.png>)

Sur cette capture d'écran, vous pouvez voir que nous allons acheter des sCLAM avec un rabais de 3,66% (le prix d'achat étant de 9,20$ alors que le prix du marché et des 9,54$), mais pendant toute la période de maturation (5 jours), les sCLAM achetés vont également augmenter de 6,95%. Puisque le taux de rendement est excessivement élevé (13 400% APY au moment de la rédaction de cet article), il sera important de conserver les jetons sCLAM stakés, cependant vous en revendrez une partie contre de la monnaie stable que sera ensuite déposée sur Curve afin de recevoir des jetons am3CRV supplémentaires.
 
![Félicitation, vous avez des CLAM stakés](<../../.gitbook/assets/stakedao-otter-6.png>)
 
Si vous regardez le prix des CLAMs, vous vous rendrez compte que le jeton présente une volatilité importante, cependant, le prix du jeton n'est pas "important", nous n'utilisons OtterClam que comme un multiplicateur de gains. Les projets de type Ohm sont conçus afin de réduire le prix de leur jeton natif à la valeur des actifs soutenant leur émission, ou 1$ dans la plupart des cas. Ce sont également des "monnaies de réserve", et en tant que telles, elles sont faites pour être utilisées, achetées et vendues.

{% hint style="info" %}
Les récompenses de staking sont composées et ajoutées aux jetons en cours de maturation, ils seront disponibles à la fin de la période de maturation. Ainsi, il faudra attendre que la période de maturation soit terminée avant de pouvoir collecter les gains et en revendre une partie.
{% endhint %}
 
## Strategie de farming

Comme dans la plupart des cas, le point de départ le plus judicieux pour une stratégie d'investissement reste de commencer par des positions stables. De cette façon, vous réduisez le risque de pertes impermanentes, et vous travaillez uniquement avec les bénéfices générés par votre position stable (ou notre dette dans notre cas). Ainsi, la boucle démarre par le dépôt de monnaie stable sur Curve afin de recevoir des jetons am3CRV. Ces preuves de dépôt sont alors déposées sur Stake DAO afin de recevoir des jetons sdam3CRV. Il est alors possible de déposer des reçus sur Mai Finance en collatéral afin de pouvoir emprunter des MAI. Le prêt est alors utilisé afin d'acheter des bonds sur OtterClam. Les récompenses de staking seront alors converties en monnaie stable pour reprendre la boucle au début. Veuillez noter qu'il est également possible de revendre n'importe quelle quantité de vos gains sur OtterClam. Pour ce guide, nous allons vendre 100% des gains, mail il vous est possible d'en conserver une partie afin d'augmenter votre position sur OtterClam et accroître le nombre de CLAM stakés plus rapidement, produisant toujours plus de récompenses.

Comme toujours pour nos simulations, tous les nombres seront fixés dès le départ:

* l'APY pour les jetons sdam3CRV sur Stake DAO est de 11,11%
* l'APR pour les CLAM stakés est de 13 400%

Veuillez également noter que nous n'allons pas nous occuper du remboursement de la dette et nous partons du principe que tous les prix resteront identiques. Nous allons effectuer une simulation avec 100$ de USDC comme point de départ, et nous tâcherons de conserver un CDR de 200% pour toute la durée de l'exercice. Enfin, nous assumerons pour la simplicité de la simulation qu'à la fin de chaque période de maturation des bonds sur OtterClam un nouveau bond avec un rabais de 0% sera disponible pour nos MAI empruntés. Bien entendu, vous devrez chercher des bonds avec des rabais élevés afin d'accroître vos gains.
 
![](<../../.gitbook/assets/stakedao-otter-7.png>)
 
### Jour 1

Le premier jour, vous allez pouvoir préparer l'intégralité de la stratégie:

* Déposez vos 100$ de USDC (ou USDT ou DAI, selon votre préférence) sur Curve finance
* Déposez vos am3CRV sur Stake DAO
* Déposez vos sdam3CRV dans le coffre Mai Finance correspondant
* Empruntez avec un CDR de 200%, soit 50% de MAI
* Achetez un bond de MAI sur OtterClam Finance

A cette étape, vous êtes complètement prêt et il ne vous reste plus qu'à attendre la fin de la période de maturation de votre bond pour commencer à récolter vos récompenses. Ainsi, à la fin du jour 1, vous aurez

| Position                 | valeur ($) |
|--------------------------|------------|
| sdam3CRV                 |    100.000 |
| MAI loan                 |     50.000 |
| sCLAM                    |     50.000 |
| sdam3CRV supplémentaires |      0.030 |
| sCLAM supplémentaires    |      0.000 |
 
### Jour 2, 3 et 4

Rien de remarquable, vos jetons sdam3CRV collectent des récompenses depuis AAVE, mais c'est à peu près tout, vous n'aurez aucune récolte à faire tant que le bond n'est pas arrivé à maturation.
 
### Jour 5

À la fin du jour 5, le bond est libéré, et puisqu' il a accumulé des récompenses de staking pendant la durée de maturation, vous devriez avoir à la fin du cinquième jour
 
| Position                 | valeur ($) |
|--------------------------|------------|
| sdam3CRV                 |    100.122 |
| MAI loan                 |     50.000 |
| sCLAM                    |     53.382 |
| sdam3CRV supplémentaires |      0.030 |
| sCLAM supplémentaires    |      0.722 |
 
### Jour 6

Vous avez maintenant des sdam3CRV supplémentaires avec lesquels vous allez pouvoir emprunter et acheter un nouveau bond. Cette fois-ci, il s'agira d'un très petit montant (certainement quelques centimes seulement) mais avec le temps il vous sera possible d'acheter de plus en plus de sCLAM avec vos nouveaux MAI. A la fin du jour 6, vous aurez
  
| Position                 | valeur ($) |
|--------------------------|------------|
| sdam3CRV                 |    100.875 |
| MAI loan                 |     50.437 |
| sCLAM                    |     53.820 |
| sdam3CRV supplémentaires |      0.031 |
| sCLAM supplémentaires    |      0.728 |

A partir de maintenant, vos CLAMs stakés vont commencer à produire des récompenses trois fois par jour, et il vous sera possible de composer ces gains dans votre coffre sdam3CRV, ou vous pouvez simplement composer vos gains une seule fois au cours des 5 jours de maturation de vos bonds.
 
### Routine Quotidienne

En partant du principe que vous composez vos gains tous les jours, votre routine quotidienne sera la suivante

* débloqué l'équivalent des 3 rebases quotidiennes sur OtterClam
* revendez vos jetons CLAM pour n'importe quelle monnaie stable acceptée par la pool am3CRV (USDC, USDT ou DAI)
* déposez vos crypto stables additionnelles dans la pool AAVE sur Curve Finance
* déposez vos am3CRV sur Stake DAO
* déposez vos sdam3CRV sur Mai Finance

De plus, tous les 5 jours, vous serez capables de réaliser les étapes supplémentaires:

* empruntez des MAI additionnels tout en gardant un CDR de 200%
* achetez un bon sur OtterClam avec vos MAI
  
### Résultats bruts mois après mois

Voici les résultats mois après mois

| jour |  sdam3CRV  |    CLAM    |  dette MAI |
|------|------------|------------|------------|
|   30 |    121.249 |     64.007 |     60.625 |
|   60 |    150.866 |     78.815 |     75.433 |
|   90 |    187.350 |     97.057 |     93.675 |
|  120 |    232.294 |    119.529 |    116.147 |
|  150 |    287.659 |    147.212 |    143.830 |
|  180 |    355.863 |    181.314 |    177.931 |
|  210 |    439.882 |    223.323 |    219.941 |
|  240 |    543.383 |    275.074 |    271.691 |
|  270 |    670.884 |    338.825 |    335.442 |
|  300 |    827.950 |    417.358 |    413.975 |
|  330 |  1,021.437 |    514.101 |    510.719 |
|  360 |  1,259.790 |    633.277 |    629.894 |
 
### Jour 365

Après une année complète de récoltes sur ce système, et en partant du principe que tous les prix et les taux sont restés identiques, vous aurez:

* 1 304,575$ de jetons sdam3CRV dans votre coffre sur Mai Finance
* 655,670$ de CLAM sur OtterClam
* une dette de 652,288$ en MAI

Vous pouvez facilement voir qu'à la fin de l'année, vous avez toujours un CDR de 200%. Vous pouvez retirer une partie de votre collatéral afin de rembourser votre dette et débloquer le reste du collatéral. Vous pouvez aussi rembourser votre dette en vendant vos CLAM et débloquer 100% de votre collatéral.

En conclusion, en partant de 100$ investis, vous pourriez terminer l'année avec 1 307,958$ et une dette de 652,288$, ce qui correspond à un APY équivalent de 1 207,958%.
 
{% hint style="success" }
Si vous ne vendez que 50% de vos rewards de staking chaque jour sur OtterClam Finance, et que vous conservez le reste staké, le rendement de OtterClam sera appliqué sur un montant plus important de sCLAMs et vos gains augmenteront beaucoup plus rapidement. Cependant, cette option présente beaucoup plus de risques au vu du prix du CLAM. Cependant, si le prix et le rendement du CLAM se maintient, et si vous revendez seulement 50% de vos gains, vous pourriez terminer l'année avec 3 608,447$ répartis dans votre coffre sur Mai Finance et sur OtterClam, ainsi qu'avec une dette de 750,828$ pour un APY équivalent de 2 757,619%.
{% endhint %}
 
## Avertissement

Cette stratégie est intéressante car elle présente relativement peu de risques pour votre investissement initial. En effet, votre argent travaille à partir de cryptos stables, donc votre investissement initial est en quelque sorte "protégé" et la probabilité de le perdre est relativement faible. Le risque de liquidation est quant à lui quasiment nul puisque le prix de votre collatéral est indexé sur le même prix que votre dette, et la valeur de CDR élevée vous permet de vous protéger d'une quelconque liquidation. L'utilisation d'outils supplémentaires vous permet de multiplier vos gains de façon importante, gains qui resteraient relativement faibles sans l'utilisation de ces outils additionnels.

Cependant, il est important de comprendre cette stratégie dans tous ses détails. Les risques liés à la multiplication des smart contracts sont élevés puisque nous utilisons un nombre important de protocoles. De plus, il vous faudra comprendre les bases de l'économie des projets de type Ohm, et faire abstraction du prix du CLAM qui peut varier de façon drastique. Enfin, si les taux peuvent rester les mêmes sur Stake DAO, le rendement sur OtterClam devrait quant à lui varier de façon importante et se réduire avec le temps puisque ce genre de projet ne peut soutenir des rendements aussi élevés pendant une longue période. Comme toujours, prenez le temps de lire la documentation des projets que vous utilisez, et faites en sorte de bien peser les risques encourus.
 
{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
