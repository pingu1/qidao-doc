---
description: >-
  In diesem Leitfaden erklären wir dir alles, was du wissen musst, um die
  Avalanche Chain zu benutzen.
---

# Einstieg in Avalanche

## Was ist Avalanche?

Avalanche ist eine Layer-One-Blockchain, die als Plattform für dezentrale Anwendungen und eigene Blockchain-Netzwerke fungiert. Das Avalanche-Netzwerk besteht aus drei einzelnen Blockchains: der X-Chain, C-Chain und P-Chain. Jede Chain hat einen bestimmten Zweck, der sich grundlegend von dem der anderen unterscheidet, nämlich dass alle Knotenpunkte alle Transaktionen validieren müssen. Avalanche-Blockchains verwenden je nach Anwendungsfall sogar unterschiedliche Konsensmechanismen.

Avalanche ist zu 100 % EVM-kompatibel mit der bestehenden Ethereum-Toolchain und seine C-Chain bietet dieselben Funktionen wie Ethereum, jedoch mit einem höheren Durchsatz, einer Endgültigkeit von weniger als einer Sekunde und viel niedrigeren Transaktionsgebühren. AVAX ist dabei der native Gas-Token des Avalanche-Netzwerks.

## Der Einstieg ins Avalanche-Ökosystem

Bevor du das Avalanche-Netzwerk nutzen kannst, musst du eine Wallet-Adresse erstellen. Es gibt verschiedene Wallet-Typen, die verwendet werden können, darunter **Software-Wallets** wie Metamask oder das native [Avalanche Wallet](https://wallet.avax.network) sowie **Hardware-Wallets** wie [Trezor](https://trezor.io/coins/) oder [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true).

Für dieses Tutorial werden wir Metamask verwenden. Wenn du Metamask nicht installiert hast, findest du eine Anleitung unter ["Der Start auf Polygon"](../investment-tutorials/how-to-get-started-on-polygon.md).

### Avalanche zu Metamask hinzufügen

Um das Avalanche-Netzwerk nutzen zu können, musst du es zu Metamask hinzufügen. Dazu klickst du auf das Network-Dropdown-Menü (wenn du es zum ersten Mal einrichtest, steht dort Ethereum Mainnet) und wählst dann "Custom RPC". In dem sich öffnenden Formular kannst du dann die folgenden Werte hinzufügen:

* **Network Name**: Avalanche Network
* **New RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Symbol**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Wenn du die Änderungen speicherst, schaltet Metamask automatisch auf das Avalanche-Netzwerk um.

![Du bist nun erfolgreich auf Avalanche!](../.gitbook/assets/avax\_MM.png)

## Token auf Avalanche transferieren

### Faucets

Im Avalanche-Hauptnetz gibt es derzeit keine Faucets. Wenn du AVAX benötigst, um die Gaskosten zu decken, musst du AVAX von einer zentralen Börse direkt auf deine Wallet schicken oder Token über die Elknet-Bridge überbrücken. Mehr über diese zweite Option erfährst du weiter unten im Abschnitt Bridges.

### Bridges

* [Offizielle Avalanche-Brücke](https://bridge.avax.network) - Avalanche hat seine eigene Brücke, mit der man Vermögenswerte vom Ethereum-Mainnet zu Avalanche überbrücken kann. Die Gasgebühren werden in dem überbrückten Token bezahlt und können hoch sein, da du von Ethereum überbrückst.
* [Anyswap](https://anyswap.exchange/#/bridge) ermöglicht auch die Überbrückung von Vermögenswerten zu vielen verschiedenen Chains. Es gibt Mindestbeträge für die Überbrückung, die je nach Token variieren, aber die Kosten für die Überbrückung sind eine Pauschalgebühr.
* [Celer Bridge](https://cbridge.celer.network/#/transfer) bietet Bridging-Dienste für viele Chains mit einer tollen Benutzeroberfläche. Die Überbrückungsgebühr beträgt etwa 3% für Avalanche.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) bietet eine einfach zu bedienende und intuitive Benutzeroberfläche mit niedrigen Gebühren. Nebenbei bemerkt ist Relay Chain die offiziell unterstützte Lösung, um MAI zu Avalanche zu überbrücken.
* [Elknet](https://app.elk.finance/#/elknet) ist ein Überbrückungsdienst, der von Elk Finance angeboten wird, einer dezentralen Börse, die in mehreren Netzwerken wie Avalanche, Binance, Fantom, Polygon und xDai verfügbar ist. Was Elknet von den anderen Bridges auf dieser Liste unterscheidet, ist, dass für die Überbrückung keine AVAX erforderlich ist, aber es gibt einen Haken, auf den wir weiter unten eingehen. Die Überbrückungskosten sind lediglich die Gaskosten für die Transaktion.
  * Um deine Token über Elknet nach Avalanche zu transferieren, musst du sie zunächst in Elk, den nativen Token von Elk Finance, umwandeln.
  * Dann kannst du die Bridge nutzen, um deine ELK aus den unterstützten Netzwerken nach Avalanche zu transferieren. Wenn du das Häkchen bei "Swap $ELK 1 for gas" setzt, wird ein Teil deines Transfers in AVAX umgewandelt.
  * Sobald die Überbrückung abgeschlossen ist (in der Regel in weniger als 10 Minuten), kannst du deine Wallet auf das Avalanche-Netzwerk umstellen und du siehst dein ELK und einen Teil der AVAX bereit zum Einsatz. Jetzt kannst du deinen ELK direkt auf der Website gegen jeden unterstützten Token auf Avalanche tauschen.
  * Das Gleiche kannst du in umgekehrter Richtung tun, um zu Polygon oder einer anderen unterstützten Chain zurückzukehren.

![Elknet Oberfläche](../.gitbook/assets/AVAX\_elkswap.png)

## DeFI auf Avalanche

Avalanche hat in den letzten Monaten ein starkes Wachstum erlebt, was nicht nur zur Entwicklung großartiger nativer Projekte geführt hat, sondern auch dazu, dass große DeFi-Bluechips beginnen, auf das Netzwerk umzusteigen, darunter auch Curve, das dort noch starten wird.

* [Aave](https://app.aave.com/dashboard) ist vor kurzem auf Avalanche gestartet und hat bereits einen Gesamtwert von 4 Milliarden Dollar gebunden. Zu den unterstützten Sicherheiten für Avalanche Mai Finance Vaults gehören Aave, Avalanche, Dai, Tether, USDC, WBTC und WETH. camAVAX-Token.
* [Beefy Finance](https://app.beefy.finance/#/avax) ist den meisten deFI-Nutzern wahrscheinlich bekannt, da es auf anderen Chains wie Binance, Fantom, Harmony, Polygon und anderen verfügbar ist. Beefy ist ein sogenannter Autocompounder und bietet derzeit großartige Farming-APYs sowohl für Single-Token- als auch für Dual-Token-Farmen. Beefy bietet Autocompounding-Funktionen für die LPs [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) und [MAI/USDC.e](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e), die du bei Trader Joe findest.
* [Benqi](https://app.benqi.fi/markets) ist ein Marktprotokoll ähnlich dem von Aave und war das erste seiner Art im Netzwerk. Zu den unterstützten Sicherheitstoken gehören Avalanche, Dai, Link, Tether, USDC, WBTC und WETH.

![BenQI Oberfläche](../.gitbook/assets/AVAX\_benqi.png)

* [TraderJoe](https://www.traderjoexyz.com/#/home) ist eine dezentrale Börse und hat sich mit einer intuitiven Benutzeroberfläche und einer großartigen Zapping-Funktion, die es Nutzern ermöglicht, einen Token direkt in einen Liquiditätspool-Token umzuwandeln, zu einem der Top-Projekte auf Avalanche entwickelt. TraderJoe ist außerdem offizieller Partner eines MAI-USDC LP Pool auf Avalanche.

![](../.gitbook/assets/AVAX\_joe.png)

* [YieldYak](https://yieldyak.com/farms) ist ein weiterer Autocompounder, der ebenfalls hohe Farming-APYs bietet. Seine Single-Token-Farmen arbeiten in Verbindung mit BenQI, um höhere Renditen zu erzielen, und sind daher als riskant zu betrachten.

![](../.gitbook/assets/avax\_yak.png)

## Andere nützliche Links

* [Avalanche Netzwerk](htts://avax)
* [Avalanche Community Links](https://www.avax.network/community) (Discord, Medium, Reddit, Twitter, etc)
* [Debank](https://debank.com), Portfoliomanager

## Haftungsausschluss

Dieser Leitfaden ist KEINE Finanzberatung und sollte lediglich als Bildungsinstrument betrachtet werden. Recherchiere immer selbst. Die Erörterung eines Projekts in diesem Leitfaden sollte nicht als Befürwortung des Projekts angesehen werden.
