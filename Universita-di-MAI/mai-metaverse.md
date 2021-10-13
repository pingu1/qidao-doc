---
description: >-
  Questa guida offre una panoramica delle blockchain in cui può essere usata la
  stable coin MAI e come trasferire il token tra una blockchain e l'altra.
---

# MAI Metaverse

![MAI Everywhere!](<../.gitbook/assets/Screen Shot 2021-09-13 at 1.06.42 PM.png>)

## Introduzione

MAI, a volte indicato come miMATIC, è la prima stable coin nativa della rete Polygon. È ancorata a $1,00 e il suo valore può oscillare tra $ 0,99 e $ 1,01. Puoi ottenere maggiori dettagli come viene mantenuto l'ancoraggio nella [documentazione ufficiale](https://docs.mai.finance/stablecoin-economics). Ma il fatto che MAI sia nativo su Polygon non significa che si trovi solo su quella rete. Infatti, allo stesso modo in cui puoi trovare DAI su reti diverse (DAI è in realtà un'altra stable coin proveniente dalla Mainnet di Ethereum), MAI si sta lentamente ma costantemente diffondendo anche ad altre reti. Questo articolo evidenzierà le diverse reti in cui puoi trovarlo e come trasferire i tuoi MAI da una rete all'altra.

## Polygon

### Ottenere MAI su Polygon

Come spiegato, MAI è nativa di Polygon e questo è l'unico posto (come per settembre 2021) in cui potrai generare MAI. Si può fare in questi modi:

* prendendo in prestito MAI a fronte di un collaterale che hai precedentemente depositato in un vault su Mai Finance
* scambiando USDC per MAI su [Mai Finance](https://app.mai.finance/anchor)
* vendendo un altro asset e acquistando MAI su un DEX (**D**ecentralized **EX**change) su Polygon, i più efficienti sono [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) e [1Inch](https://app.1inch.io/#/137/classic/swap).

### Usare MAI su Polygon

La stable coin MAI viene utilizzata in sempre più progetti su Polygon soprattutto ora che viene utilizzata come altre stable coin all'interno di grandi progetti come QuickSwap. A Settembre 2021, ci sono 3 farm stable su QuickSwap con un totale complessivo di $18.327.604:

* MAI-DAI con $6,553,255
* MAI-USDT con $6,316,026
* MAI-USDC con $5,458,323

Ulteriori pool possono essere trovati in altri progetti / farm / ottimizzatori di rendimento. Puoi leggere di più su cosa fare con MAI in [questo articolo dedicato](../tutorial-di-polygon/what-to-do-with-mai-on-polygon.md).

## Solana

### Ottenere MAI su Solana

Solana è una blockchain per app decentralizzate. L'obiettivo della rete è proporre commissioni basse (meno di $ 0,01) e transazioni veloci (meno di 400 ms). L'idea alla base è creare un'alternativa ad Ethereum e alle sue side chains. Tuttavia, nonostante Solana sia un concorrente diretto della rete Ethereum non vuol dire che non possa supportare gli stessi assets. In effetti, Solana ora supporta la stable coin MAI che può essere trasferita da Polygon (dove può essere generata).

Per inviare i tuoi token MAI a Solana, puoi utilizzare [AllBridge](https://allbridge.io), una piattaforma di bridge che consente di trasferire token da una blockchain all'altra. AllBridge supporta le seguenti reti:

* Ethereum Mainnet
* Polygon
* Solana
* Huobi
* Binance Smart Chain

L'interfaccia è davvero intuitiva, devi semplicemente selezionare le due reti e l'asset che vuoi trasferire tra le stesse.

![Trasferire MAI da Polygon a Solana](<../.gitbook/assets/Screen Shot 2021-09-13 at 1.52.23 PM.png>)

Il prossimo passo è indicare l'indirizzo del tuo portafoglio Solana e l'importo che vuoi trasferire. Tieni presente che MetaMask non supporta i portafogli Solana (per ora?) quindi dovrai creare un portafoglio separato su quella rete. Può essere un portafoglio web simile a MetaMask o un portafoglio app. Si prega di leggere le [raccomandazioni ufficiali del team Solana](https://docs.solana.com/wallet-guide) prima di sceglierne uno.

{% hint style="info" %}
Tieni presente che Solana non offre alcun faucet da cui ottenere i tuoi primi SOL (token nativo utilizzato per pagare le transazioni). Dovrai prima acquistare dei SOL e averli nel tuo portafoglio per poter trasferire MAI o per fare qualsiasi altra transazione.
{% endhint %}

### Usare MAI su Solana

Allo stesso modo in cui puoi utilizzare MAI su Polygon per fornire liquidità e farmare, puoi fare lo stesso su Solana. Il luogo principale in cui è possibile utilizzare MAI è [Saber](https://app.saber.so), nel pool MAI/USDC.

![Stato del pool MAI/USDC su Saber al Settembre 2021](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.11.10 PM.png>)

Una delle cose positive del pool MAI/USDC su Saber è che a differenza dei pool LP (Liquidity Providing) su QuickSwap, non è necessario fornire coppie LP con un rapporto 1:1. Puoi semplicemente depositare un singolo asset (MAI o USDC) o un rapporto sbilanciato di entrambe le stable coin. Come su Balancer.

![MAI e USDC non sono bilanciati nel pool Saber](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.13.51 PM.png>)

Ciò significa che puoi effettivamente depositare MAI al 100% senza doverne scambiare con USDC. È particolarmente conveniente ed evita l'influenza dovuta alle differenze di prezzo tra le 2 stable coin. Nota che riceverai ricompense pagate nel token nativo della farm, allo stesso modo in cui verresti ricompensato in QUICK per il farming su QuickSwap su Polygon. Puoi quindi vendere i tuoi token Saber per aumentare la tua posizione MAI/USDC.

{% hint style="info" %}
Su Solana puoi anche usare [Sunny](https://app.sunny.ag), un aggregatore che reinvestirà automaticamente le ricompense di Saber. Da notare che l'aggregatore Sunny non è convalidato dal team di Mai Finance. AllBridge e Saber sono stati partner ufficiali di Mai Finance ma i risultati non sono in alcun modo garantiti. Per favore, come al solito, fai le tue ricerche.
{% endhint %}

## Avalanche

### Ottenere MAI su Avax

Avalanche è una blockchain, progettata per fornire una piattaforma open source e un protocollo per il lancio di applicazioni DeFi e soluzioni blockchain aziendali. È un' altra soluzione alternativa a Ethereum  che supporta le stesse risorse di Ethereum, Polygon e Solana. Pertanto, ora puoi inviare i tuoi MAI da Polygon (l'unico posto, a Settembre 2021, dove puoi generare MAI) ad Avax utilizzando [Relay Chain](https://app.relaychain.com/#/transfer).

Come per AllBridge, l'interfaccia utente è abbastanza semplice. È sufficiente selezionare la rete da cui trasferire l'asset, la sua destinazione e l'asset da trasferire.

![Trasferire MAI da Polygon ad Avalanche](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.52.31 PM.png>)

Metamask supporta i [portafogli Avax](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche), quindi non avrai bisogno di alcun portafoglio aggiuntivo rispetto all'esempio precedente di Solana.

### Usare MAI su Avax

Allo stesso modo in cui puoi usare MAI per farmare su Polygon, puoi usare MAI anche su Avalanche. La piattaforma principare è [Trader Joe's](https://www.traderjoexyz.com/#/farm), al cui interno troverai un pool MAI/USDC.

![Stato del pool MAI/USDC su Trader Joe al Settembre 2021](<../.gitbook/assets/Screen Shot 2021-09-13 at 3.07.19 PM.png>)

Le farm su Avalanche funzionano in maniera molto simile a quelle su Polygon. Puoi utilizzare l'app di Trader Joe nello stesso modo in cui utilizzeresti QuickSwap. Dovrai prima creare una coppia LP utilizzando lo stesso rapporto tra MAI e USDC ed in seguito potrai depositare la coppia LP nella farm. Allo stesso modo in cui verresti pagato in QUICK quando farmi su QuickSwap, verrai ricompensato in token JOE quando farmi su Trader Joe. Puoi quindi utilizzare questi token in altri pool o venderli per reinvestire sulla coppia LP MAI/USDC.

## Fantom

### Ottenere MAI su Fantom

Fantom è una piattaforma blockchain / smart contract il cui scopo è risolvere i problemi di scalabilità di altre reti, in particolare la blockchain di Ethereum. Gli sviluppatori possono creare le proprie DApp (applicazioni decentralizzate) su quella rete e utilizzare le stesse risorse di un'altra rete. Di conseguenza puoi già trasferire MAI da Polygon a Fantom usando il bridge [AnySwap](https://anyswap.exchange/#/bridge).

Nonostante AnySwap sia una differente soluzione di trasferimento, la sua interfaccia utente è molto simile a quella di AllBridge e Relay Chain. Quando sei su Polygon, dovrai prima connettere il tuo portafoglio MetaMask, quindi selezionare l'asset che vuoi collegare (MAI) e la rete di destinazione (Fantom).

![Trasferire MAI da Polygon a Fantom attraverso AnySwap](../.gitbook/assets/image.png)

Metamask supporta i [wallets Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask), di conseguenza in pochi secondi potrai configurarlo per ottenere i tuoi MAI su Fantom e iniziare a usarli subito.

### Usare MAI su Fantom

Attualmente, il team di Mai Finance non ha partnership attive con nessuna farm su Fantom. Una volta che il team verrà a conoscenza di progetti interessati all'utilizzo di MAI, questa documentazione verrà aggiornata. Rimani sintonizzato.

## Disclaimer

I dettagli presentati in questa guida sono a scopo puramente educativo e non sono stati testati direttamente dal team che gestisce questa guida. Alcuni utenti sul server [Discord](https://discord.gg/aRghpvhV) hanno già provato a trasferire le loro risorse a Solana e/o Avalanche quindi puoi unirti alla community per porre le tue domande. Per favore, non dimenticare di fare le tue ricerche, reti diverse avranno commissioni di transazione e tempi di esecuzione diversi, programmi di ricompensa diversi, commissioni di trasferimento ecc ... Se invii i tuoi MAI ad altre reti, assicurati di poterli ritrasferire nel caso ne avessi bisogno su Polygon.

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
