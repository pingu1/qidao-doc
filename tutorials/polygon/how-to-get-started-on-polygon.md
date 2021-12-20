---
description: >-
  In dieser Anleitung erklären wir alles was du wissen musst, um anzufangen die
  verschiedenen DApps zu nutzen, die das Polygon Netzwerk auf seiner Blockchain
  zu bieten hat.
---

# Der Start auf Polygon

## Was ist Polygon?

Polygon ist ein Netzwerk, welches auf der Ethereum Blockchain aufbaut, aber dazu entwickelt wurde die Skalierungsprobleme des Ethereum Hauptnetzwerks zu umgehen. Durchschnittlich dauert eine Transaktion auf dem Polygon Netzwerk 3 bis 5 Sekunden und kostet den Bruchteil eines Cents. Hierdurch wird es möglich, zig Transaktionen pro Tag durchzuführen, selbst mit einem sehr kleinen Wallet.

Polygon ist eines der ersten sogenannten "Seiten-Netzwerke" (side chains) zu Ethereum und auch dank diesem kleinen Vorsprung zeichnet sich Polygon aus durch:

* Eine ständig wachsende Nutzerzahl
* Eine ständig wachsende Anzahl von Anwendungen
* Ein solides Gesamtanlagekapital (TVL) von derzeit ungefähr 4 Mrd. USD auf der Blockchain

Polygon hat es geschafft, Vertrauen als zuverlässige Alternative zu dem Ethereum Netzwerk aufzubauen und so die Welt der dezentralen Finanzen auch kleinen Investoren zu eröffnen, welche DeFi erkunden möchten, ohne hunderte von Euros für Transaktionen auszugeben. Angesichts der Zuverlässigkeit und Benutzerfreundlichkeit sind viele Unternehmen bereits dazu übergegangen, Polygon dazu zu benutzen Assets von Netzwerk  zu Netzwerk zu übertragen, was zur Sicherheit und Anonymität von Polygon beiträgt und das Netzwerk insgesamt stärker macht.&#x20;

## Ein Wallet erstellen

Bevor du das Polygon Netzwerk benutzen kannst, brauchst du ein entsprechendes Wallet. Es gibt viele verschiedene Wallet-Typen, **Software- (**Metamask, TrustWallet...**)** und **Hardware- (**Trezor, Ledger ...**)** Wallets. In dieser Anleitung nutzen wir das Software-Wallet _Metamask._

### Metamask downloaden

Als ersten Schritt musst du die Metamask-Erweiterung zu deinem Internetbrowser hinzufügen. Du findest diese Erweiterung auf der offiziellen [Website](https://metamask.io/index.html) von Metamask. Metamask bietet auch App-Versionen für iOS und Android an, welche du ebenfalls benutzen kannst, aber hier nicht weiter erklärt werden.

Sobald du die Erweiterung installiert hast, solltest du das Logo von Metamask bei den Erweiterungen deines Browsers sehen. Wenn du Metamask das erste Mal öffnest wirst du danach gefragt, ob du bereits einen Account hast. Wenn ja, musst du einfach deine **Seed-Phrase** einfügen. (Wie wichtig deine Seed-Phrase ist, werden wir noch erläutern). Wenn du noch keinen Account hast, musst du einen neuen erstellen. Hierzu musst du folgende Schritte ausführen:

1. Als erstes musst du ein Passwort für dein Wallet festlegen.
2. Danach solltest du dir das Video bezüglich der Wichtigkeit der Seed-Phrase und Sicherheit deines Wallets genau anschauen.
3. Sodann wird dir deine Seed-Phrase angezeigt. Diese ist der **wichtigste Teil** bei der Erstellung eines neuen Wallets, du musst deine Seed-Phrase unbedingt gut aufbewahren und sie mit niemandem teilen!  Nur mit Hilfe der Seed-Phrase kannst du das Wallet jederzeit wieder herstellen, falls du keinen Zugriff mehr auf deinen Computer oder diese Metamask-Installation hast. (Hinweis: Wer deine Seed-Phrase hat, hat damit volle Kontrolle über dein Wallet!).

Wenn du fertig bist, solltest du diese Ansicht sehen:

![Metamask's Interface](<../../.gitbook/assets/image (27).png>)

### Die Polygon Blockchain hinzufügen

Wie du in der oberen rechten Ecke von Metamask siehst, benutzt du aktuell das Ethereum Mainnet. Wenn du hier drauf klickst, kannst du andere Netzwerke auswählen, das Polygon Netzwerk ist aber bisher nicht dabei. Keine Sorge, du kannst das Polygon Netzwerk über den untersten Eintrag "Spezieller RPC" hinzufügen, füge dazu folgende Daten ein:

![](<../../.gitbook/assets/image (16).png>)

Sobald du dies getan hast, kannst du über das selbe Menü zum Polygon Netzwerk wechseln, indem du es aus der Liste der Netzwerke auswählst.

## Kostenlos MATIC erhalten

Du bist nun bereit das Polygon Netzwerk zu benutze, allerdings hast du noch kein MATIC in deinem Wallet, weshalb du so keine Transaktionen durchführen kannst. Eine Transaktion auf der Polygon Blockchain erfordert immer eine kleine Gebühr, welche in MATIC-Tokens bezahlt werden muss. (Diese Gebühr wird auch als **Gas** bezeichnet und geht an die verschiedenen Validatoren, welche das Polygon Netzwerk am Laufen halten)

Zum Glück gibt die diese [Seite](https://matic.supply) kostenlos etwas MATIC, um deine ersten Transaktionen durchzuführen (Diese Art von Seite wird auch als _Faucet_ bezeichnet). Alles was du dazu machen musst, ist dein Wallet mit der Seite zu verbinden und ein Captcha zu lösen. Diese 0,002 MATIC (weniger als 1 Cent) reichen aus, um eine Reihe von Transaktionen auf dem Polygon Netzwerk durchzuführen

![Getting FREE MATIC](<../../.gitbook/assets/image (26).png>)

Manchmal kann es vorkommen dass diese Website überlastet ist, du kannst dann auch [diese](https://macncheese.finance/matic-polygon-mainnet-faucet.php) ausprobieren, falls die erste nicht funktioniert.

Bevor es weitergeht müssen wir klarstellen, dass diese Art von Faucet nicht dafür gedacht ist es dauerhaft zu verwenden und so zu leeren. Es wird kein MATIC ausschütten, wenn du bereits zu viel MATIC auf deinem Wallet hast oder es häufiger innerhalb von 24 Std. verwendest. Sei bitte sparsam und übertreibe es nicht.&#x20;

## &#x20;Tokens zu Metamask hinzufügen

Da du jetzt etwas kostenloses MATIC in deinem Wallet hast, bist du bereit die verschiedenen DApps und Tokens auf Polygon zu nutzen. Du kannst die verschiedenen Adressen der Tokens, welche du nutzen möchtest, auf [PolygonScan](https://polygonscan.com) suchen und kopieren, um sie zu Metamask hinzuzufügen. Auf der Website musst du einfach den Namen des Tokens eingeben, welchen du hinzufügen möchtest. Wenn wir zum Beispiel nach QiDAO suchen, wird folgendes angezeigt:

![Results of writing QiDAO on PolygonScan](<../../.gitbook/assets/image (24).png>)

Du musst hier die Adresse des Contracts kopieren und bei Metamask in der Liste der Assets ganz unten auf "Token hinzufügen" klicken, um die Contract-Adresse eingeben zu können. Der Token ist ab dann in der Liste deiner Assets sichtbar:

![Qi zu Metamask hinzufügen](<../../.gitbook/assets/image (22).png>)

## Tokens auf Polygon kaufen

Du kannst jetzt anfangen, Tokens auf Polygon zu kaufen bzw. tauschen. Hierzu musst du eine **DEX** (Dezentrale Börse) nutzen, dir stehen hierzu eine ganze Reihe von DEXes zur Verfügung:  [_Quickswap_](https://quickswap.exchange/#/swap), [_Slingshot_](https://app.slingshot.finance/trade/m/MATIC/USDC), [_Dexguru_](https://dex.guru), [_Sushiswap_](https://app.sushi.com/swap), usw..

Sobald du dich für eine DEX entschieden hast, kannst du anfangen Tokens auf Polygon zu handeln, das Interface eines typischen DEXes sieht so aus:

![Buying Qi tokens using Quickswap](<../../.gitbook/assets/image (25).png>)

{% hint style="info" %}
Eine weitere interessante Dapp für den Handel von Tokens ist [Zapper](https://zapper.fi/es/exchange). Zapper sucht auf den verschiedenen DEXes nach dem besten Wechselkurs für deinen Tausch, ein guter Weg, um beim Handel etwas zu sparen.
{% endhint %}

## Deine Wallet-Historie anschauen

Es ist oft wichtig, vergangene Transaktionen bzw. die Historie deines Wallets im Blick zu haben, herzu bietet sich die Website [DeBank](https://debank.com) an. DeBank gibt dir einen Überblick über die vergangenen Transaktionen deines Metamask-Wallets und zeigt dir dein gesamtes Portfolio auf allen damit verbundenen Blockchains und deine NFTs an. Dies ist nützlich, wenn du z.B. deine vergangenen Qi Airdrops vergleichen möchtest, welche du durch das Staking von Qi verdient hast.

![All the transactions made in our new Metamask address](<../../.gitbook/assets/image (10).png>)

Wie du hier siehst, habe ich 800.000 DxDex.io Tokens in meinem Wallet, aber ich habe nichts gemacht um diese Tokens zu erhalten und weiß nicht, woher diese kommen. Dies ist ein weit verbreiteter Scam-Versuch, du solltest diese Tokens ignorieren und nicht mit Tokens interagieren, welche du nicht kennst. DeBank gibt dir auch die Möglichkeit, Zugriffsberechtigungen zu verwalten und diese wieder zu entziehen.

## Nützliche Links

Hier sind noch ein paar Links, welche du nützlich finden könntest um dich auf dem Polygon Netzwerk zurechtzufinden:

* [Quickswap](https://quickswap.exchange/#/swap)
* [AAVE](https://app.aave.com)
* [PolygonScan](https://polygonscan.com/gastracker/): hier siehst du auch die aktuellen Gaspreise für Transaktionen

## Haftungsausschluss&#x20;

Diese Anleitung ist keine Anlageempfehlung oder Anlageberatung, sie dient ausschließlich Bildungszwecken. Für die Vollständigkeit und Richtigkeit wird keine Haftung übernommen.

{% hint style="info" %}
Bitte sei dir bewusst, dass eine Strategie die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem späteren Zeitpunkt schlechter laufen kann oder sogar minus macht. Informiere dich immer selbst, beobachte den Markt und kümmere dich um deine Investments, du trägst die alleinige Verantwortung.
{% endhint %}
