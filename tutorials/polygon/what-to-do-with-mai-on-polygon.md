---
description: >-
  In diesem Tutorial werden die verschiedenen Optionen vorgestellt, mit denen du
  deinen frisch erworbenen MAI auf Polygon verwenden kannst.
---

# Was du mit MAI auf Polygon machen kannst

## Ziel des Tutorials

Das Ziel dieses Tutorials ist es nicht, im Detail zu zeigen, was du mit deinem MAI Stable Coin machen kannst, sondern eine Liste aller Webseiten und DeFi-Anwendungen zu erstellen, die du auf Polygon nutzen kannst, um deinen MAI direkt oder in Kombination mit anderen Stable Coins zu verwenden. Wenn du mehr über bestimmte Möglichkeiten zur Verwendung von MAI wissen willst, kannst du dir andere Anleitungen auf dieser Seite ansehen oder dir auf Discord oder Telegram Hilfe holen.

Bitte beachte, dass diese Liste nicht vollständig ist und es auch nie sein wird, da jede Woche neue Dapps im Netzwerk auftauchen. Ich kann sie nicht alle überprüfen, also werde ich nur die wichtigsten Optionen oder die bekanntesten / am meisten "gesicherten" Optionen vorstellen.

Wenn du möchtest, dass ein bestimmtes Projekt aufgelistet wird, tritt bitte der Qi-Community auf [Discord](https://discord.gg/mQq55j65xJ) bei.

{% hint style="info" %}
Ich werde keine Mai Finance-Farmen vorstellen. Dieses Thema verdient ein eigenes Tutorial, denn Qi ist nicht wie jeder andere beliebige Farm-Token.
{% endhint %}

## Farme Bluechip-Projekte

Bluechip-Projekte sind die DeFi-Anwendungen, die sich als solide erwiesen haben und ein geringeres Risiko darstellen. Sie sind in der Regel auditiert und das Team, das hinter ihnen steht, arbeitet schon lange an ihnen. Sie haben in der Regel keinen hohen effektiven Jahreszins, aber man kann ihnen trauen.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) ist ein automatisierter Portfoliomanager, Liquiditätsanbieter und Preissensor. Auf der Plattform kannst du deine Kryptowährungen verleihen und Gebühren von Händlern kassieren, die dein Portfolio nach Arbitragemöglichkeiten neu ausbalancieren. Wenn du mehr über Balancer wissen willst, dann lies bitte die offizielle Dokumentation]\(https://docs.balancer.fi).

Im Polygon-Netzwerk bietet Balancer einen Pool an, der aus den 4 wichtigsten Stable Coins besteht: DAI, USDC, USDT und MAI (miMATIC). Dieser stabile Pool hat derzeit einen ziemlich stabilen APR von \~20%.

<<<<<<< HEAD
![Stable coin pool, August 2021](../../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)
=======
![Stable coin pool state as of August 2021](../../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

Das Beste an Balancer ist, dass du die 4 Token gar nicht besitzen musst, um in den Pool einzuzahlen. Balancer generiert automatisch eine ausgewogene Kombination mit jeder Einzahlung, die du tätigst. Das heißt, wenn du MAI im Wert von 100$ hast, kannst du sie einfach in den Balancer-Pool einzahlen und den Algorithmus sie so verteilen lassen, dass ein Verhältnis von 25% für jeden Coin entsteht, abhängig von ihrem jeweiligen Preis zum Zeitpunkt der Einzahlung.

Die Belohnung für den Pool wird mit dem BAL-Token ausgezahlt, der wöchentlich verteilt wird. Zusätzlich zum BAL-Token können weitere Belohnungen gewährt werden, je nachdem, an welchem Pool du teilgenommen hast. Du kannst die verschiedenen [Anreizprogramme hier](https://balancer-incentives.web.app) einsehen. In unserem Fall bringt dir die Teilnahme am stabilen Pool auch Belohnungen in Form von MATIC und Qi ein.

Der komplette Ablauf würde in etwa so aussehen

![](../../.gitbook/assets/screen-shot-2021-08-11-at-11.34.45-am.png)

Wenn du mehr darüber wissen willst, wie du Mai Finance nutzen kannst, um deine Kryptowährung zu verleihen und MAI zu leihen (anstatt deine Kryptowährung zu verkaufen, um MAI zu kaufen), lies andere Anleitungen auf dieser Seite. Du kannst sogar AAVE in den Kreislauf einbeziehen, um noch mehr zu verdienen.

### Curve finance



Ein kleiner Click-Bait hier. [Curve](https://polygon.curve.fi) ist eine weitere Plattform, auf der du dein Krypto-Vermögen in Pools verleihen kannst, die Einnahmen generieren, aber nicht direkt MAI (noch nicht?). Die Pools, an denen wir interessiert sind, sind

* der AAVE-Pool, der zwischen 5% und 15% APR (APR variiert stark) auf ein Stable Coin-Trio (DAI/USDC/USDT) generiert. Der Pool funktioniert genau wie Balancer in der Weise, dass du dem Pool mit einem einzigen Asset beitreten kannst, das vom Protokoll auf AAVE verwendet wird.
* der atricrypto-Pool, der sich aus dem Stable Coin-Trio zusammensetzt und auch wETH und wBTC enthält, um unbeständige Verluste abzufedern. Dieser Pool hat einen APR zwischen 25% und 30%. Das Team von Mai Finance bemüht sich derzeit darum, dass auch MAI in diesen Pool aufgenommen wird, so dass du mit deinem geprägten MAI direkt in diesen Pool einsteigen kannst.

Während du darauf wartest, dass das Curve-Protokoll MAI als gültigen Stable Coin in seine Pools aufnimmt, kannst du deine Lieblingskryptowährung mit Curve nutzen, indem du folgende Schritte befolgst (Beispiel mit MATIC)

* Hinterlege deinen MATIC-Token bei AAVE und sammle amWMATIC
* Hinterlege deine amWMATIC bei Mai Finance und sammle camWMATIC (die Belohnungen von AAVE werden in die camWMATIC-Tokens umgewandelt)
* Verwende die camWMATIC als Sicherheit bei Mai Finance und leihe dir MAI dafür.
* Verwende die [Tauschseite](https://app.mai.finance/swap) auf Mai Finance, um alle deine MAI in USDC zu tauschen.
* Dann kannst du
  * Mit deinen USDC in den atricrypto-Pool auf Curve einsteigen und 25 bis 30 % Belohnung erhalten
  * Dem AAVE-Pool auf Curve mit deinen USDC beitreten und eine Belohnung von 5% bis 15% erhalten

<<<<<<< HEAD
Belohnungen auf Curve werden gewährt in

* Automatisch zusammengesetzte USDC, die deine Position im Pool erhöhen (es wird eine Mischung aus USDC/USDT/DAI und möglicherweise wBTC/wETH für den Atricrypto-Pool sein)
* WMATIC, mit denen du dann die obige Schleife wiederholen und dein Darlehen und dein investiertes Kapital erhöhen kannst
* CRV-Token, der auch als Sicherheit bei Mai Finance verwendet werden kann, um mehr MAI zu leihen und dein investiertes Kapital zu erhöhen

=======
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)
![](../../.gitbook/assets/screen-shot-2021-08-11-at-12.14.27-pm.png)

### AAVE

Es gibt eine vollständige Anleitung, wie du Mai Finance nutzen kannst, um deine [Aave Token zu hebeln](leverage-aave-tokens.md). Das ist zwar keine direkte Nutzung von MAI Stable Coin, aber wir können uns vorstellen, dass AAVE in Zukunft auch einen MAI-Pool haben wird, in dem du deine Kryptowährung verleihen kannst.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) ist wahrscheinlich eine der bekanntesten DEX (Decentralized EXchange) auf Polygon mit SushiSwap und 1Inch. Es ist auch ein AMM (Automated Market Maker), der es den Nutzern ermöglicht, im Polygon-Netzwerk mithilfe von Liquiditätspools effizient zu handeln. Für jeden Handel an der Börse fällt eine Gebühr an, die teilweise an die Nutzer/innen umverteilt wird, die ihre Liquidität auf der Plattform hinterlegen.

Die Art und Weise, wie du MAI auf QuickSwap nutzen kannst, ähnelt sehr einer [regulären Yield Farm](secure-your-yield-farming-profits.md). Wenn du also die genauen Schritte für den Eintritt in den MAI/USDC-Pool auf QuickSwap benötigst, ist es wahrscheinlich besser, diesen Artikel zu lesen.

Wenn du derzeit dem MAI/USDC LP (**L**iquidität **P**rovider) Pool auf QuickSwap beitrittst, erhältst du

* Handelsgebühren
* QUICK-Tokens

<<<<<<< HEAD
![MAI/USDC pool auf QuickSwap, August 2021](../../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)
=======
![Details of the MAI/USDC pool on QuickSwap as of August 2021](../../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

## Degen Farmenand aggregators

### Adamant



[Adamant](https://adamant.finance/home) ist ein Aggregator, der alle "besten" Farmen auf Polygon auflistet und dich direkt über seine Website teilnehmen lässt. Wenn du dein Vermögen (LP-Token) in einen bestimmten Pool auf Adamant einzahlst, ernten die Algorithmen die Belohnungen, die der Pool gewährt, und setzen einen Teil der Belohnung automatisch in deine LP-Position um. Der Rest der Belohnung wird in der Regel in WMATIC umgewandelt, das dann an die Inhaber des ADDY-Tokens (natives Token von Adamant) weiterverteilt wird. Schließlich erhältst du auch eine Belohnung in Form von ADDY-Tokens, die du ernten und 90 Tage lang halten kannst, um einen Teil der WMATIC-Dividenden zu erhalten.

Generell ist Adamant eine gute Wahl, wenn dir der Farm-Token egal ist und du deine Belohnungen nicht mehrmals am Tag manuell zusammensetzen möchtest. Außerdem generiert es mehr Einnahmen, da du zusätzlich zu den Belohnungen des Pools einige ADDY-Belohnungen erhältst.

Adamant unterstützt derzeit ein paar Pools, die das MAI/USDC LP-Paar akzeptieren. Die Pools sind auf

* QuickSwap: QUICK Belohnung wird in mehr MAI/USDC LP und WMATIC Belohnungen getauscht
* DinoSwap: Die Dino Belohnung wird in mehr MAI/USDC LP und WMATIC Belohnungen getauscht
* Mai Finance: Qi Belohnung wird in mehr MAI/USDC LP und WMATIC Rewards getauscht

<<<<<<< HEAD
![QuickSwap MAI/USDC Pool auf Adamant](../../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)
=======
![QuickSwap MAI/USDC pool on Adamant](../../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

{% hint style="info" %}
Die Screenshots des QuickSwap-Pools auf der QuickSwap-Website (siehe Absatz oben) und von Adamant wurden am selben Tag aufgenommen, zeigen aber unterschiedliche APYs (Annual Percentage Yield).
{% endhint %}

Du kannst sehen, dass der APY bei Adamant etwas höher ist als bei QuickSwap direkt. Die Aufschlüsselung der Belohnung sieht wie folgt aus

* 12,88% QUICK mit automatischer Aufzinsung (d.h. die QUICK Belohnung wird in mehr LP Token umgewandelt)
* 9,16% ADDY Belohnung (nicht aufgezinst)
* 3,40% Gebührenanteil-Dividende (ADDY wird täglich eingefordert)

Das bedeutet, dass von den 20,92%, die QuickSwap gewährt, nur 12,88% zur Erhöhung deiner LP-Position verwendet werden, der Rest wird in WMATIC-Dividenden umgewandelt. Du kannst deine ADDY-Belohnung täglich (oder jederzeit) einfordern und sie staken, was wiederum anforderbare WMATIC-Dividenden generiert. Mit anderen Worten: Adamant _scheint_ die bessere Option zu sein, weil es bessere APYs und automatisch zusammengesetzte Belohnungen bietet, aber in Wirklichkeit sind auch hier viele manuelle Aktionen erforderlich.

{% hint style="info" %}
Die Nutzung von Adamant hat auch einen starken Einfluss auf die Preise der nativen Token. Da Adamant die Farm-Token ständig verkauft, um mehr LP-Paare und WMATIC als Dividenden an ihre ADDY-Inhaber zu generieren, ist der Verkaufsdruck auf Farm-Token sehr hoch und kann erklären, warum ihr Preis ständig sinkt.
{% endhint %}

### Andere MAI/USDC LP Farmen

MAI wird auf Polygon immer beliebter und da QuickSwap das MAI/USDC-Paar unterstützt, wird es jetzt auch von vielen Farmen unterstützt. In der folgenden Liste werden einige Projekte vorgestellt, bei denen du mit MAI/USDC Erträge erzielen kannst

* DinoSwap
* Augury
* Polypup
* ...

Andere Farmen akzeptieren möglicherweise auch den MAI/USDC-Pool. Wenn du über neue Farmen und ihr Startdatum informiert bleiben willst, empfehle ich dir, einen Blick auf den [RugDoc.io-Kalender](https://rugdoc.io/calendar/) für Polygon-Farmen zu werfen und möglicherweise auch auf den Rest ihrer Website, die einen sehr klugen Überblick über jede Farm sowie ihre potenziellen Risiken bietet.

## Impermax

### Etwas Erklärung vorab

[Impermax](https://polygon.impermax.finance) ist eine Plattform, die es Nutzern ermöglicht, ihre LP-Tokens für höhere Renditen zu nutzen. Das Ziel ist ganz einfach: Indem man LP-Token zur Verfügung stellt und sie als Sicherheit verwendet, kann man mehr von den 2 Basiswerten leihen, um mehr LP-Token zu generieren und den Kreislauf zu wiederholen.

<<<<<<< HEAD
![Impermax loop](../../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)
=======
![Impermax loop explained](../../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

Dabei ist der/die Nutzer/in einem impermanenten Verlust ausgesetzt, der durch die Anzahl der Wiederholungen der Schleife noch vergrößert wird. Auch das Risiko eines Totalverlusts wird vervielfacht, wenn zu viele Schleifen angewendet werden. Wenn nämlich der APR vervielfacht wird, werden die Preisschwankungen der beiden Coins, die das Paar bilden, durch die Hebelwirkung verstärkt, was zu einer schnelleren Liquidation führt.

Bei Stable Coins ist das Risiko einer Liquidation jedoch geringer, da die Preisschwankungen vernachlässigbar sind. Das bedeutet auch, dass die Collateral to Debt Ratio (CDR) sehr nahe bei 100% liegen kann, was zu einer hohen Anzahl von Schleifen und damit zu einem hohen effektiven Jahreszins führt.

Beachte, dass Impermax Gebühren erhebt, wenn du einen Kredit aufnimmst und deine Position hebelst. Die Gebühr entspricht 0,1 % deiner endgültigen Position. Wenn ich z.B. MAI/USDC im Wert von 100 USD habe und das 50-fache hebele, ist meine endgültige Position 5.000 USD wert und ich zahle eine Gebühr von 4,90 USD für die 4.900 USD, die ich geliehen habe.

Der Effekt der Schleifenbildung bei der Kombination von Krediten und Darlehen ermöglicht es, den endgültigen effektiven Jahreszins zu vervielfachen. Bei einem anfänglichen effektiven Jahreszins von 20 % für das Paar MAI/USDC mit einem CDR von 110 %, der 50-maligen Durchführung der Schleife und der Verwendung der Formel

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

Wir können leicht einen endgültigen effektiven Jahreszins von 228% erhalten. Es gibt noch einige andere Faktoren, die sich auf den endgültigen effektiven Jahreszins auswirken, nämlich der Leihzins (Kreditzinsen für das Ausleihen weiterer LP-Token) und das Angebot bzw. die Nachfrage nach den beiden Vermögenswerten, aus denen sich das LP-Paar zusammensetzt (was sich direkt auf den Leihzins auswirkt).

Da alle Zinssätze durch die Anzahl der Anwendungen der Schleife vergrößert werden, variiert der effektive Jahreszins drastisch und kann manchmal für kurze Zeit negativ werden (dein LP-Token wird dann zur Rückzahlung des negativen effektiven Jahreszinses verwendet).

### Hebeln des MAI/USDC Paars

Am Ende verwendest du den Basiszins auf einen viel größeren Wert, der viel größere Zinsen einbringt und damit den effektiven Jahreszins deiner ursprünglichen Position erhöht.

<<<<<<< HEAD
![Ein Beispiel des Impermax Dashboards mit einem anfänglichen $70.52 MAI/USDC Paar](../../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)
=======
![An example of Impermax dashboard with an initial $70.52 MAI/USDC pair](../../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

Ich kann ganz einfach sehen, wie viel ich als Sicherheit einsetze, wie viel ich ursprünglich investiert habe, wie hoch die Leverage Ratio ist und wie hoch die Liquidationswerte aufgrund der Leverage Ratio sind. Mit dieser Position erhalte ich zum Zeitpunkt der Erstellung dieses Artikels die folgenden Ratios

<<<<<<< HEAD
![Gewinne und Verluste zum Zeitpunkt des Hebelns](../../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)
=======
![Earnings and spendings estimation at a given time](../../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

Der effektive Jahreszins wird in IMX-Token gewährt, die entweder in mehr MAI/USDC getauscht werden können (nutze die Macht von Mai Finance, um Kredite zu 0 % Zinsen aufzunehmen, RFTM) oder um Liquidität in bestimmten Pools zu schaffen, die IMX auf Impermax akzeptieren.

### MAI zum Leihen bereitstellen

In der App kannst du auch Liquidität für diejenigen bereitstellen, die ihre Positionen hebeln wollen (sie brauchen Basiswerte, um mehr LP-Token zu generieren). Das Verleihen von Vermögenswerten ist eine großartige Möglichkeit, um Rendite zu erzielen und den Kreditnehmern das gesamte Risiko zu überlassen. Je mehr Nutzerinnen und Nutzer leihen, desto höher ist auch der APR des Angebots.

<<<<<<< HEAD
![Raten für MAI auf Impermax zum Zeitpunkt des Tutorials](../../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)
=======
![Rates for supplying and borrowing MAI on Impermax at a given time](../../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

Dies ist eine weitere tolle Möglichkeit, deinen 0%-Kredit bei Mai Finance zu optimieren. Du musst nicht nur nichts bezahlen, um dir MAI zu leihen, sondern kannst auch eine Menge Zinsen verdienen, indem du es einfach auf Impermax einzahlst.

## Haftungsausschluss

Alles an diesem Tutorial ist rein informativ. Das Ziel ist es, Projekte vorzustellen, die ich für wertvoll halte, damit sich die Kryptowelt auf Polygon weiterentwickeln kann. Ich habe natürlich nicht über Mai Finance als Farm gesprochen, denn dafür wird es bald ein eigenes Tutorial geben. Abschließend sei gesagt, dass dieser Leitfaden ABSOLUT NICHT dafür gedacht ist, einfach so angewendet zu werden, er ist keine Finanzberatung und du solltest nicht blindlings dem folgen, was ich geschrieben habe. Bitte lies die Dokumente der verschiedenen Projekte, die ich erwähnt habe, bevor du in ihre Plattformen investierst.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
