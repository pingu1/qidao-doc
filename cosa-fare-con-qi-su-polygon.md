---
description: >-
  Questo tutorial illustra le varie opzioni di utilizzo di Qi, il token nativo
  di Mai Finance su Polygon. Analizzeremo anche se Qi è una buona opportunità di
  investimento e cosa ne determina il prezzo.
---

# Cosa fare con Qi su Polygon

## Introduzione

Qi (\[tʃ Í] o _chee_), è il token nativo di Mai Finance. Alcuni lo usano per votare e per il QIP (Proposte di miglioramento QiDAO), alcuni lo mettono a rendita per ottenerne ancora di più e alcuni semplicemente lo usano per farmare. Puoi trovare alcune ottime informazioni su come utilizzare il Qi sulla piattaforma Mai Finance nella [guida dedicata alla rendita passiva](Universita-di-MAI/ottenere-una-rendita-passiva-con-qidao.md).

Questa guida, come la maggior parte dei tutorial sugli investimenti, si concentrerà principalmente sul farming e la messa a rendita, questa volta utilizzando il token Qi. Vedremo come è possibile ottenere molti Qi e come utilizzarli sulle diverse piattaforme di Polygon.

I farmer coscienziosi solitamente consigliano di essere umili, vendere ciò che si ottiene e prendere profitti. Ma io personalmente ti dirò:

> Dai un pesce a un uomo e mangerà per un giorno. Insegna a un uomo a pescare e per tutta la vita non soffrirà la fame.

Quindi prendete le vostre canne da pesca e seguite la guida.

## Cosa fare con i tuoi Qi su Polygon

### Messa a rendita (stake)

Non dedicherò troppo tempo a questo argomento, c'è già una guida completa. Tieni presente che Mai Finance sta raccogliendo entrate e ne ridistribuisce una parte molto ampia a chi mette in stake Qi. Mettere in stake il tuo Qi su Mai Finance è uno dei migliori usi del token e a partire da settembre 2021, il 23% di tutto il Qi circolante risulta in stake in media per 2 anni.

### Farming su una coppia LP

Anche in questo caso ci sono già altre pagine che presentano come includere il token Qi nella tua strategia di farming per generare rendimenti e non vendere mai nessuno dei tuoi farm token. Guarda le guide [Impilare le dApp come mattoncini Lego](impilare-le-dapp-come-mattoncini-lego.md) o [Farmare o mettere in Stake?](farmare-o-mettere-in-stake-o-entrambe.md) per ulteriori dettagli.

Come rapido promemoria, Qi è abbinato a diversi token per formare coppie LP (Liquidity Provider) su QuickSwap in modo da poter farmare:

* Qi-WMATIC su Mai Finance ed ottenere ricompense in token Qi
* Qi-WETH su QuickSwap ed ottenere ricompense in token QUICK
* Qi-QUICK su QuickSwap ed ottenere ricompense in token QUICK

![LP pool su QuickSwap per la coppia Qi-WETH](<.gitbook/assets/image (19) (2) (1).png>)

### Farm singolo di Qi

Qi può essere utilizzato anche su [Impermax](https://polygon.impermax.finance). Impermax è una piattaforma in cui sarai in grado di sfruttare una coppia di LP specifica più volte per aumentare i tuoi profitti da QuickSwap.

Funziona in questa maniera, prenderai in prestito i 2 token che formano la coppia che vuoi farmare, li combinerai in più token LP e farmerai in leva, con una posizione di un valore molto più alto. Nella maggior parte dei casi, i tassi di prestito sono ampiamente compensati dall' APR della farm, dandoti dei premi netti positivi.

![Posizione in leva(5x) di Qi-WETH su Impermax](<.gitbook/assets/image (10).png>)

Possiamo vedere che l'APR finale su Impermax è 393,88% sfruttando la leva 5x a fronte di un APY base del 239,68% su QuickSwap.

{% hint style="info" %}
Nota bene che Impermax fornisce APR stimati (premi percentuali annuali) mentre QuickSwap fornisce APY stimati (rendimenti percentuali annuali), il che significa che QuickSwap presuppone che tu reinvesta le tue ricompense ogni giorno. L'APY del 239,68% su QuickSwap corrisponde a un APR del 122,49%.
{% endhint %}

Ma ovviamente per prendere in prestito Qi e WETH per mettere in leva la tua posizione su Impermax, devi prenderli da qualche parte. Ciò viene reseo possibile perché altri utenti (o te stesso) forniscono entrambi i token separatamente. Più token vengono presi in prestito, più alto diventa il tasso di prestito e più basso è l'APR finale, a volte negativo.

![Statistiche di Qi e WETH per il mercato Qi-WETH su Impermax](<.gitbook/assets/image (11).png>)

Per il nostro esempio ci concentreremo su Qi. Puoi notare che la supply totale di Qi è di $427,21 e l'importo totale preso in prestito nelle posizioni con leva è di $321,44, con un tasso di utilizzo del 75,24%. Impermax ha un meccanismo interno che calcola automaticamente l'APR di fornitura (APR che otterranno gli utenti che prestano Qi) e l'APR di prestito (percentuale della ricompensa da farming che verrà sottratta quando si ripaga il prestito).

Questo significa che puoi fornire Qi esclusivamente su Impermax e ottenere, nel nostro esempio, il 43,73% di APR, al momento in cui scriviamo questo articolo. Al variare della domanda e dell'offerta, anche l'APR dell'offerta aumenterà/diminuirà. Quando fornisci singoli token su Impermax, verrai ricompensato con il token che fornisci, il che significa che questa strategia ti farà accumulare più Qi nel tempo.

Mentre sei su Impermax, puoi anche utilizzare l'opzione leva per ottenere premi IMX. Consiglio di leggere la [guida Staking](impilare-le-dapp-come-mattoncini-lego.md) per avere maggiori dettagli su come includere Impermax nella tua strategia di farming.

### Balancer

Balancer è davvero una bella cassetta degli attrezzi per qualsiasi strategia, specialmente quelle che includono Qi e/o MAI. Balancer propone un equivalente del farming di coppie LP ma con più di 2 token forniti in un rapporto 1:1. Il pool può avere 3, 4 o 5 token (a volte anche di più) con peso diverso, e l'algoritmo che gestisce il pool fa in modo che il rapporto per ogni token sia sempre rispettato, vendendone alcuni e acquistandone altri per mantenere l'equilibrio previsto. 

Il pool che vogliamo usare qui è un pool che contiene Qi, WMATIC, BAL, USDC e MAI. Questo pool ti ricompenserà con entrambi i token Qi e BAL e puoi già vedere che sarai in grado di combinare entrambi nel pool. Lo straordinario vantaggio dei pool su Balancer è che non è necessario fornire tutti i token che formano il pool nel rapporto corretto, l'algoritmo lo farà per te. Ciò significa che puoi effettivamente depositare solo Qi nel pool e lasciare che l'algoritmo faccia il resto per riequilibrare tutto.

![](<.gitbook/assets/Schermata 2021-10-03 alle 20.23.02.png>)

Come nota a margine, i token BAL possono (o saranno presto) essere utilizzati come garanzia su Mai Finance, il che significa che avrai la possibilità di depositare i tuoi token BAL nel Vault BAL su Mai Finance e prendere in prestito MAI. Inoltre, prendere in prestito MAI a fronte dei tuoi BAL ti renderà idoneo per i premi Qi che alimenteranno il pool su Balancer.

![Ciclo completo tra Mai Finance e Balancer](<.gitbook/assets/image (13).png>)

L'APR del vault BAL determinerà quanto sia interessante avere il vault nel ciclo o se sarà meglio depositare i tuoi Qi nel pool di Balancer.

## Capire il prezzo di Qi

Ottenere molti Qi è un conto ma se il token perde valore nel tempo, è davvero una buona strategia tenerlo? 

In questa sezione, cercheremo di capire i diversi fattori che incidono direttamente sul prezzo di Qi in modo che quando inizierai a investire i tuoi Qi avrai un'idea migliore di come il suo prezzo può variare e quale impatto avrà sull'ecosistema Qi.

### Emissione di Qi

Uno dei principali fattori che influenzerà il prezzo del Qi è la velocità con cui verranno creati. Come ben sai il prezzo è sempre guidato dalla domanda e dall'offerta. Se c'è molta offerta e domanda molto bassa, il prezzo scenderà naturalmente. Quindi capire come viene generato il Qi è fondamentale per stimarne il valore nel tempo. 

Attualmente ci sono 2 fonti di emissione di Qi: ricompense per il farming e ricompense per i vault.

![LP Farm su Mai Finance ad Ottobre 2021](<.gitbook/assets/Schermata 2021-10-03 alle 20.32.00.png>)

Se vuoi farmare su MAI Finance puoi scegliere tra la coppia MAI/USDC e la coppia Qi/WMATIC ( ad Ottobre 2021).

* La coppia MAI/USDC è ricompensata con 0.5 Qi / blocco
* La coppia Qi/WMATIC è ricompensata con 1 Qi / blocco

Su Polygon, il tempo di blocco previsto è di 2 secondi e poiché ci sono 86.400 secondi in un giorno, questo significa che il pool MAI/USDC viene premiato con 21.600 Qi ogni giorno e Qi/WMATIC con 43.200 Qi.

I pool su Mai Finance da soli sono responsabili della creazione di 64,800 Qi quotidianamente.

Per quanto riguarda i vault, ogni vault riceve un'emissione di 0,05 Qi/blocco ovvero un'emissione giornaliera di 2.160 Qi, e attualmente ci sono 10 Vault per un totale di 21.600 Qi assegnati come ricompense del Vault.

Ciò significa che ogni giorno vengono coniate e distribuiti agli utenti l'equivalente di 86.400 Qi.

### Ottimizzatori dei rendimenti

Gli ottimizzatori dei rendimenti sono piattaforme che reinvestono automaticamente le ricompense da farm con alcune strategie predefinite offrendo ricompense aggiuntive per invogliare gli utenti all'utilizzo del protocollo stesso. La strategia nella maggior parte dei casi prevede di vendere gran parte delle ricompense e riutilizzare i profitti in un altro modo all'interno della piattaforma stessa.

Ad esempio, Adamant offre il farming della coppia di LP Qi/WMATIC sulla loro piattaforma, con la seguente distribuzione di ricompense:

![Qi-WMATIC pool su Adamant](<.gitbook/assets/image (15).png>)

![Dettaglio dell' APR del 179.23% offerto da Adamant](<.gitbook/assets/image (14).png>)

Noterai che l'APR complessivo è superiore a quello di Mai Finance ma solo perché Adamant sta assegnando ulteriori premi ADDY agli utenti. La quantità di Qi che viene effettivamente ridistribuita è del 98,45% rispetto al 134,42% che si può ottenere su Mai Finance.

Di questa ricompensa Qi del 98,45% la metà viene venduta direttamente per acquistare WMATIC ed aggiungere token LP QI/WMATIC all'investimento iniziale dell'utente.

Con 100 $ di token LP, supponendo che l'APR e i prezzi dei token rimangano gli stessi per un anno intero e supponendo che non ci siano reinvestimenti otterresti dopo un anno di farming:

* $134.42 in Qi su Mai Finance
* $98.45 in Qi/WMATIC token o $49.23 in Qi su Adamant

Ciò significa che, nel processo, $85,20 di Qi vengono semplicemente venduti direttamente sul mercato ovvero più del 60% dell'emissione totale assegnata al pool su Adamant.

E Adamant non è l'unica piattaforma che propone lo stesso tipo di servizio. Alcuni altri esempi sono Beefy Finance e Kogecoin. Dei $4,9 milioni di TVL nella farm Qi/WMATIC su Mai Finance, $ 2,3 milioni provengono direttamente da Adamant, $41k da Beefy e $12k da Kogecoin. Insieme, queste 3 piattaforme rappresentano oltre il 50% del valore bloccato su Mai Finance. Una stima grezza è che oltre il 30% dell'emissione giornaliera totale di Qi viene scaricata da queste piattaforme, esercitando una pressione di vendita molto negativa sul token, diminuendo il suo prezzo, il che spiega in parte perché Qi abbia difficoltà a mantenere un prezzo elevato.

### Capire le coppie di LP

Quando si farma fornendo coppie LP, il token LP viene effettivamente utilizzato per fornire liquidità agli utenti che stanno scambiando un token con un altro. Nel nostro esempio di Qi/WETH quando qualcuno acquista WETH, parte di questo token può essere tolto dal pool LP e venduto all'utente che lo richiede.

A questo punto, dato che un po' di WETH è stato tolto dal pool, c'è un disequilibrio: meno WETH rispetto alla quantità di Qi. L'algoritmo incaricato di mantenere il rapporto del pool 1:1 venderà quindi un po' di Qi da questo pool per riacquistare altro WETH e ricreare l'equilibrio perso. L' esatto opposto accade quando qualcuno compra Qi, WETH in quel caso viene venduto per riacquistare un po' di Qi e ristabilire l'equilibrio del pool.

Lo stesso fenomeno si verifica quando uno dei 2 token che compongono la coppia guadagna o perde valore. Ad esempio, supponiamo che il prezzo Qi sia $ 1 e il prezzo ETH sia $1.000 e che abbiamo un pool che ha un valore di $100 di Qi e $100 di WETH. Significa che il pool contiene 100 Qi e 0,1 WETH.

Ora, se il prezzo di ETH sale a $2.000 e se il pool rimane con la stessa quantità di token, avremmo $100 di Qi ma $200 di WETH e avremmo perso l'equilibrio. Quindi, l'algoritmo del pool venderà un po' di ETH per comprare un po' di Qi. Nel nostro semplice esempio, verranno venduti $50 di ETH per acquistare $50 di Qi con questo risultato:

* 150 Qi con un controvalore di $150
* 0.075 ETH con un controvalore di $150

Ciò significa che quando il prezzo di uno dei 2 token sale, il pool crea una certa domanda per l'altro, aumentando anche il suo prezzo. È però vero anche il contrario: se un token perde valore, l'altro verrà venduto per mantenere un rapporto 1:1, facendo scendere il prezzo. Questo spiega anche in parte la fluttuazione del prezzo del Qi rispetto alla fluttuazione del prezzo di WETH e WMATIC (i 2 token principali a cui è abbinato il Qi).

![Prezzo di Qi (sinistra) VS Prezzo di WMATIC (destra)](<.gitbook/assets/image (17).png>)

### Mancanza di casi d'uso

Infine, il mancato utilizzo di Qi o la mancanza di casi d'uso noti, può spiegare perché il prezzo del token sta scendendo. Le persone che raccolgono Qi dalle ricompense Vault e/o farmano su Mai Finance lo venderanno semplicemente mentre ha ancora il valore sufficiente a realizzare un profitto, senza una visione a lungo termine ed è assolutamente comprensibile. Questa guida cerca in realtà di promuovere diversi modi per utilizzare i tuoi token Qi senza venderli ma se il prezzo non aumenta o se non puoi generare benefici in altri token (e quindi perdita di profitto), ci sono pochissimi vantaggi detenerli.

### Come possiamo favorire un aumento del prezzo?

Se vogliamo che il prezzo di Qi salga (e chi non lo vorrebbe), ci sono alcune opzioni

* Ridurre le emissioni: con 86.400 nuovi Qi coniati ogni giorno, l'offerta è molto alta. Riducendo questa emissione, l'offerta potrebbe essere inferiore e con una minore offerta, il prezzo dovrebbe in teoria aumentare. Tuttavia, l'emissione attuale per le farm deve rimanere la stessa perché fanno parte di una partnership in corso con QuickSwap. Sono stati lanciati incentivi Vault e sono un modo fantastico per promuovere la piattaforma di prestito, spingendo le persone a prendere prestiti, quindi tagliare queste emissioni probabilmente non è una buona idea.
* Farmare responsabilmente: non sto dicendo che Adamant sia il principale colpevole o che sia un cattivo prodotto. In effetti, includo questa piattaforma nella maggior parte delle mie strategie e la uso quotidianamente. Tuttavia, cerco di farmare in pool per i quali ho meno preoccupazioni che il token venga venduto. Se vuoi farmare su Adamant in un pool che utilizza la farm Mai Finance, tieni presente che partecipi ad abbattere il prezzo di Qi. Se non ti interessa va benissimo.
* Comprendere come funzionano le cose: i prezzi di TUTTE le crypto valute sono altamente volatili e il più delle volte, il prezzo di BTC ed ETH influenza il prezzo di tutti gli altri token. Questo non succede per caso o per un trucco magico. Inoltre, tieni presente che quando alcune persone guadagnano denaro, è perché altre ne stanno perdendo. Non ci sono soldi gratis e i soldi magici su Internet non sono così magici.
* Trova nuovi modi per utilizzare i tuoi token Qi. Questa guida fornirà sempre idee che ti aiuteranno ad aumentare il volume del tuo portafoglio e a vendere il minor numero di token possibile. I cicli chiusi sono i migliori perché l'output di un prodotto alimenta l'input di quello successivo, creando una bella interconnessione tra protocolli che crescerà nel tempo.

Tieni presente anche che:

$$
Valore = Quantità * Prezzo
$$

Quando il prezzo scende ma la tua quantità aumenta, il tuo valore potrebbe aumentare o almeno non diminuire così velocemente.

## Disclaimer

Questa guida è il risultato di molte discussioni sul prezzo di Qi sul canale [Discord](https://discord.gg/aRghpvhV). Mi sono reso conto che alcune persone che si lamentavano del prezzo non comprendevano appieno le ragioni per cui il prezzo del Qi era in costante tendenza al ribasso. Questo porta a frustrazione e delusione che è molto negativa per Qi, il prodotto Mai Finance e l'intero ecosistema DeFi in generale. Tuttavia, non c'è assolutamente alcuna garanzia che il prezzo possa mai salire, quindi se vuoi mantenere i tuoi Qi e investirli per favore fai le tue ricerche e fallo a tuo rischio. Pianifica correttamente la tua strategia e attieniti ad essa.

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
