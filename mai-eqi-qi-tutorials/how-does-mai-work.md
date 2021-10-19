---
description: >-
  Ein gutes Verständnis darüber, wie MAI funktioniert, ist für jeden Investor,
  der Mai Finance wirklich verstehen will, von entscheidender Bedeutung. In
  diesem Artikel wirst du lernen, wie MAI als Stabl
---

# Wie funktioniert MAI?

## Was ist ein Stablecoin?

Bevor wir uns damit beschäftigen, was MAI ist, müssen wir verstehen, was ein Stablecoin ist. Ein Stablecoin ist eine Art von Kryptowährung, die darauf ausgelegt ist, einen stabilen Marktpreis zu bewahren. Die meisten Stablecoins sind an den US-Dollar gekoppelt (eine Währung, bei der der Preis so gestaltet ist, dass er gleich bleibt wie ein bestimmter Vermögenswert), aber es gibt auch andere Stablecoins, die an andere Rohstoffe wie Gold (wie EGold) oder Silber (SilverCoin) gekoppelt sind.

Es gibt jedoch 2 Hauptkategorien, in die alle Stablecoins eingeordnet werden können: **gesicherte **und nicht **gesicherte**. Bei den **gesicherten **Stablecoins handelt es sich um solche, die die Vermögenswerte halten, an die ihre Währung gekoppelt ist, während die **nicht gesicherten** Stablecoins Algorithmen verwenden, um das Angebot an Token zu kontrollieren und den Preis auf einem bestimmten Niveau zu halten.

## Die IRON Finance Katastrophe

Wenn du dich schon länger mit Kryptowährungen beschäftigst, erinnerst du dich vielleicht an das Desaster der TITAN- und IRON-Token. Aber für alle, die es nicht wissen, gibt es hier eine kurze Zusammenfassung. IRON Finance war ein Projekt mit zwei Token, dem IRON Stablecoin und dem TITAN Token. Der IRON Stable-Coin war jedoch nicht vollständig mit Stablecoins gesichert. Das Verhältnis zur Ausgabe von IRON war 75% USDC und 25% TITAN Token. Das war im Grunde ein Rezept für eine Katastrophe.

Im Juni 2021 erreichte der TITAN-Token ein ATH von 65 $, was dazu führte, dass eine Reihe von Investoren, die stark in den Coin investiert hatten, beschlossen, zu verkaufen. Dies führte zu einem Problem, da der Preis von TITAN auf der Grundlage von Angebot und Nachfrage festgelegt wird. Als das verfügbare Angebot an TITAN stieg, begann der Preis zu sinken. Dies führte zu einem enormen Verkaufsdruck, so dass der Preis von TITAN noch schneller fiel. Als TITAN also rapide zu fallen begann, verlor IRON seinen Rückhalt und schließlich seine Preisbindung - seinen Peg.

![Preis des TITAN Token](../.gitbook/assets/iron.jpg)

![Preis des IRON stablecoin](../.gitbook/assets/titan.jpg)

Man fing an, den IRON Stablecoin zu kaufen, um ihn für USDC zu verkaufen und so schnelles Geld zu verdienen, was eine riesige Arbitragemöglichkeit darstellte (das bedeutet, von den Preisschwankungen der Token zu profitieren). Lange Rede, kurzer Sinn, der Verlust bei diesem Vorfall wurde auf fast 1,75 Milliarden Dollar geschätzt. Gibt es nun einen Unterschied zwischen dem Stablecoin IRON und dem Stablecoin MAI?

## Was ist MAI?

MAI ist eine Stablecoin, der durch gebundene Sicherheiten gesichert ist. Die Ausgabe von MAI kann entweder durch die Hinterlegung von genehmigten Token in Vaults oder durch die Verwendung von **Anchor **erfolgen.

Bei der Prägung von MAI durch die Hinterlegung von genehmigten Token muss das **CDR **(Collateral to Debt Ratio) zwischen 150% liegen, das heißt, wenn du eine Sicherheit im Wert von $100 hinterlegst, dürfen deine neu geprägten MAI höchstens $66,6667 wert sein. Auf die Gründe hierfür werden wir später in diesem Artikel eingehen.

Eine weitere Möglichkeit, MAI zu prägen, ist der [Anchor](https://app.mai.finance/anchor), d.h. wenn du einen Stablecoin (ab September 2021 kannst du MAI mit DAI, USDC und USDT prägen) gegen MAI tauschst, werden neue MAI geprägt und der hinterlegte Stablecoin wird im Treasury als Sicherheit gehalten. Wenn du in der Zwischenzeit deine Stablecoins zurücktauschst, werden die MAI, die du zur Verfügung gestellt hast, verbrannt.

![Stablecoins die du gegen MAI eintauschen kannst](<../.gitbook/assets/image (9).png>)

Wie du auf dem Bild unten sehen kannst, ist der Preis des MAI Stablecoins fast immer in der Nähe von $1. Das liegt daran, dass, wie die offizielle Dokumentation sagt, der MAI Stablecoin den Nutzern erlaubt, sich in risikofreier Arbitrage durch Anchor zu engagieren, wenn der Preis von MAI unter $0,99 fällt oder über $1,01 steigt.

![Preis von Mai in den letzten 90 Tagen](<../.gitbook/assets/image (7) (1) (1) (2).png>)

## Warum ist der Wert immer nahe $1?

Die Bindung an 1 $ wird durch 2 Mechanismen aufrechterhalten: durch Anchor oder durch Hinterlegung von Sicherheiten in den Tresoren. In diesem Abschnitt des Artikels wirst du verstehen, warum.

### Anchor

Anchor ermöglicht es Nutzern, MAI mit Stablecoins zu prägen und Stablecoins gegen MAI einzulösen. Wie du auf dem Bild unten sehen kannst, gibt es eine 1%ige Gebühr, wenn du deine Stablecoins in MAI tauschst oder umgekehrt. Es gibt dafür zwei Hauptgründe:

* Die Prägegebühr von 1 % für die Erstellung von MAI legt eine Preisobergrenze von 1,01 $ fest.
* Die 1%ige Gebühr für den Rücktausch von stabilen Münzen in MAI legt eine Preisuntergrenze von $0,99 fest

![](<../.gitbook/assets/image (8).png>)

* Wenn sich der Markt in einem Abwärtstrend befindet: Der Markt verkauft seine volatilen Vermögenswerte und kauft Stablecoins, um einen Wertverlust der volatilen Vermögenswerte zu vermeiden. Das bedeutet, dass der Markt MAI kaufen will, wodurch der Preis steigt.
* Wenn sich der Markt in einem Aufwärtstrend befindet: Der Markt kauft volatilere Vermögenswerte, wenn deren Preis niedrig ist, und verwenden dafür ihre Stablecoins. Das bedeutet, dass die Leute ihre MAI verkaufen, was ihren Preis nach unten treibt.

Eine Preisobergrenze und eine Preisuntergrenze zu haben, hilft MAI, nicht allzu sehr von seinem Peg abzuweichen. Wie du jedoch auf dem Bild des MAI-Charts gesehen hast, kannst du an risikoarmen Arbitragemöglichkeiten teilnehmen (was bedeutet, dass du deine Stablecoins verkaufen kannst, wenn MAI unter $1 liegt oder MAI verkaufen kannst, wenn es über $1 liegt, um ein paar schnelle Dollars zu verdienen).Was die Ursachen für die Schwankungen des MAI-Preises angeht, so könnte es dafür zwei Hauptgründe geben:

.

### Hinterlegung von Sicherheiten in Tresoren

Um MAI in den Tresoren von Mai Finance zu prägen, musst du dort Sicherheiten hinterlegen und ein CDR (Collateral to Debt Ratio) über einem bestimmten Schwellenwert haben, in diesem Fall 150% (dieser Prozentsatz kann sich jedoch in Zukunft ändern, wenn die Gemeinschaft dies beschließt). Das bedeutet, dass die Tresore immer überbesichert sein werden (um 150%), um sicherzustellen, dass es immer Sicherheiten für die geprägten Stablecoins gibt. Sollte ein Tresor weniger als 150 % CDR haben, könnte er von der Gemeinschaft teilweise liquidiert werden, so dass jemand einen Teil seiner Sicherheiten verlieren könnte, wenn ein Liquitador einen Teil seiner Schulden bezahlt.

Wenn der Wert der Sicherheiten steigt, können Stablecoins ausgegeben werden, da ein Anstieg des Sicherheitenpreises das Verhältnis zwischen Sicherheiten und Schulden erhöht. Umgekehrt können bei sinkendem Wert der Sicherheiten weniger stabile Münzen ausgegeben werden, um zu verhindern, dass die CDR unter die 150 %-Marke fällt.

## Nachwort

Wie du in diesem Artikel gesehen hast, ist der MAI Stablecoin ein **überbesicherter **Typ von, was bedeutet, dass es immer genug Sicherheiten gibt, um den Preis des MAI Token zu stützen. Dies sollte jenen Anlegern, die zögern, in Projekte zu investieren, die Stablecoins prägen, eine gewisse Beruhigung verschaffen. Außerdem solltest du wissen, dass mit der Ausweitung von MAI auf andere Blockchains mehr MAI auf dem Markt sein wird, was zu einer geringeren Volatilität des MAI-Preises führen sollte.

Kürzlich wurden die Tresoranreize bei Mai Finance eingeführt. Wenn du verstehen willst, was das ist, bleib dran, denn es wird einen Artikel zu diesem Thema geben. Diese wird noch mehr zur Stabilität des MAI-Preises beitragen.

## Haftungsausschluss

Den Originalartikel des Mai Finance Teams über MAI findest du [hier](https://docs.mai.finance/stablecoin-economics).

Dieser Leitfaden ist definitiv keine Finanzberatung, er wurde mit einem pädagogischen Ziel vor Augen erstellt.

{% hint style="info" %}
Denk daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht funktionieren (oder Ihnen Geld kosten) kann. Bitte bleib immer informiert, beobachte die Märkte, behalte deine Investitionen im Auge und stell wie immer deine eigenen Recherchen an.
{% endhint %}
