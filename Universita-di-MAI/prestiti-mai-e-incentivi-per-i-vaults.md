---
description: >-
  Questo articolo è una spiegazione dettagliata di come è possibile utilizzare
  Mai Finance per prendere in prestito MAI a interesse 0% ed essere pagati per
  farlo, con interesse negativo.
---

# Prestiti MAI e incentivi per i Vaults

## Introduzione

Il core business di Mai Finance è la piattaforma di prestito. Invece di vendere le loro crypto valute per acquistare altri assets, le persone sono in grado depositarle su Mai Finance e prendere in prestito usandole come garanzia. Ciò offre l'opportunità di mantenere assets di alto valore (WBTC, WETH ...) pur essendo in grado di ottenere altri assets e rendimenti da farm. Così il prestito viene utilizzato per generare entrate, mentre il collaterale a garanzia acquisisce valore.

Uno degli altri grandi vantaggi dell'utilizzo di Mai Finance è che non esiste un programma di rimborso. In altre parole, prendi in prestito stable coin MAI usando la tua crypto valuta come garanzia, non paghi alcun interesse e puoi ripagare il tuo debito quando vuoi. Vedi i diversi articoli sulla [gestione del debito](rimborso-del-debito-perche-e-quando.md) per ulteriori dettagli. L'unica commissione che pagherai a MAI è una commissione di rimborso corrispondente allo 0,5% del valore che hai preso in prestito, che paghi quando rimborsi il prestito e che viene detratta dalla tua garanzia.

Ad esempio, se hai depositato $200 di WETH per prendere in prestito $100 di MAI, quando ripagherai il tuo prestito dovresti pagare una commissione di $0,50 che verrà prelevata direttamente dal tuo deposito WETH.

Se questa non fosse già una straordinaria opportunità, il team di Mai Finance ha introdotto nel Settembre 2021 gli incentivi per i Vault pagati in Qi, il token nativo di Mai Finance. In altre parole, depositando i tuoi assets su Mai Finance in un Vault potrai prendere in prestito MAI e verrai anche pagato per farlo. Questo articolo presenta in dettaglio come funziona questa funzionalità.

## Vaults - Cosa sono e come funzionano

### Creazione del Vault

Su Mai Finance, i Vault sono casseforti speciali in cui è possibile depositare i propri assets. Attualmente, ci sono 10 tipi di Vault:

![I vari vault che è possibile creare su Mai Finance](<../.gitbook/assets/image (1).png>)

Ci sono 2 tipi differenti di Vaults:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

e

* camWETH
* camWBTC
* camWMATIC
* camAAVE

I primi 6 depositi nell'elenco sono per assets semplici mentre gli ultimi 4 sono per camToken. I camToken auto reinvestono i token di mercato AAVE sono la rappresentazione di un deposito che avresti potuto fare su AAVE a sua volta depositato nei pool di rendimento di Mai Finance. Mentre i tuoi assets generano rendimenti su AAVE (e mentre le ricompense vengono automaticamente reinvestite nel pool di rendimento), puoi comunque prendere in prestito la stable coin MAI usandoli come garanzia.

Come nota a margine, puoi vedere nello screenshot qui sopra che la pagina di creazione mostra alcune informazioni molto importanti:

* MAI available: questo corrisponde al tetto massimo del debito, il numero massimo di MAI che possono essere coniate dai depositi nei Vault.
* Min Coll. ratio: questo è il Collateral to Debt ratio (CDR) minimo per il vault
* Vault Incentives APR: è l'APR delle ricompense

### Capire il tetto massimo di debito

Il numero massimo di MAI che si può generare in un vault specifico dipende da quanti assets sono depositati nello stesso. I massimali di debito sono implementati per assicurarsi che il mercato non sia invaso da MAI in un tempo molto breve, che potrebbe influenzare il prezzo della stable coin.

Ad esempio, se un investitore istituzionale depositasse 5.000 WBTC in una volta sola e fosse in grado di prendere in prestito $100.000.000 di MAI, scambiandoli tutti con più WBTC, questo potrebbe far scendere il prezzo di MAI così tanto che il prezzo si discosterebbe troppo dal suo ancoraggio, mettendo a rischio l'intera piattaforma. Il tetto del debito è il meccanismo che impedisce che ciò accada: c'è una quantità massima di MAI che può essere coniata per un determinato tipo di Vault.

Quando viene raggiunto il tetto del debito, viene registrato il momento in cui non ci sono più MAI disponibili da coniare e il sistema aumenta automaticamente il tetto del debito dopo 48 ore. Questo è considerato un tempo sufficiente per la stabilizzazione del prezzo di MAI (in caso di alta pressione di vendita a seguito di una grande vendita di MAI).

Questo significa che per 48 ore nessuno sarà in grado di prendere in prestito più MAI da un Vault che ha raggiunto il suo tetto massimo di debito, a meno che dei debiti non vengano rimborsati.

Come nota a margine, più MAI sono sul mercato, più stabile è il prezzo. In effetti, una vendita massiccia di MAI avrà un minor impatto se ci sono più MAI in circolazione.

* Se qualcuno vende 1.000 MAI mentre ci sono solo 10.000 MAI in circolazione, la vendita corrisponde al 10%
* Se qualcuno vende 1.000 MAI mentre ci sono 10.000.000 MAI in circolazione, la vendita corrisponde allo 0.01%

Il tetto del debito non viene aumentato in modo incrementale ma esponenziale: più MAI sono in circolazione minore sarebbe l'impatto che avrebbe una grande vendita, di conseguenza il tetto del debito potrà essere aumentato sempre di più.

{% hint style="info" %}
Quando prendi in prestito MAI, può succedere che l'importo massimo di MAI che puoi prendere in prestito sia limitato dal tetto del debito, indipendentemente dal valore corrente della tua garanzia e dall'importo corrente di MAI che hai già preso in prestito. In tal caso, puoi attendere 48 ore prima di poter effettivamente prendere in prestito più MAI.
{% endhint %}

### Capire il rapporto Collaterale - Debito

Il CDR o **C**ollateral to **D**ebt **R**atio è il rapporto tra il valore degli assets depositati nel Vault rispetto all'importo di MAI che hai preso in prestito.&#x20;

Ad esempio, se hai depositato $200 di WETH per prendere in prestito $100 di MAI, il tuo CDR sarebbe

$$
CDR=\frac{ValoredelCollaterale}{Valore del Debito}=\frac{200}{100}=200\%
$$

Mantenere un CDR superiore al 100% significa che, in qualsiasi momento, le garanzia sono superiori al debito. Questo è obbligatorio per garantire che la stable coin MAI sia sovra-collateralizzata ed è uno dei fondamenti della tokenomics di Mai Finance. Puoi ottenere maggiori dettagli in merito nella [Documentazione ufficiale Mai Finance](https://docs.mai.finance/stablecoin-economics).

Ogni tipo di Vault ha un rapporto CDR minimo accettato, al di sotto del quale il deposito è considerato a rischio perché l'importo preso in prestito non sarebbe coperto da collaterali a sufficienza. A questo punto chiunque può liquidare il Vault, il che significa che una parte del debito viene rimborsata dal liquidatore che può poi ottenere in rimborso una parte dei collaterali depositati. Ancora una volta, puoi trovare maggiori dettagli sul processo di liquidazione nella documentazione ufficiale.

Quando prendi in prestito MAI a fronte di un determinato collaterale, riceverai alcuni suggerimenti su qual è l'importo massimo di MAI che puoi prendere in prestito e quale sarebbe l'impatto sullo "stato di salute" del tuo Vault a seconda dell'importo preso in prestito, come puoi vedere nello screenshot qui sotto:

![Stato di salute del Vault a seconda dell'importo preso in prestito](<../.gitbook/assets/image (2).png>)

È molto importante tenere d'occhio il tuo CDR e mantenere un rapporto debito/collaterale sano per:

* evitare di essere liquidati
* contribuire alla salute dell'intera piattaforma Mai Finance assicurando che il volume MAI in circolazione sia adeguatamente supportato

Il CDR "sano", come definito dal team di Mai Finance, è compreso tra il 25% e il 270% oltre al valore CDR minimo. Come nota a margine, puoi anche controllare le nostre guide strategiche per vedere come puoi essere più conservativo/aggressivo nell'operare in altri progetti o [ripagare il tuo debito](../tutorial/polygon/come-far-fruttare-i-tuoi-token-su-aave.md#esempio-con-numeri) facendo rendere il tuo prestito.

## Incentivi per i Vaults

### Capire gli incentivi per i Vaults

Nel settembre 2021, Mai Finance ha introdotto gli incentivi per i Vaults. Si tratta di una ricompensa assegnata dalla piattaforma Mai Finance a chiunque prenda in prestito MAI e partecipi alla crescita della piattaforma.&#x20;

Ogni tipo di Vault (tra i 10 disponibili) riceve 0,05 Qi per blocco, che viene poi distribuito tra tutti gli utenti che hanno un buon rapporto Collateral to Debt. L'APR del Vault è definito dall'importo corrente di MAI preso in prestito.&#x20;

Ad esempio, Ben e Kila sono 2 amici che hanno depositato i loro ETH nei Vault WETH su Mai Finance.

* Ben ha depositato l'equivalente di $2,000 in ETH e preso in prestito 1,000 MAI
* Kila ha depositato l'equivalente di $10,000 in ETH e preso in prestito 6,000 MAI

L'importo attuale di MAI presi in prestito dagli utenti che hanno depositato WETH nei Vault è 1,000,000 MAI.

Sia Ben che Kila sono idonei agli incentivi del Vault perché Ben ha un CDR di 200% e Kila ha un CDR del 166.67%. Ben, col suo prestito, ha lo 0.1% del totale dei prestiti, mentre Kila ha lo 0.6%.

La quantità totale di Qi assegnata al Vault WETH (o a qualsiasi Vault) è:

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86.400 è il numero di secondi in un giorno e su Polygon il tempo per blocco è di 2 secondi, il che significa che il numero previsto di blocchi ogni giorno è 86.400 / 2 = 43.200. Quindi, l'emissione per ogni Vault è di 2.160 Qi/giorno.

**Nota:** Il tempo per blocco è aumentato ultimamente ed è di circa 2,6 secondi. Tuttavia, tutti gli APR e APY visualizzati su tutte le app presuppongono un tempo per blocco di 2 secondi. Per favore DYOR e controlla il tempo per blocco attuale su [PolygonScan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Quindi, se lo stato del Vault rimane lo stesso, Ben riceverà lo 0,1% dei 2.160 Qi distribuiti mentre Kila riceverà lo 0,6%.

* Ben otterrà 2.16 Qi giornalieri, una ricompensa giornaliera del 0.216%, o un APR del 78.84%
* Kila otterrà 12.96 Qi giornalieri, una ricompensa giornaliera del 0.216%, o un APR del 78.84%

Come nota a margine, 2.160 Qi per 1.000.000 MAI è una ricompensa giornaliera dello 0,216% o del 78,84% ovvero l'APR del Vault.

{% hint style="info" %}
È facile notare che l'APR del Vault è direttamente collegato all'importo dei MAI presi in prestito. Più MAI vengono presi in prestito, più basso è l'APR. Come nota a margine, l'importo di MAI che può essere preso in prestito è anche limitato dal tetto massimo di debito, che viene aumentato con la domanda di MAI.
{% endhint %}

Come ulteriore verifica possiamo calcolare l'APR teorico per il Vault MATIC in base ai numeri pubblicati sull' [analytics page](https://app.mai.finance/analytics) di Mai Finance. L'importo dei MAI presi in prestito dal Vault MATIC è 799.328. La ricompensa è di 216 Qi al giorno per quel Vault. Ciò corrisponde ad un APR del:

$$
APR=\frac{QiRicompense*Qi_{Prezzo}}{MAI_{inprestito}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

Questo corrisponde più o meno all'APR del Vault MATIC, come mostrato nello screenshot seguente:

![APR del Vault MATIC su Mai Finance dopo il lancio degli incentivi Vault](<../.gitbook/assets/image (23) (2) (3) (3).png>)

### Calcolare gli APRs dei Vault disponibili

Con gli stessi dati dell'esempio sopra è possibile calcolare gli APR di partenza per tutti i depositi

| Tipo di Vault |  APR di partenza |
| ------------- | ---------------- |
| MATIC         | 44.29%           |
| WETH          | 24.03%           |
| LINK          | 27.41%           |
| AAVE          | 164.14%          |
| CRV           | 159.96%          |
| WBTC          | 36.92%           |
| camWETH       | 25.46%           |
| camWMATIC     | 44.33%           |
| camAAVE       | 167.23%          |
| camWBTC       | 47.38%           |

{% hint style="info" %}
Come puoi vedere, alcuni depositi genereranno più ricompense di altri. Inoltre, puoi vedere che è molto importante depositare i tuoi assets il prima possibile per beneficiare di un APR elevato prima che il tetto del debito venga alzato e che venga preso più prestito (abbassando l'APR).

Puoi anche notare che se mantieni il tuo prestito per un anno o più, la commissione di rimborso dello 0,5% sarà facilmente compensata dal programma di ricompensa.
{% endhint %}

### Distribuzione degli incentivi

Le ricompense assegnati dagli incentivi del Vault saranno distribuite allo stesso modo del Qi messi in stake. Ogni mercoledì, le ricompense in Qi per gli incentivi Vaults della settimana conclusa saranno saranno inviati ai rispettivi portafogli.

## FAQs sugli incentivi per i Vaults

Se vuoi saperne di più sul modo in cui funzionano gli incentivi per i Vault, ecco una FAQ ufficiale dal server [Discord](https://discord.gg/aRghpvhV).

* **Quali Vaults riceveranno ricompense?**

In questo momento a tutti i tipi di Vaults sono state assegnate ricompense Qi

* **Quante ricompense vengono date per gli incentivi al prestito?**

0.05 Qi/blocco per ogni tipo di Vault

*   **Quanti MAI devo prendere in prestito per guadagnare ricompense?**

    Per gli incentivi al prestito dei Vault, devi restare tra il 25% e il 270% sopra al rapporto di liquidazione per essere idoneo a ricevere le ricompense in token QI. Questo significa:
* _Matic_ - Rapporto di liquidazione minimo 150% - Idoneo agli incentivi con rapporto tra il 175% e 420%
* _Tokens_: - Rapporto di liquidazione minimo 130% - Idoneo agli incentivi con rapporto tra il 155% e 400%&#x20;
* _CamTokens_: - Rapporto di liquidazione minimo 135% - Idoneo agli incentivi con rapporto tra i 160% e 405%
*   **Come posso vedere se il mio Vault sta guadagnando ricompense?**

    Se vedi l'emoji del fuoco nella pagina della panoramica del Vault, significa che il Vault sta guadagnando ricompense
* **Quanto guadagnerò?**

La tua percentuale delle ricompense si basa sulla percentuale di MAI che hai preso in prestito rispetto all'importo totale di MAI presi in prestito da quel tipo di Vault.

* **Quanto dureranno questi incentivi?**

La durata prevista del programma di incentivi al prestito è di 3 mesi. La DAO può votare per interrompere gli incentivi prima della fine dei 3 mesi o votare per estendere il programma.

* **Come otterrò le ricompense?**

Qi saranno airdroppati direttamente ai portafogli dei Vault idonei.

* **Come viene estrapolata l'idoneità alle ricompense?**

L'idoneità alle ricompense viene calcolata per blocco. Guadagnerai ricompense per i blocchi in cui avevi aderito durante la settimana.

* **Quando iniziano il monitoraggio delle ricompense per la settimana?**

Seguiremo lo stesso programma di eQi. Puoi trovare i numeri dei blocchi nella pagina [Boost](https://app.mai.finance/boost).

## Disclaimer

Questa guida è stata scritta **prima** del lancio degli incentivi per i Vault, il che significa che gli APR mostrati in questo documento sono soggetti a modifiche e/o potrebbero non essere accurati. L'importo dei MAI presi in prestito, il tetto del debito e il valore del token Qi influiranno notevolmente sull'APR finale di ciascun tipo di Vault. Per favore, assicurati di investire in modo responsabile.

{% hint style="info" %}
Tieni presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farti perdere denaro) in un altro. Tieniti aggiornato, monitora i mercati, tieni d'occhio i tuoi investimenti e come sempre, fai le tue ricerche.
{% endhint %}
