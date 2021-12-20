---
description: >-
  In questa guida spiegheremo tutto ciò che devi sapere per iniziare a
  utilizzare le diverse DApp disponibili sulla blockchain Avalanche.
---

# Come iniziare con Avalanche

## Cos'è Avalanche?

Avalanche è una blockchain di primo livello (Layer-1) che funziona come piattaforma per applicazioni decentralizzate e reti blockchain personalizzate. La rete Avalanche è composta da tre blockchain individuali: X-Chain, C-Chain e P-Chain. Ogni chain ha uno scopo distinto, totalmente distinto l'uno dall'altro, con l'obbiettivo di fare in modo che tutti i nodi convalidino tutte le transazioni. Le blockchain Avalanche utilizzano anche diversi meccanismi di consenso in base ai loro casi d'uso.

Avalanche è compatibile al 100% compatibile EVM e con la toolchain Ethereum esistente e la sua C-Chain offre le stesse funzionalità di Ethereum ma con un capacità di calcolo più elevato, un tempo di esecuzione ridotto e commissioni di transazione molto più basse. AVAX è il token gas nativo della rete Avalanche.

## Primi passi con Avalanche

Prima di utilizzare la rete Avalanche, è necessario creare un portafoglio. Esistono diversi tipi di portafoglio che possono essere utilizzati, inclusi \*\*portafogli software\*\* come Metamask o quello nativo della rete [Avalanche Wallet](https://wallet.avax.network), oltre agli \*\*hardware wallets \*\* come [Trezor](https://trezor.io/coins/) o [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true).

Ai fini di questo tutorial, utilizzeremo Metamask. Se non hai installato Metamask, puoi trovare le istruzioni nel tutorial [Come iniziare con Polygon](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/italian/tutorial-di-polygon/come-iniziare-con-polygon).

### Aggiungere la rete Avalanche a Metamask

Per utilizzare la rete Avalanche, dovrai aggiungerla a Metamask. Per farlo, dovrai entrare nelle Impostazioni di Metamask, selezionare "Reti" (se è la prima volta che lo configuri, troverai pre impostate solo la rete Ethereum Mainnet e le reti testnet) e selezionare "Aggiungi Rete". Dovrai quindi compilare i campi con i seguenti parametri:

* **Nome Rete**: Avalanche Network
* **Nuovo RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Simbolo**: AVAX
* **URL del Block Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Salva le modifiche e Metamask selezionerà automaticamente la rete Avalanche. Se così non fosse cliccando sul menu a tendina potrai selezionarla manualmente.

![Ottimo lavoro! Ora sei su Avalanche!](<../../.gitbook/assets/image (40).png>)

## Trasferire assets da un'altra blockchain verso Avalanche (Bridging)

### AVAX Faucets

Al momento non ci sono faucets (contratti che ti "regalano" qualche $AVAX per le prime transazioni) disponibili sulla rete principale di Avalanche. Se hai bisogno di $AVAX per coprire i costi del gas, dovrai inviare $AVAX direttamente al tuo portafoglio da uno exchange centralizzato o trasferendo i tuoi assets usando il bridge Elknet. Maggiori informazioni su questa seconda opzione nella sezione Bridges di seguito.

### Bridges

* [Official Avalanche bridge](https://bridge.avax.network) - Avalanche ha un proprio bridge che può essere utilizzato per trasferire gli assets dalla rete principale di Ethereum ad Avalanche. Le commissioni vengono pagate nel token di origine e possono essere abbastanza elevate visto che stiamo partendo da Ethereum.
* [Anyswap](https://anyswap.exchange/#/bridge) consente di trasferire gli assets tra molteplici chain diverse. Ci sono importi minimi richiesti per il trasferimento e variano a seconda del token ma il costo del bridging è a tariffa fissa.
* [Celer Bridge](https://cbridge.celer.network/#/transfer) offre trasferimenti da e verso molte chain con un' interfaccia utente semplice e curata. La commissione di bridging è di circa il 3% verso Avalanche.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) offre un'interfaccia intuitiva e facile da usare e commissioni basse. Come nota a margine, Relay Chain è la soluzione ufficialmente supportata per [trasferire MAI ad Avalanche](../../Universita-di-MAI/mai-metaverse.md#avalanche).
* [Elknet](https://app.elk.finance/#/elknet) è un servizio di bridging offerto da Elk Finance, è un exchange decentralizzato disponibile su più reti tra cui Avalanche, Binance Smart Chain, Fantom, Polygon e xDai. Ciò che distingue Elknet dagli altri bridge in questo elenco è che non è richiesto AVAX per il bridging, ma c'è un problema che vedremo di seguito. La commissione di trasferimento è solo il costo del gas per la transazione.
  * Per spostare i tuoi token su Avalanche tramite Elknet, dovrai prima convertirli in $ELK, il token nativo di Elk Finance.
  * Potrai quindi utilizzare il bridge per spostare gli $ELK dalla chain di partenza ad Avalanche, inoltre selezionando "Swap $ELK 1 for gas", un $ELK sarà convertito in $AVAX per permetterti di coprire i costi delle prime transazioni su Avalanche.
  * Una volta completato il bridging (di solito meno di 5 minuti), dovrai selezionare la rete Avalanche nel tuo portafoglio Metamask e vedrai i tuoi $ELK e un po' di $AVAX pronti per essere usati. Ora potrai scambiare i tuoi $ELK con qualsiasi token supportato su Avalanche, direttamente da Elk Finance.
  * Lo stessa cosa può essere fatta al contrario per tornare a Polygon o a qualsiasi altra chain supportata.

![Interfaccia Elknet](<../../.gitbook/assets/image (37).png>)

## DeFI su Avalanche

Avalanche ha visto una grande crescita negli ultimi mesi che ha portato non solo allo sviluppo di importanti nuovi progetti nativi ma anche all'arrivo dei big player assodati della deFi che hanno di recente pubblicato le loro piattaforme (ad esempio Aave) o che arriveranno a breve (come Curve).

* [Aave](https://app.aave.com/dashboard) è stato lanciato di recente su Avalanche e ha già visto $4 miliardi di valore totale bloccato(TVL). I token supportati come collaterali su Avalanche includono $AAVE, $AVAX, $DAI, $USDT, $USDC, $WBTC e $WETH. I token camAVAX saranno accettati come garanzia per i depositi su Mai Finance.
* [Beefy Finance](https://app.beefy.finance/#/avax) è ben noto alla maggior parte degli utenti deFI in quanto è disponibile su altre chain tra cui Binance Smart Chain,Polygon, Fantom e Harmony. Beefy è noto come un auto compounder (reinveste automaticamente le rewards delle farms) e attualmente fornisce ottimi APY sia per il farm single token che dual token. Beefy offre funzionalità di auto reinvestimento per le coppie [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) e [MAI/USDC.e ](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e)LPs che trovate sulla piattaforma Trader Joe.
* [Benqi](https://app.benqi.fi/markets) è un protocollo di mercato simile ad Aave ed è stato il primo del suo genere sulla rete Avalanche. I token collaterali supportati includono $AVAX, $DAI, $LINK, $USDT, $USDC, $WBTC e $WETH.

![Interfaccia di BenQI](<../../.gitbook/assets/image (36).png>)

* [TraderJoe](https://www.traderjoexyz.com/#/home) è un exchange decentralizzato ed è diventato uno dei migliori progetti su Avalanche con un'interfaccia utente intuitiva e una innovativa funzionalità di zapping che consente agli utenti di convertire un token direttamente in un pool di liquidità. TraderJoe è anche partner ufficiale del pool [MAI-USDC LP Avalanche](../../Universita-di-MAI/mai-metaverse.md#usare-mai-su-avax).

![Interfaccia di TraderJoe](<../../.gitbook/assets/image (39).png>)

* [YieldYak](https://yieldyak.com/farms) è un altro auto compounder che fornisce alti APY sul farming. Le sue farm single token  sono create sulla base di BenQI per sfruttare rendimenti più elevati e sono quindi da considerarsi rischiose.

![Interfaccia di YieldYak](<../../.gitbook/assets/image (41).png>)

## Altri link utili

* [Avalanche Network](htts://avax)
* [Avalanche community links](https://www.avax.network/community) (Discord, Medium, Reddit, Twitter, etc)
* [Debank](https://debank.com), Gestione portafoglio multi-chain

## Disclaimer

Questa guida NON è un consiglio finanziario e va considerata a pure scopo educativo. Fai sempre le tue ricerche. La discussione di un progetto in questa guida non deve essere considerata come un'approvazione del progetto stesso.
