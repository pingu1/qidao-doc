---
description: >-
  In this guide we'll explain everything you need to know in order to start
  using the Fantom chain.
---

# Einstieg in Fantom

## Was ist Fantom

Fantom ist eine Ethereum-Alternative für Blockchain-Designer. Als quelloffene Smart-Contract-fähige Blockchain ermöglicht sie es Designern, sichere, umfassende und modulare DApps (**D**ecentralized **App**lications) zu entwickeln.

Die Chain wurde entwickelt, um alle Einschränkungen der vorherigen Generation von Blockchain-Plattformen zu überwinden, die manchmal als das Blockchain-Trilemma bezeichnet werden: Dezentralisierung, Sicherheit und Skalierbarkeit. Um einen dieser Aspekte zu verbessern, muss dies auf Kosten eines der beiden anderen gehen. Fantom versucht, dieses Problem dank seines DAG (Directed Acyclic Graphs) basierten Lachesis aBFT (Asynchronous Byzantine Fault Tolerant) Konsensmechanismus zu lösen, der es ermöglicht, leistungsstark, skalierbar und sicher zu sein. Erste Benchmarks haben gezeigt, dass Fantom problemlos über 20.000 Transaktionen pro Sekunde verarbeiten kann.

Schließlich ist Fantom zu 100% EVM (**E**thereum **V**irtual **M**achine) kompatibel, was bedeutet, dass DApps, die auf EVM-kompatiblen Netzwerken entwickelt wurden, auch auf Fantom eingesetzt werden können. Das bringt noch einen weiteren Vorteil für die Nutzerinnen und Nutzer, denn MetaMask und andere Web3-Anwendungen sind ebenfalls mit Fantom kompatibel. Du kannst innerhalb derselben Wallet nahtlos von Polygon oder Avalanche zu Fantom wechseln.

## Der Einstieg in Fantom

Fantom ist EVM-kompatibel. Wenn du bereits eine Wallet für andere EVM Chains (Ethereum Mainnet, Polygon oder Avalanche) hast, kannst du sie nutzen. Andernfalls musst du eine Wallet-Adresse erstellen. Es gibt verschiedene Arten von Wallets, die verwendet werden können: **Software-Wallets** wie Metamask oder [fWallet](https://pwawallet.fantom.network/#/), oder **Hardware-Wallets** wie [Trezor](https://trezor.io/coins/) oder [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/).

Für diese Anleitung werden wir Metamask benutzen, aber du kannst auch jede andere Software/Hardware Wallet benutzen. Wenn du eine Anleitung brauchst, wie du Metamask installierst, findest du sie im [Polygon-Leitfaden](../polygon/how-to-get-started-on-polygon.md).

### Fantom zu Metamask hinzufügen

Um das Fantom-Netzwerk nutzen zu können, musst du es manuell in Metamask konfigurieren. Dazu klickst du oben im Metamask-Fenster auf das Dropdown-Menü " Network" (wo das Netzwerk angezeigt wird, das du gerade verwendest, standardmäßig das Ethereum Mainnet) und wählst dann "Custom RPC". Mit den folgenden Informationen kannst du dich mit Fantom verbinden:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Nachdem du deine Änderungen gespeichert hast, wechselt die Metamask automatisch zum Fantom-Netzwerk.

![DU bist jetzt erfolgreich auf Fantom!](../../.gitbook/assets/ftm-mm0.png)

If you need more details to setup Metamask, you will find additional info on the [official Fantom guide](https://docs.fantom.foundation/tutorials/set-up-metamask).

### FTM faucet

Jetzt, wo du auf FTM bist, brauchst du einige FTM (native Token, die zur Deckung der Gaskosten verwendet werden). Du kannst entweder einige FTM-Token von anderen Chains überbrücken oder einen Faucet benutzen, der genug FTM-Token in deine Wallet einzahlt, um ein paar Transaktionen durchzuführen. Den [Haupt-Faucet auf Fantom](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas) findest du auf SpookySwap, einem der wichtigsten DEXes dort (**D**ecentralized **Ex**change). Beachte, dass es sich um einen Service von SpookySwap handelt, der auf Discord basiert und einen gültigen Discord-Account voraussetzt, der mehr als 30 Tage lang aktiv ist (es ist jedoch nicht erforderlich, 30 Tage lang auf dem SpookySwap Discord-Server zu sein).

* Sobald du dem [SpookySwap Discord](http://discord.gg/AqbsWsWDgn) Server beigetreten bist und deinen Account verifiziert hast, gehe zum Bereich #faucets.

![](<../../.gitbook/assets/image (42) (1).png>)

* Gib im Kanal #faucet einfach den Befehl `!faucet` ein und der Bot schickt dir ein paar $FTM. Beachte, dass du nur 1 Interaktion alle 30 Tage machen kannst.
* Wenn du überprüfen willst, ob du dein FTM-Token richtig erhalten hast, kannst du auf den Namen des Fantom Tip Bots klicken, um direkt mit ihm zu interagieren und `!balance` eingeben

![Danke Fantom Tip Bot und SpookySwap](<../../.gitbook/assets/image (45) (1).png>)

* Jetzt musst du nur noch deine FTM-Token an deine Wallet-Adresse schicken, indem du den Befehl `!withdraw <Deine_Wallet-Adresse>` verwendest. Du findest deine Wallet-Adresse oben im Metamask-Fenster.

![Auszahlung aus deinem Discord account](../../.gitbook/assets/ftm-faucet.png)

![Frische Einzahlung im  Metamask wallet](../../.gitbook/assets/ftm-mm.png)

## Token auf Fantom übertragen

### Überbrücke Stable-Coins / ETH / BTC

Wenn du Stable Coins zu Fantom überbrücken willst, kannst du die folgende Liste von Brücken verwenden:

* [AnySwap](https://anyswap.exchange/#/bridge): Dies ist die offiziell unterstützte Brücke, um MAI, die du auf Polygon geprägt hast, nach Fantom zu schicken (siehe den [MAI metaverse](../../MAI-university/mai-metaverse.md#fantom) Leitfaden für Details). Diese Lösung unterstützt viele Assets und viele Chains, so dass es für dich einfach ist, deine Kryptowährungen nach Fantom zu schicken. Die Transaktionsgebühren und die voraussichtliche Ausführungszeit findest du in den Hinweisen am unteren Rand der Bridging-UI.

![MAI von Polygon nach Fantom übertragen](<../../.gitbook/assets/ftm\_anyswap (1).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): bietet Überbrückungsdienste für viele Chains für die meisten Stable Coins, mit Gebühren zwischen 0,04% und 0,19% für die Überbrückung zu Fantom an (DYOR).
* [xpollinate](https://www.xpollinate.io): niedrige Gebühren und stellt sicher, dass es auf der Ziel-Chain genügend Liquidität für den Token gibt, den du überbrücken willst. Je geringer die Liquidität (oder je größer der zu überbrückende Betrag), desto länger dauert der Transfer.

### Andere Assets übertragen

* Binance CEX: Du kannst den FTM-Token auf Binance kaufen und ihn direkt zu Fantom übertragen, aber das ist der einzige Token, den du übertragen kannst.
* [SpookySwap](https://spookyswap.finance/bridge): Unterstützt viele Netzwerke und viele Token, die du an Fantom senden kannst.
* AnySwap: siehe die Beschreibung, die im Abschnitt Stable Coin.

## DeFi auf Fantom

Fantom hat am Ende des Sommers 2021 eine ziemlich beeindruckende Expansion erlebt, vor allem durch Belohnungsprogramme, die dazu beigetragen haben, Investoren und Entwickler auf die Chain zu locken. Das Wachstum wurde auch von Blue-Chip-Projekten unterstützt, die ihre DApps im September 2021 auf Fantom bereitstellten, darunter Curve und SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Diese Anwendung ist Balancer sehr ähnlich. Du kannst einige Token gegen andere eintauschen und auch an ausgewogenen Pools teilnehmen, die aus mehreren Token bestehen. Dies ist auch der erste offizielle Partner von Mai Finance auf Fantom und der einzige Ort, an dem du deine MAI tauschen oder sie in einem MAI-USDC-Pool verwenden kannst.

![MAI für etwas mehr  FTM eintauschen](<../../.gitbook/assets/image (44) (1).png>)

*
  * [SpookySwap](https://spookyswap.finance): Dies ist die größte DEX (**D**ecentralized **Ex**change) auf Fantom, wo du deine Token gegen andere tauschen, Liquidität einzahlen und Renditen farmen kannst, ziemlich genau so, wie du es bei QuickSwap auf Polygon tun würdest. SpookySwap belohnt dich mit dem BOO-Token, dem nativen Token der Plattform. Nebenbei bemerkt: Wenn du deine BOO-Token stakst, erhältst du dafür xBOO, einen ertragsabhängigen Token, mit dem du zusätzliche Belohnungen verdienen kannst (dasselbe Prinzip wie beim Dragon Syrup auf QuickSwap).
  * [SpiritSwap](https://app.spiritswap.finance): Eine traditionelle AMM- und Yield Farming-Plattform, auf der du Token tauschen, LP-Token erstellen und Yield in Liquiditätspools farmen kannst. SpiritSwap bezahlt dich mit SPIRIT-Tokens, die du auf der Plattform staken kannst, um inSPIRIT-Tokens zu erhalten (SPIRIT ist für eine bestimmte Zeit gesperrt), das Pendant zu veCRV-Tokens. Du kannst SpiritSwap auch zum Leihen und Ausleihen nutzen, während du auf Mai Finance auf Fantom wartest.
  * [Tarot](https://www.tarot.to): Tarot ist die Fantom-Version von Impermax, wo du deine LP-Token von SpookySwap (oder anderen DEXs/AMM) verwenden kannst, um auf der Plattform zu farmen. Du kannst auch einzelne Token einzahlen und sie an die speziellen Pools verleihen, wo andere sie ausleihen können, um neue LP-Token zu generieren und ihre Farmingmenge zu hebeln. Sei dir der Liquidatoren bewusst, wenn du deine LPs in einem Pool ausleihst, in dem die Auslastung hoch ist.
  * [Scream](https://scream.sh): Das ist ein Klon von Compound, bei dem du deine Token verleihen und gegen sie leihen kannst. Wenn du deine Token ausleihst, erzeugst du Belohnungen in Form der Token, die du verliehen hast, sowie SCREAM-Tokens, die du auf anderen Plattformen verwenden kannst.
  * [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve ist das Blue-Chip-Projekt, das jeder gut kennt. Hier kannst du deine Token in bestimmte Pools einzahlen (du musst keinen ausgeglichenen Betrag einzahlen) und wirst in den Token belohnt, die du leihst, sowie in CRV- und wFTM-Token.

![DAI+USDC dual pool auf Curve Fantom](../../.gitbook/assets/ftm-crv.png)

Es gibt noch viele andere Möglichkeiten auf Fantom, die in anderen Leitfäden beschrieben werden.

## Andere nützliche Links

* [Fantom Explorer](https://explorer.fantom.network)
* [Fantom Gas Checker](https://ftmscan.com/gastracker)
* Offizieller Fantom Discord server
* [DeBank](https://debank.com) Portfolio Verwaltung

## Haftungsausschluss

Dieser Leitfaden ist KEINE Finanzberatung und sollte lediglich als Bildungsinstrument betrachtet werden. Recherchiere immer selbst. Die Projekte, die in diesem Leitfaden vorgestellt werden, zeigen nur die Möglichkeiten des Netzwerks und sind nicht als Befürwortung des Projekts zu verstehen.

{% hint style="info" %}
_Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst._
{% endhint %}
