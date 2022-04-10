---
description: >-
  Solarbeam ha una pool di farming MAI-MOVR con un bel APR. Oggi vedremo come
  sfruttarlo .
---

# Farming di MAI su SolarBeam

La maggior parte dei tutorial presentati in questa guida utilizzano stable coin come posizione iniziale. Ciò è dovuto principalmente al fatto che le coppie di stable coin non sono influenzate dall' impermanent loss né dalla volatilità di altri asset. È quindi quasi impossibile perdere il vostro capitale iniziale e potete utilizzare strategie più rischiose con i guadagni delle vostre farm per aumentare i rendimenti.

Oggi stiamo provando un altro approccio su Moonriver con Solarbeam, attualmente l'unica applicazione che utilizza $MAI. La coppia LP (**L**iquidity **P**rovider) è $MAI-$MOVR. $MAI è la stable coin di Mai Finance che potrete anche trasferire su Moonriver o coniare da un vault e $MOVR è il token gasfee nativo di Moonriver. In quanto tale, $MOVR avrà sempre una sorta di utilità e non dovrebbe mai scendere di prezzo troppo drasticamente. Questa non è una coppia stabile, ma l'unica parte variabile del token è legata al $MOVR, il che lo rende comunque un buon punto di partenza.

Vediamo come possiamo generare rendimenti molto elevati con un ciclo di chiuso su Moonriver senza scaricare troppi token farm nel frattempo.

![](../../.gitbook/assets/solarbeam-1.png)

## SolarBeam

### Farming di MAI su Solarbeam

Solarbeam è il primo e principale **DEX** (**EX**change **D**ecentralizzato) e AMM (**M**arket **M**aker **A**utomatico) su Moonriver e la seconda applicazione in termini di TVL sulla blockchain. È anche il primo vero partner Moonriver di Mai Finance e offre un pool $MAI-$MOVR che viene ricompensato con i loro token nativi, il token $SOLAR. Questo è anche il posto in cui troverete un po' di liquidità per $MAI.

![Pool MAI-MOVR su Solarbeam a Dicembre 2021](../../.gitbook/assets/solarbeam-2.png)

L'APR (**A**nnual **P**ercentage **R**ate) dell'84% è piuttosto alto a causa del basso utilizzo della pool, che lo rende anche un punto di partenza perfetto per la nostra strategia. Riceverete questo APR (corrispondente al 131% di APY se volete confrontarlo con qualcosa come $MAI-$WMATIC su QuickSwap per riferimento) e la ricompensa verrà pagata in token $SOLAR. A dicembre 2021, 1 SOLAR = 3,78 USDC.

### Staking singolo di SOLAR

La maggior parte dei fork di Uniswap ora propone lo staking per il proprio token nativo e anche Solarbeam lo sta facendo. Potete mettere in staking $SOLAR in un Vault per ottenere più $SOLAR e a seconda della durata dello stake, otterrete tariffe molto interessanti (fino al 200% di APR per un blocco di 30 giorni), ma utilizzeremo lo staking per guadagnare token esterni. In effetti, potete mettere in staking i token $SOLAR per ricevere un sacco di altri token da diverse app su Moonriver, e quello che stiamo cercando è il token $ROME.

![Staking di SOLAR per ottenere ROME su Solarbeam](../../.gitbook/assets/solarbeam-3.png)

Noterete che il pool di $ROME è quello con l'APR più basso, ma è comunque abbastanza alto, e presto vedrete che i nostri token $ROME si moltiplicheranno a un ritmo pazzesco.

## Rome DAO

Rome DAO è un altro grande player su Moonriver. È un fork di OHM (copia Olympus DAO) che utilizza il token $ROME come token nativo. Potrete mettere in stake i vostri token $ROME sull'applicazione per ottenere rendimenti molto elevati. L'obiettivo di ogni fork di OHM è di avere più token nativi messi in stake e attirare liquidità per poter sostenere l'emissione.Se avete bisogno di maggiori dettagli sui fork di OHM, controllate il nostro [tutorial su Klima DAO](../polygon/ohm-forks-on-polygon-the-case-of-klima.md) per Polygon.

![Staking di ROME su Rome DAO per un 771% di APR a Dicembre 2021](../../.gitbook/assets/solarbeam-4.png)

Dato che otterremo i token $ROME da Solarbeam, dovremmo essere in grado di metterli in staking su Rome DAO e il sistema di rebase li farà crescere molto più rapidamente. Per questa strategia, metteremo in stake i token $ROME su Rome DAO e venderemo il 50% della ricompensa giornaliera, che attualmente corrisponde a circa l'1% del deposito su Rome DAO.

## Mai Finance

Mai Finance è una piattaforma di prestito in cui potete depositare i vostri assets crypto e prendere in prestito la stable coin $MAI con un interesse dello 0%. L'unica commissione che verrà mai addebitata su Moonriver è la commissione di rimborso dello 0,5% del prestito.

![Vaul ETH su Moonriver con un sacco di MAI disponibili](../../.gitbook/assets/solarbeam-5.png)

Per la nostra strategia, utilizzeremo un deposito di $ETH. Il token $ROME che verrà estratto dallo staking pool di Roma DAO sarà suddiviso come segue:

* 33% verrà swappato con $MOVR su Solarbeam
* 66% verrà swappto con $ETH su Solarbeam

Potrete quindi depositare gli $ETH su Mai Finance per prendere in prestito $MAI con un CDR (**C**ollateral to **D**ebt **R**atio) del 200% per rimanere nella zona sicura e cercare di prevenire la liquidazione. I $MAI presi in prestito verranno quindi utilizzati per creare ulteriori token LP $MAI-$MOVR che verranno poi aggiunti alla posizione iniziale su Solarbeam.

Ad esempio, per ogni $1 di $ROME che estrarrete da Roma DAO otterrete

* $0.33 di $MOVR
* $0.66 di $ETH depositati Mai Finance
* $0.33 di $MAI presi in prestito a fronte degli $ETH
* $0.66 in token LP $MAI-$MOVR da aggiungere su Solarbeam

## Strategia di farming

La seguente simulazione è fatta assumendo alcune cose:

* Tutte le tariffe e i prezzi rimangono gli stessi per l'intero periodo della simulazione, 1 anno nel nostro caso
  * 84% di APR su $MAI-$MOVR nella farm su Solarbeam
  * 108% di APR dallo staking di $SOLAR per farmare $ROME
  * 771% di APR su Rome DAO con lo staking di $ROME
* Tutti le ricompense e i programmi sono attivi per un anno intero
* 50% dei guadagni giornalieri su Rome DAO sono venduti il 33% per $MOVR ed il 66% per $ETH
* Investimento iniziale di $100 nella coppia LP $MAI-$MOVR

![](../../.gitbook/assets/solarbeam-6.png)

### Giorno 1

Il giorno 1, depositate semplicemente i vostri $100 di $MAI-$MOVR su Solarbeam e raccoglierete i vostri token $SOLAR alla fine della giornata. Questo vi darebbe il seguente risultato:

| MAI-MOVR | SOLAR | ROME  | ETH   | Additional LP |
| -------- | ----- | ----- | ----- | ------------- |
| 100.000  | 0.230 | 0.000 | 0.000 | 0.000         |

### Giorno 2

Il giorno 2, manterrete la vostra posizione $MAI-$MOVR per farmare più $SOLAR, ma metterete in stake anche le prime ricompense di token $SOLAR per iniziare ad ottenere alcuni token $ROME. Alla fine del giorno 2, otterreste:

| MAI-MOVR | SOLAR | ROME  | ETH   | Additional LP |
| -------- | ----- | ----- | ----- | ------------- |
| 100.000  | 0.460 | 0.001 | 0.000 | 0.000         |

### Giorno 3

All'inizio del giorno 3, dovreste essere in grado di raccogliere i tuoi primi token $ROME dalla ricompensa giornaliera del 50%. Probabilmente non è una buona idea farlo il giorno 3 con solo $100 di investimento iniziale perché l'importo è abbastanza insignificante. Venderete il 33% per $MOVR e il 66% per $ETH che depositerete nel vostro vault su Mai Finance, quindi prenderete in prestito $MAI a fronte della vostra garanzia.

| MAI-MOVR | SOLAR | ROME  | ETH      | Additional LP |
| -------- | ----- | ----- | -------- | ------------- |
| 100.000  | 0.690 | 0.002 | 0.000005 | 0.000005      |

A questo punto il sistema è completamente avviato.

## Risultati del farming

### Routine quotidiana

Una volta che il sistema è completamente avviato, ecco la vostra routine quotidiana

* raccogliete $SOLAR dal pool $MAI-$MOVR
* mettete in stake i $SOLAR ottenuti
* raccogliete i $ROME dal pool di stakin $SOLAR
* mettete in stake i $ROME ottenuti
* togliete dallo stake il 50% dei guadagni giornalieri da Rome DAO (corrispondenti a circa \~1.5)
* scambiate il 66% dei vostri $ROME per $ETH
* scambiate il 33% dei vostri $ROME per $MOVR
* depositate $ETH nel vault $ETH su Mai Finance
* prendete in prestito il 50% del deposito in stable coin $MAI
* usate i $MAI presi in prestito per formare la coppia LP con $MOVR
* depositate la coppia LP $MAI-$MOVR

### Risultati grezzi mese dopo mese

| giorno | MAI-MOVR | SOLAR in stake | ROME in stake | ETH     |
| ------ | -------- | -------------- | ------------- | ------- |
| 30     | 100.021  | 7.135          | 0.352         | 0.023   |
| 60     | 100.190  | 14.045         | 1.550         | 0.200   |
| 90     | 100.713  | 20.978         | 3.911         | 0.740   |
| 120    | 101.872  | 27.968         | 7.869         | 1.925   |
| 150    | 104.052  | 35.072         | 14.023        | 4.148   |
| 180    | 107.788  | 42.378         | 23.204        | 7.947   |
| 210    | 113.814  | 50.019         | 36.559        | 14.065  |
| 240    | 123.142  | 58.178         | 55.580        | 23.525  |
| 270    | 137.175  | 67.158         | 82.767        | 37.745  |
| 300    | 157.848  | 77.321         | 120.875       | 58.681  |
| 330    | 187.841  | 89.226         | 174.234       | 89.041  |
| 360    | 230.861  | 103.358        | 248.711       | 132.575 |

### Giorno 365

Dopo un anno intero di farming, avreste

* $239.633 in $MAI-$MOVR su Solarbeam
* $106.358 in $SOLAR su Solarbeam
* $263.708 in $ROME in stake su Rome DAO
* $141.450 in $ETH su Mai Finance
* $68.817 di debito $MAI su Mai Finance

I $MAI-$MOVR aggiuntivi non corrispondono completamente al debito perchè stiamo utilizzando un terzo dei token $ROME scambiato per ottenere metà dei nuovi token LP.

Questo ciclo vi darebbe quindi un APY equivalente del 583,15% da una posizione iniziale relativamente stabile.

## Disclaimer

Le cose principali da capire da questa strategia sono che Moonriver è attualmente sotto utilizzato e i tassi di ricompensa sono molto interessanti. Inoltre, non appena usate un fork di OHM nella vostra strategia per reinvestire una parte dei vostri guadagni, i tassi di ricompensa sono così folli che realizzerete un profitto molto importante fintanto che manterrete abbastanza token nella DAO per generare ricompense.

Tenete presente, tuttavia, che i progetti avranno tassi di ricompensa variabili che non saranno garantiti nell'arco di un anno. Assicuratevi di comprendere tutto il progetto in cui state investendo, fate le vostre ricerche e assicuratevi di investire solo ciò che siete disposti a perdere. Dato che questa strategia parte con un investimento iniziale stabile, l'unica cosa a rischio qui sono i vantaggi di altri sistemi. Questa guida non può essere considerata un avallo dei progetti che utilizza.
