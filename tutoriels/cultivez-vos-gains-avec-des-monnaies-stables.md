---
description: >-
  Cette page présente en détails les différentes stratégies "sans risques" qui
  vous permettront de cultiver vos gains de façon sécuritaire.
---

# Cultivez vos gains avec des monnaies stables

## Idée générale

Lorsque vous commencez à récolter des gains dans des fermes de rendement sur Polygon, vous exposez vos investissements au succès ou à son échec. Ce guide ne présente pas ce que sont les fermes de rendement (yield farms), ni comment vous devriez les exploiter. Si vous aves besoin d'aide à leur sujet, vous trouverez facilement des tutoriels sur internet. Vous pouvez également rejoindre la communauté QiDAO sur [Discord](https://discord.gg/mQq55j65xJ), et nous nous ferons un plaisir de vous aider.

Le principal problème lorsque vous exploitez une ferme de rendement est que vous avez le choix entre

* vendre les jetons natifs à la ferme afin d'augmenter vos positions moins risquées
* ré-investir les jetons pour accroître vos gains (aussi connus sous le terme de hyper-compounding)

Ce guide va présenter étape par étape la façon d'utiliser la plateforme Mai Finance pour sécuriser vos gains tout en accroissant vos investissements et gagner encore plus.

{% hint style="info" %}
Afin d'illustrer en détails comment maximiser vos gains, j'utiliserai l'une des dernières fermes de rendement de [Polypup](https://ball.polypup.finance). Ceci n'est qu'à but éducatif et ne devrait absolument pas être considéré comme un conseil financier. Veuillez également noter que le terme "sans risques" est uniquement basé sur mon opinion personnelle. Comme toujours, veuillez faire vos propres recherches. Pour finir, je ne recommande pas d'exploiter cette ferme.
{% endhint %}

![](../.gitbook/assets/screen-shot-2021-08-09-at-10.20.26-am.png)

## Cycle de vie de vos "plantations"

### Préparez vos cultures

Comme m'a un jour dit un humble cultivateur:

> _**Personne ne devrait acheter ce qu'il peut gagner**_

Dans ce guide, nous allons mettre en place autant de barrières de protection que possible. Afin d'atteindre ce but, nous allons exploiter la ferme de rendement en n'utilisant que des monnaies stables, ce qui permettra de mettre notre investissement à l'abris des pertes impermanentes (Impermanent Losses). La plupart des fermes de rendement acceptent les paires de monnaies stables dans leurs réserves de liquidité (**L**iquidity **P**ool), et comme la monnaie MAI gagne en popularité et en visibilité, vous pourrez facilement trouver des fermes proposant la paire MAI/USDC. C'est la paire avec laquelle nous travaillerons dans ce guide.

Afin de commencer à cultiver la paire MAI/USDC, il faut commencer par acheter ces monnaies stables. Mai Finance vous permet d'emprunter la monnaie MAI en déposant des fonds comme collatéral. Pour notre exemple, nous assumerons avoir des MATIC prêts à l'emploi dans notre portefeuille. En déposant nos MATIC dans notre [coffre MATIC](https://app.mai.finance/vaults/matic) sur Mai Finance, nous allons pouvoir emprunter des MAI. Si vous avec besoin de détails sur l'utilisation des coffres, veuillez rejoindre le serveur Discord et poser vos questions à la communauté. Vous pouvez également lire les autres tutoriels sur ce site afin d'avoir des détails supplémentaires.

{% hint style="info" %}
Vous pouvez déposer vos jetons MATIC dans le coffre dédié, mais vous pouvez également les déposer sur AAVE afin de recevoir des jetons amWMATIC que vous pourrez déposer sur Mai Finance dans la page d'optimisation des rendements. Avec les camWMATIC reçus, vous pourrez utiliser ces jetons comme collatéral tout en bénéficiant du rendement apporté par AAVE. Veuillez vous référer à l'article sur les [effets de levier sur les tokens AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/fr/tutoriels/tirez-parti-aave-tokens) pour plus de détails.
{% endhint %}

Une fois en possession de vos MAI, vous pouvez utiliser la [page d'échange](https://app.mai.finance/anchor) (swap page, ou anchor page) sur Mai Finance afin de convertir la moitié de votre monnaie stable en USDC. En effet, lorsque vous cultivez une paire de monnaie stable, la paire doit toujours être constituée d'un ratio 1:1 en valeur pour chaque token la composant.

![Utilisation de la page d'échange afin de convertir 30 MAI en USDC](../.gitbook/assets/screen-shot-2021-08-09-at-6.28.28-am.png)

En fonction de la ferme de rendement sur laquelle vous allez cultiver, vous avez maintenant besoin de combiner une paire (MAI et USDC) sur le bon site d'échange (plateforme DEX pour **D**ecentralized **Ex**change). Dans notre exemple avec Polypup, cette ferme accepte les paires provenant de [QuickSwap](https://quickswap.exchange/#/), c'est donc cette plateforme d'échange que nous utiliserons pour créer la paire MAI/USDC.

![Création de la paire LP à partir des monnaies stables MAI et USDC](../.gitbook/assets/screen-shot-2021-08-09-at-6.29.16-am.png)

Nous sommes maintenant prêts à cultiver notre paire stable.

### Planter et récolter les jetons natifs

Maintenant que nous sommes en possession de jetons LP, nous pouvons commencer les plantations dans la ferme de rendement et les déposer dans la réserve appropriée. Ceci va nous permettre par la suite de récolter les tokens natifs à la ferme. Dans notre exemple, nous allons déposer nos jetons MAI/USDC et nous allons récolter des jetons BALL.

![La réserve nous fait gagner des jetons BALL](../.gitbook/assets/screen-shot-2021-08-09-at-10.58.19-am.png)

Au moment d'écrire cet article, vous pouvez voir que la réserve MAI/USDC a un rendement de 176.99%. C'est un rendement annualisé (**A**nnual **P**ercentage **R**ate). En fonction du montant de liquidité disponible dans la réserve, et en fonction du prix du token BALL, ce rendement va fortement fluctuer avec le temps.

{% hint style="info" %}
Il est très important de noter que lorsque vous déposez des tokens LP, la plupart des fermes de rendement vont prélever un certain pourcentage, généralement entre 2% et 4%. Ces frais sont directement prélevé sur le montant déposé. Soyez très attentif à ces frais, et préparez-vous mentalement à possiblement perdre tout ou partie de ces frais si la ferme est un échec.
{% endhint %}

Maintenant que notre paire de monnaies stables est dans la réserve, nous allons gagner des bénéfices sous forme de tokens natifs. Il est possible de les récolter à tout moment. Veuillez noter que le prix de ces tokens va être extrêmement volatil, particulièrement lors des premiers jours de la ferme, il est donc important de les récolter régulièrement et de les vendre lorsque vous jugez qu'ils ont une valeur intéressante. Plus longtemps vous attendrez, plus vous vous exposez au risque de finir avec un sac de tokens qui ne valent plus rien. Dans la capture d'écran ci-dessus, cliquez simplement sur `Harvest` et vous récolterez vos BALLs.

### Accroissez la valeur de vos tokens de ferme

Nous avons récolté nos premiers tokens. En général à cette étape, vous avez le choix entre

* vendre les jetons et acheter quelque chose ayant une valeur plus sûre (votre crypto préférée est un excellent exemple)
* ré-injecter les tokens dans la ferme

Mai Finance vous offre une troisième option vous permettant de faire les deux à la fois. Une fois que les jetons natifs sont récoltés, vous pouvez simplement utiliser votre DEX préféré supportant le token natif. D'habitude, vous pourrez trouver un lien vers la plateforme d'échange dans le menu de la ferme de rendement. Ce lien vous dirigera directement vers la bonne page permettant de faire l'échange plus facilement. Veillez tout de même à vous assurer que le site n'est pas un site de phishing, faites attention à l'URL. Toutes les fermes ne sont pas tenues par des développeurs exemplaires. 

![J'échange mes jetons BALL contre des MATIC](../.gitbook/assets/screen-shot-2021-08-09-at-11.14.29-am.png)

À cette étape, je suis à nouveau en possession de jetons MATIC dans mon portefeuille, ce qui correspond à la première étape de préparation. Je vais donc pouvoir utiliser ces nouveaux tokens en les déposant sur Mai Finance et emprunter de la monnaie stable MAI, faire l'échange pour des USDC, créer des nouveaux jetons de liquidité et les re-déposer dans la ferme. En opérant de la sorte, 100% de mes gains sont transformés en MATIC (valeur bien plus sûre que les jetons BALL), et je ré-injecte 50% (empruntés sous forme de MAI) dans la ferme pour accroître mes gains. Notez qu'en réalité, je ne ré-injecte que 46% à cause des frais de dépôt de 4%.

Vu d'un autre angle, le rendement (APR) de la ferme est appliqué en intégralité à la crypto dans votre coffre su Mai Finance. Si vous déposez des nouveaux tokens dans la réserve (composition), vous recevez 50% du rendement (APY, ou Annual Percentage Yield) sous forme de nouveaux jetons LP.

## Estimation des gains

Tous les résultats présentés ci-dessous partent du principe que

* Nous avons démarré avec l'équivalent de 60 MAI empruntés sur Mai Finance, avec l'équivalent de 120,00$ de MATIC dans le coffre dédié.
* Le rendement de la ferme reste fixe à 176.99%, ce qui se traduit par un rendement quotidien de 0.484%
* La valeur du MATIC et du BALL reste stable pour toute la période concernée

Ces hypothèses sont bien entendu complètement fausses. Vous vous rendrez compte que les rendements des fermes varient très fortement, et diminuent rapidement au fur et à mesures que le montant de liquidité investi augmente, et que le prix du token natif varie avec le temps.

### Estimation brute

| Jour | valeur du LP value | valeur des gains | composition des MATIC | nouveaux LP créés |
| :--: | -----------------: | ---------------: | --------------------: | ----------------: |
|   1  |             $57.60 |           $0.279 |                $0.279 |            $0.139 |
|   2  |            $57.734 |           $0.280 |                $0.559 |            $0.140 |
|   3  |            $57.874 |           $0.280 |                $0.840 |            $0.140 |
|   4  |            $58.014 |           $0.281 |                $1.121 |            $0.141 |
|   5  |            $58.155 |           $0.282 |                $1.403 |            $0.141 |
|   6  |            $58.296 |           $0.282 |                $1.686 |            $0.141 |
|   7  |            $58.437 |           $0.283 |                $1.969 |            $0.142 |
|   8  |            $58.579 |           $0.284 |                $2.253 |            $0.142 |
|   9  |            $58.721 |           $0.285 |                $2.538 |            $0.142 |
|  10  |            $58.863 |           $0.285 |                $2.823 |            $0.143 |
|  11  |            $59.006 |           $0.286 |                $3.109 |            $0.143 |
|  12  |            $59.149 |           $0.287 |                $3.396 |            $0.143 |
|  13  |            $59.292 |           $0.287 |                $3.684 |            $0.144 |
|  14  |            $59.436 |           $0.288 |                $3.972 |            $0.144 |
|  15  |            $59.580 |           $0.289 |                $4.261 |            $0.144 |
|  16  |            $59.725 |           $0.289 |                $4.551 |            $0.145 |
|  17  |            $59.870 |           $0.290 |                $4.841 |            $0.145 |
|  18  |            $60.015 |           $0.291 |                $5.132 |            $0.145 |

* Le premier jour, les frais de 4% sont appliqués sur nos 60$ initiaux de paire MAI/USDC
* À la fin du premier jour, le revenue généré (0,279$) est transféré en intégralité dans le coffre MATIC
* À la fin du premier jour, puisque nous avons ajouté des fonds au coffre, nous pouvons emprunter plus de MAI
* Afin de conserver un ratio dette/collateral supérieur à 200%, nous n'empruntons que 50% du dépôt, soit 0,139$
* Au début du deuxième jour, nous ajoutons les 0,139$ de paire MAI/USDC dans la ferme, et payons 4% de frais de dépôt
* Au début du deuxième jour, nous recommençons avec 0,134$ additionnels de tokens LP

### Estimation des rendements APR, APY et de l'augmentation de revenus

La simulation a été arrêtée après 18 jours. Passé cette date, il est possible de se rendre compte que nous sommes à nouveau à 60$ de tokens LP. Cela veut dire que nous avons récolté assez de bénéfices pour rembourser les frais de dépôt initiaux, ce qui devrait être le but principal de n'importe quel "fermier".

Passé le 18ème jour, en restant dans la ferme, nous allons générer seulement du profit. Et puisque nous utilisons des monnaies stables pour récolter des gains, il y a quasiment 0% de risques de pertes liées à la fluctuation des tokens composant la paire LP (pertes impermanentes), ce qui veut dire qu'il n'y a "plus aucun risque" à rester dans la ferme. 

On peut également considérer que les 2,40$ de frais de dépôt initiaux sont remboursés au jour 9 puisque c'est le moment où la valeur des gains transférés sous forme de MATIC ont été atteints dans notre coffre. Si nous avions ré-investi 100% des tokens de ferme en nouveaux tokens LP, c'est au bout du 9ème jour que nous aurions couvert les frais initiaux.

En termes de gains, les revenus composés ajoutés aux tokens LP sont seulement de 50% par rapport à ce que la ferme propose. Cela veut dire que pour un rendement de 176.99% annoncé par la ferme, la croissance réelle de notre revenu (dans la ferme) n'est que de 88.495% annuellement, ou 0.242% quotidiennement.

Il est également possible de calculer le gain exact qui sera généré après un nombre de jour donné, en partant du principe que vous composez vos gains de façon quotidienne, en utilisant la formule suivante donnant le ROI (**R**eturn **O**n **I**nvestment, ou retour sur investissement):

$$
ROI_{JourN}=InvestissementInitial*(1+APRQuotidien)^{JourN}-InvestissementInitial
$$

Dans le cas d'une ferme prélevant 4% de frais d'entrée, vous devrez multiplier ce total par 96%. Dans notre cas, on peut rapidement vérifier que la formule fonctionne en comparant le résultat avec le montant obtenu dans le tableau du paragraphe précédant

$$
ROI_{Jour1} = [60 * (1+0.00242)^{1}-60]*0.96=$0.1396523836
$$

$$
ROI_{Jour365}=[60*(1+0.00242)^{365}-60]*0.96=$81.80752927
$$

Ainsi, en commençant avec 60,00$ et en générant 81.81$ au bout d'un an, nous obtenons un APY de 136,34%.

Il est possible de comparer ce résultat avec le rendement annualisé (APY) théorique de la ferme donnant un rendement global (APR) de 88,495% en utilisant la formule suivante:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Ceci donne, avec un APR de 88,495% et N = 365 (composition quotidienne)

$$
APY = ( 1 + \frac{0.88495}{365})^{365}-1=142.02\%
$$

Veuillez noter que l'estimation ci-dessus ne tient pas compte des frais de 4% de frais d'entrée, d'où la légère différence avec le résultat précédant.

Le gain en MATIC quant à lui est simplement le double de ce que la ferme gagne en montant de tokens LP, et il est possible de calculer le retour sur investissement après un nombre de jours donné en utilisant la même formule qu'avant, et en multipliant par 2:

$$
ROI_{Jour365} = [60 * (1 + 0.00242)^{365} - 60]*0.96*2=$163.6150585
$$

C'est le montant en MATIC que nous pourrions gagner en restant dans la ferme pendant un an complet, avec un investissement initial de 60$ de MAI/USDC, en partant du principe que le rendement reste le même sur un an. Cela nous donne également un rendement composé de 272,69%, ce qui est plus ou moins le rendement composé annuel affiché par la ferme (le rendement annuel composé affiché ne tenant pas compte des frais d'entrée). 

### Récapitulatif après un an de récolte

Au bout d'un an, nous aurions

* 283,62$ de MATIC dans le coffre (initialement 120,00$ + 163,62$ de bénéfice)
* 141,82$ de dette (initialement 60,00$ + 81,82$ d'emprunt ré-investi)
* 141,82$ de jetons MAI/USDC dans la ferme

## Avertissement

Tout ce qui est présenté dans cette stratégie par du principe que

* La ferme de rendement conserve un rendement stable pour la réserve de liquidité MAI/USDC (ce qui est bien entendu totalement faux)
* Il est possible de récolter des gains sur une ferme donnée pendant une année complète (ce qui n'est pas possible, ce genre de fermes ayant une durée de vie moyenne de quelques jours à quelques mois, et des programmes de rendement avec une date de fin pré-déterminée)

Par exemple, le rendement (APR) pour la réserve MAI/USDC sur Polypup après 24h est tombé à 128.13%, principalement à cause de la valeur du token BALL qui a chuté drastiquement pendant les quelques premiers jours de la ferme.

Veuillez également noter que "récolter" des gains avec des monnaies stables peut paraître comme étant la façon la moins risquée de le faire car vous n'êtes pas impacté par les pertes impermanentes. Cependant, vous n'avez aucune garantie que vous pourrez rembourser votre dépôt initial de 4%. Vous pourrez trouver quelques fermes proposant des frais d'entrée de 0% ou 1%, même sur les réserves composées de tokens non-natifs (des réserves de jetons de liquidité dont aucun des deux n'est un token natif).

Récolter vos gains de façon régulière et les échanger contre des monnaies ayant une valeur réelle est considéré comme étant la meilleure stratégie lorsque vous exploitez des fermes de rendement. Emprunter des MAI et ré-injecter une portion de vos gains dans la ferme va vous permettre d'augmenter vos bénéfices (malgré les frais d'entrée qu'il faudra constamment payer). Cependant, il existe d'autres stratégies qui pourront vous permettre de maximiser vos gains, comme de conserver votre montant initial de jeton LP stables, et de ré-injecter vos gains sous forme de jetons LP natifs (qui ont des rendements plus élevés la plupart du temps, car exposés aux pertes impermanentes).

{% hint style="info" %}
Veuillez garder à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut parfaitement performer lamentablement (voir vous faire perdre de l'argent) dans d'autres circonstances. Restez informés, vérifiez les marchés, gardez un oeil sur vos investissements, et comme toujours, faites vos propres recherches.
{% endhint %}
