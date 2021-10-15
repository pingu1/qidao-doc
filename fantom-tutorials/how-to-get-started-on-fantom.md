---
description: >-
  In questa guida spiegheremo tutto ciò che devi sapere per iniziare a
  utilizzare le diverse DApp disponibili sulla blockchain Fantom.
---

# Come iniziare con Fantom

## Cos'è Fantom?

Fantom è un'alternativa a Ethereum. In quanto blockchain abilitata agli smart contract open source, consente agli sviluppatori di creare DApp (applicazioni decentralizzate) sicure, complete e modulari.

La chain è stata progettata per superare tutte le limitazioni della precedente generazione di  blockchain, nel settore conosciute come il trilemma blockchain: decentralizzazione, sicurezza e scalabilità. Per migliorare uno di questi limiti bisogna scendere a compromessi su uno degli altri due. Fantom ha cercato di risolvere questo problema grazie al suo meccanismo di consenso basato su DAG (**D**irected **A**cyclic **G**raphs) Lachesis aBFT (**A**synchronous **B**izantine **F**ault **T**olerant), che gli consente di ottenere alte prestazioni, scalabilità e sicurezza. I benchmark iniziali hanno dimostrato la capacità di Fantom di gestire oltre 20.000 transazioni al secondo.

Infine, Fantom è 100% EVM (**E**thereum **V**irtual **M**achine) compatibile, ciò significa che le DApp che sono state sviluppate su reti compatibili con EVM sono facilmente implementabili anche su Fantom. Questo porta anche altri vantaggi per gli utenti dato che MetaMask e altre applicazioni web3 sono già compatibili con Fantom. E' quindi immediato passare senza problemi da Polygon o Avalanche a Fantom all'interno dello stesso portafoglio.

## Iniziare con Fantom

Essendo Fantom compatibile con EVM, se hai già un portafoglio per altre chain EVM (Ethereum Mainnet, Polygon o Avalanche), potrai utilizzarlo da subito. Se sei ai primi passi, è il momento di creare il tuo portafoglio. Esistono diversi tipi di portafoglio che possono essere utilizzati: **software wallets** come [Metamask](how-to-get-started-on-fantom.md#what-is-fantom) e [fWallet](https://pwawallet.fantom.network/#/) oppure **hardware wallets** come [Trezor](https://trezor.io/coins/) e [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/).

Per questa guida e per essere allineati alle altre nostre guide basate su Metamask utilizzeremo Metamask, ma sentiti libero di utilizzare qualsiasi altro portafoglio software/hardware che preferisci. Se hai bisogno di istruzioni su come installare Metamask, puoi trovarle nella guida [come iniziare con Polygon](../tutorial-di-polygon/come-iniziare-con-polygon.md).

### Aggiungere la rete Fantom a Metamask

Per utilizzare la rete Fantom, dovrai aggiungerla a Metamask. Per farlo, dovrai entrare nelle Impostazioni di Metamask, selezionare "Reti" (se è la prima volta che lo configuri, troverai pre impostate solo la rete Ethereum Mainnet e le reti testnet) e selezionare "Aggiungi Rete". Dovrai quindi compilare i campi con i seguenti parametri:

* **Nome Rete**: Fantom Opera
* **Nuovo RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Simbolo**: FTM
* **URL del Block Explorer**: https://ftmscan.com

Salva le modifiche e Metamask selezionerà automaticamente la rete Avalanche. Se così non fosse cliccando sul menu a tendina potrai selezionarla manualmente.

![Ottimo lavoro! Ora sei su Fantom!](../.gitbook/assets/ftm-mm0.png)

Se hai bisogno di maggiori dettagli per configurare Metamask, troverai ulteriori informazioni nella guida ufficiale del team [Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask).

### FTM faucet

Ora che sei su FTM, avrai bisogno di $FTM (token nativo utilizzato per pagare le commissioni di transazione). Puoi trasferire alcuni token $FTM da altre chain o utilizzare un faucet (contratti che ti "regalano" qualche $FTM per le prime transazioni) per ottenere qualche token $FTM per eseguire le transazioni. Il [faucet principale di Fantom](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas) si trova su SpookySwap, uno dei DEX più importanti della rete (**Ex**change **D**ecentralizzato). Nota che il servizio offerto da SpookySwap si basa su Discord e richiede un account Discord valido attivo da più di 30 giorni per evitare richieste eccessive (non è necessario essere all'interno del server Discord di SpookySwap per 30 giorni).

* Una volta entrato nel server di [SpookySwap Discord](http://discord.gg/AqbsWsWDgn) ed esserti verificato col bot, vedrai vari canali, entra in  #faucet.

![Canale #faucet all'interno del server Discord di SpookySwap](<../.gitbook/assets/image (42).png>)

* Nel canale #faucet, dovrai inviare il comando`!faucet` ed il bot interagirà con te e ti garantirà qualche $FTM. Il limite massimo è di una richiesta ogni 30 giorni.
* Se vuoi verificare di aver ricevuto correttamente i tuoi token $FTM, puoi fare clic sul nome "Bot Fantom Tip" per interagire direttamente col bot e digitare `!balance`

![Grazie Fantom Tip Bot e SpookySwap](<../.gitbook/assets/image (45).png>)

* Tutto quello che devi fare ora è ricevere i tuoi token $FTM all'indirizzo del tuo portafoglio usando il comando `!withdraw <indirizzo del tuo portafoglio>`. L'indirizzo del tuo portafoglio si trova nella parte superiore della finestra di Metamask.

![Ritirare i tuoi token dal tuo account Discord](../.gitbook/assets/ftm-faucet.png)

![Deposito ricevuto dal faucet al wallet Metamask](../.gitbook/assets/ftm-mm.png)

## Trasferire assets da un'altra blockchain verso Fantom (Bridging)

### Trasferimento di stable coins / ETH / BTC

Se vuoi trasferire stable coin su Fantom, puoi utilizzare il seguente elenco di bridge:

* [AnySwap](https://anyswap.exchange/#/bridge): Questo è il bridge ufficialmente supportato per il trasferimento dei $MAI coniati su Polygon a Fantom(guarda la guida [MAI metaverse](../Universita-di-MAI/mai-metaverse.md) per maggiori dettagli). Questa soluzione supporta numerosi assets e diverse chain in modo da facilitare il più possibile il trasferimento di crypto valute a Fantom. Vi invitiamo a controllare **sempre** le note nella parte inferiore dell'interfaccia utente di bridging per conoscere le commissioni di transazione e il tempo di esecuzione previsto aggiornati.

![Trasferimento di MAI da Polygon a Fantom](<../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): offre servizi di bridging per molte chain e per la maggior parte delle stable coins, con commissioni che vanno dallo 0.04% allo 0.19% per il trasferimento verso Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): propone commissioni basse e garantisce che ci sia abbastanza liquidità sulla chain di destinazione per il token che trasferire. Minore è la liquidità (o maggiore è l'importo da coprire), più si allunga il tempo necessario al trasferimento.

### Trasferire altri assets

* Binance CEX: potrai acquistare il token $FTM su Binance e trasferirlo direttamente al tuo portafoglio ma è l'unico token che potrai trasferire attraverso la rete Fantom.
* [SpookySwap](https://spookyswap.finance/bridge): supporta molte reti e molti token che potrai inviare a Fantom.
* AnySwap: vedi descrizione sopra nella sezione stable coins.

## DeFi su Fantom

Fantom ha visto un'espansione piuttosto impressionante alla fine dell'estate 2021, in particolare con programmi di ricompensa che hanno contribuito ad attrarre investitori e sviluppatori sulla chain. La crescita è stata supportata anche da progetti "blue chip" che hanno portato le loro DApp su Fantom a settembre 2021, tra queste Curve e SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Questa applicazione è molto simile a Balancer. Sarai in grado di scambiare alcuni token per altri e anche depositare in pool di farming bilanciati composti da più token. Balancer è il primo partner ufficiale di Mai Finance su Fantom nonchè l'unico posto (ad Ottobre 2021) dove potrai scambiare i tuoi $MAI o depositarli in un pool MAI-USDC.

![Scambiare MAI per FTM](<../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): Questo è il DEX più grande (**D**ecentralized **Ex**change) su Fantom in cui sarai in grado di scambiare i tuoi token con altri, depositare liquidità e farmare più o meno nello stesso modo in cui lo faresti su QuickSwap su Polygon. SpookySwap ti ricompenserà con il token $BOO, il token nativo della piattaforma. Come nota a margine, quando metti in stake i tuoi token $BOO, otterrai in cambio $xBOO, un token di rendimento, e potrai usarli per guadagnare ricompense extra (stesso principio del Dragon's Syrup su QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): Automatic Marker Maker tradizionale e piattaforma di farming in cui sarai in grado di scambiare token, creare token LP e farmare in pool di liquidità. SpiritSwap ti pagherà con i token $SPIRIT che puoi mettere in stake sulla piattaforma ottenendo in cambio i token $inSPIRIT ($SPIRIT sarà bloccato per un certo periodo di tempo), ispirandosi al modello di veCRV. Puoi anche usare SpiritSwap per prestare e prendere in prestito, in attesa che  Mai Finance approdi su Fantom.
* [Tarot](https://www.tarot.to): Tarot è la versione Fantom di Impermax, dove potrai utilizzare i tuoi token LP da SpookySwap (o altri DEX/AMM) e usarli per farmare sulla piattaforma. Puoi anche depositare singoli token e prestarli su pool specifici in cui le persone potranno prenderli in prestito per generare nuovi token LP e sfruttare il loro rendimento. Fai molta attenzione al rischio liquidazione se usi i tuoi LP in un pool in cui la percentuale di utilizzo è elevata.
* [Scream](https://scream.sh): Scream è un clone di Compound in cui potrai prestare i tuoi token e prenderli in prestito usandoli come collaterale. Prestare i tuoi token ti farà guadagnare ricompense nel token prestato oltre ai token $SCREAM che potrai utilizzare come meglio ritieni opportuno.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve è il progetto blue chip che tutti ben conosciamo dove potrai depositare i tuoi token in pool specifici (non è necessario depositare un importo bilanciato) e sarai ricompensato nei token prestati oltre ai token $CRV e $wFTM.

![Pool DAI+USDC di Curve su Fantom](../.gitbook/assets/ftm-crv.png)

Ci sono molte altre opportunità su Fantom che non mancheremo di descrivere in altre guide.

## Altri link utili

* [Fantom explorer](https://explorer.fantom.network)
* [Fantom gas checker](https://ftmscan.com/gastracker)
* [Fantom Discord](how-to-get-started-on-fantom.md#ftm-faucet) 
* [DeBank](https://debank.com), gestione portafoglio multi-chain

## Disclaimer

Questa guida NON è un consiglio finanziario e va considerata a pure scopo educativo. Fai sempre le tue ricerche. La discussione di un progetto in questa guida non deve essere considerata come un'approvazione del progetto stesso.

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
