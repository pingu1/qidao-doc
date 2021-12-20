---
description: >-
  DeFi muss nicht kompliziert sein. In diesem Artikel erfährst du, wie du mit
  einer risikoarmen Strategie über Mai Finance in die DeFi einsteigen und
  trotzdem angemessene Zinsen bekommen kannst.
---

# camDAI Starterguide

## Einleitung

Die meisten Menschen haben Angst, wenn sie an DeFi denken. Die Volatilität dieses Marktes kann dazu führen, dass man eine Menge Geld verliert, und es gibt so viele Möglichkeiten, dass die Suche nach der richtigen Strategie ziemlich komplex sein kann. Wenn du jedoch die richtigen Werkzeuge verwendest, kannst du mit einigen einfachen und risikoarmen Strategien gute Ergebnisse erzielen und wahrscheinlich mit komplexeren und riskanteren Optionen konkurrieren.

In diesem Leitfaden stellen wir dir eine Anlagestrategie vor, die auf Stable Coin mit Hebelwirkung basiert und ein gewisses Risiko für höhere Zinsen beinhaltet.

## Was bedeutet es zu hebeln?

![Die Geschichte des Goldschürfes unluQi ](../../.gitbook/assets/canDAI-farwest.png)

Wir befinden uns im fernen Westen, während des großen Goldrausches. Die Banken wollen Gold kaufen, um den Leuten Geld zu leihen und dafür Zinsen zu bekommen, und die Bergleute wollen reich werden, indem sie ihr Gold an die Banken verkaufen.

Du bist ein Bergarbeiter, hast aber nicht viel Glück. Du hast nur ein einziges Nugget gefunden. Aber du bist superschlau und anstatt zu schürfen, hast du einen anderen Plan!

Du triffst eine Bank und erklärst ihr, dass du Gold hast. Du kannst das Gold bei der Bank als Sicherheit hinterlegen, d.h. du überlässt es der Bank, das Gold für Leute zu verwenden, die es brauchen, und die Bank gibt dir Zinsen auf deine Einlage.

Weil du das Gold verliehen hast, erklärt sich die Bank außerdem bereit, dir Geld zu leihen, und falls du dein Darlehen nicht zurückzahlen kannst, erhältst du Zinsen. Die Bank wird sich selbst mit dem Gold bezahlen, das du eingezahlt hast. Cool, jetzt bekommst du Zinsen für das Gold, das du bei der Bank hast, und sie hat dir etwas Geld gegeben.

Damit beschließt du, einen Bergmannskollegen zu treffen und sein Gold mit deinem Bargeld zu kaufen. So kann er sich auf den Abbau konzentrieren und bekommt Bargeld für das gefundene Gold. Alle sind glücklich.

Du triffst dich wieder mit der Bank und zahlst das gekaufte Gold ein. Das bedeutet, dass du mehr Zinsen bekommst und die Bank dir mit dem zusätzlichen Gold, das du eingezahlt hast, mehr Geld leihen kann. Du hast mehr Gold, das den Zinsen der Bank ausgesetzt ist, und etwas mehr Bargeld. Es wird Zeit, dass du zurückkommst, um zu sehen, ob dein Freund noch mehr Gold gefunden hat, und dann wiederholst du das Ganze immer wieder.

Das nennt man Hebelwirkung. Stell dir vor, du findest eine Bank, bei der du dir Bargeld zu 0 % Zinsen leihen kannst, und du hast eine solide Gelddruckmaschine nur durch die Zinsen, die du bekommst.

## Unsere Hebelwerkeuge

### AAVE

[AAVE](https://app.aave.com) ist eine Plattform zum Verleihen und Ausleihen, auf der du dein Vermögen hinterlegen kannst. Wenn du auf AAVE leihst, erhalten deine hinterlegten Token eine Rendite. Für unsere Strategie verleihen wir DAI, einen Stable Coin (mit Preisbindung an den US-Dollar). Auf AAVE können DAI im Wert von 100 US-Dollar über einen Zeitraum von einem Jahr eine Rendite zwischen 4 und 10 % erzielen.

![AAVE Markt auf Polygon, Stand Oktober 2021](../../.gitbook/assets/canDAI-aave.png)

Wenn du dein Vermögen auf AAVE einzahlst, erhältst du einen Einzahlungsnachweis. In unserem Beispiel erhalten wir, da wir DAI einzahlen, amDAI-Token in unserer Wallet (aave market DAI). Diese Quittung musst du unbedingt aufbewahren, denn du brauchst sie, um deine DAI von AAVE abzuheben. Das ist die Bank, die dein Gold in unserem Far-West-Vergleich annehmen wird.

### Mai Finance

[Mai Finance](https://app.mai.finance) ist eine Kreditplattform, die es dir ermöglicht, Vermögenswerte in einem Vault zu hinterlegen und gegen den Wert dieser Einlage einen Kredit aufzunehmen. Wenn wir auf den Vergleich mit der Bank zurückkommen, wäre es eine Bank, bei der du einen Kredit aufnehmen kannst, aber der Kredit kommt nicht von dem, was andere Leute verleihen. Stattdessen druckt die Bank Geld, das deiner persönlichen Einlage entspricht, so dass du nur gegen dich selbst einen Kredit aufnimmst.

Mai Finance wird den amDAI auf seinem [Renditeinstrument](https://app.mai.finance/yield) akzeptieren. Das Rendite-Instrument ist nur ein Zwischeninstrument zwischen AAVE und dem Vault von Mai Finance. Wie du auf dem AAVE-Screenshot sehen kannst, erzeugt das Ausleihen von DAI eine Belohnung von 8,75% in DAI (mit Zinseszins), aber auch 2,01% in MATIC. Das Renditeinstrument von Mai Finance sammelt diese MATIC-Belohnung ein und tauscht sie gegen mehr DAI ein, die dann deinem DAI-Depot hinzugefügt werden. Der APY (**A**nnual **P**ercentage **Y**ield) auf der Mai Finance Seite zeigt daher die aggregierten Zinsen von AAVE.

![Rendite auf Mai Finance](../../.gitbook/assets/camDAI-yield.png)

Sobald du deinen amDAI auf dem Renditeinstrument hinterlegt hast, erhältst du etwas camDAI in deinem Wallet (compounding amDAI). Das ist eine Quittung, die deinen Anteil am amDAI-Pool des Renditeinstruments angibt. Übrigens: Da camDAI deinen Anteil am amDAI-Pool darstellt, ist das Verhältnis zwischen amDAI und camDAI nicht 1:1. In diesem Artikel siehst du weitere Details.

Du kannst deine camDAI-Token in einem Vault bei Mai Finance deponieren und dir dann MAI (eine Stable Coin mit Preisbindung an $1) gegen deine Sicherheiten leihen. In unserem Vergleich aus dem fernen Westen handelt es sich um eine zweite Bank, bei der du einen Barkredit aufnehmen kannst, der auf der Menge Gold basiert, die du bei der ersten Bank eingezahlt hast. Diese zweite Bank akzeptiert die Quittung der ersten Bank als Garantie, falls du deinen Kredit nicht zurückzahlen kannst.

### Zapper

[Zapper](https://zapper.fi/dashboard) ist ein Schweizer Taschenmesser von DeFi auf Polygon. Diese Plattform ermöglicht es dir, Renditen in Liquiditätspools zu farmen, dein Vermögen direkt von der Plattform aus an AAVE zu verleihen, ein Dashboard deiner verschiedenen Investitionen zu präsentieren und einige Währungen in andere Währungen zu tauschen. Das ist die letzte Funktion, die wir nutzen werden, um den MAI Stable Coin, den wir gerade geliehen haben, in mehr DAI zu tauschen.

![Taushe MAI gegen DAI](../../.gitbook/assets/camDAI-zapper.png)

In unserem Beispiel aus dem fernen Westen ist Zapper der Goldschürfer, der dein Geld annimmt und dir Gold verkauft.

### Balancer

Wie du im Screenshot oben sehen kannst, verwendet Zapper Balancer das Protokoll, um den Swap zu betreiben. [Balancer](https://polygon.balancer.fi/#/) ist ein automatisierter Portfoliomanager, Liquiditätsanbieter und Preissensor, mit dem du Liquidität bereitstellen (und dafür Gebühren erhalten) oder Währungen mit Hilfe der Liquiditätspools tauschen kannst.

Für unseren Leitfaden werden wir Balancer nutzen, um unsere Investitionen etwas mehr Volatilität auszusetzen und bessere Zinsen zu erhalten. Dies ist jedoch zu 100 % optional.

## Strategiebeschreibung

### Hauptstrategie

Auch wenn wir erklärt haben, was AAVE ist, wird unsere Strategie eine Funktion von Mai Finance nutzen, um die DAI-Hinterlegung auf AAVE, die amDAI-Hinterlegung im Renditeinstrument und die camDAI-Hinterlegung im camDAI-Vault zu automatisieren.

![](../../.gitbook/assets/camDAI-zapDAI.png) ![](../../.gitbook/assets/camDAI-zapdeposit.png)

Die Schaltfläche `Zap in using DAI` öffnet ein Popup-Fenster, mit dem du dein DAI in den Vault einzahlen kannst und die AAVE-Einzahlung im Hintergrund durchführst. Das spart eine Menge Zeit und etwas Gas.

Das wird unser erster Schritt sein. Angenommen, wir haben DAI im Wert von 100 Dollar, dann werden wir sie bei Mai Finance in einem camDAI Vault hinterlegen. So können wir uns gegen diese erste Einzahlung MAI leihen.

Der minimale CDR (**C**Sicherheiten zu **D**Schulden **R**atio) für camDAI beträgt 110%. Das bedeutet, dass die Ratio zwischen deinen Sicherheiten (den DAI im Wert von $100) und dem Kredit, den wir bekommen, über 110% bleiben muss.

{% hint style="danger" %}
Wenn diese CRD Ratio den Mindestwert von 110% erreicht, bedeutet das, dass deine Sicherheiten an Wert verlieren und deine Schulden möglicherweise größer werden als der Wert deiner Sicherheiten. An diesem Punkt kann dein Vault liquidiert werden: Jemand kann einen Teil deiner Schulden zurückzahlen und einen Teil deiner Sicherheiten als Entschädigung erhalten. Da aber sowohl DAI als auch MAI Stable Coins sind, die an den US-Dollar gebunden sind, ist das Risiko einer großen Differenz zwischen den beiden Vermögenswerten sehr gering, was diese Strategie ziemlich sicher macht.
{% endhint %}

Um das Liquidationsrisiko möglichst gering zu halten, werden wir versuchen, einen CDR von 115% einzuhalten. Um herauszufinden, wie viel MAI wir leihen können, um bei einem CDR von 115% zu bleiben, verwenden wir diese Formel:

$$
MAI_{available} = \frac{Collateral_{value} - Debt_{value} * Target_{CDR}}{Target_{CDR}}
$$

Bei einem Beleihungswert von 100 USD, noch keinen Schulden und einem angestrebten CDR von 115%, können wir uns wie folgt einen Kredit aufnehmen:

$$
MAI_{available}=\frac{100 - 0*1.15}{1.15}=86.95
$$

​Dann kannst du die geliehenen MAI gegen DAI tauschen und den Vorgang wiederholen. So sollten deine Sicherheiten und Schulden aussehen:

| Loop # | Sicherheit | Schulden | Kreditrahmen | Equivalent APY | DAI liquidation price |
| ------ | ---------- | -------- | ------------ | -------------- | --------------------- |
| 1      | 100.000    | 0.000    | 86.956       | 10.42%         | 0                     |
| 2      | 189.956    | 86.956   | 75.614       | 19.48%         | 0.512                 |
| 3      | 262.571    | 162.571  | 62.751       | 27.36%         | 0.681                 |
| 4      | 328.323    | 228.323  | 57.175       | 34.21%         | 0.765                 |
| 5      | 385.498    | 285.498  | 49.718       | 40.17%         | 0.815                 |
| 6      | 435.216    | 335.216  | 43.233       | 45.35%         | 0.847                 |
| 7      | 478.449    | 278.448  | 37.593       | 49.85%         | 0.870                 |
| 8      | 516.042    | 416.042  | 32.690       | 53.77%         | 0.887                 |
| 9      | 548.732    | 448.732  | 28.426       | 57.18%         | 0.899                 |
| 10     | 577.158    | 477.158  | 24.718       | 60.14%         | 0.909                 |
| 11     | 601.877    | 501.877  | 21.494       | 62.72%         | 0.917                 |
| 12     | 623.371    | 523.371  | 18.691       | 64.96%         | 0.924                 |
| 13     | 642.062    | 542.062  | 16.253       | 66.90%         | 0.929                 |
| 14     | 658.315    | 558.315  | 14.133       | 68.60%         | 0.933                 |
| 15     | 672.448    | 572.448  | 12.289       | 70.07%         | 0.936                 |
| 16     | 684.737    | 584.737  | 10.686       | 71.35%         | 0.939                 |
| 17     | 695.423    | 595.423  | 9.293        | 72.46%         | 0.942                 |

Wir hören bei 17 Schleifen auf, aber du kannst auch mehr machen, wenn du willst.

Am Ende der 17 Schleifen hättest du 695,423 $ an Sicherheiten und 595,423 $ an Schulden. Das entspricht einem CDR von 116,79%, was sicher genug sein sollte, um eine Liquidation zu verhindern.

Wenn wir die 10,42% APY berücksichtigen, die das Renditeinstrument gewährt, würde dies Folgendes ergeben

$$
Interests = Collateral_{value}*APY=695.423*10.42\%= \$72.463
$$

Wenn wir bedenken, dass die anfängliche Investition nur $100 betrug, entspricht das einem APY von 72,463% beim einmaligen Staken eines Stable Coins!

### Alternative Strategie

Um ein wenig in hochvolatile Anlagen zu investieren, kannst du die gleiche Schleife wie oben verwenden, aber nur 90 % des geliehenen MAI hebeln und die 10 % verwenden, um etwas anderes zu kaufen. In diesem Beispiel verwenden wir die 10%, um Qi (den nativen Token von Mai Finance) zu kaufen und den Qi-BAL-Pool auf Balancer zu nutzen, der derzeit einen APR (**A**nnual **P**ercentage **R**evenue) von 107,12% hat.

![Qi-BAL pool state as of October 2021](../../.gitbook/assets/camDAI-balancer.png)

Da wir weniger DAI in den camDAI Vault einspeisen, werden wir auch weniger Schleifen betreiben. Der Ablauf wird folgendermaßen aussehen:

| Loop # | Sicherheit | Schuld  | Qi     | Available loan | Equivalent APY | DAI liquidation price |
| ------ | ---------- | ------- | ------ | -------------- | -------------- | --------------------- |
| 1      | 100.000    | 0.000   | 0.000  | 86.957         | 10.42%         | 0                     |
| 2      | 178.261    | 86.957  | 8.696  | 68.053         | 35.22%         | 0.537                 |
| 3      | 239.509    | 155.009 | 15.501 | 53.259         | 54.63%         | 0.712                 |
| 4      | 287.441    | 208.268 | 20.827 | 41.681         | 69.82%         | 0.797                 |
| 5      | 324.954    | 249.949 | 24.995 | 32.620         | 81.71%         | 0.846                 |
| 6      | 354.312    | 282.569 | 28.257 | 25.529         | 91.01%         | 0.877                 |
| 7      | 377.288    | 308.097 | 30.810 | 19.979         | 98.29%         | 0.898                 |
| 8      | 395.269    | 328.076 | 32.808 | 15.636         | 103.99%        | 0.913                 |
| 9      | 409.341    | 343.712 | 34.371 | 12.237         | 108.45%        | 0.924                 |
| 10     | 420.354    | 355.948 | 35.595 | 9.576          | 111.94%        | 0.931                 |



Am Ende der 10 Schleifen erhältst du

* 420.354 USD an DAI als Sicherheiten
* 355.948 $ an Schulden
* 35,595 $ Qi

Die gleichen Berechnungen wie im vorherigen Fall führen zu den folgenden Ergebnissen

* Ein endgültiger CDR von 118,09%, der als sicher genug angesehen werden sollte, um eine Liquidation zu verhindern
* $43.800 an Zinsen auf DAI aus den 10,42% APY, die das Zinsinstrument gewährt
* $68.139 an Zinsen auf deine Qi aus dem Balancer-Pool, wenn du davon ausgehst, dass du die Qi- und BAL-Belohnungen im Qi-BAL-Pool aufzählen wirst
* Ein Gesamt-APY von 111,94%

Diese Strategie birgt insofern mehr Risiken, als dass die Investition in den Qi-BAL-Pool nicht garantiert ist. Allerdings bekommst du ein kleines Stückchen Qi, das dich am QiDAO-Protokoll teilhaben lässt. Wenn du die BAL-Belohnung bei Mai Finance als Sicherheit verwendest und einen Kredit aufnimmst, kannst du auch wieder in den camDAI Vault oder in den Qi-BAL-Pool investieren. Wenn du das tust, hast du auch Anspruch auf Belohnungen, die jede Woche in Qi ausgezahlt werden.

## Zusammenfassung

Mit minimalen Investitionen und geringem Wartungsaufwand kannst du mit deinem DAI ziemlich solide Ergebnisse erzielen, indem du es hebelst. Da DAI ein Stable Coin ist, der über mehrere Chains hinweg eine hohe Liquidität aufweist, ist das Risiko relativ gering, dass DAI aus der Preisbindung fällt und dein Vault liquidiert wird. Diese Art von "Set and Forget"-Setup ist ein guter Ausgangspunkt für jeden DeFi-Anfänger und die Chancen stehen gut, dass diese Strategie in einem Bullenmarkt genauso funktioniert wie in einem Bärenmarkt. Zum Schluss haben wir noch erklärt, wie du dieselbe Strategie nutzen kannst, um einen Teil deines Kredits zu übernehmen und die vielen Möglichkeiten von DeFi auf Polygon auszuprobieren.

## Haftungsauschluss

Alles, was in diesem Tutorial vorgestellt wird, ist ein Bildungsinhalt, der die von Mai Finance angebotene Hebelwirkung veranschaulichen soll. Wir haben nicht über die Rückzahlung der Schulden gesprochen, weil es dazu bereits Artikel auf dieser Seite gibt, aber du solltest bedenken, dass Mai Finance eine Rückzahlungsgebühr von 0,5 % auf den geliehenen Betrag erhebt. Wie immer gilt: Mach deine eigenen Nachforschungen und zögere nicht, Fragen auf dem [Discord-Server der DAO](https://discord.com/invite/qidaoprotocol) Community zu stellen.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
