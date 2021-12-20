---
description: >-
  Ce guide présente une stratégie qui met en lumière les intéractions entre Mai
  Finance, QuickSwap et Adamant après le lancement de nouvelles fermes de
  rendement sur Mai Finance et QuickSwap.
---

# Farming ou Staking? Ou les deux?

![](<../../.gitbook/assets/Screen Shot 2021-09-03 at 9.24.12 AM.png>)

## Intro

Lorsque vous utilisez des applications de finance décentralisée (DeFi, **De**centralize **Fi**nance), particulièrement quand vous utilisez des fermes de rendement, vous avez tendance à accumuler des jetons offert par les applications. Si la plus part des personnes vendent ces jetons pour acheter plus de leurs crypto-monnaies favorites, nous allons essayer de démontrer des manières de les garder et utiliser pour augmenter nos revenus.\
Pour ce faire, nous utiliserons les nouvelles réserves de liquidité (Liquidity Pools) lancées sur QuickSwap, début de septembre 2021, qui utilisent le jeton Qi de Mai Finance. Si vous ne connaissez pas les applications QuickSwap et Adamant, visitez [Stack DApps like Lego Bricks](stack-dapps-like-lego-bricks.md).

## Présentation de la stratégie

### Les fermes

Pour maximiser nos gains, nous utiliserons les 3 applications suivantes:

* Mai Finance
* QuickSwap
* Adamant

Ainsi que les réserves de liquidité suivantes:

* Qi/MATIC sur Mai Finance pour générer du Qi
* Qi/WETH sur QuickSwap pour générer du QUICK et de l'ADDY
* Qi/QUICK sur Adamant pour générer de l'ADDY et du MATIC

Vous pouvez déjà voir que chaque application génère des jetons qui peuvent alimenter les autres réserves utilisées.\
L'idée est d'utiliser les Qi, récoltés sur Mai Finance, en combinaison avec les QUICK, récoltés sur QuickSwap, pour les utiliser sur Adamant. Ce dernier va générer des jetons ADDY avec lesquels nous pouvons récolter des dividendes en WMATIC. Le WMATIC peut ensuite être mis dans un coffre sur Mai Finance pour emprunter du MAI et acheter du MATIC et du WETH qui peuvent être utilisés avec du Qi pour augmenter vos positions sur Mai Finance et QuickSwap.

### Staking

Les jetons générés en excès sur Mai Finance et QuickSwap peuvent être stakés:

* Votre Qi sur Mai Finance **ET** QuickSwap est compté quand vous votez les QIPs (**Q**iDao **I**mprovement **P**roposals, propositions d'amélioration de QiDao).
* Le Qi peut être bloqué, sur Mai Finance, pour devenir éligible aux dividendes du protocole, payés en Qi et distribués chaque mercredi, ainsi qu'augmenter la valeur comptée de vos Qi lors de votes pour les QIPs. Plus de détails sur le staking du Qi bientôt.
* Le QUICK peut aussi être staké, sur QuickSwap, pour générer plus de QUICK dans l'Antre du Dragon (Dragon's Lair).
* "locked QUICK" (dQUICK) peut aussi être utiliser, sur QuickSwap, pour générer d'autres jetons via le Sirop du Dragon (Dragon's Syrup). Nous allons nous en servir pour générer de l'ADDY.
* l'ADDY généré sur Adamant est automatiquement investi (bloqué pendant 90 jours), cependant il générera des dividendes en WMATIC.
* l'ADDY peut aussi être bloqué, sur Adamant, pour augmenter les APRs/APYs (**A**nnual **P**ercentage **R**ewards / **A**nnual **P**ercentage **Y**ield) des fermes que vous cultivez sur l'app, générer plus d'ADDY, ainsi qu'augmenter vos dividendes, toujours en WMATIC.

## Préparer le système

![](<../../.gitbook/assets/Screen Shot 2021-09-08 at 6.54.08 AM.png>)

Ce qui suit est une **simulation** basée sur:

* un investissement initial de $1000 de jetons LP (**L**iquidity **P**rovider tokens, jetons de fournisseur de liquidité) Qi/MATIC et Qi/WETH.
* Les APRs/APYs indiqués par les applications le 9 septembre 2021.

Les taux ainsi que les prix des jetons vont varier**, c**ertains programmes vont finir, ... **Les résultats finaux sont juste une estimation des gains possibles si tout reste stable, ce qui ne sera jamais le cas.**

### 1er jour

{% hint style="info" %}
**ATTENTION:** Les fermes utilisées ici ont été déployé quelques heures avant la publication de guide. Les APRs/APYs vont changer et des modifications seront apportées d'ici quelques jours. S'il vous plait, **faites vos recherches**.
{% endhint %}

Puisque nous avons $500 de Qi/MATIC LP et $500 de Qi/WETH LP, nous allons les déposer sur Mai Finance et QuickSwap.\
Remarque: si vous avez une préférence pour Mai Finance ou QuickSwap, vous pouvez changer le ratio 50/50 utilisé ici.

* $500 de Qi/MATIC sur Mai Finance, avec une APR de 1160.65%
* $500 de Qi/WETH sur QuickSwap, avec une APR de 1817.44%

Nous utiliserons les APRs suivante pour le reste de la simulation:

* dQUICK via l'Antre du Dragon est de 17.28%
* ADDY via le Syrop du Dragon est de 17.08%
* Qi/QUICK sur Adamant pour les jetons LP est de 133%
* Qi/QUICK sur Adamant pour des ADDY est de 131%
* WMATIC sur Adamant est de 35% des jetons ADDY bloqués

Puisque l'APR sur Mai Finance est plus faible que sur QuickSwap, nous combinerons tous les Qi générés sur Mai Finance avec les QUICK générés par QuickSwap via la ferme Qi/QUICK (jeton Qi/QUICK LP). Il est attendu d'avoir un excès de QUICK. Bien évidemment, si vous avez utilisé une répartition différente pour l'investissement initial vous pourriez avoir un excès de Qi.

Au bout d'un jour, nous avons:

| Jetons générés       | Valeur en dollars |
| -------------------- | ----------------- |
| dQUICK sur QuickSwap | 8.997             |
| ADDY sur QuickSwap   | 0                 |
| Qi/QUICK sur Adamant | 31.799            |
| ADDY sur Adamant     | 0                 |
| WMATIC sur Adamant   | 0                 |

### 2nd jour

le dQUICK déposé dans le Syrop du Dragon de QuickSwap, et la pair Qi/QUICK sur Adamant, commencent à générer de l'ADDY. À la fin de la journée, nous aurions:

| Jetons générés       | Valeur en dollars |
| -------------------- | ----------------- |
| dQUICK sur QuickSwap | 17.998            |
| ADDY sur QuickSwap   | 0.0042            |
| Qi/QUICK sur Adamant | 63.713            |
| ADDY sur Adamant     | 0.114             |
| WMATIC sur Adamant   | 0                 |

N'oubliez pas de récupérer vos récompenses journalières sur Adamant pour commencer à toucher aux dividendes, en WMATIC.

### 3ème jour

L'ADDY récolté sur Adamant commence à générer des dividendes en WMATIC. À la fin de la journée, nous aurions:

| Jetons générer       | Valeur en dollars |
| -------------------- | ----------------- |
| dQUICK sur QuickSwap | 27.004            |
| ADDY sur QuickSwap   | 0.025             |
| Qi/QUICK sur Adamant | 95.743            |
| ADDY sur Adamant     | 0.343             |
| WMATIC sur Adamant   | 0.0001            |

À partir du 4ème jour, nous pouvons:

* Récupérer les dividendes d'Adamant, en WMATIC
* Déposer une partie des WMATIC sur Mai Finance et emprunter du MAI contre
* Échanger le MAI contre du WETH
* Déposer le WMATIC restant avec du Qi générer dans la ferme sur Mai Finance
* Déposer le WETH acquis avec le reste du Qi dnas la ferme sur Quickswap

Ici, le système est complètement opérationel et nous pouvons estimer les revenus.

## Résultat

### Routine quotidienne

Elle est composée des transactions suivantes:

* Récolter le Qi sur Mai Finance
* Récolter le WMATIC sur Adamant
* Déposer 66% du WMATIC sur Mai Finance
* Emprunter du MAI pour 50% du dépot
* Échanger le MAI pour du WETH
* Ajouter à la paire Qi/WMATIC sur QuickSwap
* Déposer les Qi/WMATIC LPs sur Mai Finance
* Ajouter à la paire Qi/WETH sur QuickSwap
* Déposer les Qi/WETH LPs sur QuickSwap
* Récolter le Quick sur QuickSwap
* Ajouter à la paire Qi/QUICK sur QuickSwap
* Déposer le reste du QUICK dans l'Antre du Dragon
* Déposer le dQUICK dans le Syrop du Dragon
* Recolter l'ADDY depuis le Syrop du Dragon
* Récolter l'ADDY sur Adamant
* Déposer du Qi/QUICK sur Adamant
* Déposer l'ADDY récolté sur Adamant (bloquage)

### Résultats mois par mois

| Mois | dQUICK    | Qi/QUICK   | ADDY       | <p>Qi/MATIC <br>Qi/WETH</p> |
| ---- | --------- | ---------- | ---------- | --------------------------- |
| 1    | $280.96   | $1,040.78  | $54.97     | $0.91                       |
| 2    | $557.79   | $2,162.98  | $224.36    | $7.89                       |
| 3    | $842.08   | $3,413.73  | $521.09    | $27.85                      |
| 4    | $1,138.60 | $4,816.62  | $960.17    | $68.48                      |
| 5    | $1,454.30 | $6,405.18  | $1,559.60  | $138.44                     |
| 6    | $1,798.77 | $8,224.86  | $2,341.64  | $247.49                     |
| 7    | $2,184.58 | $10,335.38 | $3,334.13  | $406.84                     |
| 8    | $2,627.76 | $12,813.60 | $4,572.23  | $629.47                     |
| 9    | $3,148.40 | $15,757.01 | $6,100.39  | $930.60                     |
| 10   | $3,771.42 | $19,288.05 | $7,974.83  | $1,328.32                   |
| 11   | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31                   |
| 12   | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79                   |

### Day 365

Après une année complète, l'état final de notre investissement serait:

| Jetons généres                  | Valeur en dollars |
| ------------------------------- | ----------------- |
| dQUICK sur QuickSwap            | 5,628.29          |
| ADDY sur QuickSwap              | 365.25            |
| Qi/QUICK sur Adamant            | 29,733.58         |
| ADDY sur Adamant                | 13,587.56         |
| Qi/MATIC + Qi/WETH additionels  | 2,631.07          |

Note: la simulation étant déjà assez complexe, l'ADDY généré par la ferme sur QuickSwap n'a pas été récolté et ajouté, sur Adamant, quotidiennement. Par ailleurs, nous tenons en compte uniquement l'ADDY investi. Après la période de 90 jours, si vous les récoltez et les bloquez, vous augmentez votre ADDY généré encore plus, générant ainsi plus de WMATIC.

Finalement, après un an, un revenu valant $51,580.50 a été généré; avec un investissement initial de $1,000, cela nous donne une APY de 5,087.39%.\


## Avertissement

**Ce guide n'est pas** **un conseil financier**, il a été écrit a but éducationnel. La variation des prix, de l'offre et de la demande, les dates de fin des programmes, pertes impermanentes, ..., sont **des variables importantes qui n'ont pas été prises en compte ici**.

Le but n'était pas d'écrire une recette à suivre à l'aveugle alors, s'il vous plait, **faites vos recherches et vos propres simulations**, et n'investissez que ce que vous êtes prêts à perdre.

{% hint style="info" %}
Gardez à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut moins bien fonctionner, voir vous faire perdre de l'argent, à un autre. Restez informé, surveillez les marchés et vos investissements, et, encore une fois, **faites vos recherches**.
{% endhint %}
