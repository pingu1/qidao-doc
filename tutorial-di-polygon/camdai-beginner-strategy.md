---
description: >-
  La DeFi non deve essere complicata. Questo articolo presenta come accedere
  alla DeFi utilizzando Mai Finance con una strategia a basso rischio e ottenere
  comunque interessi ragionevoli.
---

# Strategia camDAI per principianti

## Introduzione

La maggior parte delle persone ha paura quando pensa alla DeFi. C'è sempre un fattore di rischio da tenere in considerazione quando si utilizzano le crypto valute, la volatilità di questo mercato può far perdere molti soldi e ci sono così tante opportunità che trovare la strategia giusta può essere piuttosto complesso. Tuttavia, quando si utilizzano gli strumenti corretti, alcune strategie facili e a basso rischio possono ottenere buoni risultati e possono probabilmente competere con opzioni più complesse e rischiose.

In questo articolo cercheremo di presentare una strategia di investimento basata su stable coin con leva, con un pizzico di rischio in più per ottenere interessi superiori.

## Capire il concetto di leva

![Storia di un cercatore d'oro sfortunato](../.gitbook/assets/canDAI-farwest.png)

Siamo nel Far West, durante la grande corsa all'oro. Le banche vogliono comprare oro per poter prestare denaro alle persone e ottenere interessi su questi prestiti e i minatori vogliono arricchirsi vendendo il loro oro alle banche.

Sei un minatore ma non molto fortunato. Hai trovato solo una pepita. Tuttavia, sei super intelligente e invece di continuare a spaccarti la schiena minando e sperando, hai un altro piano!

Vai in una banca e gli comunichi che hai dell'oro. Puoi depositare l'oro in banca come garanzia, il che significa che lasci che la banca usi quell'oro per le persone che vogliono usarlo e la banca ti darà alcuni interessi sul tuo deposito.

In più, dato che hai prestato dell'oro, la banca accetta di farti prendere in prestito denaro da loro e nel caso in cui tu non sia in grado di rimborsare il prestito la banca tratterrà l'oro che hai depositato. Bene, ora stai guadagnando interessi sull'oro che hai in banca e in più ti hanno dato dei soldi.

Quindi decidi di andare a trovare un collega minatore e comprare il suo oro con i soldi che ti hanno prestato. Questo gli permette di concentrarsi sull'estrazione mineraria e ottenere denaro per l'oro che ha trovato. Sono tutti felici.

Torni in banca e depositi l'oro che hai comprato. Questo genera maggiore interesse e ora la banca ti consente di prendere in prestito altro denaro coperto dall'oro in più che hai depositato. Hai più oro che matura interessi dalla banca e qualche soldo in più. È ora di tornare indietro per vedere se il tuo amico ha trovato più oro e ripetere ancora e ancora.

Ciò che abbiamo visto in questo esempio viene definito in gergo leva. Ora immagina di poter trovare una banca che ti permetta di prendere in prestito contanti a un interesse dello 0% e ti renderai conto di avere tra le mani una macchina che genera denaro grazie agli interessi che stai ricevendo.

## Presentazione degli strumenti

### AAVE

[AAVE](https://app.aave.com) è una piattaforma di deposito e prestito in cui è possibile depositare i propri assets. Depositando su AAVE, i tuoi token depositati guadagneranno rendimento. Per la nostra strategia, depositeremo $DAI, una stable coin (ancorata al dollaro USA). Su AAVE, $100 di $DAI genereranno potenzialmente tra il 4% e il 10% di rendimento nell'arco di 1 anno.

![Mercati AAVE disponibili su Polygon ad Ottobre 2021](../.gitbook/assets/canDAI-aave.png)

Quando depositi i tuoi assets su AAVE, riceverai un "certificato" di deposito sotto forma di token. Nel nostro esempio, dato che stiamo depositando $DAI, otterremo il token amDAI nel nostro portafoglio (**a**ave **m**arket DAI). Devi assolutamente conservare questo token perché ti servirà per ritirare i tuoi $DAI da AAVE. Questa è la banca che accetterà il tuo oro nel nostro esempio del Far West.

### Mai Finance

[Mai Finance](https://app.mai.finance) è una piattaforma di prestito che ti permetterà di depositare alcuni assets in un Vault e prendere in prestito a fronte del valore di questo deposito. Se torniamo all'analogia con la banca, sarebbe una banca che ti permette di prendere un prestito ma il prestito non deriva da ciò che altri stanno prestando. La banca invece, stampa denaro corrispondente al tuo deposito personale, di conseguenza prendi in prestito solo contro te stesso.

Mai finance accetta la tua ricevuta di deposito amDAI (AAVE) all'interno del suo [strumento di rendimento](https://app.mai.finance/yield) (sezione Yield). Lo strumento di rendimento è uno strumento intermedio tra AAVE e il Vault su Mai Finance. Come puoi vedere nello screenshot AAVE, il deposito $DAI ti farà guadagnare l'8,75% in $DAI (auto reinvestito), ma anche il 2,01% di ricompensa in $MATIC. Lo strumento di rendimento su Mai Finance raccoglierà questa ricompensa $MATIC e la scambierà con altri $DAI che verranno aggiunti al tuo deposito $DAI. L'APY (Annual Percentage Yield) sul sito Mai Finance mostra quindi gli interessi aggregati di AAVE.

![Strumenti di rendimento su Mai Finance](../.gitbook/assets/camDAI-yield.png)

Una volta depositato il tuo amDAI nello strumento di rendimento, otterrai il token camDAI nel tuo portafoglio (amDAI reinvestito automaticamente). Questa è una ricevuta che indica la tua quota del pool amDAI nello strumento di rendimento. Come nota a margine, dato che camDAI è una rappresentazione della tua quota del pool amDAI, il rapporto tra amDAI e camDAI non è 1:1. Leggi [questo articolo](leverage-aave-tokens.md#amtokens-vs-camtoken) per ulteriori dettagli.

Ora puoi [depositare i tuoi tokens camDAI](https://app.mai.finance/vaults)  in un Vault su Mai Finance e sarai quindi in grado di prendere in prestito alcuni $MAI (una stable coin ancorata a $ 1) a fronte della tua garanzia (collaterale). Nel nostro esempio sul Far West, questa sarebbe una seconda banca che ti consente di prendere un prestito in contanti in base alla quantità di oro che hai depositato nella prima banca. Questa seconda banca accetta la ricevuta della prima banca come garanzia nel caso in cui non sia possibile rimborsare il prestito.

### Zapper

[Zapper](https://zapper.fi/dashboard) è un coltellino svizzero della DeFi su Polygon. Questa piattaforma ti consentirà di farmare in pool di liquidità, depositare i tuoi assets su AAVE direttamente dalla loro piattaforma, controllare i tuoi investimenti attraverso una dashboard e inoltre di scambiare alcune coin con altre coin. Questa è l'ultima funzionalità che utilizzeremo per scambiare la stable coin $MAI che abbiamo appena preso in prestito per ulteriori $DAI.

![Swap di MAI per DAI](../.gitbook/assets/camDAI-zapper.png)

Nel nostro esempio del Far West, Zapper è il minatore d'oro che accetta il tuo denaro in cambio dell'oro.

### Balancer

Come puoi vedere nello screenshot qui sopra, Zapper usa Balancer come protocollo per fare lo swap. [Balancer](https://polygon.balancer.fi/#/) è un gestore di portafoglio automatizzato, fornitore di liquidità e tracker di prezzi in cui sarai in grado di fornire liquidità (e ottenere commissioni da questo) o scambiare valute utilizzando i pool di liquidità.

Per la nostra strategia, utilizzeremo Balancer per esporre i nostri investimenti a un po' più di volatilità e ottenere interessi migliori. Questo è facoltativo al 100%.

## Descrizione della strategia

### Strategia principale

Anche se abbiamo spiegato cos'è AAVE, la nostra strategia utilizzerà una funzionalità di Mai Finance per automatizzare il deposito di $DAI su AAVE, il deposito amDAI nello strumento di rendimento e il deposito camDAI nel Vault camDAI.

![](../.gitbook/assets/camDAI-zapDAI.png) ![](../.gitbook/assets/camDAI-zapdeposit.png)

Il pulsante `Zap in using DAI` aprirà un popup che ti consentirà di depositare i $DAI nel Vault e contemporaneamente gestirà il tuo deposito su AAVE. Questo fa risparmiare un sacco di tempo e un po' di commissioni di transazione.

Questo sarà il nostro primo passo. Supponendo di avere $100 di $DAI, li depositeremo su Mai Finance in un Vault camDAI. Questo ci consentirà di prendere in prestito $MAI a fronte di questo deposito iniziale.

Il CDR minimo (**R**apporto tra **D**ebito e **C**ollaterale) per camDAI è del 110%. Questo significa che il rapporto tra la tua garanzia (il valore di $100 di $DAI) e il prestito che stai per ottenere deve rimanere al di sopra del 110%.

{% hint style="danger" %}
Se questo rapporto CDR raggiunge il valore minimo del 110%, significa che la tua garanzia sta perdendo valore e il tuo debito potrebbe quindi superare il valore della tua garanzia. A questo punto, il tuo Vault diventa "liquidabile": qualcuno può ripagare una parte del tuo debito e ottenere una parte del tuo collaterale a garanzia come ricompensa. Tuttavia, poiché sia ​​$DAI che $MAI sono stable coin ancorate al dollaro USA, il rischio di trovarsi in una situazione in cui ci sia una grossa differenza di valore tra i 2 asset è molto basso, il che rende questa strategia abbastanza sicura.
{% endhint %}

Per mantenere basso il rischio di liquidazione, cercheremo di mantenere un CDR del 115%. Per sapere quanto $MAI possiamo prendere in prestito per rimanere a un CDR del 115%, utilizzeremo questa formula:

$$
MAI_{disponibile} = \frac{Collaterale_{valore} - Debito_{valore} * Obbiettivo_{CDR}}{Obbiettivo_{CDR}}
$$

Con un valore collaterale di $100, nessun debito e un CDR target del 115%, ecco quanto possiamo prendere in prestito:

$$
MAI_{disponibile}=\frac{100 - 0*1.15}{1.15}=86.95
$$

​Potrai quindi scambiare il $MAI che hai preso in prestito con $DAI e ripetere il ciclo più volte. Ecco come dovrebbero evolvere la tua garanzia e il tuo debito, ad ogni ciclo aggiuntivo:

| Ciclo # | Collaterale totale | Debito totale | Prestito disponibile | APY Equivalente | Prezzo di liquidazione DAI |
| ------- | ------------------ | ------------- | -------------------- | --------------- | -------------------------- |
| 1       | 100.000            | 0.000         | 86.956               | 10.42%          | 0                          |
| 2       | 189.956            | 86.956        | 75.614               | 19.48%          | 0.512                      |
| 3       | 262.571            | 162.571       | 62.751               | 27.36%          | 0.681                      |
| 4       | 328.323            | 228.323       | 57.175               | 34.21%          | 0.765                      |
| 5       | 385.498            | 285.498       | 49.718               | 40.17%          | 0.815                      |
| 6       | 435.216            | 335.216       | 43.233               | 45.35%          | 0.847                      |
| 7       | 478.449            | 278.448       | 37.593               | 49.85%          | 0.870                      |
| 8       | 516.042            | 416.042       | 32.690               | 53.77%          | 0.887                      |
| 9       | 548.732            | 448.732       | 28.426               | 57.18%          | 0.899                      |
| 10      | 577.158            | 477.158       | 24.718               | 60.14%          | 0.909                      |
| 11      | 601.877            | 501.877       | 21.494               | 62.72%          | 0.917                      |
| 12      | 623.371            | 523.371       | 18.691               | 64.96%          | 0.924                      |
| 13      | 642.062            | 542.062       | 16.253               | 66.90%          | 0.929                      |
| 14      | 658.315            | 558.315       | 14.133               | 68.60%          | 0.933                      |
| 15      | 672.448            | 572.448       | 12.289               | 70.07%          | 0.936                      |
| 16      | 684.737            | 584.737       | 10.686               | 71.35%          | 0.939                      |
| 17      | 695.423            | 595.423       | 9.293                | 72.46%          | 0.942                      |

Ci fermeremo a 17 cicli ma puoi farne anche di più se vuoi.

Alla fine dei 17 cicli, otterresti $695.423 di garanzia e $595.423 di debito. Corrispondente a un CDR del 116,79% che dovrebbe essere abbastanza sicuro da prevenire la liquidazione.

Se consideriamo l'APY del 10,42% ottenuto dallo strumento di rendimento, questo genererebbe

$$
Interessi = Collateral_{valore}*APY=695.423*10.42\%= \$72.463
$$

Se consideriamo che l'investimento iniziale era di soli $100, questo è un APY equivalente del 72,463% sul singolo staking di una stable coin!

### Strategia alternativa

Per ottenere una piccola esposizione ad assets ad alta volatilità, puoi utilizzare lo stesso ciclo di cui sopra ma sfruttare solo il 90% dei $MAI presi in prestito e utilizzare il 10% per acquistare qualcos'altro. In questo esempio utilizzeremo il 10% per acquistare $Qi (il token nativo di Mai Finance) e utilizzeremo il pool Qi-BAL su Balancer che al momento offre un APR (**A**nnual **P**ercentage **R**evenue) del 107.12%.

![Pool Qi-BAL ad Ottobre 2021](../.gitbook/assets/camDAI-balancer.png)

Dato che stiamo reinvestendo meno $DAI nel Vault camDAI, faremo anche meno cicli. L'evoluzione sarà simile a questa:

| Ciclo # | Collaterale totale | Debito totale | Qi     | Prestito disponibile | APY Equivalente | Prezzo di liquidazione DAI |
| ------- | ------------------ | ------------- | ------ | -------------------- | --------------- | -------------------------- |
| 1       | 100.000            | 0.000         | 0.000  | 86.957               | 10.42%          | 0                          |
| 2       | 178.261            | 86.957        | 8.696  | 68.053               | 35.22%          | 0.537                      |
| 3       | 239.509            | 155.009       | 15.501 | 53.259               | 54.63%          | 0.712                      |
| 4       | 287.441            | 208.268       | 20.827 | 41.681               | 69.82%          | 0.797                      |
| 5       | 324.954            | 249.949       | 24.995 | 32.620               | 81.71%          | 0.846                      |
| 6       | 354.312            | 282.569       | 28.257 | 25.529               | 91.01%          | 0.877                      |
| 7       | 377.288            | 308.097       | 30.810 | 19.979               | 98.29%          | 0.898                      |
| 8       | 395.269            | 328.076       | 32.808 | 15.636               | 103.99%         | 0.913                      |
| 9       | 409.341            | 343.712       | 34.371 | 12.237               | 108.45%         | 0.924                      |
| 10      | 420.354            | 355.948       | 35.595 | 9.576                | 111.94%         | 0.931                      |

Alla fine dei 10 cicli, otterresti:

* $420.354 di $DAI come collaterale
* $355.948 di debito
* $35.595 di Qi

La stessa formula matematica dell'esempio precedente fornisce i seguenti risultati:

* Un CDR finale del 118.09%, che dovrebbe essere considerato sufficientemente sicuro da prevenire la liquidazione
* $43.800 di interessi su DAI grazie all' APY del 10.42% ottenuto dallo strumento di rendimento
* $68.139 di interessi sui tuoi Qi grazie al pool di Balancer, dato per assunto che andrai a reinvestire le ricompense Qi e BAL nel pool Qi-BAL
* Un APY totale del 111.94%

Questa strategia presenta maggiori rischi visto che l'investimento nel pool Qi-BAL non è garantito. Tuttavia, otterrai un po' di esposizione al Qi, che ti consentirà di partecipare al protocollo QiDAO. Se utilizzi le ricompense BAL su Mai Finance come collaterale e prendi in prestito, sarai anche in grado di reinvestire nel Vault camDAI o nel pool Qi-BAL. Se lo fai, avrai anche diritto ad ulteriori ricompense per il prestito, pagate in Qi ogni settimana.

## Conclusione

Con un investimento minimo e poca necessità di starci dietro con tante transazioni è possibile ottenere risultati piuttosto buoni semplicemente sfruttando i tuoi $DAI. Dato che $DAI è una stable coin con molta liquidità su più chain, il rischio che $DAI abbia grosse fluttuazioni e che di conseguenza il tuo Vault venga liquidato è relativamente basso. È il tipo di configurazione "imposta e dimentica" che può facilmente essere un ottimo punto di partenza per qualsiasi principiante della DeFi ed è probabile che questa strategia si comporti allo stesso modo indipendentemente dal fatto che ci si trovi in un mercato rialzista o in un mercato ribassista. Infine, abbiamo anche spiegato come puoi utilizzare la stessa strategia testando un'altra delle tante opportunità offerte da Polygon sulla DeFi.

## Disclaimer

Tutto ciò che è stato presentato in questo articolo è da ritenersi a puro scopo educativo ed è stato realizzato per illustrare le opzioni di leva proposte da Mai Finance. Non abbiamo parlato di rimborso del debito perché ci sono altri articoli dedicati su questo sito ma è importante tenere presente che Mai Finance addebita una commissione di rimborso dello 0,5% sull'importo preso in prestito. Come sempre, fai le tue ricerche e non esitare a fare domande alla community del [server Discord di Mai Finance](https://discord.com/invite/qidaoprotocol).

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
