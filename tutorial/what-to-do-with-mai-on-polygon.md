---
description: Questo tutorial illustra le varie opzioni di utilizzo dei tuoi MAI su Polygon.
---

# Cosa fare con Mai su Polygon

## Obbiettivo di questo tutorial

L'obiettivo di questo tutorial non è presentare in dettaglio cosa puoi fare con la tua stable coin MAI ma avere un elenco di tutti i siti Web e applicazioni DeFi che puoi utilizzare su Polygon che ti permettano di utilizzare i tuoi MAI direttamente o in combinazione con altre stable coin. Per maggiori dettagli su modi specifici di utilizzare MAI, puoi fare riferimento ad altri tutorial su questo sito o ottenere aiuto su [Discord](https://discord.gg/aRghpvhV) o [Telegram](https://t.me/QiDaoProtocol).

Si prega di notare che l'elenco non è completo e non lo sarà mai poiché ci sono nuove dApp lanciate ogni settimana sulla rete. Non possiamo recensirle tutte quindi presenterò solo le opzioni principali, ovvero le opzioni più famose/più "sicure".

Se vuoi che un particolare progetto sia elencato, per favore unisciti alla comunità Qi su [Discord](https://discord.gg/mQq55j65xJ).

{% hint style="info" %}
Non presenterò le farm di Mai Finance. Questo argomento merita il suo tutorial, perché Qi non è come qualsiasi altro token farm.
{% endhint %}

## Farmare in sicurezza sui progetti maggiori \(bluechip\)

I progetti Bluechip sono le applicazioni DeFi che si sono dimostrate solide e presentano un rischio minore. Di solito sono controllati e il team di sviluppo ci ha lavorato per molto tempo. Di solito non hanno APR \(tasso percentuale annuo\) altissimi ma sono affidabili e sicure.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) è un gestore di portafoglio automatizzato, fornitore di liquidità e rilevatore di prezzi. Sulla piattaforma potrai prestare le tue crypto valute e riscuotere commissioni dai trader, che riequilibrano il tuo portafoglio seguendo opportunità di arbitraggio. Se hai bisogno di maggiori dettagli su Balancer, vai a leggere il [documento ufficiale](https://docs.balancer.fi/).

Sulla rete Polygon, Balancer propone un pool composto dalle 4 principali stable coin: DAI, USDC, USDT e MAI \(miMATIC\). Questo pool stabile ha attualmente un APR abbastanza stabile di ~ 20%.

![Stable coin pool state as of August 2021](../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)

La cosa più bella di Balancer è che non hai assolutamente bisogno di possedere le 4 monete da depositare nel pool. Balancer genererà automaticamente una combinazione bilanciata a prescidere dal  deposito effettuato. Ciò significa che se hai 100$ di MAI, puoi semplicemente depositarli nel pool di Balancer e lasciare che l'algoritmo lo coverta correttamente per avere un rapporto del 25% per ogni moneta a seconda del loro rispettivo prezzo al momento del deposito.

I premi per il pool vengono pagati utilizzando il token BAL, distribuito su base settimanale. Oltre al token BAL, possono essere concessi premi aggiuntivi a seconda del pool in cui hai depositato. Puoi controllare i differenti [programmi di incentivi qui](https://balancer-incentives.web.app/). Nel nostro caso, la partecipazione al pool stabile ti farà guadagnare anche premi MATIC e Qi.

Il ciclo completo può essere rappresentato così:

![](../.gitbook/assets/screen-shot-2021-08-11-at-11.34.45-am.png)

Se hai bisogno di maggiori dettagli su come utilizzare Mai Finance per depositare le tue crypto valute e prendere in prestito MAI \(invece di vendere le tue crypto valute per acquistare MAI\), leggi altre guide su questo sito. Puoi anche [includere Aave](https://app.gitbook.com/@qidao-qimps/s/mai-finance-tutorials/~/drafts/-Ml1OUN9zNLQIeHPCX6O/v/italian/tutorial/far-fruttare-i-tuoi-token-aave/@drafts) per generare ulteriori profitti.

### Curve finance

Un po' di click-bait qui. [Curve](https://polygon.curve.fi/) è un'altra piattaforma in cui potrai depositare le tue crypto valute  in pool che genereranno entrate ma non direttamente MAI \(non ancora?\). I pool che ci interessano sono:

* il pool AAVE che genera tra il 5% e il 15% APR \(APR molto variabile\) su un trio di stable coin \(DAI/USDC/USDT\). Il pool funziona esattamente come Balancer nel senso che puoi entrare nel pool utilizzando un singolo asset che verrà utilizzato su AAVE dal protocollo.
* il pool atricrypto  è composto dal trio di stable coin \(DAI/USDC/USDT\) e include anche wETH e wBTC per mitigare l'impermanent loss. Questo pool ha un APR compreso tra il 25% e il 30%. Il team di Mai Finance sta attualmente cercando di aggiungere MAI a questo pool, il che significa che potresti essere in grado di depositare direttamente i tuoi MAI.

In attesa che il protocollo Curve accetti MAI come stable coin valida nei propri pool, puoi comunque utilizzare la tua crypto valuta preferita con Curve seguendo questi passaggi \(esempio con MATIC\):

* Deposita i tuoi token MATIC su AAVE ed ottieni amWMATIC
* Deposita i tuoi amWMATIC su Mai Finance ed ottieni camWMATIC \(le ricompense AAVE saranno aggiunte ai token camWMATIC\)
* Usa i token camWMATIC come collaterale su Mai Finance e prendi in prestito MAI
* Usa la [pagina di swap](https://app.mai.finance/swap) su Mai Finance per scambiare tutti i tuoi MAI per USDC
* Ora puoi
  * Entrare nel pool di atricrypto su Curve con i tuoi USDC e ottenere un APR dal 25% al ​​30%
  * Entrare nel pool AAVE su Curve con i tuoi USDC e ottenere un APR dal 5% al ​​15%

Le ricompense su Curve sono date in:

* USDC automaticamente reinvestiti che accrescono la tua posizione nel pool \(sarà un mix di USDC/USDT/DAI e possibilmente wBTC/wETH nel caso del pool atricrypto\)
* WMATIC che puoi utilizzare per ripetere il ciclo di cui sopra e aumentare il tuo prestito e capitale investito
* CRV, che possono essere utilizzati anche come collaterale su Mai Finance per prendere in prestito più MAI e aumentare il capitale investito

![](../.gitbook/assets/screen-shot-2021-08-11-at-12.14.27-pm.png)

### AAVE

C'è una guida completa su come usare Mai Finance per [far fruttare i tuoi token su Aave](https://app.gitbook.com/@qidao-qimps/s/mai-finance-tutorials/~/drafts/-Ml1OUN9zNLQIeHPCX6O/v/italian/tutorial/far-fruttare-i-tuoi-token-aave/@drafts) This is not doing a direct use of MAI stable coin, but we can imagine that, in the future, AAVE will also have a MAI pool where you will be able to lend your crypto.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) is probably one of the most famous DEX \(Decentralized EXchange\) on Polygon with SushiSwap and 1Inch. It's also an AMM \(Automated Market Maker\) that allows users to efficiently trade on the Polygon network using liquidity pools. Any trade on the exchange is subject to a fee that is partially redistributed to users who deposit their liquidity on the platform.

The way you can use MAI on QuickSwap is very similar to a [regular yield farm](https://qidao-qimps.gitbook.io/mai-finance-tutorials/en-investment-tutorials/secure-your-yield-farming-profits) so if you need to get exact steps to enter the MAI/USDC pool on QuickSwap, it's probably better for you to read this article.

Currently, if you enter the MAI/USDC LP \(**L**iquidity **P**rovider\) pool on QuickSwap, you will earn

* trading fees
* QUICK tokens

![Details of the MAI/USDC pool on QuickSwap as of August 2021](../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

## Degen farms and aggregators

### Adamant

[Adamant](https://adamant.finance/home) is an aggregator that is listing all the "best" farms on Polygon and let you enter them directly from their website. By depositing your assets \(LP tokens\) on a specific pool on Adamant, the algorithms will harvest the rewards granted by the pool and automatically compound part of the reward into your LP position. The rest of the reward is usually converted in WMATIC that is then redistributed to the holders of the ADDY token \(native token of Adamant\). Finally, you get a reward in ADDY tokens as well that you can harvest and vest for 90 days, earning you part of the WMATIC dividends.

In general, Adamant is a good place to go if you don't really care about the farm token, and if you don't want to compound your rewards manually several times a day. It also generates more revenue since you get some ADDY rewards in addition to the reward granted by the pool.

Adamant currently supports a few pools that accept the MAI/USDC LP pair. The pools are on

* QuickSwap: QUICK reward is swapped into more MAI/USDC LP and WMATIC rewards
* DinoSwap: Dino reward is swapped into more MAI/USDC LP and WMATIC rewards
* Mai Finance: Qi reward is swapped into more MAI/USDC LP and WMATIC rewards

![QuickSwap MAI/USDC pool on Adamant](../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)

{% hint style="info" %}
The screenshots of the QuickSwap pool on QuickSwap website \(see paragraph above\) and Adamant have been taken the same day, but are showing different APYs \(**A**nnual **P**ercentage **Y**ield\).
{% endhint %}

You can see that the APY on Adamant is a little bit higher than on QuickSwap directly. The reward breakdown is as follows

* 12.88% Auto-compounded QUICK \(meaning the QUICK reward is transformed into more LP tokens\)
* 9.16% ADDY reward \(not compounded\)
* 3.40% fee share dividend \(claiming ADDY daily\)

This means that, out of the 20.92% granted by QuickSwap, only 12.88% is used to increase your LP position, the rest is swapped into WMATIC dividends. You will be able claim your ADDY reward daily \(or anytime\) and stake them, which will will in turn generate claimable WMATIC dividends. In other words, Adamant _seems_ a better option because it has better APYs and compound rewards automatically, but in reality it involves a lot of manual actions too.

{% hint style="info" %}
Using Adamant also has a strong impact of native token prices. Indeed, because Adamant is constantly selling the farm tokens to generate more LP pairs and WMATIC as dividends to their ADDY holders, the sell pressure is very high on farm tokens and can explain why their price is consistently decaying.
{% endhint %}

### Other farms accepting MAI/USDC LP pair

MAI getting more and more popularity on Polygon, and because QuickSwap supports the MAI/USDC pair, a lot of farms are now supporting it too. The following list will present a few projects on which you can earn yield using MAI/USDC

* DinoSwap
* Augury
* Polypup
* ...

Other farms may also accept the MAI/USDC pool. If you want to stay informed about new farms and their launch date, I strongly recommend taking a look at the [RugDoc.io calendar](https://rugdoc.io/calendar/) for Polygon farms, and possibly to the rest of their website which will present a very smart overview of each farm, as well as their potential risks.

## Impermax

### A little bit of explanation

[Impermax](https://polygon.impermax.finance/) is a platform that let users leverage their LP tokens for higher yields. The goal is very simple: by providing LP tokens and using them as collateral, one can then borrow more of the 2 underlying assets to generate more LP tokens and repeat the loop.

![Impermax loop explained](../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)

When doing so, the user is exposed to impermanent loss, and the loss is magnified by the number of times the loop is repeated. The risk of liquidation is also multiplied when too many loops are applied. Indeed, if the APR is multiplied, the price variation of the two coins forming the pair is amplified by the lever effect, leading to faster liquidation.

With stable coins, the risk of liquidation is lower though, because the price variation is negligible. This also means that the Collateral to Debt Ratio \(CDR\) can be very close to 100%, leading to a high number of loops, hence a high APR.

Note that Impermax is charging fees when you borrow and leverage your position. The fee corresponds to 0.1% of your final position. As an example, if I have $100 worth of MAI/USDC and I leverage 50x, my final position will worth $5,000 and I will pay a $4.90 fee corresponding to the $4,900 that I borrowed.

The effect of looping the lending/borrowing combination allows to multiply the final APY. With an initial APY of 20% for MAI/USDC pair with a CDR of 110%, operating the loop 50 times, and using the formula

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

We can easily get a 228% final APR. There are some other elements that will affect the final APR, namely the borrowing APR \(loan interest for borrowing more LP tokens\), and the supply/demand of both assets composing the LP pair \(directly driving the borrowing APR\).

Also, because all the rates are magnified by the number of times the loop is applied, the APR will vary drastically, and can sometimes become negative for short amount of times \(your LP token will be used to repay the negative APR\).

### Leveraged position of my MAI/USDC pair

In the end, you are using the base APR on a much bigger value, which is earning much bigger interests, increasing the APR of your initial position.

![An example of Impermax dashboard with an initial $70.52 MAI/USDC pair](../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)

I can see very easily how much I'm using as collateral, how much I initially invested, what's the leverage ratio, and what are the liquidation values due to the leverage ratio. This position will give me the following ratios at the time of writing

![Earnings and spendings estimation at a given time](../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)

The APR is granted in IMX token that can either be swapped for more MAI/USDC \(use the power of Mai Finance to borrow at 0% interest, RFTM\), or used to provide liquidity on specific pools accepting IMX on Impermax.

### Supplying MAI to borrowers

Indeed, on the app you can also provide liquidity to those who want to apply leveraging loops to their positions \(they will need underlying assets to generate more LP tokens\). Lending assets is a great way to earn yield and let the borrowers take all the risks. Also, the more users are borrowing, the higher the supply APR will be.

![Rates for supplying and borrowing MAI on Impermax at a given time](../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)

This is another great way to optimize your 0% loan on Mai Finance. Not only you don't have to pay anything to borrow MAI, but you can earn a lot of interest just by depositing it on Impermax.

## Disclaimer

Everything is this tutorial is purely educational. The goal is to bring light to projects that I think are worthy for people evolving in the crypto world on Polygon. I obviously didn't talk about Mai Finance as a farm because a dedicated tutorial will be written very soon. Finally, this guide is ABSOLUTELY NOT meant to be applied as is, it's not any financial advice and you should not follow blindly what I wrote. Please read the docs of the different projects I mentioned before considering investing on their platforms.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly \(or make you lose money\) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

