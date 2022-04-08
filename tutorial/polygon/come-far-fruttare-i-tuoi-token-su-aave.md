---
description: >-
  Questo tutorial mostra passo per passo come gli utenti possono far fruttare i
  propri investimenti in crypto combinando intelligentemente i prestiti a tasso
  0% di Mai Finance al protocollo Aave.
---

# Come far fruttare i tuoi token su Aave

## Quando un'immagine vale più di mille parole

![](<../../.gitbook/assets/image (21) (1) (1).png>)

## Ma in fondo mille parole non sono poi così male

L'immagine sopra mostra come puoi utilizzare Mai Finance per aumentare la rendita dei tuoi investimenti in crypto valute.&#x20;

Supponiamo che adori MATIC e pensi che attualmente sia sottovalutato. Pensi che abbia il potenziale per raggiungere $2, $5 o anche $10 per token (e potresti non avere tutti i torti). Tuttavia, sei un piccolo investitore ed hai solo $100 di token MATIC nel tuo portafoglio su Polygon. Attraverso questo tutorial mostreremo come puoi generare più MATIC dai tuoi token attuali, perché l'"hodling" è cosa buona e giusta ma mettere a rendita il tuo investimento lo è ancora di più.

### Utilizzare Aave per aumentare il tuo capitale

[Aave](https://app.aave.com) è una piattaforma di deposito e prestito in cui puoi depositare i tuoi token MATIC (insieme ad altri token). Depositando su Aave, i tuoi token depositati guadagneranno un rendimento. Ad esempio, i tuoi $100 di MATIC genereranno potenzialmente un tasso di rendita dell'1,2% nell'arco di 1 anno (APY). A volte, Aave proporrà anche campagne specifiche che forniranno premi aggiuntivi oltre agli APY di deposito di base. Dato che i tuoi token MATIC sono nel pool Aave, l'interesse generato viene automaticamente reinvestito, ciò significa che la quantità di MATIC che detieni crescerà nel tempo.

![In questo esempio, ho depositato 0.2 MATIC](../../.gitbook/assets/screen-shot-2021-08-06-at-5.29.53-pm.png)

Depositando il tuo token MATIC su Aave, ricevi una quantità equivalente di amWMATIC (aave market wrapped MATIC). Potresti non vedere questi token direttamente nel tuo portafoglio a meno che tu non li aggiungi manualmente ma li possiedi.

![Posso vedere i 0.20 MATIC che ho depositato da DeBank](../../.gitbook/assets/screen-shot-2021-08-06-at-5.31.01-pm.png)

### Utilizzare Mai Finance per far crescere i tuoi token Aave

Mai Finance può accettare i tuoi token amWMATIC sulla pagina "Yield" del sito web. Depositando i tuoi amWMATIC su Mai Finance i tuoi fondi verranno "trasferiti" da Aave a Mai Finance.&#x20;

Noterai che il rendimento generato da Mai Finance è lo stesso che otterresti su Aave.

Tuttavia, oltre all'APY di base, Mai Finance reinvestirà anche le eventuali ricompense Aave aggiuntive disponibili per il token scelto (nel nostro esempio MATIC), generando così un rendimento passivo maggiore nel token scelto. Nel nostro esempio (vedi sopra), Aave fornisce l'1,16% di APY per i MATIC depositati ed un APR "premio" aggiuntivo del 3,69% pagato in MATIC ma questo "premio" aggiuntivo non genera alcun rendimento. Depositando il tuo amWMATIC su Mai Finance, il "premio" viene raccolto periodicamente e reinvestito sul tuo deposito principale in modo da ottenere anche su di esso il tasso di interesse dell'1,16%.

![I miei 0.2 MATIC ora sono depositati su Mai Finance genereranno un rendimento del 4.93% annuale](../../.gitbook/assets/screen-shot-2021-08-06-at-5.45.00-pm.png)

Quando gli amWMATIC vengono depositati su Mai Finance, in cambio si ottengono i camWMATIC. Il rapporto tra questi due token non è perfettamente 1:1, questo perché camMATIC rappresenta in realtà una quota del pool amWMATIC su Mai, all'interno del quale interessi e premi vengono automaticamente reinvestiti. E' importante anche evidenziare che quando depositi gli amWMATIC su Mai Finance, questi token vengono rimossi da Aave. Tuttavia, se ritiri i tuoi amWMATIC da Mai Finance, li ritroverai su Aave.

{% hint style="info" %}
Il solo deposito del tuo amWMATIC (o qualsiasi amToken) su Mai Finance ti consentirà di generare più entrate rispetto a depositare i tuoi soldi su Aave. In effetti, il fatto che il tuo interesse di base e il tuo premio aggiuntivo siano auto-reinvestiti significa che non devi richiedere manualmente il tuo premio, convertirlo nel token di tua scelta e depositarlo di nuovo.
{% endhint %}

### amTokens VS camToken

Molte persone hanno difficoltà a capire la differenza tra amToken e camToken. L'amToken è una rappresentazione dei tuoi fondi depositati su AAVE sotto forma di token. Il loro importo è ancorato all'importo che hai depositato su AAVE. Tuttavia, camToken rappresenta una quota del pool amToken su Mai Finance.&#x20;

Supponiamo che quando il pool amToken è stato creato su Mai Finance, ci fossero 1.000 amToken e tu ne hai depositati 100. Dato che il pool è appena stato creato, il rapporto tra amToken e camToken è 1:1 e tu possiedi il 10% del pool. Dopo un anno, supponendo che nessuno abbia aggiunto nè rimosso altri amToken, il pool avrà generato un interesse del 4,93% e ora nel pool ci sarebbero 1049,3 amToken. Tuttavia, sei in possesso sempre solo del 10% del pool, rappresentato dai tuoi 100 camToken. Il rapporto ora è 1:1,0493, il che significa che 1 camToken ora vale 1,0493 amToken.

### Prendere in prestito MAI (stable coin)

Mai Finance ti consente di prendere in prestito la stable coin MAI quando depositi fondi. Uno dei principali vantaggi è che i token camWMATIC (e altri camToken) possono essere utilizzati come garanzia. Su Mai Finance, i tuoi camWMATIC continueranno a generare interesse mentre li utilizzi come collaterale, ciò si traduce in un aumento del CDR (Collateral to Debt Ratio). Più a lungo mantieni i tuoi prestiti, più facilmente sarai in grado di rimborsare lo 0,5% di commissioni di rimborso addebitate dalla piattaforma.

{% hint style="info" %}
Quando camWMATIC viene depositato in un Vault, il saldo sulla pagina Yield sarà 0. Tuttavia, ciò non significa che non comporti interessi e ricompense AAVE.
{% endhint %}

Quando accederai alla pagina Vault e selezionerai camWMATIC dal menu a discesa del vault, ti verrà data la possibilità di creare un nuovo vault in cui puoi depositare il tuo camWMATIC. Tieni in consiederazione che devi mantenere un Collateral to Debt Ratio (CDR) di almeno il 155% quando prendi in prestito a fronte dei tuoi camWMATIC.

![I miei 0.2 MATIC sono completamente usati come collaterale](../../.gitbook/assets/screen-shot-2021-08-06-at-5.57.55-pm.png)

**Nota**: in questa pagina potrai vedere il valore del tuo collaterale in USD e il valore varia in base al tipo di collaterale, al valore del token e ai vantaggi generati dal pool camWMATIC.

**Suggerimento**: quando deposito un collaterale per prendere in prestito MAI, prendo sempre in prestito il 50% del valore del collaterale. Idealmente, è meglio rimanere al di sopra del 200% del valore di Collateral to Debt Ratio (CDR) e se il valore del mio collaterale sta crescendo (perchè il token non perde valore e gli interessi continuano ad essere reinvestiti) mi sento abbastanza al sicuro. Inoltre, quando aggiungo ulteriore collaterale a un vault, non cerco di tornare ad un CDR del 200% , a meno che il CDR non sia al di sotto. Io prendo sempre in prestito fino al 50% (vedi l'esempio con i numeri sotto).

{% hint style="info" %}
E' importante ricordarsi che è propria responsabilità visitare di tanto in tanto la pagina del Vault per verificare di essere sempre al di sopra del rapporto di liquidazione e possibilmente aggiungere ulteriore collaterale se si inizia a scendere al di sotto di un certo "limite di sicurezza". A seconda del profilo di rischio, questa soglia di sicurezza può variare di caso in caso.
{% endhint %}

![In questo caso ho un debito di 0.1USD mantenendo un CDR del 214.56%](../../.gitbook/assets/screen-shot-2021-08-06-at-6.07.34-pm.png)

Ho preso in prestito $0,10 di MAI, che si traduce in un CDR del 214,56%. Ora divertiamoci un po' con i miei soldi.

### Comprare altri MATIC

Ora posso tranquillamente andare sul mio DEX preferito (QuickSwap o SushiSwap ad esempio) e scambiare i miei MAI con più MATIC.

![](../../.gitbook/assets/screen-shot-2021-08-06-at-6.10.35-pm.png)

Dopo lo scambio, ho più MATIC nel mio portafoglio.

### Ripetere il ciclo

Inizialmente avevo 0,20 MATIC nel mio portafoglio. Questi MATIC ora sono depositati su Mai Finance, generando un rendimento del 4,93% annuo ed ho in aggiunta 0,09 MATIC resi disponibili grazie ai MAI che ho preso in prestito. Questi 0,09 MATIC aggiuntivi possono essere depositati su Aave, proprio come i miei MATIC iniziali e ripartire con lo stesso processo.

### In che momento dovrei fermare il ciclo?

In termini di passaggi, l'approccio migliore è fermarsi quando si deposita la camWMATIC nel Vault . In questo modo si aumenta il rapporto collaterale/debito e di conseguenza si riduce il rischio di essere liquidati. Tuttavia, a seconda dell'ultimo importo depositato, questo potrebbe essere abbastanza trascurabile. Per quanto riguarda il numero di cicli, di solito mi fermo quando sono entro l'1% del mio investimento iniziale. Nel caso dell'esempio, continuerei il ciclo fino a depositare 0.002 camWMATIC. Potrei anche fermarmi prima se il prezzo del gas pagato per le transazioni diventa più alto di quello che potrei guadagnare continuando il ciclo.

## Esempio con numeri

Gli esempi che seguono si basano su $1.000 di MATIC, con diversi rapporti CDR e mostrano come sfruttare le tue posizioni attraverso Mai Finance.

### 200% di rapporto Collaterale/Debito&#x20;

| Ciclo numero | Investimento |  Debito | Rendimento stimato |
| :----------: | -----------: | ------: | -----------------: |
|       1      |    1 000,00$ | 500,00$ |             49,30$ |
|       2      |    1 500,00$ | 750,00$ |             73,95$ |
|       3      |    1 750,00$ | 875,00$ |             86,75$ |
|       4      |    1 875,00$ | 937,50$ |             92,44$ |
|       5      |    1 937,50$ | 968,75$ |             95,52$ |
|       6      |    1 968,75$ | 984,38$ |             97,06$ |
|       7      |    1 984,38$ | 992,19$ |             97,83$ |
|       8      |    1 992,19$ |       - |             98,21$ |

Aggiungere più debito oltre il ciclo n.7 aumenterebbe il mio investimento di meno di $10 (1% del mio investimento iniziale), quindi questo è il momento giusto per fermarmi. L' aumento dell'APY è trascurabile in questa fase e il mio rapporto collaterale/debito rimane del 200,79%, abbastanza sicuro.&#x20;

Come si può facilmente vedere, l'utilizzo di una combinazione di Aave e Mai Finance si traduce in quasi il doppio dell'APY iniziale e un'esposizione di mercato significativamente maggiore al token scelto rispetto alla semplice detenzione o utilizzo del solo Aave.

### 175% di rapporto Collaterale/Debito

| Ciclo numero | Investimento |    Debito | Rendimento stimato | APY Equivalente |
| :----------: | -----------: | --------: | -----------------: | --------------: |
|       1      |    1 000,00$ |   571,43$ |             49,30$ |          4,930% |
|       2      |    1 571,43$ |   897,96$ |             77,47$ |          7,747% |
|       3      |    1 897,96$ | 1 084,55$ |             93,57$ |          9,357% |
|       4      |    2 084,55$ | 1 191,17$ |            102,77$ |         10,277% |
|       5      |    2 191,17$ | 1 252,10$ |            108,02$ |         10,802% |
|       6      |    2 252,10$ | 1 286,91$ |            111,03$ |         11,103% |
|       7      |    2 286,91$ | 1 306,81$ |            112,74$ |         11,274% |
|       8      |    2 306,81$ | 1 318,18$ |            113,73$ |         11,373% |
|       9      |    2 318,18$ | 1 324,67$ |            114,29$ |         11,429% |
|      10      |    2 324,67$ |         - |            114,61$ |         11,461% |

L'aggiunta di più debito oltre il ciclo n.9 non aumenterebbe il mio investimento di più di $10, quindi questo è il punto giusto in cui fermarmi. Il CDR risultante da 9 cicli è 175,49%.&#x20;

Possiamo facilmente vedere che con un approccio più aggressivo l'APY finale è anche più appetibile. Questo è generalmente vero con qualsiasi strategia DeFi: maggiore è il rischio, maggiore è la potenziale ricompensa.

### Ancora più numeri

Se sei incline alla matematica, puoi calcolare il tuo investimento finale in base all'investimento iniziale e al rapporto collaterale/debito che desideri raggiungere. La formula è la seguente:

$$
InvestimentoFinale = InvestimentoIniziale *\sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

Dove n rappresenta il numero di cicli che si desidera applicare e CDR è il rapporto collaterale/debito che si vuole mantenere in percentuale. Nell'esempio di un CDR obbiettivo del 200% con 7 loop, il calcolo è il seguente:

$$
InvestimentoIniziale = 1000 *\sum_{i=0}^{7}{\frac{100}{200}}^i
$$

$$
InvestimentoFinale = 1000 * (\frac{1}{2}^0 + \frac{1}{2}^1 + \frac{1}{2}^2 + \frac{1}{2}^3 + \frac{1}{2}^4 + \frac{1}{2}^5 + \frac{1}{2}^6 + \frac{1}{2}^7)
$$

$$
InvestimentoFinale = 1000 * (1 + 0.5 + 0.25 + 0.125 + 0.0625 + 0.03125 + 0.015625 + 0.0078125)
$$

$$
InvestimentoFinale = 1000 * 1.9921875 = 1992.1875
$$

Utilizzando lo stesso metodo, puoi anche calcolare il tuo APY finale con l'equazione seguente:

$$
APY equivalente = APY iniziale * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

E ancora, con il nostro CDR obbiettivo del 200%, un APY iniziale del 4,93% e 7 loop, calcoliamo lo stesso APY finale come mostrato nelle tabelle sopra

$$
APY equivalente = 4.93 * 1.9921875 = 9.821484375
$$

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Tutto ciò che viene presentato in questa strategia presuppone quanto segue: &#x20;

* L' APY di Aave è stabile e rimane lo stesso nell'arco di 1 anno (l'APY avrà qualche variazione)&#x20;
* L' APR che Polygon ha concesso ad Aave è stabile e rimane lo stesso nell'arco di 1 anno (il che è improbabile)
* Il token MATIC mantiene un prezzo relativamente stabile nell'arco di 1 anno (anche questo improbabile)

{% hint style="info" %}
Tenete presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farvi perdere denaro) in un altro. Tenetevi aggiornati, monitorate i mercati, tenete d'occhio i vostri investimenti e come sempre, fate le vostre ricerche.
{% endhint %}
