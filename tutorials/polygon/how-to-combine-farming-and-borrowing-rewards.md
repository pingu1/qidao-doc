---
description: >-
  Auf dieser Seite erfährst du, wie du Yield Farming mit den Belohnungen von Mai
  Finance kombinieren kannst, um deine Gesamtrendite zu steigern.
---

# So kombinierst du Belohnungen aus Farming und Vault-Belohnungen

## Einleitung

Im September 2021 führte Mai Finance Vault Belohnungen ein, um das Kreditgeschäft zu fördern und die Leute dazu zu bringen, ihre Token zu benutzen, um MAI zu leihen. Es geht nicht nur darum, einen Kredit mit 0% Zinsen und einer geringen Rückzahlungsgebühr aufzunehmen, jetzt können sich die Leute auch dafür bezahlen lassen, Geld zu leihen. In diesem Leitfaden wird eine Strategie vorgeschlagen, die auf dem Stable Coin-Farming basiert und Augury Finance als Quelle für Token nutzt, die die Vaults von Mai Finance füttern, was zu hohen Kreditanreizen und zusätzlichem MAI führt, das dann wieder in die Farm eingespeist wird.

![](<../../.gitbook/assets/image (7).png>)

### Vorstellung der Anwendung und der PoolsAugury Finance

Augury Finance ist ein Rendite-Aggregator, der sich nicht darauf konzentriert, deine LP (**L**iquidität **P**ool) Token automatisch zu vermehren. Stattdessen verkauft Augury automatisch die Farm-Token der Farmen, die es nutzt, um andere Token in ihren _Infusionen zu kaufen._

Du kannst zum Beispiel das Paar DFYN-WETH auf Augury farmen

![Beispiel: DFYN-WETH pool auf Augury Finance](<../../.gitbook/assets/image (32).png>)

Diese Infusion nutzt DinoSwap als zugrunde liegende Farm und ein LP-Token, das man auf DFYN erhalten kann. Mit einem effektiven Jahreszins von 123,43% werden Nutzer, die Liquidität in diesen Pool einzahlen, belohnt mit

* 30% von WETH
* 20% von LINK
* 20% von WBTC
* 15% von USDT
* 15% von WMATIC

Wenn du auf DinoSwap farmst, wirst du mit DINO-Tokens bezahlt, deren Preis sehr volatil ist. Bei anderen Aggregatoren wie Adamant oder Beefy würdest du deine LP-Position erhöhen, aber bei Augury "sicherst" du deine Position, indem du Token bekommst, die weniger stark schwanken können. Der Nachteil ist, dass deine anfängliche Position im Laufe der Zeit nicht wächst, da 100% der geernteten DINO in die Token umgewandelt werden, aus denen die Belohnung bei Augury besteht.

{% hint style="info" %}
Augury Finance verwendet 3 verschiedene Infusionstypen, die unterschiedliche Einzahlungsgebühren und Leistungsgebühren haben. Bitte informiere dich über die verschiedenen Stufen und vergewissere dich, dass du ihre Auswirkungen auf deine Anbaustrategie verstehst.
{% endhint %}

In unserer Strategie werden wir die USDT-UST-Tier2-Farm nutzen, die Nutzer mit einer Mischung aus WETH/WBTC/LINK/WMATIC/USDC belohnt, da Mai Finance 4 Vaults für 4 der 5 Token anbietet, die wir als Belohnung erhalten werden. Um unsere Gewinne zu maximieren, werden wir AAVE zwischen dem Output von Augury und den Vaults auf Mai Finance einfügen, da 3 der 5 Token, die wir ernten werden, auf AAVE ausgeliehen werden können.

![Stable coin Farm: USDT-UST für unsere Strategie](<../../.gitbook/assets/image (31).png>)

### Curve

Curve ist ein Blue-Chip-Projekt, das Nutzer belohnt, die Blue-Chip-Token verleihen. Die Belohnung setzt sich aus automatisch zusammengesetzten Token (die der Investition wieder hinzugefügt werden), WMATIC-Tokens und CRV-Tokens zusammen, zwei Token, die auch als Sicherheiten bei Mai Finance akzeptiert werden.

Eines der interessantesten Dinge an Curve und seinen Pools ist, dass man für einen bestimmten Pool nicht die genaue Menge jedes Tokens hinterlegen muss. Stattdessen kann man einen einzelnen Token angeben und der Algorithmus, der den Pool verwaltet, passt die anderen Token automatisch an, indem er einen Teil der Einlage verkauft und die anderen Token kauft, um das richtige Verhältnis im Pool aufrechtzuerhalten.

Wir werden den atricrypto3-Pool verwenden, der jede Kombination von WBTC/WETH/USDC/USDT/DAI akzeptiert, und wir werden diesem Pool die USDC hinzufügen, die der Pool im August generieren wird.

![Details vom atricrypto3 Pool auf Curve, Stand: September 2021](<../../.gitbook/assets/image (30).png>)

### AAVE

Wie bereits im Abschnitt über Augury erwähnt, wird AAVE verwendet, um eine kleine Belohnung zu den auf Augury gefarmten Token hinzuzufügen, bevor wir sie auf Mai Finance verwenden. Anstatt unsere WBTC, WETH und WMATIC direkt auf Mai Finance zu deponieren, werden wir diese Token auf AAVE hinterlegen und das Renditeinstrument von Mai Finance nutzen, um die Belohnungen von AAVE in den amToken-Pools automatisch zu verdoppeln und die camToken als Sicherheiten in Vaults zu verwenden. Weitere Details zu diesem Teil findest du im [Tutorial über AAVE-Token](leverage-aave-tokens.md).

![AAVE Belohnungen, Stand September 2021](<../../.gitbook/assets/image (29).png>)

### Balancer

Balancer ist ein weiteres Blue-Chip-Projekt wie Curve. Du kannst bestimmte Token in Pools einzahlen, die aus mehr als 2 Token bestehen, und du zahlst einen einzigen Token ein. Der Pool wird automatisch so ausgeglichen, dass jeder Token, aus dem sich der Pool zusammensetzt, zu gleichen Teilen enthalten ist.

Für unsere Strategie werden wir den Pool WETH/BAL/Qi/MAI/USDC verwenden. Dieser Pool nimmt die Qi-Token auf, die in den Vaults von Mai Finance gesammelt werden, und belohnt uns mit zusätzlichen Qi und BAL-Token, die wir auf Mai Finance im BAL Vault deponieren können, damit wir mehr MAI prägen und unsere Farming-Position auf Augury erhöhen können.

![Balancer 5-pool , Stand September 2021](<../../.gitbook/assets/image (23).png>)

## Starten wir das System

![](<../../.gitbook/assets/image (19).png>)

Im Folgenden wird eine Simulation mit einer Anfangsinvestition von ETH im Wert von $1.000 erzeugt, die im camWETH Vault hinterlegt wird, um MAI im Wert von $500 zu leihen, die in USDT-UST im Wert von $500 umgewandelt werden. Diese Simulation geht von folgenden Belohnungen für die verschiedenen Systeme aus

* USDT-UST Farming APR von 22,53%
* amWBTC APR von 0,39%
* amWETH APR von 1,71%
* amWMATIC APR von 3,80%
* atricrypto3 APR von 3,86% auto-compounded LP token, 13,09% WMATIC und 17,63% CRV
* 5-Token Balancer Pool mit APR von 43,46% bei einem BAL:Qi Verhältnis von 1:6
* Vault Belohnungen APRs von
  * 23,28% für camWBTC
  * 21,52% für camWETH
  * 32,93% für camWMATIC
  * 24,51% für LINK
  * 116,71% für CRV
  * 62,38% für BAL

Diese APRs können sich auf den verschiedenen Plattformen ändern, und es gibt keine Garantie dafür, dass sie ein ganzes Jahr lang gelten, aber wir nehmen sie für diese Simulation so an, wie sie sind, um eine Vorstellung von der möglichen Gesamt-APR des Systems zu bekommen. Um die Simulation weiter zu "vereinfachen", werden wir weder Preisschwankungen noch Transaktionsgebühren berücksichtigen. Außerdem wird bei dieser Simulation berücksichtigt, dass die Belohnungen für den Vault bei Mai Finance und den Balancer täglich statt wöchentlich aufgezinst werden, während diese Belohnungen derzeit wöchentlich per Airdrop auf die Wallet der Nutzer/innen übertragen werden. Schließlich nehmen wir für diese Simulation an, dass der CDR (**C**Sicherheiten zu **D**Schulden **R**atio) immer 200% beträgt, d.h. wir leihen uns nur die Hälfte dessen, was wir eingezahlt haben, um die Belohnungen zu erhalten, aber einfache Liquidationen zu verhindern.

### Tag 1

Wenn du noch WETH im Wert von $1.000 hast, zahle es auf AAVE ein, um amWETH zu erhalten, dann zahle dein amWETH auf [Mai Finance](https://app.mai.finance/yield) ein, um camWETH zu erhalten, und schließlich zahle dein camWETH in den entsprechenden Vault ein, um 500 MAI leihen zu können.

Verwende den [Anchor](https://app.mai.finance/anchor), um deine MAI in USDT umzuwandeln (oder verwende einen anderen DEX wie [QuickSwap](https://quickswap.exchange/#/), wenn es im Anchor keine Liquidität gibt), dann kannst du mit [DFYN](https://exchange.dfyn.network/#/) 50% deiner USDT in UST tauschen und ein USDT-UST-Paar bilden, das du dann auf [Augury](https://augury.finance/infusions/) einzahlen kannst. Beachte, dass du auch einige OMEN benötigst, die du bei QuickSwap kaufen kannst.

Am Ende von Tag 1 ernten wir also die folgenden Belohnungen

| Belohnungstyp                 | Wert in Dollar |
| ----------------------------- | -------------- |
| WBTC aus Farming              | 0.123          |
| WETH aus Farming              | 0.031          |
| WMATIC aus Farming            | 0.031          |
| LINK aus Farming              | 0.031          |
| USDC aus Farming              | 0.092          |
| Qi Belohnungen aus den Vaults | 0.295          |

Das sind nur die Belohnungen, die wir am Ende des ersten Tages vom Farmen und Leihen bekommen.

### Tag 2

Belohnungen werden geerntet, WBTC, WETH und WMATIC werden an die entsprechenden Vaults auf Mai finance geschickt, nachdem sie AAVE und das Rendite-Instrument auf Mai getroffen haben. LINK werden direkt in den LINK Vault eingezahlt und USDC werden an Curve im atricrypto3 Pool geschickt. Die Qi Belohnung wird an Balancer gesendet. Zu diesem Zeitpunkt können wir weitere MAI aus den 3 camToken Vaults und dem LINK Vault leihen (genau gesagt MAI im Wert von 0,13 USD) und mit den geliehenen MAI weitere USDT-UST Paare erstellen.

Am Ende von Tag 2 ernten wir also die folgenden Belohnungen

| Belohnungstyp                 | Wert in Dollar |
| ----------------------------- | -------------- |
| WBTC aus Farming              | 0.123          |
| WETH  aus Farming             | 0.031          |
| WMATIC  aus Farming + Curve   | 0.031          |
| LINK  aus Farming             | 0.031          |
| USDC  aus Farming             | 0.093          |
| CRV Belohnungen von Curve     | 0.00004        |
| BAL Belohnungen               | 0.00005        |
| Qi Belohnungen aus den Vaults | 0.296          |

An diesem Punkt ist das System vorbereitet und die Belohnungen fließen so, dass jeder Schritt den nächsten nach sich zieht und eine nette kleine Schleife entsteht.

## Farming Ergebnisse

### Täglicher Ablauf

Der Tagesablauf setzt sich aus den folgenden Vorgängen zusammen

* Belohnungen auf Augury ernten
* Einzahlung von WBTC, WETH und WMATIC auf AAVE
* Einzahlung von amWBTC, amWETH und amWMATIC auf Mai Finance in das Rendite-Instrument
* Hinterlege camWBTC, camWETH und camWMATIC in den jeweiligen Vaults auf Mai Finance
* Einzahlung von LINK in den LINK Vault auf Mai Finance
* Einzahlung von USDC in den atricrypto3-Pool auf Curve
* Sammle WMATIC von Curve und verwende sie im camWMATIC Vault
* Sammle CRV von Curve und verwende sie im CRV Vault
* Leihe MAI aus den verschiedenen Vaults
* Wandle MAI bei Mai Finance über den Anchor in USDT um
* Wandle 50% der USDT in UST auf DFYN um
* Erstelle ein neues USDT-UST LP-Paar auf DFYN
* Deponiere die neuen LP-Tokens bei Augury

### Wöchentliche Zusatzroutine

Außerdem erhältst du wöchentliche Belohnungen in BAL (von deiner Qi-Einzahlung auf Balancer) und Qi-Token (von den Belohnungen im Vault). Dazu musst du

* Den Qi-Token auf Balancer einzahlen
* Den BAL-Token bei Mai Finance im BAL Vault deponieren
* Leih dir MAI von deiner zusätzlichen BAL-Einzahlung und wandle sie in USDT-UST um, um auf Augury zu farmen

### Rohergebnisse über die Monate

| Monat | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |
| ----- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- |
| 1     | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |
| 2     | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |
| 3     | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |
| 4     | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |
| 5     | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |
| 6     | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |
| 7     | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |
| 8     | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |
| 9     | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |
| 10    | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |
| 11    | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |
| 12    | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |

Ein paar Anmerkungen:

* Das Wachstum des USDT-UST-Pools ist das einzige Ergebnis von zusätzlichem MAI, das von Vaults geliehen wurde.
* Der CRV-Pool ist aufgrund der sehr geringen Menge an USDC, die auf Curve eingezahlt wurde, fast inexistent.
* Der BAL Vault ist unbedeutend, da 14,28% der Belohnung für Balancer in BAL-Token ausgezahlt werden, der Rest in Qi-Token
* Der Betrag im Balancer-Pool ist der größte Gewinn und ergibt sich nur aus den Belohnungen für Vault und Balancer

### Tag 365

Nach einem ganzen Jahr wäre der Endzustand unserer Investition:

| Position    | Wert in Dollar |
| ----------- | -------------- |
| USDT-UST    | 553.24         |
| atricrypto3 | 36.20          |
| Balancer    | 137.62         |
| camWBTC     | 47.45          |
| camWETH     | 1,029.19       |
| camWMATIC   | 14.39          |
| LINK        | 11.84          |
| CRV         | 0.017          |
| BAL         | 3.93           |

Die Gesamtschuld ist die gesamte USDT-UST-Position, also $553,24, und die gesamte Belohnung beträgt $280,63, was einem effektiven Jahreszins von 28,06% entspricht.

### Vergleich mit anderen Strategien&#x20;



28% APY beim Farmen von Stable Coins sind nicht schlecht, aber wie sieht das im Vergleich zu anderen, einfacheren Strategien aus, die wir mit ETH im Wert von $1.000 anwenden können? Schauen wir uns die endgültigen APY für die folgenden Strategien an

* 8-fache Hebelung von amWETH über AAVE: Hierfür verwenden wir den genauen Ablauf, der im [AAVE token guide](leverage-aave-tokens.md) beschrieben ist.
* Vollständig stabiles Farmen auf Augury: Bei dieser Strategie verkaufen wir das WETH und farmen mit USDT-UST im Wert von $1.000 auf der gleichen Infusion auf Augury.
* Vollständig stabiles Farmen auf QuickSwap: Bei dieser Strategie nutzen wir den camWETH Vault, um von der Belohnung im Vault zu profitieren, und farmen mit MAI im Wert von $500 auf QuickSwap (MAI-DAI zu 19,78% APY), wobei wir den dQUICK Vault auf Mai Finance nutzen, um zusätzliche MAI zu leihen und wieder in den Farmpool zu investieren (dQUICK Vaults mit einem APR von 55,72%)

| Strategie                       | Finales APY |
| ------------------------------- | ----------- |
| Strategie in diesem Guide       | 28.06%      |
| Hebel AAVE Token 8x             | 46.46%      |
| Nur Stable-coin Farm auf Augury | 22.53%      |
| Quickswap Farm + dQUICK vault   | 35.96%      |

## Haftungsausschluss

Diese Strategie ist wirklich interessant und nutzt die meisten Vaults von Mai Finance. Dieser Leitfaden wurde vor allem geschrieben, um zu zeigen, dass dies ab September 2021 der Teil ist, der die meisten Belohnungen beim Faming von Stable Coins bringt. Allerdings ist diese Strategie nicht unbedingt die interessanteste und beinhaltet eine Menge Handgriffe auf verschiedenen Plattformen. Schließlich ist Augury ein fantastisches Tool, das spezielle Token generiert, die in verschiedene Strategien eingebunden werden können, aber wahrscheinlich nicht ausschließlich zum Farmen von Stables. Übrigens: Bei der Berechnung des endgültigen APY wurden weder Einzahlungsgebühren noch Performancegebühren berücksichtigt.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
