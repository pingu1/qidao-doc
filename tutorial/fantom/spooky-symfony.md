---
description: >-
  Prendere un prestito non è esattamente un debito quando si utilizza questo
  prestito come punto di partenza per una strategia di investimento. È un vero
  investimento.
---

# A Spooky Symfony

## Introduzione

Prendere un prestito garantito dai vostri assets è sempre un'arma a doppio taglio: può aiutarvi a dare il via a una strategia di investimento o a sfruttare i vostri assets, ma a un certo punto avrete un debito che dovrete ripagare. In questa guida utilizzeremo un prestito preso su Market.XYZ, un protocollo di prestito su cui potrete prendere in prestito $MAI con un basso tasso di interesse e utilizzare questo prestito per farmare la maggior parte dei protocolli più importanti su Fantom. Useremo la strategia per rimborsare il prestito e vedere quanto velocemente questo può essere fatto per sbloccare gli assets depositati come garanzia.

{% hint style="info" %}
Questa guida non è un consiglio finanziario, è stata realizzata con uno scopo educativo in mente. Dovete prestare attenzione alle variazioni di prezzo, domanda e offerta, programmi di ricompensa, date di conclusione, impermanent loss ecc... L'obiettivo non è proporre ricette che possano essere seguite alla cieca, quindi per favore fate i compiti e le vostre simulazioni e investite solo ciò che siete disposti a perdere.
{% endhint %}

![](../../.gitbook/assets/spooky-symfony-1.png)

## Protocolli su Fantom : Dobbiamo usarli tutti

In questa strategia, utilizzeremo molte coppie di LP (**L**iquidity **P**rovider) su molti protocolli diversi, quindi abbiamo pensato che sarebbe stata una buona idea darvi un breve riepilogo di ciò che ogni protocollo sta facendo.

### Market.XYZ

[Market.XYZ](https://fantom.market.xyz) è un protocollo di prestito che crea diversi locker per i suoi partner. Sarete in grado di depositare singoli asset o token LP come garanzia e prendere in prestito altri asset a fronte dei vostri depositi. Poiché state prendendo in prestito a fronte di una garanzia, è importante assicurarsi di non essere liquidati. Una liquidazione si verifica quando il valore degli assets che avete depositato come garanzia scende al di sotto del valore del prestito che avete contratto. Questo è il motivo per cui è importante assicurarsi che il rapporto tra i 2 valori rimanga relativamente alto e che il vostro collaterale non perda troppo valore quando il mercato scende.

Al fine di mitigare il rischio di liquidazione, utilizzeremo il token LP $FTM-$USDC come garanzia

* L' impermanent loss su questa coppia è relativamente basso
* $USDC è una stablecoin ancora al dollaro US
* $FTM è il token gas nativo di Fantom, ha una grande liquidità ed è usato ovunque
* Le percentuali di ricompensa sulla coppia $FTM-$USDC sono alte, il che significa che anche se il prezzo di $FTM rimane lo stesso, il valore del tuo collaterale aumenterà

Potrete prendere in prestito a fronte della coppia $FTM-$USDC dal [pool LP Spooky](https://fantom.market.xyz/pool/10) su market.xyz. I passaggi per depositare i vostri assets sono i seguenti:

* Creare [l'LP token $FTM-$USDCLP su SpookySwap](https://spookyswap.finance/add/FTM/0x04068DA6C83AFCFA0e13ba15A6696662335D5B75) fornendo liquidità in un rapporto 1:1 per entrambi gli asset
* Depositare l'LP token $FTM-$USDC su Beefy finance per ottenere una ricevuta $mooBooFTM-$USDC (cercate la piattaforma SpookySwap e l'asset $USDC nei filtri di ricerca)
* Depositare il token di ricevuta $mooBooFTM-$USDC su Market.xyz

![Mercato di lending/borrow su MarketXYZ a Febbraio 2022](../../.gitbook/assets/spooky-symfony-2.png)

Quando i vostri token di ricevuta sono su Market.XYZ, ricevete comunque la ricompensa APY fornita da Beefy. Ciò significa che i vostri assets stanno ancora generando rendimenti per voi mentre prendete in prestito a fronte degli stessi. Questo è uno strumento molto potente, soprattutto quando vedete che $mSPLP-$FTM-$USDC (moo Spookyswap FTM-USDC = mooBooFTM-USDC) sta guadagnando il 51,4% di APY e potete prendere in prestito $MAI al 2,56% di Aprile. In altre parole, la vostra garanzia cresce più velocemente del vostro debito, quindi in teoria potete benissimo rimborsare il vostro prestito con gli interessi della vostra garanzia.

{% hint style="info" %}
Come nota a margine, potete vedere che il locker LP Spooky offre anche la possibilità di prendere in prestito a fronte di altri token LP: $ETH-$FTM, $DAI-$FTM, $BTC-$FTM e $fUSDT-$FTM. A seconda degli assets che avete nel vostro portafoglio, delle vostre convinzioni e della vostra tolleranza al rischio, potete utilizzare qualsiasi LP Spookyswap come garanzia.
{% endhint %}

Per questo tutorial, limiteremo anche il rischio prendendo in prestito con un CDR (**C**ollateral to **D**ebt **R**atio) del 200%. Ciò significa che prenderemo in prestito il 50% del valore della nostra garanzia. Maggiori informazioni nella sezione sulla strategia di farming. I rapporti di liquidazione sono espressi come LTV (**L**oan **t**o **V**alue) che è l'opposto del CDR. Potete vedere che l'LTV per il token $mooBooFTM-$USDC è del 60%, al di sopra del quale verrete liquidati. Ciò equivale a un CDR del 166,67%. Con un obiettivo del 200% di CDR, siamo il 33% al di sopra del rapporto di liquidazione, che può essere rischioso o meno, a seconda della vostra tolleranza al rischio.

{% hint style="danger" %}
Market.XYZ consente solo prestiti con un valore minimo di 0,05 $ETH (\~$170,00 al momento della scrittura). Assicuratevi di depositare abbastanza garanzie se volete prendere in prestito dai diversi locker.
{% endhint %}

### BeethovenX

[BeethovenX](https://beets.fi/#/) è un **E**xchange **D**ecentralizzato ed un **M**arket **M**aker **A**utomatizzato "forkato" da Balancer. Sarete in grado di depositare i vostri assets in pool di liquidità o completare semplici swap. Sono stati solidi partner del protocollo QiDAO, fornendo token LP per le farm che potete trovare su Mai Finance. Utilizzeremo due diversi pool su BeethovenX per questa strategia

* The Monolith: un pool incentivato che è stato aperto per Exodia, un fork di Ohm che [vi abbiamo presentato in questo tutorial](investing-in-discounted-assets-using-bonds.md). Potrete depositare i vostri token $MAI direttamente in questo pool e raccogliere i rendimenti
* Pirate Party: un pool incentivato dedicato ai token $LQDR, il token nativo di Liquid Driver, un altro grande protocollo che utilizzeremo in questa guida

![Pool The Monolith su BeethovenX con 20% di $MAI a Febbraio 2022](../../.gitbook/assets/spooky-symfony-3.png)

![Pool Pirate Party su BeethovenX con 80% di $LQDR a Febbraio 2022](../../.gitbook/assets/spooky-symfony-4.png)

Come sempre, il più grande vantaggio dell'utilizzare BeethovenX (o Balancer) è che potete depositare singoli asset nei pool invece di dover fornire token in un rapporto bilanciato.

### SpookySwap

[Spookyswap](https://spookyswap.finance) è il più grande fork di Uniswap V2 su Fantom, una piattaforma in cui potrete scambiare assets e fornire liquidità per molte coppie di trading. Spookyswap è anche un solido partner di Mai Finance e propone un pool $MAI-$USDC. La partnership si è estesa tramite Market.XYZ dove potrete prendere in prestito $MAI a fronte di alcune coppie LP specifiche (vedi la sezione su Market.xyz) così come i vostri token $BOO e $BOO in staking, il token nativo di Spookswap.

Per questa guida, utilizzeremo due diversi token LP di SpookySwap:

* $FTM-$USDC che sarà utilizzato come punto di partenza per la strategia. Questo token LP viene utilizzato come garanzia su market.xyz
* $FTM-$BOO dato che è uno dei pool di SpookySwap accettati su Liquid Driver con l'APR più alto. Scambieremo le ricompense $BEETS del Monolith con questa coppia (ulteriori informazioni nella sezione Strategia di Farming)

### Liquid Driver

[Liquid Driver](https://www.liquiddriver.finance) è un ottimizzatore di rendimenti su cui potrete depositare token LP da diverse farm e guadagnare rendimenti su di essi. Il modo in cui funziona l'ottimizzatore di rendimento consiste nel raccogliere i token di ricompensa della piattaforma di destinazione e combinarli per te. Questo è utile poiché il gas su Fantom può essere costoso. Viene prelevata una commissione di performance, ma una parte delle entrate del protocollo viene ridistribuita agli staker $LQDR. $LQDR è il token nativo di Liquid Driver.

Per questa strategia, utilizzeremo la coppia LP $FTM-$BOO perché è un pool con uno dei più alti APR in LQDR per Spookyswap.

![LP $FTM-$BOO e $FTM-$USD su LiquidDriver a Febbraio 2022](../../.gitbook/assets/spooky-symfony-5.png)

## Strategia di Farming

Per questa strategia, utilizzeremo Market.XYZ come punto di partenza per prendere in prestito $MAI a fronte dei token LP $mooBooFTM-$USDC. I $MAI presi in prestito saranno depositati su BeethovenX nel pool The Monolith. Dato che questo è il pool con il tasso di ricompensa più alto nella nostra strategia, lo utilizzeremo come motore per ripagare il nostro debito: il 50% dei $BEETS verrà venduto per ripagare il debito su Market.xyz e il 50% verrà convertito in Token LP $FTM-$BOO. I token $FTM-$BOO verranno depositati su LiquidDriver per raccogliere i token $LQDR che verranno poi messi in staking nel pool Pirate Party su BeethovenX. Una volta che il debito è stato completamente rimborsato, i premi $BEETS saranno completamente convertiti in token $FTM-$BOO. Le ricompense $BEETS fornite dal pool Pirate Party saranno anche combinate in più $FTM-$BOO.

Per questa simulazione utilizzeremo i seguenti numeri

* Iniziamo con un valore di $1.000 di token $mooBooFTM-$USDC
* L'APR per il token $mooBooFTM-$USDC fornito da SpookySwap tramite Beefy è 41.5%
* Il tasso di prestito per $MAI è 2.56%
* BeethovenX dà un APR del 304,17% per The Monolith e del 175,77% per Pirate Party
* LiquidDriver dà un APR del 82% per la coppia LP $FTM-$BOO

Come al solito per le nostre simulazioni, assumiamo che tutti i prezzi rimangano gli stessi per l'intero periodo di 1 anno, le tariffe rimangano le stesse e utilizziamo anche gli APR forniti così come sono. In realtà, i prezzi e le tariffe varieranno e gli APR sono composti da commissioni di trading e token di ricompensa, che possono influire sul risultato finale. È anche importante notare che per questa simulazione **non vengono prese in considerazione commissioni di transazione**. Infine, stiamo utilizzando molti protocolli e ogni protocollo può presentare rischi sugli smart contracts. Assicuratevi di fare le vostre ricerche prima di utilizzare una piattaforma e investite solo ciò che siete disposti a perdere.

Potete trovare la nostra simulazione Spooky Symfony [in questo SpreadSheet](https://docs.google.com/spreadsheets/d/19s6kBnT5w0b9GKuTkDiiD1u\_ZoeNUZtI9XYxEmk\_WM0/edit?usp=sharing). Sentitevi liberi di copiarlo e giocarci per vedere come funziona il loop e come le diverse tariffe possono influenzare il vostro APY finale.

![](../../.gitbook/assets/spooky-symfony-6.png)

### Giorno 1

Il giorno 1, dovete creare il vostro collaterale per Market.xyz. Ottenete una porzione uguale di $FTM e $USDC e fornite liquidità su SpookySwap per creare il token LP $FTM-$USDC. Questi token verranno depositati su Beefy, che vi darà il token di ricevuta $mooBooFTM-$USDC. Questo è il token che verrà utilizzato come garanzia su Market.xyz e a fronte del quale prenderete in prestito $MAI. Dal momento che vogliamo mantenere un CDR del 200%, prenderemo in prestito $500 di $MAI. Infine, i token $MAI verranno messi in stake su BeethovenX nel pool The Monolith.

Alla fine del primo giorno, avrete

| posizione      | valore ($) |
| -------------- | ---------- |
| mooBooFTM-USDC | 1,000.000  |
| the monolith   | 500.000    |
| pirate party   | 0.000      |
| BEETS rewards  | 4.167      |
| FTM-BOO        | 0.000      |
| LQDR rewards   | 0.000      |
| MAI debt       | 500.000    |

### Giorno 2

Il giorno 2, dovrete fare questo

* swappare il 50% dei vostri $BEETS per $MAI per rimborsare una piccola parte del vostro prestito
* swappare l'altro 50% di $BEETS da aggiungere alla coppia LP $FTM-$BOO. Potete scambiare su BeethovenX e creare la coppia LP su SpookySwap oppure fare tutto su SpookySwap.
* aggiungere la coppia LP $FTM-$BOO su Liquid Driver per iniziare a raccogliere i token $LQDR.

Alla fine del secondo giorno, avrete

| posizione      | valore ($) |
| -------------- | ---------- |
| mooBooFTM-USDC | 1,001.137  |
| the monolith   | 500.000    |
| pirate party   | 0.000      |
| BEETS rewards  | 4.167      |
| FTM-BOO        | 2.083      |
| LQDR rewards   | 0.005      |
| MAI debt       | 497.952    |

### Giorno 3

Ripetete le operazioni del Giorno 2, quindi raccogliete i vostri primi token $LQDR. Questi verranno depositati su BeethovenX nel pool Pirate Party per ottenere ricompense $BEETS extra e alla fine del Giorno 3 avrete

| posizione      | valore ($) |
| -------------- | ---------- |
| mooBooFTM-USDC | 1,002.275  |
| the monolith   | 500.000    |
| pirate party   | 0.005      |
| BEETS rewards  | 4.167      |
| FTM-BOO        | 4.167      |
| LQDR rewards   | 0.000      |
| MAI debt       | 495.903    |

{% hint style="info" %}
I guadagni del pool Pirate Party sono troppo piccoli per essere significativi a questo punto, ma ne otterrete di più nel tempo.
{% endhint %}

### Routine Giornaliera

A questo punto la strategia è completamente operativa. La vostra routine quotidiana sarà composta da

* raccogliere le ricompense $BEETS da The Monolith
* raccogliere le ricompense $BEETS da Pirate Party
* swappare 50% dei $BEETS per $MAI se avete ancora un debito in sospeso
* ripagare una parte del vostro debito se ne avete ancora
* swappare il resto dei $BEETS per la coppia LP $FTM-$BOO
* depositare la coppia LP $FTM-$BOO su LiquidDriver
* raccogliere i $LQDR
* depositarli nel Pirate Party

Questa strategia non è molto efficiente dal punto di vista del consumo di gasfee, quindi potreste considerare di completare la routing solo una volta alla settimana o anche meno frequentemente.

### Risultati grezzi mese per mese

Ecco i risultati "grezzi" mese dopo mese, come potete anche calcolarli grazie al foglio di calcolo di Google collegato sopra.

| giorno | FTM-USDC  | The Monolith | Pirate Party | FTM-BOO   | MAI debito |
| ------ | --------- | ------------ | ------------ | --------- | ---------- |
| 30     | 1,033.503 | 500.000      | 1.901        | 60.500    | 440.541    |
| 60     | 1,069.343 | 500.000      | 8.031        | 123.652   | 378.905    |
| 90     | 1,106.425 | 500.000      | 18.452       | 187.988   | 317.139    |
| 120    | 1,144.794 | 500.000      | 33.265       | 254.136   | 255.242    |
| 150    | 1,184.493 | 500.000      | 52.612       | 322.738   | 193.216    |
| 180    | 1,225.569 | 500.000      | 76.681       | 394.462   | 131.058    |
| 210    | 1,268.069 | 500.000      | 105.704      | 470.006   | 68.770     |
| 240    | 1,312.043 | 500.000      | 139.963      | 550.105   | 6.351      |
| 270    | 1,357.542 | 500.000      | 181.427      | 691.752   | 0.000      |
| 300    | 1,404.619 | 500.000      | 233.046      | 846.443   | 0.000      |
| 330    | 1,453.328 | 500.000      | 295.350      | 1,009.331 | 0.000      |
| 360    | 1,503.726 | 500.000      | 368.942      | 1,182.000 | 0.000      |

### Giorno 365

Alla fine di un anno intero di farming con questo sistema, avreste fatto

* $1,512.294 in token LP $FTM-$USDC su Market.xyz
* $500.000 in $MAI nel pool The Monolith
* $382.353 in $LQDR nel pool Pirate Party
* $1.211.845 in token LP $FTM-$BOO su Market.xyz
* un debito finale che viene completamente ripagato dopo giorno #243

Questo equivale a un APY totale del 260.65%.

### Effetto del rimborso del debito sul risultato complessivo

Nella maggior parte delle nostre guide, non rimborsiamo alcun debito come parte della strategia. Ciò è, nella maggior parte dei casi, dovuto al fatto che stiamo utilizzando un prestito con interessi dello 0% preso da Mai Finance. Qui prendiamo in prestito su Market.XYZ con un tasso di finanziamento del 2,56% e ripaghiamo il debito con il 50% delle $BEETS raccolte da The Monolith.

Se destinate più del 50% al rimborso del debito, pagherete meno interessi, ma farete crescere le vostre posizioni molto più lentamente su Liquid Driver. Se dedicate meno del 50% al rimborso del debito, otterrete più ricompense dalle altre piattaforme, ma pagherete anche più interessi su Market.xyz.

Ecco una piccola tabella che indica l'effetto delle $BEETS assegnate al rimborso del debito sull'APY complessivo:

| BEETS % | APY Complessivo | debito ripagato dopo |
| ------- | --------------- | -------------------- |
| 100     | 242.85          | 122 days             |
| 90      | 245.06          | 135 days             |
| 80      | 247.75          | 152 days             |
| 70      | 251.05          | 174 days             |
| 60      | 255.23          | 203 days             |
| 50      | 260.65          | 244 days             |
| 40      | 267.92          | 305 days             |
| 33.5    | 274.09          | 364 days             |

Se utilizzate meno del 33,5% dei vostri premi $BEETS per ripagare il vostro debito, avrete ancora un po' di $MAI da rimborsare dopo un anno intero.

È anche bene capire che se ripagate più velocemente, aumenta anche il vostro CDR in modo più significativo, il che vi consente di allontanarvi più velocemente dal rapporto di liquidazione.

## Varianti da considerare

Questa strategia presenta molte varianti che presentano vantaggi diversi.

### Mai Finance VS Market.xyz

Potete prendere in prestito $MAI da [Mai Finance](https://app.mai.finance) a interesse 0%. Ad esempio, se usate $mooScreamFTM invece di $mooBooFTM-$USDC come garanzia, questo presenterà i seguenti vantaggi:

* Non avete impermanent loss sulla vostra garanzia
* Prendete in prestito allo 0% con una singola commissione di rimborso dello 0,5%, che sarà nella maggior parte dei casi molto inferiore agli interessi che pagherete su Market.xyz (se ci sono $MAI da prendere in prestito per questo vault)
* Potete ottenere premi $QI per i prestiti sulla piattaforma, che vi permetteranno di partecipare alla governance del protocollo, oltre a ottenere dividendi se li mettete in stake. Ciò aumenterà i vostri guadagni annuali
* Siete protetti da tassi di prestito molto fluttuanti su Market.xyz. Mai Finance presterà regolarmente nuovi $MAI per mantenere i tassi di prestito il più bassi possibile, ma non è una garanzia che non salga. Potete controllare le metriche per il mercato dei prestiti [qui](https://metrics.market.xyz/d/HChNahwGk/fuse-pool-details?orgId=1\&refresh=10s\&var-poolID=10\&var-chain=250).

Tuttavia, i token $mooScreamFTM ottengono un APY molto più basso rispetto ai token $mooBooFTM-$USDC.

### Stake dei LQDR

Se mettete in stake i vostri $LQDR invece di usarli nel pool Pirate Party, guadagnere alcuni dividendi da Liquid Driver che vengono pagati in diversi asset ($LQDR, $WFTM, $LINSPIRIT, $BOO, $SPELL e $BEETS). Riceverete anche $xLQDR che vi consentirà di partecipare alla governance di Liquid Driver e possibilmente $LINSPIRIT per votare sull'assegnazione dei premi su Spirit Swap. Si prega di controllare attentamente la pagina xLQDR per maggiori dettagli.

### Stake dei BEETS

Se i $BEETS di The Monolith giocano un ruolo importante in questa strategia, potete utilizzare totalmente quelle del Pirate Party come segue:

* depositate i $BEETS nel pool Fidelio Duetto ($BEETS-$FTM)
* mettete in stake il token LP su BeethovenX per ricevere $fBEETS
* mettete in stake $fBEETS per ottenere i dividendi del protocollo

Ciò vi consentirà anche di votare sui miglioramenti del protocollo BeethovenX, nonché sull'assegnazione delle ricompense per i diversi pool sulla piattaforma. Ciò è particolarmente utile per mantenere un APR alto su The Monolith.

### Usare il pool FTM-BEETS su Spookyswap

Nella nostra strategia, vendiamo tutte le ricompense $BEETS di The Monolith. Tuttavia, potreste anche integrare il pool $FTM-$BEETS di Spookyswap nel loop. Dovreste vendere il 50% dei $BEETS per $FTM e combinare i due token in una nuova coppia LP che vi farà guadagnare $BOO. Potete quindi decidere di creare l'LP $FTM-$BOO e depositare su Liquid Driver, oppure potete mettere in stake $BOO su SpookySwap. Notate che se mettete in stake $BOO, avrete la possibilità di depositare i token di ricevuta $xBOO e guadagnare token $LQDR direttamente e potete persino utilizzare i token $xBOO come garanzia su Market.xyz. Questo mattoncino lego aggiuntivo apre molte possibilità.

{% hint style="info" %}
Tenete d'occhio questa coppia in particolare nel caso in cui diventi disponibile su Liquid Driver. Questa potrebbe essere un'opzione migliore di quella $FMT-$BOO.
{% endhint %}

### Usare i FTM-USDC su Liquid Driver

Dopo che il vostro prestito è stato completamente rimborsato, potete conservare i token $mooBooFTM-$USDC su Market.xyz o su Beefy e continueranno ad accumulare ricompense. Tuttavia, potete anche rimuovere la coppia di LP da Beefy e depositarla su Liquid Driver per ottenere più $LQDR.

Come nota a margine, mentre state rimborsando il vostro prestito, il valore del vostro rapporto garanzia/debito cresce (il collaterale sta guadagnando ricompense e aumenta di valore mentre il debito si sta riducendo dopo ogni rimborso parziale). Ciò significa che potete ritirare il collaterale pezzo per pezzo per mantenere un CDR sicuro e depositarlo su Liquid Driver per più token $LQDR.

### Mantenete una piccola perdita di profitto

Questo sistema è un circuito chiuso che si autoalimenta. Tuttavia, potete benissimo continuare a vendere parti di $BEETS per altri assets dopo aver finito di rimborsare il vostro prestito su Market.xyz. Ad esempio, potreste convertire i $BEETS in $USDC o in un'altra coppia di farm, oppure aumentare una delle vostre posizioni che guadagna più ricompense di quelli concessi per la coppia $FTM-$USDC.

## Disclaimer

Questa guida è stata principalmente progettata per mostrare il modo in cui potete ripagare un debito utilizzando i rendimenti da farm. La velocità con cui ripagate il vostro debito influenzerà notevolmente il rendimento globale, ma presenta anche alcuni aspetti molto positivi, il principale è la riduzione del rischio di liquidazione.&#x20;

Ovviamente, potete facilmente adattare questa strategia, cambiare pezzi del ciclo con altri, sostituire i protocolli con qualcosa che preferite ecc ... Tuttavia, assicuratevi di leggere tutta la documentazione disponibile per i protocolli che desiderate utilizzare e assicuratevi di comprendere tutti i diversi rischi.

{% hint style="info" %}
Questa guida non è assolutamente un consiglio finanziario, è stata realizzata a solo scopo educativo. Dovete prestare attenzione alle variazioni di prezzo, domanda e offerta, date di fine dei programmi di ricompensa, impermanent loss ecc... L'obiettivo non è quello di proporre ricette che possono essere seguite alla cieca quindi, per favore, fate i compiti e fate le vostre simulazioni e investite solo ciò che siete disposti a perdere.
{% endhint %}
