---
description: >-
  In diesem Leitfaden erklären wir dir alles, was du wissen musst, um die
  Harmony Chain zu benutzen.
---

# Einstieg in Harmony

## Was ist Harmony?

Harmony ist eine Blockchain, die versucht, die Probleme zu lösen, mit denen das Ethereum Mainnet zu kämpfen hat: ein zufriedenstellendes Gleichgewicht zwischen Dezentralisierung und Skalierbarkeit zu erreichen. Das Hauptaugenmerk der Chain liegt auf einem hohen Transaktionsdurchsatz, Geschwindigkeit und Energieeffizienz. Dies wird erreicht, indem das Sharding von Validatoren, die in Gruppen zusammengefasst werden, um Transaktionen gleichzeitig zu verarbeiten, optimal ausgenutzt wird. Um die Skalierbarkeit zu unterstützen, wird die Anzahl der Shards erhöht, was ebenfalls zu einer schnelleren Transaktion beiträgt. Mehr über Harmony und seine Technologie erfährst du in der [offiziellen Dokumentation](https://docs.harmony.one/home/general/technology).

## Los gehts auf Harmony

Um das Harmony-Netzwerk nutzen zu können, brauchst du eine Wallet-Adresse. Da Harmony ein EVM-kompatibles Netzwerk (**E**thereum **V**irtual **M**achine) ist, akzeptiert es die gleichen Wallets wie andere EVM-kompatible Chains, einschließlich Web-Wallets wie Metamask oder Nifty, und du kannst deine Hardware-Wallets wie Trezor oder Ledger verwenden.

Für dieses Tutorial werden wir uns wie bei allen anderen Anleitungen auf dieser Seite an Metamask halten. Wenn du Metamask nicht installiert hast, findest du eine Anleitung auf [Der Start auf Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Harmony zu Metamask hinzufügen

Wenn du die neueste Version von Metamask installiert hast, solltest du bereits Zugriff auf die Harmony Chain haben und musst nichts weiter tun, als "Harmony One" im Netzwerk-Dropdown oben in Metamask auszuwählen. Du kannst auch selbst eine neue RPC einrichten, um auf Harmony zuzugreifen, indem du diese Schritte ausführst. Öffne das Metamask-Popup, klicke auf das Symbol deiner Wallet, navigiere zu "Einstellungen", wähle "Netzwerke" und suche "Harmony One". Die Daten, die du erhalten solltest, sind wie folgt:

* **Netzwerkname:** Harmony One
* **Neue RPC URL:** https://api.harmony.one
* **Chain ID:** 1666600000
* **Währungssymbol:** ONE
* **Block Explorer URL:** https://explorer.harmony.one/

Speichere die Änderungen und Metamask wird sich automatisch auf das Harmony-Netzwerk umstellen:

![Glückwunsch!! Du bist jetzt auf Harmony](../../.gitbook/assets/Harmony-onboarding-1.png)

## Bridging zu Harmony One

### Faucets

Es gibt keinen offiziellen Faucets, um deine ersten ONE-Token für deine ersten Transaktionen zu bekommen. Meistens musst du einige Token von einer anderen Chain über die offizielle [Harmony-Bridge](https://bridge.harmony.one/erc20) überbrücken, mit der du bestimmte Assets entweder vom Ehtereum Mainnet oder von Binance zu Harmony überbrücken kannst. Eine Liste der Projekte, mit denen du ONE über Fiat Gateways oder Exchange Gateways beziehen kannst, findest du in [diese Liste](https://docs.harmony.one/home/developers/harmony-stack#bridges-fiat-gateways-exchanges), die vom Harmony-Team zusammengestellt wurde.

Wie immer kannst du auch [ElkNet](https://app.elk.finance/#/elknet) nutzen, um ELK-Token von anderen Chains zu Harmony zu transferieren. Wenn du das tust, achte darauf, das Kästchen `Swap $ELK 1 for gas` anzukreuzen, das einen Teil deiner übertragenen Token in ONE tauscht, wodurch du auch den Rest deiner ELK-Token in mehr ONE oder andere Assets tauschen kannst.

### Bridges

* [Multichain.org](https://app.multichain.org/#/router) (früher bekannt als AnySwap) ist der offizielle Partner von Mai Finance, mit dem du deine MAI-Token von Polygon und anderen Chains auf Harmony übertragen kannst. Übrigens: Multichain arbeitet Hand in Hand mit den Entwicklern von Mai Finance, um sicherzustellen, dass die MAI, die du zu Harmony überbrückst, die gleichen sind, die du dir auf der Lending-Plattform leihen kannst. Ein Hub auf Harmony ist nicht nötig. Gehe einfach zum Multichain-Router, wähle das Herkunftsnetzwerk, den Token, den du übertragen willst, und das Zielnetzwerk aus und schon bist du fertig. Beachte die Mindestbeträge für Transfers, die Transfergebühren und die Überbrückungsdauer, aber sobald du das getan hast, bekommst du dein Asset auf Harmony.

![Überbrücke MAI von Polygon zu Harmony One](../../.gitbook/assets/Harmony-onboarding-2.png)

* Mit der [Official Harmony Bridge](https://bridge.harmony.one/erc20) kannst du, wie im vorherigen Absatz erklärt, bestimmte Vermögenswerte vom Ethereum Mainnet oder BSC übertragen.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) ist eine weitere Lösung, wenn du etwas auf Harmony übertragen möchtest. Überprüfe ihre Anwendung, um zu sehen, welche Assets überbrückbar sind.
* [ElkNet](https://app.elk.finance/#/elknet) ist ein besonderer Fall, denn mit der Bridge von Elk Finance kannst du den ELK-Token von jeder EVM-kompatiblen Chain zu jeder anderen EVM-kompatiblen Chain übertragen, auf der sie eingesetzt werden.

## DeFi auf Harmony

Da Harmony One ein Netzwerk ist, das schnelle und sichere Transaktionen sowie sehr günstiges Gas bietet, wurden viele EVM-kompatible DApps (**D**ecentralized **App**lications) in diesem Netzwerk implementiert. Die folgende Liste enthält _nicht_ alle, aber du kannst das Netzwerk und seine DApps selbst erkunden. Eine [umfassendere Liste findest du auf DefiLlama](https://defillama.com/chain/Harmony).

* [ViperSwap](https://viper.exchange/#/swap): Dies ist der erste Partner von Mai Finance auf Harmony One. Es handelt sich um einen regulären Uniswap v2 Fork, eine DEX (**D**ecentralized **Ex**change) und AMM (**A**utomated **M**arket **M**aker), bei der du deine Vermögenswerte tauschen, LP (**L**iquidity **P**roviding) Token erstellen und Belohnungen farmen kannst, indem du Händlern Liquidität zur Verfügung stellst. Die Belohnung wird mit dem VIPER-Token bezahlt, den du in der App für weitere Belohnungen staken kannst. Hier findest du MAI-Liquidität, um deine MAI zu tauschen oder Belohnungen mit deinen MAI zu farmen.

![MAI-ONE und MAI-VIPER Pools auf ViperSwap, Stand Dezember 2021](../../.gitbook/assets/Harmony-onboarding-3.png)

Du wirst feststellen, dass die APRs (**A**nnual **P**ercentage **R**ate) auf Pools sehr hoch sind. Das liegt vor allem am Belohnungsformat auf ViperSwap: Wenn du deine Belohnung einforderst, können 5% der VIPER-Tokens direkt verwendet werden, während 95% bis zum 25.12.2021 gesperrt sind. Anschließend wird die Belohnung über ein ganzes Jahr gesperrt, was bedeutet, dass du nicht sofort auf deine Gewinne beim Farmen zugreifen kannst, sondern dass sie SEHR langsam abfließen werden. Es gibt noch eine weitere Besonderheit bei den ViperSwap-Pools: Du musst eine Abhebungsgebühr zahlen, die sinkt, wenn du deine LP-Token über einen längeren Zeitraum stakst. Die Gebühr trifft von 25%, wenn du innerhalb desselben Blocks wie die Einzahlung abhebst (um Flashloan-Operationen zu verhindern), auf 0,01%, wenn du nach einem Monat abhebst. Mehr Details in der offiziellen Dokumentation über [Belohnungen beim Farmen](https://docs.venomdao.org/viper/tokenomics#bbd0) und [LP-Abhebungsgebühren](https://docs.venomdao.org/viper/fees).

<<<<<<< HEAD
* [DeFi Kingdom](https://game.defikingdoms.com/#/): Dies ist ein besonders interessantes Projekt, das DeFi und Gamification miteinander verbindet. Sein nativer Token, der JEWEL-Token, wird als Belohnung für das Farmen von Nutzern verwendet, die Liquidität bereitstellen, kann aber auch im Spiel oder auf dem Marktplatz eingesetzt werden. Das gesamte Universum von DeFi Kingdom (oder DFK) zu erklären, würde zu viel Zeit für diesen Leitfaden in Anspruch nehmen, daher empfehlen wir dir dringend, [die offizielle Dokumentation](https://docs.defikingdoms.com) zu lesen.
=======
* [DeFi Kingdom](https://game.defikingdoms.com/#/): This is a particularly interesting project that is mixing DeFi and Gamification. Its native token, the JEWEL token, is used as a farming reward for users that are providing liquidity, but it can be used in game or in the marketplace. Explaining the entire universe of DeFi Kingdom (or DFK) would take too much time for this guide, so we strongly recommend reading [the official documentation](https://docs.defikingdoms.com/).
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

![Hauptkarte von DeFi Kingdom, Stand Dezember 2021](../../.gitbook/assets/Harmony-onboarding-4.png)

<<<<<<< HEAD
* [SushiSwap](https://app.sushi.com) ist das berühmte DEX/AMM, das es auch bei vielen anderen Chains gibt. Tausche, biete Liquidität an, farm ONE und SUSHI Yields.
* [Curve Finance](https://harmony.curve.fi) ist eine weitere Chain-übergreifende Anwendung, mit der du Liquidität (3pool und Tricrypto) bereitstellen kannst und die dich mit zusammengesetzten Token sowie ONE und CRV belohnt.
* [Beefy Finance](https://app.beefy.finance/#/harmony) ist ein Renditeoptimierer, den wir bereits in vielen unserer Leitfäden vorstellen, da er auf vielen Chains vertreten ist. Derzeit kannst du deine LP-Token von Curve und SushiSwap einzahlen und die Belohnungen der Farmen durch den Beefy Compounder in weitere LP-Token umwandeln lassen.
* Die [Euphoria DAO](https://app.euphoria.money/#/dashboard) ist derzeit die größte OHM-Fork auf Harmony und wurde von der Venom DAO entwickelt, die auch hinter ViperSwap steht. Du kannst verschiedene Assets bonden und bekommst dafür den WAGMI-Token. Stake WAGMIs für mehr WAGMI mit irrsinnigen APY (**A**nnnual **P**ercentage **Y**ield) wie bei den meisten OHM-Projekten.
=======
* [SushiSwap](https://app.sushi.com) is the famous DEX/AMM that is also present on many other chains. Swap, provide liquidity, farm ONE and SUSHI yields.
* [Curve Finance](https://harmony.curve.fi/) is another cross-chain application that will let you provide liquidity (3pool and tricrypto) and will reward you with compounded tokens, as well as ONE and CRV.
* [Beefy Finance](https://app.beefy.finance/#/harmony) is a yield optimizer that we already present in many of our guides since it's present on many chains. Currently, you will be able to deposit your LP tokens from Curve and SushiSwap, and let the Beefy compounder aggregate the rewards provided by the farming platform into more LP tokens.
* [Euphoria DAO](https://app.euphoria.money/#/dashboard) is currently the biggest Ohm-fork on Harmony, and developped by the Venom DAO also behind ViperSwap. You can bond a few different assets and get their native asset, the WAGMI token. Stake WAGMIs for more WAGMI with insane APY (**A**nnual **P**ercentage **Y**ield) as for most OHM projects.
>>>>>>> dd7bf1b (GitBook: [#262] Optimism + Arbi + BNB + Moonbeam)

## Mai Finance auf Harmony

Mai Finance startet auf Harmony One im Dezember 2021 und dieser Leitfaden ist ziemlich kurz vor dem Startdatum, so dass die Anwendung vielleicht schon aktualisiert wurde, wenn du ihn liest.

Du kannst deine WETH- oder ONE-Token bei Mai Finance (https://app.mai.finance/vaults/create) einzahlen, um den Stable Coin MAI zu leihen. Dann kannst du MAI tauschen, um dein Vermögen zu hebeln, Marginhandel zu betreiben oder auf ViperSwap Renditen zu farmen.

![MAI Finance vaults, Stand Dezember 2021](../../.gitbook/assets/Harmony-onboarding-5.png)

## Haftungsausschluss

Wie üblich stellt dieser Leitfaden keine Finanzberatung dar und sollte lediglich als Bildungsinstrument betrachtet werden. Recherchiere immer selbst. Die Erörterung eines Projekts in diesem Leitfaden sollte nicht als Befürwortung des Projekts angesehen werden.

{% hint style="info" %}
Denke daran, dass eine Strategie, die zu einem bestimmten Zeitpunkt gut funktioniert, zu einem anderen Zeitpunkt schlecht abschneiden (oder Geldverluste erzeugen) kann. Bitte bleibe informiert, beobachte die Märkte, behalte deine Investitionen im Auge und recherchiere wie immer selbst.
{% endhint %}
