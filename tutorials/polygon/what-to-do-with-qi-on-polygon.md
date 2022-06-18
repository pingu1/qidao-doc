---
description: >-
  Dieser Leitfaden erklärt dir im Detail, wie du dein Qi, den nativen Token von
  Mai Finance, auf Polygon einsetzen kannst. Außerdem analysieren wir, ob Qi
  eine gute Investitionsmöglichkeit ist und was s
---

# Was du mit Qi auf Polygon machen kannst

## Einleitung

Qi (\[tʃ Í] oder _chee_), ist der native Token von Mai Finance. Manche benutzen ihn, um abzustimmen und QIP (**Q**iDAO **I**Verbesserung **P**Vorschläge) zu stellen, andere staken ihn, um noch mehr Qi zu bekommen, und manche farmen einfach damit. Du kannst einige sehr gute Informationen darüber finden, wie du Qi auf der Mai Finance Plattform in dem [Leitfaden ](../../MAI-university/earning-passive-income-with-qidao.md)zum passiven Einkommen nutzen kannst.

In diesem Leitfaden geht es, wie in den meisten Investitions-Tutorials, vor allem um das Farmen und Ernten von Gewinnen, dieses Mal mit dem Qi-Token. Wir werden sehen, wie du eine Menge Qi generieren kannst und wie du sie auf den verschiedenen Plattformen auf Polygon einsetzen kannst.

Bescheidene Farmer werden dir manchmal sagen, dass du bescheiden bleiben, deine Ernte verkaufen und Gewinne mitnehmen solltest. Aber ich persönlich finde, das trifft es eher:

> Gib einem Mann einen Fisch und du ernährst ihn für einen Tag. Lehre einen Mann zu fischen, und du ernährst ihn ein Leben lang.

Also, schnapp dir deine Angel und folge dem Guide

## Qi auf Polygon

### Staking

Ich werde nicht zu viel Zeit auf diesen Teil verwenden, es gibt bereits einen vollständigen Leitfaden zu diesem Thema. Denke einfach daran, dass Mai Finance Einnahmen sammelt und einen großen Teil davon an Qi-Staker umverteilt. Dein Qi auf Mai Finance zu staken, ist eine der besten Verwendungsmöglichkeiten für den Token, und ab September 2021 sind 23% aller zirkulierenden Qi im Durchschnitt für 2 Jahre gesperrt.

### LP Farmen

Auch hier gibt es bereits ein paar andere Seiten, die zeigen, wie du den Qi-Token in deine Farming-Strategie einbinden kannst, um Erträge zu generieren und nie einen deiner Farm-Token zu verkaufen. Siehe[ DApps stapeln wie Legosteine](stack-dapps-like-lego-bricks.md) oder [Farming oder Staken](farming-or-staking-or-both.md) für Details.

Zur Erinnerung: Qi wird mit verschiedenen Token gepaart, um LP (**L**iquidität **P**Provider) Paare auf [QuickSwap](https://quickswap.exchange/#/quick) zu bilden, so dass du Folgendes farmen kannst

* Qi-WMATIC auf Mai Finance und Belohnung mit Qi-Tokens
* Qi-WETH auf QuickSwap und mit QUICK-Token belohnt wirst
* Qi-QUICK auf QuickSwap und Belohnung mit QUICK-Token

<<<<<<< HEAD
=======
![LP pool on QuickSwap for the Qi-WETH pair](<../../.gitbook/assets/image (19) (2) (1).png>)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)


![LP pool auf QuickSwap für das Qi-WETH Paar](<../../.gitbook/assets/image (19) (2).png>)

### Qi Farmen

Qi kann auch ausschließlich auf [Impermax](https://polygon.impermax.finance) verwendet werden. Impermax ist eine Plattform, auf der du ein bestimmtes LP-Paar mehrfach einsetzen kannst, um deine Gewinne aus dem QuickSwap zu erhöhen.

Das funktioniert so: Du leihst dir die 2 Token, die das Paar bilden, das du farmen willst, kombinierst sie zu mehr LP-Token und farmst mit einer viel höheren Position. In den meisten Fällen werden die Leihgebühren durch die Farming APR weitgehend ausgeglichen, sodass du eine positive Bilanz ziehen kannst.

![Hebel deine Qi-WETH Position auf Impermax](<../../.gitbook/assets/image (20).png>)

Wir sehen hier, dass der endgültige effektive Jahreszins für die Belohnung bei Impermax 393,88% beträgt, nachdem er 5-fach gehebelt wurde, basierend auf einem effektiven Jahreszins von 239,68% bei QuickSwap.

{% hint style="info" %}
Beachte auch, dass Impermax geschätzte effektive Jahreszinsen (**A**nual **P**ercentage **R**ewards) angibt, während QuickSwap geschätzte APYs (**A**nual **P**ercentage **Y**ields) angibt, was bedeutet, dass QuickSwap davon ausgeht, dass du deine Belohnungen täglich zusammensetzt. Die 239,68% APY bei QuickSwap entsprechen einem effektiven Jahreszins von 122,49%.
{% endhint %}

Um Qi und WETH bei Impermax zu leihen, musst du sie dir irgendwoher besorgen. Das ist nur möglich, weil einige andere Nutzer (oder du selbst) beide Token auch separat anbieten. Je mehr Token geliehen werden, desto höher wird der Leihsatz und desto niedriger wird der endgültige effektive Jahreszins, der manchmal sogar ins Negative trifft.

![Qi und WETH Statistik für den Qi-WETH Markt auf Impermax](<../../.gitbook/assets/image (11).png>)

Für unser Beispiel werden wir uns auf Qi konzentrieren. Du siehst, dass das Gesamtangebot an Qi 427,21 $ beträgt und der Gesamtbetrag, der in der gehebelten Position verwendet wird, 321,44 $, was eine Auslastungsrate von 75,24 % ergibt. Impermax verfügt über einen internen Mechanismus, der automatisch den Angebots-APR (den effektiven Jahreszins, den diejenigen, die Qi verleihen, erhalten) und den Leih-APR (den Prozentsatz der gefarmten Belohnung, der für die Rückzahlung des Darlehens abgezogen wird) berechnet.

Das bedeutet, dass du Qi ausschließlich auf Impermax anbieten kannst und in unserem Beispiel einen effektiven Jahreszins von 43,73 % erhältst, zum Zeitpunkt der Erstellung dieses Artikels. Da Angebot und Nachfrage schwanken, wird auch der effektive Jahreszins steigen/fallen. Wenn du einzelne Token auf Impermax anbietest, wirst du mit den Token belohnt, die du anbietest, was bedeutet, dass du mit dieser Strategie im Laufe der Zeit mehr Qi erzeugen kannst.

Bei Impermax kannst du auch die Hebelwirkung nutzen, um IMX Belohnungen zu erhalten. Bitte lies [den Stacking-Guide](stack-dapps-like-lego-bricks.md), um mehr darüber zu erfahren, wie du Impermax in deine Farming-Strategie einbauen kannst.

### Balancer

Balancer is a really nice toolbox for any strategy, especially the ones that include Qi and/or MAI. BBalancer ist ein wirklich guter Werkzeugkasten für jede Strategie, vor allem für diejenigen, die Qi und/oder MAI beinhalten. Balancer bietet ein Äquivalent zum LP Pair Mining, allerdings mit mehr als 2 Token, die in einem 1:1 Verhältnis bereitgestellt werden. Der Pool kann 3, 4 oder 5 Token (manchmal auch mehr) mit unterschiedlichem Gewicht enthalten. Der Algorithmus, der den Pool verwaltet, sorgt dafür, dass die Ratio für jeden Token immer eingehalten wird, indem er einige verkauft und andere kauft, um das Gleichgewicht zu halten.

Der Pool, den wir hier verwenden wollen, besteht aus Qi, WMATIC, BAL, USDC und MAI. Dieser Pool belohnt dich sowohl mit Qi- als auch mit BAL-Münzen, und du siehst schon, dass du beides in den Pool einbringen kannst. Ein weiterer großer Vorteil der Pools auf Balancer ist, dass du nicht alle Token, die den Pool bilden, in der richtigen Ratio bereitstellen musst, sondern dass der Algorithmus das für dich übernimmt. Das heißt, du kannst tatsächlich nur Qi in den Pool einzahlen und den Algorithmus den Rest erledigen lassen, um alles wieder ins Gleichgewicht zu bringen.

![Details des Pools, Stand September 2021](<../../.gitbook/assets/image (17).png>)

Übrigens: BAL-Token können als Sicherheiten bei Mai Finance verwendet werden, was bedeutet, dass du die Möglichkeit hast, deine BAL-Token im BAL Vault bei Mai Finance zu lagern und MAI dafür zu leihen. Außerdem erzeugst du durch das Ausleihen von MAI für deine BAL-Token Qi-Belohnungen, die den Pool auf Balancer speisen.

![Farming Kreis: Mai Finance & Balancer](<../../.gitbook/assets/image (18).png>)

Die APR von BAL-Gewölben bestimmt in hohem Maße, wie interessant es ist, das Vault in der Schleife zu haben, oder ob es besser ist, dein Qi in den Pool des Balancers zu mischen.

### Der Preis von Qi

Eine Menge Qi zu bekommen ist eine Sache, aber wenn der Token im Laufe der Zeit an Wert verliert, ist es dann wirklich eine gute Strategie, ihn zu behalten? In diesem Abschnitt werden wir versuchen, die verschiedenen Faktoren zu verstehen, die sich direkt auf den Preis von Qi auswirken, damit du, wenn du anfängst, deine Qi zu investieren, eine bessere Vorstellung davon bekommst, wie der Preis schwanken kann und welchen Einfluss du auf das Qi-Ökosystem hast.

### Qi Ausschüttung

Einer der Hauptfaktoren, der den Preis von Qi beeinflusst, ist die Rate, mit der sie erzeugt werden. Der Preis wird nämlich immer von Angebot und Nachfrage bestimmt. Wenn es ein großes Angebot und eine sehr geringe Nachfrage gibt, wird der Preis natürlich zusammenbrechen. Daher ist es wichtig zu verstehen, wie Qi erzeugt wird, um seinen Wert im Laufe der Zeit zu schätzen.

Derzeit gibt es 2 Quellen für Qi: Belohnungen aus der Landwirtschaft und Belohnungen aus dem Vault.

![LP Farmen auf Mai Finance, Stand September 2021](<../../.gitbook/assets/image (12).png>)

Wenn du Yield Farming mit MAI-Finanzierung betreibst, hast du die Wahl zwischen dem MAI/USDC-Paar und dem Qi/WMATIC-Paar (ab September 2021).

* Das MAI/USDC-Paar wird mit 0,5 Qi/Block belohnt.
* Das Qi/WMATIC-Paar wird mit 1 Qi/Block belohnt.

Auf Polygon beträgt die erwartete Blockzeit 2 Sekunden, und da ein Tag 86.400 Sekunden hat, bedeutet das, dass der MAI/USDC-Pool jeden Tag mit 21.600 Qi belohnt wird und der Qi/WMATIC-Pool mit 43.200 Qi.

Allein die Pools von Mai Finance sind täglich für 64.800 neue Qi verantwortlich.

Jeder Vault erhält 0,05 Qi/Block oder 2.160 Qi pro Tag, und es gibt derzeit 10 Vaults, die insgesamt 21.600 Qi als Belohnung für Vaults erhalten.

Das bedeutet, dass jeden Tag das Äquivalent von 86.400 neuen Qi geprägt und an die Nutzer/innen verteilt wird.

### Yield optimizer

Renditeoptimierer sind Plattformen, die die Belohnungen automatisch mit einigen vordefinierten Strategien zusammensetzen und zusätzliche Belohnungen für dich bereitstellen, damit du ihre Seite auswählen kannst. Ein großer Teil der geernteten Belohnungen wird jedoch direkt verkauft und auf diesen Plattformen anderweitig weiterverwendet.

Adamant bietet dir zum Beispiel an, das Qi/WMATIC-LP-Paar auf seiner Plattform zu farmen, wobei die Belohnung folgendermaßen verteilt wird

![Qi-WMATIC pool auf Adamant](<../../.gitbook/assets/image (15).png>)

![Details der 179.23% APR von Adamant](<../../.gitbook/assets/image (14).png>)

Wenn der effektive Jahreszins höher ist als bei Mai Finance, liegt das nur daran, dass Adamant zusätzliche ADDY Belohnungen an die Bauern verteilt. Die Menge an Qi, die tatsächlich an die Landwirte verteilt wird, beträgt 98,45% im Vergleich zu den 134,42%, die du bei Mai Finance bekommen kannst.

Von diesen 98,45% Qi-Belohnungen wird die Hälfte direkt verkauft, um WMATIC zu kaufen und zusätzliche LP-Token zu bilden, die dann an die Landwirte ausgegeben werden.

Bei einem LP-Token im Wert von 100$ und unter der Annahme, dass der effektive Jahreszins und die Token-Preise ein ganzes Jahr lang gleich bleiben und es keine Zinseszinsen gibt, würdest du nach einem Jahr Farmen Folgendes erhalten

* 134,42 $ an neuem Qi bei Mai Finance
* neue Qi/WMATIC-Token im Wert von 98,45 $ oder neue Qi im Wert von 49,23 $ bei Adamant

Das bedeutet, dass Qi im Wert von $85,20 einfach direkt auf dem Markt verkauft wird, was mehr als 60 % der Gesamtemission entspricht, die dem Pool auf Adamant zugewiesen wird.

Und Adamant ist nicht die einzige Plattform, die diese Art von Service anbietet. Einige andere Beispiele sind Beefy Finance und Kogecoin. Von den 4,9 Mio. $ TVL in der Qi/WMATIC-Farm auf Mai Finance kommen 2,3 Mio. $ direkt von Adamant, 41.000 $ von Beefy und 12.000 $ von Kogecoin, was für diese drei Plattformen mehr als 50 % des auf Mai Finance gesperrten Wertes ausmacht. Eine grobe Schätzung zeigt, dass mehr als 30 % des gesamten täglichen Qi-Ausstoßes von diesen Plattformen verkauft werden, was einen sehr negativen Verkaufsdruck auf den Token ausübt und seinen Preis senkt, was teilweise erklärt, warum Qi Schwierigkeiten hat, seinen hohen Preis zu halten.

### LP Paare verstehen

Wenn du Yield Farming betreibst, indem du LP-Paare anbietest, werden die LP-Token dazu verwendet, Nutzern, die einen Token gegen einen anderen tauschen, Liquidität zu verschaffen. Wenn in unserem Beispiel Qi/WETH jemand WETH kauft, kann ein Teil des Tokens aus dem LP-Pool genommen und an den Nutzer verkauft werden, der es benötigt.

Da ein Teil der WETH aus dem Pool entnommen wurde, gibt es ein Ungleichgewicht: weniger WETH für die gleiche Menge Qi. Der Algorithmus, der dafür zuständig ist, das Verhältnis von 1:1 im Pool aufrechtzuerhalten, verkauft dann etwas Qi aus diesem Pool, um mehr WETH zurückzukaufen und ein perfektes Verhältnis von 1:1 wiederherzustellen. Das Gegenteil passiert auch, wenn jemand Qi kauft, d.h. WETH wird verkauft, um Qi zurückzukaufen.

Das gleiche Phänomen tritt auf, wenn einer der beiden Token, aus denen das Paar besteht, an Wert gewinnt oder verliert. Als Beispiel nehmen wir an, dass der Qi-Preis bei 1 $ und der ETH-Preis bei 1.000 $ liegt und dass wir einen Pool mit Qi im Wert von 100 $ und WETH im Wert von 100 $ haben. Das bedeutet, dass der Pool 100 Qi und 0,1 WETH enthält. Das bedeutet dass der Pool aus 100 Qi und 0.1 WETH besteht.

Wenn nun der ETH-Preis auf 2.000 US-Dollar steigt und der Pool die gleiche Menge an Token behält, hätten wir Qi im Wert von 100 US-Dollar, aber WETH im Wert von 200 US-Dollar, und wir hätten den Restbetrag verloren. Daher wird der Algorithmus, der für den Pool verantwortlich ist, ein wenig ETH verkaufen, um Qi zu kaufen. In unserem einfachen Beispiel werden ETH im Wert von $50 verkauft, um Qi im Wert von $50 zu kaufen, und der Endzustand wäre

* 150 Qi mit einem Wert von $150
* 0,075 ETH mit einem Wert von $150

Das bedeutet auch, dass, wenn der Preis eines der beiden Token steigt, der Pool eine Nachfrage nach dem anderen Token schafft, was dessen Preis ebenfalls in die Höhe treibt. Das Gegenteil ist der Fall: Wenn einer der Token an Wert verliert, wird der andere verkauft, um die 1:1 Ratio aufrechtzuerhalten, was den Preis nach unten treibt. Das erklärt zum Teil auch die Preisschwankungen von Qi im Vergleich zu WEHT und WMATIC (den beiden Hauptmünzen, mit denen Qi gepaart ist).

![Price von Qi (links) VS Preis von WMATIC (rechts)](<../../.gitbook/assets/image (13).png>)

### Fehlende Einsatzmöglichkeiten

Schließlich kann die fehlende Verwendung von Qi oder das Fehlen von bekannten Anwendungsfällen erklären, warum der Preis des Tokens sinkt. Leute, die Qi aus Belohnungen im Vault sammeln und/oder auf Mai Finance farmen, werden es einfach verkaufen, solange es noch einen "gewissen" Wert hat, um einen Gewinn zu erzielen, ohne eine langfristige Perspektive zu haben. Dieser Leitfaden versucht, verschiedene Möglichkeiten aufzuzeigen, wie du deine Qi-Münzen nutzen kannst, ohne sie zu verkaufen, aber wenn der Preis nicht steigt oder du keine Vorteile durch andere Münzen erzielen kannst (auch bekannt als Gewinnverlust), hat es wenig Vorteile, sie zu stacken.

### Wie können wir helfen, den Preis zu erhöhen?



Wenn wir wollen, dass der Preis von Qi steigt (und wer würde das nicht wollen), gibt es ein paar Möglichkeiten.

* Die Emission reduzieren: Mit 86.400 neuen Qi, die täglich ausgegeben werden, ist das Angebot sehr hoch. Wenn wir diesen Ausstoß verringern, kann das Angebot geringer ausfallen, und mit weniger Angebot sollte der Preis theoretisch steigen. Allerdings muss die aktuelle Emission für die Farmen gleich bleiben, da sie Teil einer aktuellen Partnerschaft mit QuickSwap sind. Die Vault-Anreize wurden eingeführt und sind eine wunderbare Möglichkeit, die Kreditplattform zu fördern und die Leute dazu zu bringen, Kredite aufzunehmen, also ist die Reduzierung dieser Emissionen wahrscheinlich eine weitere schlechte Idee.
* Verantwortungsvoll wirtschaften: Ich behaupte nicht, dass Adamant der Hauptschuldige ist oder ein schlechtes Produkt darstellt. Ich beziehe diese Plattform sogar in die meisten meiner Strategien ein und nutze sie täglich. Allerdings versuche ich, in Pools zu farmen, bei denen ich weniger Bedenken habe, dass der Token gedumpt wird. Wenn du in einem Pool, der die Mai Finance Farm nutzt, auf Adamant Yields farmen willst, solltest du daran denken, dass du an der Qi-Abschreibung teilnimmst. Wenn dir das nichts ausmacht, ist das völlig in Ordnung.
* Verstehe, wie die Dinge funktionieren: Die Preise ALLER Kryptowährungen sind sehr volatil, und die meiste Zeit diktiert der Preis von BTC und ETH den Preis aller anderen Token. Das geschieht nicht auf magische Weise. Außerdem solltest du verstehen, dass manche Leute Geld verdienen, weil andere Geld verlieren. Geld gibt es nicht umsonst, und magisches Internet-Geld ist eigentlich gar nicht so magisch.
* Finde neue Wege, um deine Qi-Token zu verwenden. In diesem Leitfaden findest du immer wieder Ideen, die dir helfen, das Volumen deines Portfolios zu erhöhen und so wenige Token wie möglich zu verkaufen. Geschlossene Kreisläufe sind am besten, denn der Output eines Produkts speist den Input des nächsten und schafft so eine schöne Blase, die mit der Zeit nur noch größer wird.

Erinnere dich das immer gilt:

$$
Wert = Anzahl * Preis
$$

Wenn der Preis sinkt, aber deine Menge steigt, kann dein Wert steigen oder zumindest nicht so schnell sinken.

### Haftungsausschluss

Dieser Leitfaden ist das Ergebnis vieler Diskussionen über den Qi-Preis im Discord-Kanal. Ich habe festgestellt, dass einige Leute, die sich über den Preisverfall beschweren, die Gründe für den anhaltenden Abwärtstrend des Qi-Preises nicht vollständig verstanden haben. Das führt zu Frustration und Täuschung, was für Qi, das Mai Finance Produkt und das gesamte DeFi Ökosystem im Allgemeinen sehr negativ ist. Es gibt jedoch keine Garantie dafür, dass der Preis jemals wieder steigen wird. Wenn du also deine Qi behalten und investieren möchtest, recherchiere bitte selbst und tu es auf eigenes Risiko. Plane deine Strategie richtig und halte dich daran.

{% hint style="info" %}
Bedenke, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geld verlieren) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
