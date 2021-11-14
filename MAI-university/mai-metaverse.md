---
description: >-
  Dieser Leitfaden gibt einen Überblick über die verschiedenen Chains, auf denen
  der MAI Stable Coin verwendet werden kann, und wie du den nativen Coin auf
  andere Netzwerke übertragen kannst.
---

# MAI Metaverse

![](../.gitbook/assets/screen-shot-2021-09-13-at-1.06.42-pm.png)

## Intro

MAI, manchmal auch als miMATIC bezeichnet, ist der erste Stable Coin aus dem Polygon-Netzwerk. Er ist an den Preis von 1,00 $ gebunden und sein Wert kann zwischen 0,99 $ und 1,01 $ schwanken. Wie die Preisbindung aufrechterhalten wird, erfährst du in der [offiziellen Dokumentation](https://docs.mai.finance/stablecoin-economics). Allerdings gibt es MAI nicht nur auf Polygon, weil es dort beheimatet ist. Genauso wie DAI in verschiedenen Netzwerken zu finden ist (DAI ist ein weiterer Stable Coin aus dem Ethereum Mainnet), breitet sich MAI langsam aber sicher auch auf andere Netzwerke aus. In diesem Artikel stellen wir dir die verschiedenen Netzwerke vor, in denen du MAI finden kannst, und zeigen dir, wie du deinen MAI von einem Netzwerk in ein anderes übertragen kannst.

## Polygon

### MAI auf Polygon erhalten





Wie bereits erklärt, ist MAI in Polygon beheimatet und das ist der einzige Ort ( Stand September 2021), an dem du MAI prägen kannst, indem du entweder

* MAI gegen Sicherheiten leihen, die du zuvor in einem Vault bei Mai Finance hinterlegt hast
* Tausch von USDC gegen MAI auf [Mai Finance](https://app.mai.finance/anchor)
* einen anderen Vermögenswert verkaufst und MAI auf einem DEX (**D**ezentralisierte **EX**-Börse) auf Polygon kaufst. Die effizientesten sind [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) oder [1Inch](https://app.1inch.io/#/137/classic/swap).

### MAI auf Polygon nutzen

Der MAI Stable Coin wird in immer mehr Projekten auf Polygon eingesetzt, vor allem jetzt, wo er wie andere Stable Coins in großen Projekten wie QuickSwap verwendet wird. Im September 2021 gibt es 3 Stable Farms auf QuickSwap mit einer Gesamtsumme von 18.327.604 $:

* MAI-DAI mit $6.553.255
* MAI-USDT mit $6.316.026
* MAI-USDC mit 5.458.323 $

Weitere Pools findest du bei anderen Projekten / Ertragsfarmen / Ertragsoptimierern. Was du mit deinem MAI Stable Coin machen kannst, erfährst du in dem entsprechenden Artikel.

## Solana

### MAI auf Solana übertragen

Solana ist eine Blockchain-Plattform für dezentralisierte Apps. Das Ziel des Netzwerks ist es, niedrige Gebühren (weniger als $0,01) und schnelle (weniger als 400ms) Transaktionen anzubieten. Die Idee dahinter ist, eine Alternative zum Ethereum Mainnet und seinen Side Chains zu schaffen. Solana ist jedoch nicht deshalb ein direkter Konkurrent des Ethereum-Netzwerks, weil es nicht die gleichen Assets unterstützt. Tatsächlich unterstützt Solana jetzt den Stable Coin MAI, der von Polygon aus überbrückt werden kann (wo er geprägt werden kann).

Um deine MAI-Token nach Solana zu schicken, kannst du [AllBridge](https://allbridge.io) nutzen, eine Bridging-Plattform, mit der du Token von einer Chain zur anderen übertragen kannst. AllBridge unterstützt die folgenden Netzwerke:

* Ethereum Mainnet
* Polygon
* Solana
* Huobi
* Binance Smart Chain

Die Benutzeroberfläche ist wirklich intuitiv, denn du musst nur die beiden Netzwerke und den Vermögenswert auswählen, den du zwischen den beiden transferieren möchtest.

![MAI von Polygon nach Solana senden](../.gitbook/assets/screen-shot-2021-09-13-at-1.52.23-pm.png)

Im nächsten Schritt gibst du die Adresse deiner Solana Wallet und den Betrag an, den du überweisen möchtest. Beachte, dass MetaMask (noch?) keine Solana-Wallets unterstützt, du musst also eine eigene Wallet in diesem Netzwerk erstellen. Dabei kann es sich entweder um eine Web-Wallet wie MetaMask oder um eine App-Wallet handeln. Bitte lies die [offiziellen Empfehlungen von Solana](https://docs.solana.com/wallet-guide), bevor du dich für eine entscheidest.

{% hint style="info" %}
Beachte, dass Solana keinen Faucet anbietet, an dem du dein erstes SOL (natives Token, das zur Bezahlung von Transaktionen verwendet wird) bekommst. Du musst zuerst einige SOL kaufen und sie in deiner Wallet haben, damit du MAI auf deine Wallet übertragen kannst.
{% endhint %}

### MAI auf Solana nutzen

Genauso wie du MAI auf Polygon einsetzen kannst, um Liquidität zu schaffen und Erträge zu erwirtschaften, kannst du das auch auf Solana tun. Der wichtigste Ort, an dem du MAI einsetzen kannst, ist [Saber](https://app.saber.so), im MAI/USDC-Pool.

![MAI/USDC pool auf Saber, Stand Sept. 2021](../.gitbook/assets/screen-shot-2021-09-13-at-2.11.10-pm.png)

Das Gute am MAI/USDC-Pool auf saber ist, dass du im Gegensatz zu LP-Pools (**L**iquidität **P**providing) auf QuickSwap keine LP-Paare mit einer Ratio 1:1 bereitstellen musst. Du kannst einfach einen einzelnen Vermögenswert (**MAI** oder **USDC**) oder eine (un)ausgewogene Ratio der beiden Stable Coins hinterlegen.

![MAI und USDC sind im Saberpool nicht ausgeglichen](../.gitbook/assets/screen-shot-2021-09-13-at-2.13.51-pm.png)

Das bedeutet, dass du tatsächlich 100% MAI-Einlagen von Mai Finance nutzen kannst, ohne sie in USDC tauschen zu müssen. Das ist besonders praktisch und verhindert, dass du durch kleine Preisunterschiede zwischen den beiden Stable Coins beeinträchtigt wirst. Beachte, dass du Belohnungen in dem nativen Farm-Token ausbezahlt bekommst, genauso wie du in QUICK bezahlt wirst, wenn du auf QuickSwap auf Polygon farmst. Du kannst deine Saber-Tokens dann verkaufen, um deine MAI/USDC-Position zu erhöhen.

{% hint style="info" %}
Auf Solana kannst du auch [Sunny](https://app.sunny.ag) verwenden, einen Aggregator, der die Belohnungen von Saber automatisch aufstockt. Beachte, dass der Sunny-Aggregator nicht vom Mai-Finance-Team validiert wurde. AllBridge und Saber sind offizielle Partner von Mai Finance, aber die Ergebnisse sind nicht garantiert. Bitte recherchiere wie immer selbst.
{% endhint %}

## Avalanche

### MAI auf Avax übertragen

Avalanche ist ein Blockchain-Netzwerk, das eine Open-Source-Plattform und ein Layer-1-Protokoll für die Einführung von DeFi-Anwendungen und Blockchain-Lösungen für Unternehmen bietet. Es ist eine weitere Alternative zum Ethereum Mainnet, die die gleichen Assets wie Ethereum Mainnet, Polygon und Solana unterstützt. So kannst du jetzt deine MAI von Polygon (ab September 2021 der einzige Ort, an dem du MAI prägen kannst) über [Relay Chain](https://app.relaychain.com/#/transfer) an Avax senden.

Was AllBridge angeht, ist die Benutzeroberfläche recht einfach. Du wählst einfach das Netzwerk aus, aus dem das Asset überbrückt werden soll, das Ziel und das zu übertragende Asset.

![MAI von Polygon auf Avalanche übertragen](../.gitbook/assets/screen-shot-2021-09-13-at-2.52.31-pm.png)

Metamask **unterstützt** [Avax-Wallets](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche), du brauchst also keine zusätzliche Wallet wie für Solana.

### MAI auf Avax nutzen

Genauso wie du MAI zum Farmen von Erträgen auf Polygon verwenden kannst, kannst du MAI auf Avalanche verwenden. Der wichtigste Ort dafür ist [Trader Joe's Farmen](https://www.traderjoexyz.com/#/farm), wo du einen MAI/USDC-Pool findest.

![MAI/USDC Pool bei Trader Joe; Stand: Sept. 2021](../.gitbook/assets/screen-shot-2021-09-13-at-3.07.19-pm.png)

Die Farmen auf Avalanche funktionieren sehr ähnlich wie die auf Polygon. Du kannst Trader Joe's App also genauso nutzen wie QuickSwap. Du musst zuerst ein LP-Paar auf der Website mit der gleichen Ratio von MAI und USDC erstellen und dann das LP-Paar auf der Farm einzahlen. Genauso wie du bei QuickSwap in QUICK bezahlt wirst, erhältst du bei Trader Joe eine Belohnung in Form von JOE-Tokens. Du kannst diese Token dann in anderen Pools einsetzen oder sie verkaufen, um dein MAI/USDC-Paar zu erhöhen.

## Fantom

### MAI auf Fantom übertragen

Fantom ist eine Blockchain-/Smart-Contract-Plattform, deren Ziel es ist, die Skalierbarkeitsprobleme anderer Netzwerke zu lösen, insbesondere der Ethereum-Blockchain. Entwickler können ihre DApps (\*\*Dezentrale **App**Anwendungen) auf diesem Netzwerk erstellen und die gleichen Assets wie auf anderen Netzwerken verwenden. So kannst du schon jetzt MAI von Polygon zu Fantom übertragen, indem du die Brücke von [AnySwap](https://anyswap.exchange/#/bridge) benutzt.

AnySwap ist eine weitere Bridging-Lösung, deren Benutzeroberfläche der von AllBridge und Relay Chain sehr ähnlich ist. Auf Polygon musst du zuerst deine MetaMask Wallet verbinden und dann das zu überbrückende Asset (MAI) und das Zielnetzwerk (Fantom) auswählen.

![MAI von Polygon auf Fantom übertragen](../.gitbook/assets/image.png)

Metamask **unterstützt** [fantom wallets](https://docs.fantom.foundation/tutorials/set-up-metamask), also ist es sehr einfach, dein MAI auf Fantom einzurichten und es sofort zu benutzen.

### MAI auf Fantom nutzen

Derzeit hat das Mai Finance Team keine Partnerschaft mit einer Yield Farm auf Fantom. Sobald das Team von Projekten erfährt, die MAI nutzen, wird diese Dokumentation aktualisiert. Warte noch etwas ab.

## Haftungsausschluss

Die Details in diesem Leitfaden sind rein informativ und wurden nicht direkt von dem Team, das diesen Leitfaden erstellt, getestet. Einige Nutzer auf dem Discord-Server haben bereits versucht, ihr Vermögen zu Solana und/oder Avalanche zu überbrücken, also kannst du der Discord-Community beitreten und deine Fragen stellen. Bitte vergiss nicht, deine eigenen Nachforschungen anzustellen, denn verschiedene Netzwerke haben unterschiedliche Transaktionsgebühren und Ausführungszeiten, verschiedene Belohnungsprogramme, Überbrückungsgebühren usw. Wenn du deine MAI an andere Netzwerke sendest, stelle sicher, dass du sie zurückbrücken kannst, falls du sie auf Polygon brauchst.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
