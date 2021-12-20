---
description: >-
  In diesem Artikel wird ausführlich erklärt, wie du Mai Finance nutzen kannst,
  um MAI zu 0 % Zinsen zu leihen und dich dafür bezahlen zu lassen, indem du
  dein 0 %-Zins-Darlehen in ein Negativzins-Darle
---

# MAI Kredite und Vault-Anreize

## Intro

Mai Finance ist in erster Linie eine Kreditplattform. Anstatt deine Kryptowährungen zu verkaufen, um andere Vermögenswerte zu kaufen, bist du in der Lage, deine Investitionen auf Mai Finance zu parken und gegen sie zu leihen. Dies bietet die Möglichkeit, hochwertige Vermögenswerte (WBTC, WETH ...) zu behalten und gleichzeitig andere Vermögenswerte und Farmin-Erträge zu erhalten. In diesem Fall wird das Darlehen zur Erzielung von Einnahmen verwendet, während die Sicherheiten an Wert gewinnen.

Ein weiterer großer Vorteil von Mai Finance ist, dass es keinen Rückzahlungsplan gibt. Mit anderen Worten: Du leihst dir MAI Stable Coin gegen deine Kryptowährung, du zahlst keine Zinsen und kannst deine Schulden zurückzahlen, wann immer du willst. Siehe die verschiedenen Artikel auf [Schuldenmanagement ](../debt-management-tutorials/debt-repayment-why-and-when.md)für weitere Details. Die einzige Gebühr, die du jemals zahlen wirst, ist eine Rückzahlungsgebühr in Höhe von 0,5 % des geliehenen Geldes, die du bei der Rückzahlung deines Kredits zahlst und die von deiner Sicherheit abgezogen wird.

Wenn Sie zum Beispiel WETH im Wert von $200 hinterlegt haben, um MAI im Wert von $100 zu leihen, müssten Sie bei der Rückzahlung Ihres Kredits eine Gebühr von $0,50 zahlen, die direkt von Ihrer WETH-Einlage abgezogen wird.

Wäre das nicht so schon eine tolle Möglichkeit, hat das Mai Finance-Team im September 2021 Vault-Anreize eingeführt, die in Qi, dem nativen Token von Mai Finance, bezahlt werden. Mit anderen Worten, wenn du dein Vermögen auf Mai Finance in einem Vault hinterlegst, um MAI zu leihen, wirst du auch dafür bezahlt. Dieser Artikel beschreibt im Detail, wie diese Funktionalität funktioniert.



## Vaults - Was sie sind und wie sie funktionieren

### Vaults erstellen

Bei Mai Finance sind Vaults spezielle Konten, in denen man seine Kryptos hinterlegen kann. Derzeit gibt es 10 Arten:

![Die unterschiedlichen Vaults auf Mai Finance](<../.gitbook/assets/image (1).png>)

Dabei lassen sich zwei Gruppen unterteilen:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

and

* camWETH
* camWBTC
* camWMATIC
* camAAVE

Die ersten 6 Vaults in der Liste sind für einfache Vermögenswerte, während die letzten 4 für camTokens sind. camTokens sind zusammengesetzte AAVE-Markt-Tokens, eine Darstellung einer Einzahlung, die du auf AAVE gemacht hast und dann auf den Ertragspools von Mai Finance hinterlegt hast. Während dein Vermögen Renditen auf AAVE generiert (und während die Belohnungen automatisch durch den Renditepool aufgezinst werden), kannst du immer noch MAI Stable Coins gegen diese Token leihen.

Als Randbemerkung, zeigt der Screenshot oben, dass die Erstellungsseite einige sehr wichtige Informationen anzeigt:

* Verfügbare MAI: Dies entspricht der maximalen Verschuldungsgrenze, also der maximalen Anzahl von MAI, die aus Tresoreinlagen geprägt werden können.
* Min. Coll. ratio: dies ist das minimale Collateral to Debt ratio (CDR) für diesen Vault
* Vault-Anreize APR

### Das Schuldenlimit

Die maximale Anzahl an MAI, die man in einem bestimmten Tresor prägen kann, hängt davon ab, wie viel Vermögen in diesem Tresor hinterlegt ist. Schuldenobergrenzen sollen sicherstellen, dass der Markt nicht innerhalb kürzester Zeit mit MAI überschwemmt wird, was den Preis des Stable Coin beeinflussen könnte.

Wenn beispielsweise eine große Institution 5.000 WBTC auf einmal einzahlt und MAI im Wert von 100.000.000 $ leihen könnte, um sie gegen weitere WBTC einzutauschen, könnte dies den Preis von MAI so weit nach unten treiben, dass der Preis zu stark von seiner Bindung abweicht, was die gesamte Plattform gefährden würde. Die Schuldenobergrenze ist der Mechanismus, der dies verhindert: Es gibt eine Höchstmenge an MAI, die für einen bestimmten Tresortyp geprägt werden kann.

Wenn die Schuldenobergrenze erreicht ist, wird der Zeitpunkt festgehalten, an dem keine MAI mehr zum Prägen verfügbar sind, und das System erhöht die Schuldenobergrenze automatisch nach 48 Stunden. Diese Zeit wird als ausreichend angesehen, damit sich der MAI-Preis stabilisieren kann (im Falle eines hohen Verkaufsdrucks nach einem großen Ausverkauf von MAI).

Das bedeutet, dass 48 Stunden lang niemand mehr MAI aus einem Tresor leihen kann, der seine Verschuldungsgrenze erreicht hat, es sei denn, eine Schuld wird zurückgezahlt.

Nebenbei bemerkt: Je mehr MAI auf dem Markt sind, desto stabiler ist der Preis. Ein massiver Verkauf von MAI ist in der Tat weniger invasiv, wenn mehr MAI im Umlauf sind.

* Wenn jemand 1.000 MAI verkauft, während nur 10.000 MAI im Umlauf sind, entspricht der Verkauf einem Anteil von 10 %.
* Wenn jemand 1.000 MAI verkauft, während 10.000.000 MAI im Umlauf sind, entspricht der Verkauf 0,01%.

Die Schuldenobergrenze wird also nicht schrittweise, sondern exponentiell erhöht: Je mehr MAI im Umlauf sind, desto weniger Auswirkungen hätte ein großer Verkauf, so dass die Schuldenobergrenze um viel mehr erhöht werden kann.

{% hint style="info" %}
Wenn du dir MAI leihst, kann es vorkommen, dass der Höchstbetrag der MAI, den du leihen kannst, durch die Schuldenobergrenze gedeckelt ist, unabhängig vom aktuellen Wert deiner Sicherheiten und dem aktuellen Betrag der MAI, die du bereits geliehen hast. Wenn du dir MAI leihst, musst du unter Umständen bis zu 48 Stunden warten, bevor du weitere MAI leihen kannst.
{% endhint %}

### "Collateral to Debt Ratio" verstehen

Das CDR, oder (C)Sicherheiten zu (D)Schulden (R)atio, ist das Verhältnis zwischen dem Wert der hinterlegten Vermögenswerte in deinem Vault und dem Betrag an MAI, den du geliehen hast.

Wenn du zum Beispiel WETH im Wert von $200 hinterlegt hast, um MAI im Wert von $100 zu leihen, wäre dein CDR wie folgt:

$$
CDR=\frac{CollateralValue}{DebtValue}=\frac{200}{100}=200\%
$$

Ein CDR von über 100% bedeutet, dass zu jedem Zeitpunkt mehr Sicherheiten als Schulden vorhanden sind. Dies ist zwingend erforderlich, um sicherzustellen, dass der MAI-Stable Coin überbesichert ist. Es ist eine der Grundlagen der Mai Finance Tokenomics. Weitere Details findest du in der offiziellen [Mai Finance Dokumentation](https://docs.mai.finance/stablecoin-economics) .

Jeder Vault-Typ hat eine akzeptierte Mindest-CDR-Quote, eine Schwelle, unter der der Vault als gefährdet gilt, weil der geliehene Betrag möglicherweise nicht durch genügend Sicherheiten gedeckt ist. An diesem Punkt kann jeder den Vault liquidieren, d.h. ein Teil der Schulden wird vom Liquidator zurückgezahlt, der dann einen Teil der hinterlegten Sicherheiten als Rückzahlung erhalten kann. Auch hier findest du weitere Details zum Liquidationsprozess in der Dokumentation. Wenn du dir MAI gegen eine bestimmte Sicherheit leihst, erhältst du einige Hinweise darauf, wie hoch der maximale Betrag ist, den du leihen kannst, und welche Auswirkungen der geliehene Betrag auf deine Gesundheitsquote hat, wie du auf dem Screenshot unten sehen kannst:

![Health mitigation depending on borrowed amount](<../.gitbook/assets/image (4).png>)

Es ist sehr wichtig, dein CDR im Auge zu behalten und ein gesundes Ratio zu halten, um

* eine Liquidation zu verhindern
* die Stabilität der gesamten Mai Finance-Plattform zu erhöhen, indem du sicherstellst, dass das im Umlauf befindliche MAI-Volumen ordnungsgemäß abgesichert ist.

Das "gesunde" CDR liegt nach der Definition des Mai Finance-Teams zwischen 25% und 270% über dem Mindest-CDR-Wert. Nebenbei bemerkt, kannst du auch in unseren Strategieanleitungen nachlesen, wie du konservative/aggressive CDRs nutzen kannst, um in andere Projekte zu [investieren](../tutorials/polygon/leverage-aave-tokens.md), oder [Tilge deine Schulden](../debt-management-tutorials/debt-repayment-how.md#rueckzahlung-mit-deiner-sicherheit) mit deiner Sicherheit.

## Vault Anreize

### Vault-Anreize - APRs

Im September 2021 führte Mai Finance Vault-Anreize ein. Dabei handelt es sich um eine Belohnung, die von der Mai Finance-Plattform an jeden vergeben wird, der MAI leiht und am Wachstum der Plattform teilnimmt.

Jeder Vault-Typ (unter den 10 verschiedenen Typen) erhält 0,05 Qi pro Block, die dann unter allen Nutzern verteilt werden, die eine gesunde Collateral to Debt Ratio haben. Der effektive Jahreszins des Vault wird durch den aktuellen Betrag der geliehenen MAI bestimmt.

Ein Beispiel: Ben und Kila sind zwei Freunde, die ihre ETH in den WETH Vault bei Mai Finance eingezahlt haben.

* Ben hat den Gegenwert von 2.000 $ ETH eingezahlt und 1.000 MAI geliehen.
* Kila hat ETH im Gegenwert von 10.000 $ eingezahlt und 6.000 MAI geliehen.

Der aktuelle Betrag an MAI, der von Nutzern geliehen wurde, die WETH im Vault eingezahlt haben, beträgt 1.000.000 MAI.

Sowohl Ben als auch Kila kommen für die Vault-Anreize in Frage, weil Ben einen CDR von 200% und Kila einen CDR von 166,67% hat. Ben besitzt mit seinem Kredit 0,1 % des gesamten geliehenen Betrags, während Kila 0,6 % besitzt.

Die Gesamtmenge an Qi, die dem WETH Vault (oder einem anderen Vault) zugewiesen wird, beträgt:

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86.400 ist die Anzahl der Sekunden an einem Tag, und auf Polygon beträgt die Blockzeit 2 Sekunden, was bedeutet, dass die erwartete Anzahl an Blöcken pro Tag 86.400 / 2 = 43.200 beträgt. Somit beträgt die Emission für jeden Vault 2.160 Qi / Tag.

**Anmerkung:** Die Blockzeit hat sich in letzter Zeit erhöht und liegt bei 2,6 Sekunden. Allerdings gehen alle APRs und APYs, die auf allen Apps angezeigt werden, von einer Blockzeit von 2 Sekunden aus. Bitte überprüfe die aktuelle [Blockzeit auf PolygonScan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Wenn der Zustand des Vault gleich bleibt, erhält Ben also 0,1% der 2.160 Qi, die verteilt werden, während Kila 0,6% der gewährten Belohnung erhält.

* Ben erhält jeden Tag 2,16 Qi, was einer täglichen Belohnung von 0,216% entspricht, oder einem effektiven Jahreszins von 78,84%.
* Kila erhält jeden Tag 12,96 Qi, was ebenfalls einer täglichen Belohnung von 0,216% oder einem effektiven Jahreszins von 78,84% entspricht.

Nebenbei bemerkt: 2.160 Qi für 1.000.000 MAI ist eine tägliche Belohnung von 0,216% oder 78,84%, was dem effektiven Jahreszins des Vault entspricht.

{% hint style="info" %}
Es ist leicht zu zeigen, dass der effektive Jahreszins des Vault direkt mit der Höhe der geliehenen MAI verknüpft ist. Je mehr MAI geliehen wird, desto niedriger ist der effektive Jahreszins. Nebenbei bemerkt, wird die Höhe der MAI, die geliehen werden können, auch durch die Schuldenobergrenze begrenzt, die mit der Nachfrage nach MAI steigt.
{% endhint %}

Zur Überprüfung können wir den theoretischen effektiven Jahreszins für den MATIC Vault anhand der Zahlen berechnen, die auf der [Analyseseite](https://app.mai.finance/analytics) von Mai Finance veröffentlicht wurden. Der Betrag der aus dem MATIC Vault geliehenen MAI beträgt 799.328. Die Belohnung beträgt 216 Qi pro Tag für diesen Vault. Das entspricht einem APR von:

$$
APR=\frac{QiAnreiz*Qi_{Preis}}{MAI_{geliehen}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

Dies entspricht mehr oder weniger dem APR des MATIC Vault, wie im folgenden Screenshot dargestellt:

![APR des MATIC vault auf Mai Finance nach Einführung der AnreizeTyp](<../.gitbook/assets/image (23) (2) (3) (5).png>)

### Berechnung der anfänglichen Vaults' APRs

Mit denselben Daten wie im obigen Beispiel lassen sich die anfänglichen effektiven Jahreszinsen für alle Vaults berechnen

| MATIC     | 44.29%  |
| --------- | ------- |
| WETH      | 24.03%  |
| LINK      | 27.41%  |
| AAVE      | 164.14% |
| CRV       | 159.96% |
| WBTC      | 36.92%  |
| camWETH   | 25.46%  |
| camWMATIC | 44.33%  |
| camAAVE   | 167.23% |
| camWBTC   | 47.38%  |

{% hint style="info" %}
Wie du siehst, bringen manche Vaults mehr Belohnungen als andere. Außerdem siehst du, dass es super wichtig ist, dein Guthaben so schnell wie möglich einzuzahlen, um von den hohen effektiven Jahreszinsen zu profitieren, bevor die Schuldenobergrenze erhöht wird und mehr Kredite aufgenommen werden (was den effektiven Jahreszins senkt). Du kannst auch sehen, dass die 0,5 % Rückzahlungsgebühr durch das Prämienprogramm leicht ausgeglichen werden, wenn du deinen Kredit ein Jahr oder länger behältst.
{% endhint %}

### Verteilung der Anreize

Die durch die Vault-Belohnungen zugewiesenen Belohnungen werden auf die gleiche Weise verteilt wie die eingesetzten Qi. Jeden Mittwoch werden die Qi, die durch das Vault-Anreizprogramm zugewiesen wurden, für die Woche vor dem Auszahlungstag per Airdrop verteilt / eingefordert.

## Vault-Anreize FAQs

Wenn du mehr über die Funktionsweise der Vault-Anreize wissen willst, findest du hier eine offizielle FAQ vom Discord-Server.

* **Welche Vaults erhalten Belohnungen?**

Im Moment werden für alle Vault-Typen Qi-Belohnungen vergeben.

* **Wie hoch sind die Belohnungen für das Ausleihen?**

0,05 Qi/Block für jeden Vault-Typ

*   **Wie viel MAI muss ich leihen, um Belohnungen zu erhalten?**

    Für die Vault-Anreize musst du zwischen 25% und 270% über der Liquidation Ratio bleiben, um Qi-Token Airdrop zu erhalten. Das bedeutet:
* _Matic_ - Liquidation Ratio 150% - Berechtigt für Incentives zwischen 175% und 420%
* _Tokens_: - Liquidation Ratio 130% - Berechtigt für Incentives zwischen 155% und 400%
* _CamTokens_: - Liquidation Ratio 135% - Berechtigt für Incentives zwischen 160% und 405%
*   **Wie sehe ich, ob mein Vault Belohnungen verdient?**

    Wenn du das Feuer-Emoji auf der Übersichtsseite deines Vault siehst, bedeutet das, dass dieser Vault Belohnungen verdient.
* **Wie viel verdiene ich?**

Dein prozentualer Anteil am Pool der Belohnungen basiert auf dem Prozentsatz der von dir geliehenen MAI im Vergleich zur Gesamtsumme der von diesem Vault-Typ geliehenen MAI.

* **Wie lange dauert das Prämienprogramm?**

Die geplante Dauer des Anreizprogramms für das Ausleihen beträgt 3 Monate. Die DAO kann darüber abstimmen, die Anreize vor Ablauf der 3 Monate zu beenden oder das Programm zu verlängern.

* Wie erhalten wir die Belohnungen?\*\*

Qi werden per Airdrop an berechtigte Vault-Inhaber verteilt.

* **Wie wird die Berechtigung für Belohnungen ermittelt?**

Die Berechtigung für Belohnungen wird pro Block berechnet. Du erhältst Belohnungen für die Blöcke, für die du in der Woche berechtigt warst.

* **Wann beginnt die Verfolgung der Belohnungen für die Woche?**

Wir folgen demselben Zeitplan wie eQi. Du kannst die Blocknummern auf der Boost-Seite finden.

## Haftungsausschluss

Dieser Leitfaden wurde vor dem Start der Vault-Anreize verfasst, was bedeutet, dass die in diesem Dokument angepriesenen effektiven Jahreszinsen (wie auch dieses Dokument) noch geändert werden können und/oder möglicherweise nicht korrekt sind. Die Höhe der geliehenen MAI, die Verschuldungsgrenze und der Wert des Qi-Tokens haben großen Einfluss auf den endgültigen effektiven Jahreszins der einzelnen Vault-Typen. Bitte achte darauf, dass du verantwortungsvoll investierst.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden kann (oder dich Geld verlieren lässt). Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
