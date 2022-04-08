---
description: >-
  Questa guida propone un'analisi completa delle diverse opzioni di leva
  proposte da Mai Finance su Fantom, utilizzando i vault Yearn e i vault Beefy.
---

# Come far fruttare i tuoi token su Fantom

## Introduzione

Mai Finance ha lanciato la sua piattaforma di prestito su Fantom con diversi tipi di Vaults, consentendo la possibilità di coniare la stable coin $MAI in base agli assets che depositerai.            Il principio è che potrai tenere le tue crypto valute e beneficiare del loro valore e contemporaneamente acquistare altre coin e farmare con APR elevati. Usare il tuo prestito per acquistare lo stesso asset che hai già depositato viene definito far fruttare i tuoi token. Ti mostreremo i vantaggi di questa strategia utilizzando 2 diverse piattaforme di prestito su Fantom per sfruttare i nostri token $DAI.

## Mettere in leva i token di un vault Yearn

### Depositare i tuoi assets su Yearn Finance

[Yearn Finance](https://beta.yearn.finance/#/home) è un insieme di protocolli su Ethereum Mainnet ed altre blockchain che consentono agli utenti di ottimizzare i propri guadagni sulle crypto valute attraverso servizi di prestito e trading. Su Fantom, il prodotto che utilizzeremo sono i Vaults. Questo è uno strumento in cui potrai depositare token singoli e ottenere rendimenti su questo deposito. Come certificato di deposito, riceverai un $yvToken. Nel nostro caso, depositeremo $DAI e riceveremo in cambio $yvDAI.

![Vaults Yearn su Fantom](../../.gitbook/assets/ftm-leverage-yv1.png)

{% hint style="info" %}
Il sito Yearn finance è ancora in modalità beta su Fantom. Il team sta ancora lavorando sulla piattaforma e gli APR/APY non vengono visualizzati. Se vai alla scheda Iron Bank, che è il protocollo di deposito/prestito sulla piattaforma, vedrai che il prestito di $DAI sta ottenendo \~ 8% di APR. Si prega di investire a proprio rischio.
{% endhint %}

### Depositare il tuo yvToken su Mai Finance

Una volta depositati i tuoi $DAI su Yearn Finance, dovresti avere $yvDAI nel tuo portafoglio. Questo è ciò che chiamiamo un token con rendimento: è un token che non ha alcun valore di per sé ma certifica la tua quota di un pool in cui i tuoi assets stanno guadagnando e in cui i premi vengono automaticamente reinvestiti. In altre parole, $DAI non cambia di valore perché è ancorato al dollaro USA ma il valore sottostante del tuo token $yvDAI aumenta.

Mai Finance accetta molti token con rendimento come garanzia, incluso $yvDAI. Ora puoi depositare questo token e prendere in prestito $MAI.

![Depositare il tuo yvToken su Mai Finance](<../../.gitbook/assets/ftm-leverage-yv2 (1).png>)

Il Vault $yvDAI ha una soglia di liquidazione del 110%, questo significa che puoi prendere in prestito $MAI con un rapporto tra il valore della tua garanzia e il valore del debito che non può scendere sotto il 110%. Attenzione, il 110% è effettivamente il rapporto raggiunto il quale il tuo Vault verrà liquidato. È necessario mantenere il rapporto al di sopra di questa soglia minima. Dato che $DAI non varia molto nel prezzo (meno di qualche centesimo in più o in meno) è possibile restare relativamente sicuri con un CDR (**C**ollateral to **D**ebt **R**atio) del 115%, ma sei libero di tenerlo più alto se preferisci.

Come sempre, per calcolare il valore del prestito che possiamo ottenere in base al valore del nostro collaterale a garanzia e al CDR target che vogliamo ottenere, utilizzeremo la seguente formula:

$$
MAI_{disponibile} = \frac{Collaterale_{valore} - Debito_{valore} * Target_{CDR}}{Target_{CDR}}
$$

​Con un valore del collaterale di $100 e nessun debito, se vogliamo mantenere un CDR sano del 115% possiamo prendere in prestito fino a

$$
MAI_{disponibile}=\frac{100-0*1.15}{1.15}=86.95
$$

Ora sei in una posizione in cui hai i tuoi guadagni $DAI in un Vault Yearn e hai anche alcune stable coins $MAI pronte per l'uso. Dato che vogliamo sfruttare la nostra posizione $DAI, scambieremo i nostri $MAI con più $DAI.

### Scambiare i tuoi $MAI su BeethovenX

Su Fantom, la principale fonte di liquidità per $MAI è [BeethovenX](https://app.beets.fi/#/trade). Questo è il protocollo principale in cui potrai scambiare i tuoi token $MAI con più $DAI, per eseguire la nostra strategia.

![Swap di $MAI per $DAI](../../.gitbook/assets/ftm-leverage-yv3.png)

Questo è l'ultimo passaggio del nostro ciclo. Ora che hai più $DAI puoi depositarli nel Vault Yearn e ripetere il ciclo. In questo modo aumenta la quantità di assets che hai nel Vault di Yearn, il che significa che raccoglierai più ricompense prestando i tuoi $DAI su quella piattaforma. L'APR/APY rimane lo stesso, ma poiché hai più assets, guadagni più rendimento e se confrontato con il tuo investimento iniziale, il tuo APR aumenta. Se vuoi avere ulteriori esempi sull'APR che puoi ottenere usando i loop yvDAI, leggi il nostro [Strategia camDAI per principianti](../../polygon-tutorials/camdai-beginner-strategy.md#main-strategy) per Polygon che utilizza la stessa identica strategia ma strumenti diversi.

{% hint style="success" %}
BeethovenX è in realtà una fantastica opportunità per fare farming con i tuoi $MAI presi in prestito. Deposita semplicemente i tuoi $MAI nel pool $MAI-$DAI-$USDC (APR di \~ 30% a partire da novembre 2021) se non puoi ottenere un APR migliore utilizzando il loop.
{% endhint %}

$$
MAI_
$$

## Far fruttare i tuoi mooScreamTokens su Mai Finance

### Depositare i tuoi assets su Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) è una piattaforma decentralizzata Multi-Chain di ottimizzazione dei rendimenti che consente ai suoi utenti di guadagnare interessi composti sulle loro crypto valute. In altre parole, puoi depositare alcuni assets o token LP da altre piattaforme su Beefy Finance e lasciare che il compounder automatico raccolga i token della farm e li reinvesta in più assets / token LP depositati. Per il nostro esempio, utilizzeremo singoli depositi $DAI su Beefy e useremo [Scream](https://scream.sh/lend) come piattaforma sottostante. Scream è un fork di Compound sul network Fantom su cui potrai prestare i tuoi asset e ottenere il token $SCREAM. Beefy venderà quindi i token $SCREAM per più $DAI.

Per depositare i nostri $DAI, visiteremo l'app Beefy Finance e selezioneremo Scream come piattaforma su cui farmare. Puoi anche aggiungere il filtro $DAI per vedere il deposito $DAI diretto.

![Deposito dei tuoi $DAI su Beefy utilizzando Scream](../../.gitbook/assets/ftm-leverage-beefy1.png)

Come puoi vedere, Beefy sta già dando un incredibile APY sui singoli depositi $DAI. Una volta depositato $DAI su Beefy, dovresti avere una prova di deposito nel tuo portafoglio sotto forma di token $mooScreamDAI. Come il token $yvDAI, il token $mooScreamDAI è un deposito con rendimento, il che significa che il tuo asset è ancora utilizzato su Scream e auto reinvestito su Beefy, generando ulteriori rendimenti. Ma sarai in grado di utilizzare questo token su Mai Finance per prendere in prestito $MAI.

### Depositare i mooScreamToken su Mai Finance

Una volta depositato il tuo $DAI su Beefy, dovresti avere $mooScreamDAI nel tuo portafoglio. Puoi utilizzare esattamente gli stessi passaggi della strategia Yearn Vault, l'unica differenza è che il rapporto di liquidazione minimo di $mooScreamDAI è del 135%. Dato che $DAI è una stable coin, è ancora possibile prendere in prestito $MAI e mantenere un CDR molto vicino al limite di liquidazione. Per il nostro esempio, punteremo a un CDR del 140% e con la stessa formula di cui sopra, possiamo calcolare la quantità di $MAI che possiamo coniare con 100$ di $DAI.

$$
MAI_{disponibile}=\frac{100-0*1.4}{1.4}=71.43
$$

​Dato che stiamo prendendo in prestito meno, potremo eseguire meno loop e l'APY equivalente finale sarà inferiore, tuttavia questa è ancora una strategia per principianti piuttosto buona.

Il resto del ciclo è lo stesso di yvDAI, il che significa che dovrai scambiare i tuoi $MAI con $DAI su BeethovenX e ripetere finché non sei soddisfatto.

## Alcune considerazioni sulle strategie in leva

Mettere in leva $DAI è considerata una strategia per principianti, nel senso che presenta pochissimi rischi (stai lavorando con stable coin) e puoi ottenere dei buoni rendimenti utilizzando al massimo 3 protocolli. Tuttavia, c'è ancora qualche rischio.

### Rischio di liquidazione

Più cicli eseguirai, maggiore sarà il rischio di liquidazione. Infatti, anche una piccola variazione del prezzo $DAI sarà amplificata dalla leva che hai applicato e anche se mantieni un CDR 5 punti al di sopra del rapporto minimo di liquidazione, il tuo Vault può essere a rischio. È sempre una buona idea interrompere i cicli di leva finanziaria nel momento in cui depositi i tuoi assets su MAI Finance e non prendere in prestito $MAI aggiuntivo per mantenere un CDR migliore.

Inoltre, in caso di liquidazione, dato il tuo Vault su MAI Finance contiene molti più assets, una liquidazione avrà anche un impatto maggiore rispetto al non aver fatto leva sulla tua posizione, semplicemente perché anche il debito che devi rimborsare è più grande.

### Rischio Tecnologico

Se usi molti protocolli, devi assicurarti che questi protocolli siano sicuri. In effetti, nella nostra strategia di leva finanziaria, se un singolo protocollo viene violato, l'intera strategia potrebbe crollare. Assicurati di fare le dovute ricerche prima di investire in progetti DeFi.

### Raggiungere il tetto di debito

Dato che queste strategie sono facili da impostare e presentano rischi bassi, c'è una domanda molto alta. Tuttavia, avrai sicuramente notato che nel processo di leva finanziaria, il $MAI preso in prestito viene scambiato con $DAI (o altri token). Se viene venduto troppo $MAI su Beethoven, il suo prezzo diminuirà lentamente e c'è il rischio che $MAI perda il suo peg, il che è piuttosto negativo per una stable coin. Per lasciare che il prezzo si stabilizzi, Mai Finance ha messo in atto diversi meccanismi di sicurezza e il più importante è il tetto del debito per ogni Vault.

Il tetto del debito rappresenta il numero massimo di $MAI che può essere coniato per un determinato Vault. Una volta raggiunto il massimale, non è più possibile prendere in prestito $MAI. Successivamente il core team responsabile di Mai Finance può decidere di aumentare il tetto o aspettare un po' di più per stabilizzare il prezzo di $MAI.

Puoi verificare in ogni momento la quantità di $MAI che può essere coniata nella [pagina di creazione del Vault](https://app.mai.finance/vaults/create), potrai quindi vedere subito quando non ci sono più $MAI coniabili e vedrai il seguente messaggio di errore:

![Messaggio di errore quando il tetto del debito è stato raggiunto](../../.gitbook/assets/ftm-leverage-error.png)

Questo messaggio di errore apparirà anche se il tuo fattore di salute è corretto. Nella maggior parte dei casi, l'unica soluzione è aspettare che il tetto venga aumentato. Tieni d'occhio Twitter o Discord per sapere quando succede.

## Disclaimer

Questa guida presenta alcuni dei modi in cui puoi utilizzare i tuoi assets su Fantom e includere Mai Finance nella tua strategia per aumentare i rendimenti. Tuttavia, come al solito, questo tutorial non è un consiglio finanziario e dovresti sempre fare le tue ricerche prima di applicare una strategia di investimento e investire in modo responsabile.

Tieni inoltre presente che questa soluzione potrebbe non essere la strategia migliore a seconda di quando prevedi di utilizzarla. Abbiamo appena evidenziato che BeethovenX ha APR piuttosto interessanti per i tuoi $MAI e puoi anche usare Beefy Finance per combinare i premi $BEETS in monete più stabili.

{% hint style="info" %}
Tenete presente che una strategia che funziona bene in un dato momento potrebbe avere un rendimento peggiore (o farvi perdere denaro) in un altro. Tenetevi aggiornati, monitorate i mercati, tenete d'occhio i vostri investimenti e come sempre, fate le vostre ricerche.
{% endhint %}
