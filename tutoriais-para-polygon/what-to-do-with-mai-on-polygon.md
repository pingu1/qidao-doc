---
description: >-
  Este tutorial irá te mostrar as diferentes maneiras de como utilizar o seu
  novíssimo MAI, na Polygon.
---

# O que fazer com MAI na Polygon

## Objetivo deste tutorial

O objetivo deste tutorial não é apresentar a você, em detalhes, o que você pode fazer com a sua stablecoin MAI, mas sim mostrar uma lista de todos os websites e aplicaçōes DeFi, na Polygon, que te permitem utilizar teu MAI diretamente, ou em combinação com outras stablecoins. Para mais detalhes sobre maneiras específicas de utilizar o MAI, você pode acessar outros tutoriais neste site, ou pedir ajudar no Discord ou Telegram.

Por favor, entenda que esta lista não esta completa, e que nunca estará, pois novos dApps são lançados todas as semanas na rede. Eu não posso avaliar eles todos, portanto, apenas apresentarei aqui as opçōes principais, ou as mais famosas e seguras.&#x20;

Se você quer ver algum projeto específico nesta lista, por favor, junte-se a comunidade Qi no [Discord](https://discord.gg/mQq55j65xJ).

{% hint style="info" %}
Eu não apresentarei as farms da Mai Finance aqui. Este assunto merece seu próprio tutorial, afinal, o token Qi não é como um token qualquer por ai.
{% endhint %}

## Farming de maneira segura em projetos bluechip

Projetos bluechip são aplicaçōes de DeFi que mostram-se excelentes, e que apresentam um baixo risco. Geralmente, são auditados, e o time por trás deles já deve estar trabalhando no projeto a um bom tempo. Eles não possuêm na maioria das vezes um APR imenso, embora sejam confiaveis.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) é um gerenciador automatizado de portfólios, provedor de liquidez, e detector de preços. Nesta plataforma, você poderá emprestar suas criptomoedas, e receber taxas dos traders, que reorganizam seu portfolio seguindo oportunidade de arbitragem. Se você precisar de mais informaçōes sobre o balancer, por favor leia o [guia oficial](https://docs.balancer.fi).

Na rede Polygon, o Balancer possui uma pool composta de 4 principais stablecoins: DAI, USDC, USDT e MAI (miMATIC). Esta pool possui atualmente uma taxa APR de aproximadamente 20%, que tem se mostrado estável.

![Pool de stablecoins em Agosto de 2021](../.gitbook/assets/screen-shot-2021-08-11-at-11.06.59-am.png)

A melhor coisa da Balancer é que você não precisa necessariamente possuir as 4 moedas para depositá-las na pool. A Balancer irá gerar automaticamente uma combinação equilibrada com qualquer seja o depósito que você fizer. Isso significa que se você tem 100$ de MAI, você pode simplesmente depositá-los na pool da Balancer e deixar o algoritmo introduzi-los corretamente para obter uma razão de 25% para cada moeda, dependendo de seu preço no momento do depósito.

Recompensas para a pool são pagas utilizando o token BAL, distribuidas semanalmente. Somado ao token BAL, recompensas adicionais podem ser garantidas dependendo da pool que você investiu. Você pode conferir os diferentes programas de incentivo[ aqui](https://balancer-incentives.web.app). No nosso caso, participar da pool de stablecoins tambem nos gerará recompensas em MATIC e Qi.

O fluxo completo seria algo semelhante a esta foto:&#x20;

![](../.gitbook/assets/screen-shot-2021-08-11-at-11.34.45-am.png)

Se você precisa de mais informações sobre como usar a Mai Finance para emprestar suas criptomoedas e tomar emprestado MAI (ao invés de vendê-las para fazer isto), leia os outros tutoriais neste site. Você pode até mesmo [incluir a AAVE no loop ](../investment-tutorials/leverage-aave-tokens.md)para ganhar ainda mais dinheiro.&#x20;

### Curve Finance

Um certo click-bait aqui. [Curve](https://polygon.curve.fi) é outra plataforma onde voce é capaz de emprestar suas criptomoedas em pools que ter geram rendimento, mas não em MAI diretamente, pelos menos ainda. As pools que nós estamos interessadas são:&#x20;

* A pool AAVE que gera entre 5% e 15% de APR (o APR varia bastante) no trio de stablecoins (DAI/USDC/USDT). Esta pool funciona exatamente como a Balancar, de modo que você participar da pool com apenas um ativo, que será utilizado na AAVE pelo protocolo.
* A pool Atricrypto que é composta do trio de stablecoins e também inclui wETH e wBTC para mitigar impermanent loss. Esta pool possui um APR que varia entre 25% e 35%. No momento, o time da Mai Finance está tentando adicionar MAI a essa pool, o que significa que você poderia entrar com o seu MAI diretamente.

Enquanto esperamos o protocolo Curve aceitar MAI como uma stablecoin válida para as suas pools, você já pode usar a sua criptomoeda favorita, seguindo as seguintes etapas, exemplificadas com MATIC:&#x20;

* Deposite seu token MATIC na AAVE e colete amWMATIC&#x20;
* Deposite seu amWMATIC na Mai Finance e colete camWMATIC (as recompensas da AAVE serão acumuladas em camWMATIC)&#x20;
* Utilize o camWMATIC como garantia na Mai Finance e tome emprestado MAI
* Utilize a [pagina](https://app.mai.finance/anchor) na Mai Finance para trocar todo o seu MAI por USDC
* Então, você poderá:
  * Entrar na pool Atricrypto na Curve com o seu USDC e receber recompensas de 25% a 30%&#x20;
  * Entrar na pool da AAVE na Curve com o seu USDC receber recompensas de 5% a 15%

Recompensas na Curve são garantidas em:

* USDC auto acumulado, que aumenta a sua posição na pool (uma misture entre USDC/USDT/DAI e possivelmente wBTC/wETH para a pool Atricrypto)
* WMATIC, que pode ser utilizado para repetir o loop acima e aumentar o seu emprestimo e capital investido
* Token CRV, que pode também ser utilizado como garantia na Mai Finance para tomar emprestado mais MAI e aumentar seu capital investido

![](../.gitbook/assets/screen-shot-2021-08-11-at-12.14.27-pm.png)

### AAVE

Há um guia completo sobre como utilizar a Mai Finance para [alavancar tokens na AAVE](../investment-tutorials/leverage-aave-tokens.md). Isso é realizado sem utilizar a stablecoin MAI diretamente, mas nós podemos imaginar que, no futuro, a AAVE também incorporará MAI em uma de suas pools, onde você poderá emprestar suas criptomoedas.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) é provavelmente uma das DEX mais famosas na rede Polygon, junto a SushiSwap e 1Inch. Ela é também uma _AMM_ (Automated Market Maker, Agente de Mercado Automatizado) que permite aos seus usuários fazer operaçōes eficientemente na rede Polygon, utilizando pools de liquidez. Qualquer operação feita na corretora é sujeita a uma taxa que é parcialmente redistribuida aos usuarios que injetam liquidez na plataforma.

A maneira como você pode usar MAI na QuickSwap é muito semelhante a uma [yield farm](secure-your-yield-farming-profits.md) normal. Então, se você precisa de informaçōes sobre como entrar na pool de MAI/USDC da QuickSwap, é provavelmente melhor para você ler este artigo.

Atualmente, ao entrar em uma pool LP (**L**iquidity **P**rovider, Provedor de Liquidez) de MAI/USDC na QuickSwap, você receberá:

* Taxas das operaçōes
* Tokens QUICK

![Detalhes da pool de MAI/USDC na QuickSwap em Agosto de 2021](../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

## Farms degen e agregadorees

### Adamant

[Adamant](https://adamant.finance/home) é um agregador que lista as "melhores" farms da Polygon e que permite você entrar nelas diretamente de seu website. Depositando seus ativos (tokens LP) em uma pool especifica na Adamant, o algoritmo irá colher as recompensas garantidas pela pool e automaticamente acumular parte das recompensas na sua posição LP. O resto da recompensa é geralmente convertido para WMATIC, que é então redistribuindo aos _holders_ do token ADDY (token nativo da Adamant). Por último, você recebe uma recompensa em tokens ADDY, assim como você faz e faz vesting por 90 dias, recebendo parte dos seus dividendos de WMATIC.&#x20;

No geral, Adamant é um bom lugar para visitar se você não liga muito para o token da farm, e se você não reacumular suas recompensas manualmente varias vezes ao dia. Também gera mais rendimento já que você ganha recompensas em ADDY somadas as recompensas garantidas pela pool.

A Adamant atualmente suporta algumas pools que aceitam o par de LP MAI/USDC. As pools estão em:

* QuickSwap: Recompensas em QUICK são trocadas por mais LP MAI/USDC e WMATIC
* DinoSwap: Recompensas em DINO são trocadas por mais LP MAI/USDC e WMATIC
* Mai Finance: Recompensas Qi são trocadas por mais LP MAI/USDC e WMATIC

![Pool de MAI/USDC da QuickSwap na Adamant](../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)

{% hint style="info" %}
Os screenshots da pool da QuickSwap no website da QuickSwap (veja paragrafo acima) e Adamant foram tirados no mesmo dia, mas estão exibindo APY's (**A**nnual **P**ercentage **Y**ield).
{% endhint %}

You can see that the APY on Adamant is a little bit higher than on QuickSwap directly. The reward breakdown is as follows

* 12.88% Auto-compounded QUICK (meaning the QUICK reward is transformed into more LP tokens)
* 9.16% ADDY reward (not compounded)
* 3.40% fee share dividend (claiming ADDY daily)

This means that, out of the 20.92% granted by QuickSwap, only 12.88% is used to increase your LP position, the rest is swapped into WMATIC dividends. You will be able claim your ADDY reward daily (or anytime) and stake them, which will will in turn generate claimable WMATIC dividends. In other words, Adamant _seems_ a better option because it has better APYs and compound rewards automatically, but in reality it involves a lot of manual actions too.

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

[Impermax](https://polygon.impermax.finance) is a platform that let users leverage their LP tokens for higher yields. The goal is very simple: by providing LP tokens and using them as collateral, one can then borrow more of the 2 underlying assets to generate more LP tokens and repeat the loop.

![Impermax loop explained](../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)

When doing so, the user is exposed to impermanent loss, and the loss is magnified by the number of times the loop is repeated. The risk of liquidation is also multiplied when too many loops are applied. Indeed, if the APR is multiplied, the price variation of the two coins forming the pair is amplified by the lever effect, leading to faster liquidation.

With stable coins, the risk of liquidation is lower though, because the price variation is negligible. This also means that the Collateral to Debt Ratio (CDR) can be very close to 100%, leading to a high number of loops, hence a high APR.

Note that Impermax is charging fees when you borrow and leverage your position. The fee corresponds to 0.1% of your final position. As an example, if I have $100 worth of MAI/USDC and I leverage 50x, my final position will worth $5,000 and I will pay a $4.90 fee corresponding to the $4,900 that I borrowed.

The effect of looping the lending/borrowing combination allows to multiply the final APY. With an initial APY of 20% for MAI/USDC pair with a CDR of 110%, operating the loop 50 times, and using the formula

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

We can easily get a 228% final APR. There are some other elements that will affect the final APR, namely the borrowing APR (loan interest for borrowing more LP tokens), and the supply/demand of both assets composing the LP pair (directly driving the borrowing APR).

Also, because all the rates are magnified by the number of times the loop is applied, the APR will vary drastically, and can sometimes become negative for short amount of times (your LP token will be used to repay the negative APR).

### Leveraged position of my MAI/USDC pair

In the end, you are using the base APR on a much bigger value, which is earning much bigger interests, increasing the APR of your initial position.

![An example of Impermax dashboard with an initial $70.52 MAI/USDC pair](../.gitbook/assets/screen-shot-2021-08-11-at-1.38.33-pm.png)

I can see very easily how much I'm using as collateral, how much I initially invested, what's the leverage ratio, and what are the liquidation values due to the leverage ratio. This position will give me the following ratios at the time of writing

![Earnings and spendings estimation at a given time](../.gitbook/assets/screen-shot-2021-08-11-at-1.41.55-pm.png)

The APR is granted in IMX token that can either be swapped for more MAI/USDC (use the power of Mai Finance to borrow at 0% interest, RFTM), or used to provide liquidity on specific pools accepting IMX on Impermax.

### Supplying MAI to borrowers

Indeed, on the app you can also provide liquidity to those who want to apply leveraging loops to their positions (they will need underlying assets to generate more LP tokens). Lending assets is a great way to earn yield and let the borrowers take all the risks. Also, the more users are borrowing, the higher the supply APR will be.

![Rates for supplying and borrowing MAI on Impermax at a given time](../.gitbook/assets/screen-shot-2021-08-11-at-1.47.56-pm.png)

This is another great way to optimize your 0% loan on Mai Finance. Not only you don't have to pay anything to borrow MAI, but you can earn a lot of interest just by depositing it on Impermax.

## Disclaimer

Everything is this tutorial is purely educational. The goal is to bring light to projects that I think are worthy for people evolving in the crypto world on Polygon. I obviously didn't talk about Mai Finance as a farm because a dedicated tutorial will be written very soon. Finally, this guide is ABSOLUTELY NOT meant to be applied as is, it's not any financial advice and you should not follow blindly what I wrote. Please read the docs of the different projects I mentioned before considering investing on their platforms.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
