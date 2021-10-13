---
description: >-
  Questa pagina presenta come combinare il farming con le ricompense sui
  prestiti forniti da Mai Finance per aumentare le tue rendite complessive.
---

# Come combinare Farming e ricompense dei prestiti

## Introduzione

A Settembre 2021, Mai Finance ha introdotto i premi dei Vaults al fine di promuovere la propria attività di prestito e consentire alle persone di utilizzare i propri token per prendere in prestito MAI. Non si tratta solo di prendere un prestito a interesse 0% con una piccola commissione di rimborso, ora le persone possono anche essere pagate per prendere in prestito denaro. Questa guida proporrà una strategia basata sul farming di stable coin utilizzando Augury Finance farm di base per i token che andranno depositati nel Vault di Mai Finance, generando ricompense sui prestiti elevate e MAI aggiuntivi che verranno poi reinvestiti nella farm.

![](<.gitbook/assets/image (29).png>)

## Applicazione e presentazione dei pools

### Augury Finance

Augury Finance è un aggregatore di rendimenti che non si concentra sulla composizione automatica dei token LP (Liquidity Pool). Diversamente, Augury vende automaticamente i token delle farm e li usa per acquistare altri token nei loro "Infusions".

Ad esempio, puoi farmare la coppia DFYN-WETH su Augury

![Esempio di mining pool DFYN-WETH su Augury Finance](<.gitbook/assets/image (30).png>)

Questo Infusion utilizza DinoSwap come farm di base e un token LP che si può ottenere su DFYN. Con un APR del 123,43%, gli utenti che depositano liquidità in questo pool verranno ricompensati con:

* 30% di WETH
* 20% di LINK
* 20% di WBTC
* 15% di USDT
* 15% di WMATIC

Farmando su DinoSwap, verrai pagato con token DINO, il cui prezzo è molto volatile. Su altri aggregatori come Adamant o Beefy, vedresti aumentare la tua posizione LP, mentre con Augury "proteggi" la tua posizione ottenendo token che hanno meno probabilità di avere una volatilità molto elevata. Lo svantaggio è che la tua posizione iniziale non crescerà nel tempo poiché il 100% delle ricompense DINO viene convertito nel set di token che compongono la ricompensa su Augury.

{% hint style="info" %}
Augury Finance utilizza 3 diversi livelli di "Infusion" che hanno commissioni di deposito e commissioni di performance differenti. Siete pregati di leggere attentamente il tipo di Infusion che si intende utilizzare e assicurarvi di comprendere il loro impatto sulla strategia di farm.
{% endhint %}

Nella nostra strategia, utilizzeremo la farm "tier2" USDT-UST che ricompensa gli utenti con un mix di WETH/WBTC/LINK/WMATIC/USDC, dato che Mai Finance propone 4 Vault per 4 dei 5 token che otterremo come ricompensa. Per massimizzare i nostri profitti, inseriremo AAVE tra le ricompense di Augury e i Vaults su Mai Finance poiché 3 dei 5 token che raccoglieremo possono essere depositati su AAVE.

![Farm di stable coin USDT-UST per la nostra strategia](<.gitbook/assets/image (31).png>)

### Curve

Curve è un progetto blue-chip che ricompensa gli utenti che depositano token blue-chip. La ricompensa è composta da token che vengono reinvestiti (autocompound), token WMATIC e token CRV, che tra l'altro sono 2 token utilizzabili come garanzia su Mai Finance.

Una delle cose più interessanti da notare su Curve e che sui suoi pool non è necessario depositare un importo esatto di ciascun token nella proporzione 50/50. Può invece essere fornito un singolo token e l'algoritmo che gestisce il pool regolerà automaticamente gli altri token vendendo una parte del deposito e acquistando gli altri token per mantenere il corretto rapporto.

Utilizzeremo il pool "atricrypto3" che accetta qualsiasi combinazione di WBTC/WETH/USDC/USDT/DAI e aggiungeremo a questo pool l'USDC che verrà generato dal pool su Augury.

![Dettaglio del pool atricrypto3 su Curve al Settembre 2021](<.gitbook/assets/image (32).png>)

### AAVE

Come accennato nel paragrafo su Augury, AAVE viene utilizzato per aggiungere una piccola ricompensa ai token farmati ​​su Augury prima di utilizzarli su Mai Finance. Invece di mettere i nostri WBTC, WETH e WMATIC direttamente su Mai Finance, depositeremo questi token su AAVE e utilizzeremo lo strumento di rendimento di Mai Finance per reinvestire automaticamente le ricompense di AAVE nei pool amToken e utilizzeremo il camToken come garanzia nei Vaults . 

Puoi ottenere maggiori dettagli su questa parte leggendo il tutorial [come far fruttare i tuoi token su AAVE](tutorial-di-polygon/come-far-fruttare-i-tuoi-token-su-aave.md).

![Ricompense per i depositi su AAVE al Settembre 2021](<.gitbook/assets/image (33).png>)

### Balancer

Balancer è un altro progetto di punta come Curve. Potrai depositare determinati token in pool composti da più di 2 token ma depositandone uno solo. Il pool viene automaticamente ribilanciato per ottenere una proporzione uguale dei token che compongono il pool.

Per la nostra strategia, utilizzeremo il pool WETH/BAL/Qi/MAI/USDC. Questo pool accetterà il token Qi che verrà raccolto dai Vaults su Mai Finance e ci ricompenserà con ulteriori Qi e token BAL che potremo depositare su Mai Finance nel Vault BAL, permettendoci di coniare più MAI e aumentare la nostra posizione nel farming su Augry.

![Pool di 5 token di Balancer al Settembre 2021](<.gitbook/assets/image (34).png>)

## Avvio del sistema

![](<.gitbook/assets/image (35).png>)

Quella che segue è una simulazione realizzata con un investimento iniziale di $1.000 di ETH che depositati nel Vault camWETH per prendere in prestito $500 di MAI, convertiti in $500 di USDT-UST. Questa simulazione presuppone le seguenti ricompense per le diverse piattaforme:

* USDT-UST APR del 22.53%
* amWBTC APR del 0.39%
* amWETH APR del 1.71%
* amWMATIC APR del 3.80%
* atricrypto3 APR del 3.86% reinvestito automaticamente, 13.09% WMATIC e 17.63% CRV
* Pool di 5 token Balancer con APR del 43.46% con rapporto BAL:Qi di 1:6
* APRs delle ricompense dei Vaults:
  * 23.28% per camWBTC
  * 21.52% per camWETH
  * 32.93% per camWMATIC
  * 24.51% per LINK
  * 116.71% per CRV
  * 62.38% per BAL

Questi APR sono tutti soggetti a modifiche e non è garantito che resteranno tali per un anno intero, tuttavia li prenderemo così come sono per questa simulazione in modo da avere un'idea del possibile APR complessivo del sistema. Al fine di "semplificare" ulteriormente la simulazione, non terremo conto delle variazioni di prezzo, né delle commissioni di transazione. 

Da notare inoltre che questa simulazione calcola le ricompese dei Vaults su Mai Finance e quelle di Balancer come se fossero reinvestite giornalmente anziché settimanalmente ma in realtà le piattaforme le distribuiscono settimanalmente direttamente al portafoglio degli utenti. Infine, per il bene di questa simulazione, assumeremo che il CDR (**C**ollateral to **D**ebt **R**atio) sia sempre del 200%, il che significa che stiamo prendendo in prestito solo la metà di ciò che abbiamo depositato, per continuare ad ottenere le ricompene ma prevenire facili liquidazioni.

### Giorno 1

Se hai ancora i tuoi $1.000 di WETH, depositali su AAVE per ottenere amWETH, quindi deposita i tuoi amWETH su [Mai Finance](https://app.mai.finance/yield) per ottenere camWETH e infine deposita i tuoi camWETH nel Vault corrispondente per poter prendere in prestito $500 di MAI.

Usa [anchor](https://app.mai.finance/anchor) per convertire i tuoi MAI in USDT (oppure puoi usare un altro DEX come [QuickSwap](https://quickswap.exchange/#/) se non c'è liquidità in anchor), successivamente puoi usare [DFYN](https://exchange.dfyn.network/#/) per swappare il 50% degli USDT in UST e poter creare la coppia USDT-UST da depositare su [Augury](https://augury.finance/infusions/). Nota che avrai anche bisogno di alcuni OMEN che puoi acquistare su QuickSwap.

Quindi, alla fine del Giorno 1, raccoglieremo le seguenti ricompense

| Tipo di ricompensa | Valore in dollari |
| ------------------ | ----------------- |
| WBTC dal farming   | 0.123             |
| WETH dal farming   | 0.031             |
| WMATIC dal farming | 0.031             |
| LINK dal farming   | 0.031             |
| USDC dal farming   | 0.092             |
| Qi dai vaults      | 0.295             |

Queste sono solo le ricompense che otterremo farmando e prendendo in prestito alla fine del primo giorno.

### Giorno 2

Le ricompense vengono riscattate, WBTC, WETH e WMATIC vengono depositati nei Vaults corrispondenti su Mai Finance dopo essere passati attraverso AAVE e la farm su Mai. I LINK vengono depositati direttamente nel Vault LINK e gli USDC depositati su Curve nel pool atricrypto3. La ricompensa Qi viene depositata su Balancer. A questo punto, possiamo prendere in prestito più MAI dai 3 depositi camToken e dal deposito LINK ($ 0,13 di MAI per l'esattezza) e usarli per aumentare la coppia USDT-UST attraverso i MAI che abbiamo preso in prestito.

Quindi, alla fine del Giorno 2, otterremo le seguenti ricompense:

| Tipo di ricompensa            | Valore in dollari |
| ----------------------------- | ----------------- |
| WBTC dal farming              | 0.123             |
| WETH dal farming              | 0.031             |
| WMATIC dal farming + Curve    | 0.031             |
| LINK dal farming              | 0.031             |
| USDC dal farming              | 0.093             |
| CRV di ricompense Curve       | 0.00004           |
| BAL dalle ricompense Balancer | 0.00005           |
| Qi dai Vaults                 | 0.296             |

A questo punto, il ciclo è innescato e le ricompense si muovono in modo tale che ogni passaggio alimenti il successivo, creando un "cerchio della vita" del farming.

## Risultati del Farming

###  Routine quotidiana

La routine quotidiana si compone delle seguenti transazioni:

* Riscattare le ricompense su Augury
* Depositare WBTC, WETH e WMATIC su AAVE
* Depositare amWBTC, amWETH e amWMATIC su Mai Finance nelle farm
* Depositare camWBTC, camWETH e camWMATIC nei rispettivi Vaults su Mai Finance
* Depositare LINK nel Vault LINK su Mai Finance
* Depositare USDC nel pool atricrypto3 su Curve
* Riscattare WMATIC da Curve e depositarli nel Vault camWMATIC
* Riscattare CRV da Curve e depositarli nel Vault CRV
* Prendere in prestito MAI dai vari Vaults
* Convertire i MAI in USDT su Mai Finance attraverso la sezione anchor
* Convertire il 50% degli USDT in UST su DFYN
* Creare la coppia USDT-UST LP su DFYN
* Depositare la coppia di tokens USDT-UST LP su Augury

### Routine Settimanale

Inoltre, riceveremo premi settimanali in BAL (dal tuo deposito di Qi su Balancer) e token Qi (dai premi del Vault). Dovremo:

* Depositare i token Qi su Balancer
* Depositare i token BAL su Mai Finance nel Vault BAL
* Prendere in prestito i MAI grazie al deposito addizionale di BAL e convertirli per creare la coppia USDT-UST pair to farm on Augury

### Risultati a grandi linee mese dopo mese

| Month | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| ----- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1     | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2     | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3     | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4     | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5     | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6     | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7     | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8     | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9     | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10    | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11    | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12    | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

Alcune note:

* La crescita del pool USDT-UST è il risultato degli ulteriori MAI presi in prestito dai Vaults
* Il pool CRV è quasi inesistente a causa della quantità molto bassa di USDC depositata su Curve
* Il Vault BAL non è importante a causa del fatto che il 14,28% della ricompensa di Balancer viene pagata in token BAL, il resto viene pagato in token Qi
* L'importo nel pool Balancer è quello che ha reso di più ed è il risultato delle ricompense Vault e delle ricompense Balancer

### Giorno 365

Dopo un anno intero, lo stato finale del nostro investimento sarebbe

| Posizione   | Valore in dollari |
| ----------- | ----------------- |
| USDT-UST    | 553.24            |
| atricrypto3 | 36.20             |
| Balancer    | 137.62            |
| camWBTC     | 47.45             |
| camWETH     | 1,029.19          |
| camWMATIC   | 14.39             |
| LINK        | 11.84             |
| CRV         | 0.017             |
| BAL         | 3.93              |

Il debito totale è in realtà l'intera posizione USDT-UST, quindi $553,24 e la ricompensa totale generata è $280,63, corrispondente a un APY finale del 28,06%.

### Comparazione con altre strategie

Ottenere un APY del 28% su stable coin non è niente male ma come si confronta con altre strategie più semplici che potremmo applicare con il valore iniziale di $1.000 di ETH? Controlliamo l'APY finale per le seguenti strategie

* Leva finanziare di amWETH x8 volte tramite AAVE: per questo, utilizzeremo il flusso esatto descritto nel tutorial [AAVE](tutorial-di-polygon/come-far-fruttare-i-tuoi-token-su-aave.md).
* Farming completamente di stable coin su Augury: per questa strategia, vendiamo WETH e farmiamo con $1.000 di USDT-UST sulla stessa "Infusion" su Augury
* Farming completamente di stable coin su QuickSwap: per questa strategia, utilizzeremo il Vault camWETH per beneficiare della ricompensa del Vault e farmeremo con $500 di MAI su QuickSwap (MAI-DAI al 19,78% APY), utilizzando il Vault dQUICK su Mai Finance per prendere in prestito MAI aggiuntivi e reinvestire nel pool di farm (vault dQUICK con un APR del 55,72%)

| Strategia                        | APY Finale |
| -------------------------------- | ---------- |
| Strategia presentata nella guida | 28.06%     |
| Leva finanziaria su AAVE x8      | 46.46%     |
| Solo stable farming su Augury    | 22.53%     |
| Quickswap farming + dQUICK vault | 35.96%     |

## Disclaimer

Questa strategia è davvero interessante e utilizza la maggior parte dei Vaults di Mai Finance ed è stata scritta principalmente per mostrare che, al Settembre 2021, genererebbe più ricompense usando stable coin. Tuttavia, questa strategia potrebbe non essere la più interessante e comporta molte operazioni che coinvolgono diverse piattaforme. Infine, Augury è uno strumento fantastico che genera token specifici che possono essere inclusi in diverse strategie ma forse meno indirizzato al farming di stable coin. Come nota a margine, non sono state prese in considerazione commissioni di deposito né commissioni di performance nel calcolo dell'APY finale.

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
