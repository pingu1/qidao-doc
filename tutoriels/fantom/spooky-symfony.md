---
description: >-
  Contracter un prêt n'est pas exactement contracter une dette lorsque vous utilisez ce prêt comme
  le point de départ d'une stratégie d'investissement. Il s'agit d'un véritable investissement.
---

# A Spooky Symfony

## Introduction

Contracter un prêt contre vos actifs est toujours une arme à double tranchant : cela peut vous aider à lancer une stratégie d'investissement ou à tirer parti de vos actifs, mais vous aurez une dette que vous devrez rembourser à un moment donné. Dans ce guide, nous utiliserons un prêt contracté sur Market.XYZ, un protocole de prêt sur lequel vous pourrez emprunter des MAI avec un faible taux d'emprunt, et utiliserons ce prêt pour farmer la plupart des protocoles éprouvés sur Fantom. Nous utiliserons la stratégie de remboursement du prêt et verrons à quelle vitesse cela peut être fait afin de débloquer les actifs déposés en collateral.

{% hint style="info" %}
Ce guide n'est absolument pas un conseil financier, il a été réalisé dans un but éducatif. Vous devez faire attention aux variations de prix, à l'offre et à la demande, aux programmes de récompense, aux dates de fin, aux pertes impermanentes, etc... Le but n'était pas de proposer des recettes à suivre aveuglément, alors faites vos devoirs et votre propre simulation, et n'investissez que ce que vous êtes prêt à perdre éventuellement.

{% endhint %}

![](<../../.gitbook/assets/spooky-symfony-1.png>)

## Fantom Protocols: Gotta use 'em all

In this strategy, we will use the a lot of different LP (**L**iquidity **P**roviding) pairs on a lot of different protocols, so we thought it would be a good idea to give you a brief recap of what each protocol is doing.

### Market.XYZ

[Market.XYZ](https://fantom.market.xyz/) est un protocole de prêt qui construit plusieurs coffres pour ses partenaires. Vous pourrez déposer des actifs uniques ou des jetons LP comme collateral, et emprunter d'autres actifs contre vos dépôts. Comme vous empruntez contre un collateral, il est important de s'assurer que vous ne serez pas liquidé. Une liquidation se produit lorsque la valeur de l'actif que vous avez déposé en collateral devient inférieure à la valeur de l'emprunt que vous avez contracté. C'est pourquoi il est important de veiller à ce que le rapport entre les deux valeurs reste relativement élevé, et que votre collateral ne perde pas trop de valeur lorsque le marché baisse.

Afin d'atténuer le risque de liquidation, nous utiliserons le jeton FTM-USDC LP comme collateral.

* La perte impermanente (IL) sur cette paire est relativement faible.
* L'USDC est un stable coin liée au dollar américain.
* FTM est le jeton de gaz natif de Fantom, il a une grande liquidité et est utilisé partout.
* Les taux de récompense sur la paire FTM-USDC sont élevés, ce qui signifie que même si le prix de FTM reste le même, la valeur de votre collateral augmentera.

Vous pourrez emprunter contre la paire FTM-USDC à partir du [Spooky LP pool] (https://fantom.market.xyz/pool/10) sur market.xyz. Les étapes pour déposer votre collatéral sont les suivantes :

* Créer [FTM-USDC LP tokens on SpookySwap] (https://spookyswap.finance/add/FTM/0x04068DA6C83AFCFA0e13ba15A6696662335D5B75) en fournissant des liquidités dans un rapport 1:1 pour les deux actifs.
* Déposez le jeton FTM-USDC LP sur Beefy finance pour obtenir un reçu mooBooFTM-USDC (recherchez la plateforme SpookySwap et l'actif USDC dans les filtres de recherche).
* Déposer le jeton de reçu mooBooFTM-USDC sur Market.xyz

![Marché de prêt de Spooky sur MarketXYZ à partir de février 2022](<../../.gitbook/assets/spooky-symfony-2.png>)

Lorsque vos jetons de reçu LP beefy sont sur Market.XYZ, vous obtenez toujours la récompense APY fournie par Beefy. Cela signifie que vos actifs continuent à générer des rendements pour vous pendant que vous empruntez . C'est un outil très puissant, surtout quand vous voyez que le mSPLP-FTM-USDC (**m**oo **S**pookyswa**p** FTM-USDC = mooBooFTM-USDC) rapporte 51,4% d'APY et que vous pouvez emprunter MAI à 2,56% APR. En d'autres termes, votre garantie croît plus vite que votre dette, donc en théorie vous pouvez très bien rembourser votre prêt avec les intérêts de votre garantie.


{% hint style="info" %}
Accessoirement, vous pouvez voir que le vault Spooky LP Pool offre également la possibilité d'emprunter contre d'autres jetons LP : ETH-FMT, DAI-FTM, BTC-FTM et fUSDT-FTM. En fonction des actifs que vous avez dans votre portefeuille, de vos convictions et de votre tolérance au risque, vous pouvez tout à fait utiliser n'importe quel LP de Spookyswap comme garantie.
{% endhint %}

Pour ce tutoriel, nous allons également limiter le risque en empruntant avec un CDR (**C**collatéral à **D**dette **R**atio) de 200%. Cela signifie que nous emprunterons 50 % de la valeur de notre garantie. Plus d'informations dans la section sur la stratégie agricole. Les ratios de liquidation sont exprimés en LTV (**L**oan **t**o **V**alue) qui est l'opposé d'un CDR. Vous pouvez voir que le LTV pour le jeton mooBooFTM-USDC est de 60%, au-delà duquel vous serez liquidé. Cela équivaut à un CDR de 166,67%. Avec un objectif de 200% de CDR, nous sommes 33% au-dessus du ratio de liquidation, ce qui peut être risqué ou non, en fonction de votre tolérance au risque.

{% hint style="danger" %}
Market.XYZ n'autorise que les prêts d'une valeur minimale de 0,05 ETH (~$170.00 au moment de la rédaction). Assurez-vous de déposer suffisamment de garanties si vous souhaitez emprunter dans les différents coffre.
{% endhint %}

### BeethovenX

[BeethovenX](https://beets.fi/#/) est une **D**ecentralized **Ex**change et **A**utomated **M**arket **M**aker fork de Balancer. Vous serez en mesure de déposer vos actifs dans des pools de liquidité, ainsi que d'échanger différents actifs sur leur application. Ils ont été de solides partenaires du protocole QiDAO, fournissant des jetons LP pour les positions de farming que vous pouvez trouver sur Mai Finance. Nous allons utiliser deux pools différents sur BeethovenX pour cette stratégie

* Le Monolithe : un pool inventif qui a été ouvert pour Exodia, un fork Ohm que [nous avons présenté dans ce tutorial] (investing-in-discounted-assets-using-bonds.md). Vous pourrez déposer vos jetons MAI directement dans ce pool et collecter des rendements
* Pirate Party : un pool incentivé dédié aux jetons LQDR, le jeton natif de Liquid Driver, un autre gros protocole que nous utiliserons dans ce guide

![Le pool Monolith sur BeethovenX avec 20% de MAI en février 2022](<../../.gitbook/assets/spooky-symfony-3.png>)

![Pool Pirate Party sur BeethovenX avec 80% de LQDR en février 2022](<../../.gitbook/assets/spooky-symfony-4.png>)

Comme toujours, le plus grand avantage d'utiliser BeethovenX (ou Balancer) est que vous pouvez déposer des actifs uniques dans les pools au lieu de devoir fournir des jetons dans un ratio équilibré.

### SpookySwap

[Spookyswap](https://spookyswap.finance/) est le plus grand fork Uniswap V2 sur Fantom, une plateforme où vous pourrez échanger des actifs et fournir de la liquidité pour de nombreuses paires. Spookyswap a également été un partenaire solide de Mai Finance et propose un pool MAI-USDC. Le partenariat s'est étendu via Market.XYZ où vous pourrez emprunter du MAI contre certaines paires LP spécifiques (voir la section sur Market.xyz) ainsi que vos tokens BOO et BOO staked, le token natif de Spookswap.

Pour ce guide, nous allons utiliser deux jetons LP différents de SpookySwap :

* FTM-USDC qui sera utilisé comme point de départ de la stratégie. Ce jeton LP est utilisé comme garantie sur market.xyz.
* FTM-BOO car c'est l'un des pools de SpookySwap accepté sur Liquid Driver avec le plus haut APR. Nous échangerons les récompenses BEETS du Monolithe contre cette paire (plus d'informations dans la section Stratégie).

### Liquid Driver

[Liquid Driver](https://www.liquiddriver.finance/) est un optimiseur de rendement sur lequel vous pourrez déposer des jetons LP de différentes fermes et gagner des rendements sur ceux-ci. Le fonctionnement de l'optimiseur de rendement consiste à récolter les jetons de récompense de la plateforme cible et à les composer pour vous. Ceci est utile car l'essence sur Fantom peut être chère. Une commission de performance est prélevée, mais une partie des revenus du protocole est redistribuée aux stakers LQDR. LQDR est le jeton natif de Liquid Driver.

Pour cette stratégie, nous utiliserons la paire de LP FTM-BOO car c'est un pool avec l'un des plus hauts APR en LQDR pour Spookyswap.

![Paires de LP FTM-BOO et FTM-USDC sur LiquidDriver en février 2022](<../../.gitbook/assets/spooky-symfony-5.png>)

## Stratégie d'exploitation

Pour cette stratégie, nous utiliserons Market.XYZ comme point de départ pour emprunter des MAI contre des jetons mooBooFTM-USDC LP. Les MAI empruntés seront déposés sur BeethovenX dans le pool The Monolith. Comme il s'agit du pool avec le taux de récompense le plus élevé dans notre stratégie, nous l'utiliserons comme moteur pour rembourser notre dette : 50% des BEETS seront vendus pour rembourser la dette sur Market.xyz, et 50% seront convertis en jetons FTM-BOO LP. Les jetons FTM-BOO seront déposés sur LiquidDriver pour collecter des jetons LQDR qui seront ensuite mis en jeu dans le pool Pirate Party sur BeethovenX. Une fois la dette entièrement remboursée, les récompenses BEETS seront entièrement converties en jetons FTM-BOO. Les récompenses BEETS fournies par le pool du Parti Pirate seront également composées en plus de FTM-BOO.

Pour cette simulation, nous allons utiliser les chiffres suivants

* Nous commençons avec une valeur de 1000 $ de jetons mooBooFTM-USDC.
* L'APR pour le jeton mooBooFTM-USDC fourni par SpookySwap via Beefy est de 41,5%.
* Le taux d'emprunt pour MAI est de 2,56%.
* BeethovenX donne un taux d'intérêt annuel de 304,17 % pour le Monolithe et de 175,77 % pour le Parti Pirate.
* LiquidDriver donne un APR de 82% pour la paire de LP FTM-BOO.

Comme d'habitude pour nos simulations, nous supposons que tous les prix restent les mêmes pendant toute la période d'un an, que les taux restent les mêmes, et nous utilisons également les TAEG fournis tels quels. En réalité, les prix et les taux varieront, et les TAEG sont composés de frais de transaction et de jetons de récompense, ce qui peut affecter le résultat final. Il est également important de noter que **aucun frais de transaction** n'est pris en compte pour cette simulation. Enfin, nous utilisons un grand nombre de protocoles, et chaque protocole peut présenter des risques liés aux contrats intelligents. Assurez-vous de faire vos propres recherches avant d'utiliser une plateforme, et n'investissez que ce que vous êtes prêt à perdre.

Vous pouvez trouver notre simulation Spooky Symfony [dans cette feuille de calcul] (https://docs.google.com/spreadsheets/d/19s6kBnT5w0b9GKuTkDiiD1u_ZoeNUZtI9XYxEmk_WM0/edit?usp=sharing). N'hésitez pas à la copier et à jouer avec elle pour voir comment la boucle fonctionne, et comment les différents taux peuvent affecter votre APY final.

![](<../../.gitbook/assets/spooky-symfony-6.png>)

### Jour 1

Le jour 1, vous devez créer votre collatéral pour Market.xyz. Obtenez une portion égale de FTM et d'USDC et fournissez la liquidité sur SpookySwap pour créer des tokens FTM-USDC LP. Ces jetons seront déposés sur Beefy, ce qui vous permettra d'obtenir le jeton de réception mooBooFTM-USDC. C'est ce jeton qui sera utilisé comme garantie sur Market.xyz et contre lequel vous emprunterez l'AMI. Comme nous voulons garder un CDR de 200%, nous emprunterons 500$ de MAI. Enfin, les jetons MAI seront placés sur BeethovenX dans le pool The Monolith.

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

On Day 2, you will have to

* sell 50% of your BEETS for MAI to repay a small fraction of your loan
* swap your BEETS rewards for FTM-BOO LP pair. You can either swap on BeethovenX and create the LP pair on SpookySwap, or do everything on SpookySwap.
* stake the FTM-BOO LPs on Liquid Driver to start collecting LQDR tokens.

At the end of the second day, you will have

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

Repeat the operation from Day 2, then harvest your first LQDR tokens. These will be deposited on BeethovenX in the Pirate Party pool to get extra BEETS rewards, and at the end of Day 3 you will have

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
Gains from the Pirate Party pool are too small to be significant at this point, but you'll get some over time.
{% endhint %}

### Daily Routine

At this point the system is fully primed. Your daily routine will consist of

* harvest BEETS rewards from The Monolith
* harvest BEETS rewards from the Pirate Party
* swap 50% of the BEETS for MAI if you still have an outstanding debt
* repay a portion of your debt if you still have some
* swap the rest of the BEETS for FTM-BOO LP tokens
* deposit the FTM-BOO on LiquidDriver
* harvest LQDR
* deposit in the Pirate Party

This strategy isn't very gas-efficient so you may consider compounding your gains only once a week, or even less frequently.

### Raw results month after month

Here are raw results month after month, as you can get them in the Google SpreadSheet linked above.
 
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

### Day 365

At the end of one full year farming this system, you would have

* $1,512.294 worth of FTM-USDC tokens on Market.xyz
* $500.000 worth of MAI in The Monolith pool
* $382.353 worth of LQDR stored in the Pirate Party pool
* $1.211.845 worth of FTM-BOO tokens on Market.xyz
* a final debt that is fully repaid after day #243

This is equivalent to a total APY of 260.65%.

### Effect of the debt repayment on the overall result

In most of our guides, we don't repay any debt as part of the strategy. This is, in most cases, due to the fact that we're using a 0% interest loan taken on Mai Finance. Here, we are borrowing on Market.XYZ with a borrowing rate of 2.56% and we repay the debt with 50% of the BEETS harvested from The Monolith.

If you allocate more than 50% to the debt repayment, you will pay less interests, but you will grow your positions much slower on Liquid Driver. If you allocate less than 50% to the debt repayment, you will get more rewards from the other platforms, but you will also pay more interests on Market.xyz.

Here's a small table that indicates the effect of the allocated BEETS to your debt repayment on your overall APY:

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

If you use less than 33.5% of your BEETS rewards to repay your debt, you will still have some MAI to repay after a complete year.

It is also good to understand that it you repay faster, you also increase your CDR in a more significant way, which allows you to get away from liquidation ratio faster.

## Variations to consider

This strategy presents many variations that present different benefits.

### Mai Finance VS Market.xyz

You can totally borrow MAI from [Mai Finance](https://app.mai.finance) at 0% interest. As an example, if you use mooScreamFTM instead of mooBooFTM-USDC as collateral, this will present the following advantages:

* You don't have any impermanent losses on your collateral
* You borrow at 0% with a single 0.5% repayment fee, which will be in most cases, much lower than the interests you will pay on Market.xyz (if there are MAI to borrow for this vault)
* You may get Qi rewards for borrowing on the platform, which will let you participate in the protocole's governance, as well as get dividends if you stake your Qi tokens. This will increase your yearly gains
* You're protected from very fluctuating borrowing rate on  Market.xyz. Mai Finance will lend new MAI regularly to keep the borrowing rates as low as possible but it's not a guarantee that it does not go up. You can check metrics for the lending market [here](https://metrics.market.xyz/d/HChNahwGk/fuse-pool-details?orgId=1&refresh=10s&var-poolID=10&var-chain=250).

However, the mooScreamFTM tokens get a much lower APY compared to the mooBooFTM-USDC tokens, so you may miss on that.

### Stake your LQDR

If you stake your LQDR instead of using it in the Pirate Party pool, you will earn some dividends from Liquid Driver that are paid in different assets (LQDR, WFTM, LINSPIRIT, BOO, SPELL and BEETS). You will also get xLQDR that will let you participate in the governance of Liquid Driver, and possibly LINSPIRIT to vote on reward allocation on Spirit Swap. Please check the [xLQDR](https://www.liquiddriver.finance/xlqdr) page carefully for more details.

### Stake your BEETS

If BEETS from The Monolith play a high role in this strategy, you can totally use the ones from the Pirate Party as follows:

* deposit the BEETS in the Fidelio Duetto pool (BEETS-FTM)
* stake the LP token on BeethovenX to receive fBEETS
* stake your fBEETS to get protocol dividends

This will also let you vote on BeethovenX protocol improvements, as well as on the reward allocation for the different pools on the platform. This is particularly useful to keep a high APR on The Monolith.

### Use the FTM-BEETS pool on Spookyswap

In our strategy, we're selling all the BEETS rewards from The Monolith. However, you could also integrate the FTM-BEETS pool from Spookyswap in your loop. You would have to sell 50% of your BEETS for FTM and combine the two tokens into a new LP pair that will earn you BOO. You can then decide to create the FTM-BOO and deposit on Liquid Driver, or you can stake your BOO on SpookySwap. Note that if you stake your BOO, you will have the possibility to deposit the xBOO receipt tokens and earn LQDR tokens directly, and you can even use the xBOO tokens as collateral on Market.xyz. This additional lego brick opens many possibilities.

{% hint style="info" %}
Keep an eye on this particular pair in case it becomes available on Liquid Driver. This may be a better option than the FMT-BOO one.
{% endhint %}

### Use your FTM-USDC on Liquid Driver

After your loan is fully repaid, you can keep the mooBooFTM-USDC tokens on Market.xyz or on Beefy, they will continue accruing rewards. However, you can also remove the LP pair from Beefy and deposit it on Liquid Driver to get more LQDR.

As a side note, while you're repaying your loan, the value of your Collateral to Debt Ratio grows (collateral is compounding rewards and grows in value while the debt is shrinking after each partial repayment). This means that you can withdraw the collateral pieces by pieces in order to keep a safe CDR, and deposit them on Liquid Driver for more LQDR tokens.

### Keep a little profit leak

This system is a closed loop that feeds itself. However, you can very well continue selling parts of your BEETS for other assets after you're done repaying your loan on Market.xyz. As an example, you could convert your BEETS rewards into USDC or another stable, or increase one of your positions that earns more rewards than the ones granted for the FTM-USDC pair.

## Disclaimer

This guide was mostly designed to showcase the way you can repay a debt using farming yields. The speed at which you repay your debt will highly influence the global reward rate, but also presents some very positive aspects, the main one being lowering the risk of liquidation.

Of course, you can very easily cut corners with this strategy, change pieces of the loop for some other ones, replace protocols with something you prefer etc ... However, make sure to read all the documentation available for the protocols that you want to use, and make sure you understand all the different risks.

{% hint style="info" %}
This guide is definitely not financial advice, it was made with an educational goal in mind. You need to pay attention to price variations, supply and demand, reward programs, end dates, impermanent losses etc ... The goal wasn't to propose recipes that can be followed blindly, so please do your homework and your own simulation, and only invest what you're ready to possibly lose.
{% endhint %}
