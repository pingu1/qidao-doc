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

Atualmente, ao entrar em uma LP pool (**L**iquidity **P**rovider, Provedor de Liquidez) de MAI/USDC na QuickSwap, você receberá:

* Taxas das operaçōes
* Tokens QUICK

![Detalhes da pool de MAI/USDC na QuickSwap em Agosto de 2021](../.gitbook/assets/screen-shot-2021-08-11-at-12.37.56-pm.png)

## Farms degen e agregadorees

### Adamant

[Adamant](https://adamant.finance/home) é um agregador que lista as "melhores" farms da Polygon e que permite você entrar nelas diretamente pelo seu website. Depositando seus ativos (tokens P) em uma pool específica na Adamant, o algoritmo irá colher as recompensas garantidas pela pool e automaticamente acumular parte das recompensas na sua posição LP. O resto da recompensa é geralmente convertido para WMATIC, que é então redistribuido aos _holders_ do token ADDY (token nativo da Adamant). Por último, você recebe recompensas em tokens ADDY, que podem ser utilizadas em harvesting e vesting por 90 dias, gerando lucro com dividendos em WMATIC.&#x20;

No geral, a Adamant é um bom lugar para visitar se você não liga muito para o token da farm, e se você prefere não reacumular suas recompensas manualmente varias vezes ao dia. Também gera mais rendimento já que você ganha recompensas em ADDY somadas as recompensas garantidas pela pool.

A Adamant atualmente suporta algumas pools que aceitam o par de MAI/USDC LP. As pools são:

* QuickSwap: Recompensas em QUICK são trocadas por mais MAI/USDC LP e WMATIC
* DinoSwap: Recompensas em DINO são trocadas por mais MAI/USDC LP e WMATIC
* Mai Finance: Recompensas Qi são trocadas por mais MAI/USDC LP e WMATIC

![Pool de MAI/USDC da QuickSwap na Adamant](../.gitbook/assets/screen-shot-2021-08-11-at-12.51.12-pm.png)

{% hint style="info" %}
Os screenshots da pool da QuickSwap no website da QuickSwap (veja parágrafo acima) e Adamant foram tirados no mesmo dia, mas estão exibindo APY's (**A**nnual **P**ercentage **Y**ield).
{% endhint %}

Você pode ver que o APY na Adamant é um pouco mais alto do que teriamos diretamente na QuickSwap. A repartição das recompensas fica assim:

* 12.88% em QUICK reacumulados automaticamente (o que significa que a recompensa QUICK é transformada em mais LP tokens)
* 9.16% em recompensas ADDY (não reacumuladas)
* 3.40% em dividendos pelas taxas (reinvidicando ADDY diariamente)

Isso significa que, dos 20.92% garantidos pela QuickSwap, apenas 12.88% são usados para aumentar a sua posição em LP, o resto é trocado por mais dividendos em WMATIC. Você será capaz de reinvidicar sua recompensa ADDY diária (ou em qualquer período) e fazer stake nela, que irá, por vez, gerar dividendos WMATIC reivindicáveis. Em outras palavras, a Adamant parece ser uma opção superior porque possui melhores APYs e recompensas reacumuladas automaticamente, embora involva também muitas açōes manuais.

{% hint style="info" %}
A Adamant também cria um forte impacto sobre os preços dos tokens nativos. De fato, porque a Adamant está constantemente vendendo os tokens da farm para gerar mais pares LP e WMATIC como dividendos aos seus investidores (holders) em ADDY, a pressão vendedora é muita alta em tokens de farm e com isso podemos explicar porque os seus preços estão consistentemente caindo.
{% endhint %}

### Outras farms que aceitam o par MAI/USDC LP

A MAI está se tornando, a cada dia, mais popular na rede Polygon, e como a QuickSwap já suporta o par MAI/USDC, muitas outras farms passaram a suportar também. A lista abaixo mostra alguns desses projetos em que você pode obter rendimentos utilizando o par MAI/USDC:

* DinoSwap
* Augury
* Polypup
* ...

Outras farms provavelmente já possuem pools de MAI/USDC. Se você deseja ficar informado sobre novas farms e sua data de lançamento, eu recomendo fortemente que você dê uma olhada no [Calendario RugDoc.io](https://rugdoc.io/calendar/) para as farms na rede Polygon. Recomendamos também olhar o resto do website, que mostra uma visão geral muito inteligente sobre cada farm, assim como possíveis riscos associados a elas.

## Impermax

### Uma pequena explicação

A [Impermax](https://polygon.impermax.finance) é uma plataforma que permite aos seus usuarios alavancarem seus LP tokens para obterem rendimentos maiores. O objetivo é muito simples: ao providenciar LP tokens e utilizá-los como garantia, você poderá tomar emprestado mais dos 2 ativos subjacentes para gerar mais LP tokens e repetir o loop.

![Loop da Impermax explicado](../.gitbook/assets/screen-shot-2021-08-11-at-1.15.21-pm.png)

Fazendo isto, o usuário é exposto a _impermanent loss (_prejuízo impermanente_)_, e o prejuízo é aumentado pelo número de loops repetidos. O risco de liquidação é também multiplicado ao serem aplicado muitos loops. De fato, se o APR é multiplicado, a variação de preço das duas moedas adjacentes do par é amplificada pelo efeito de alavanca, levando a uma liquidação mais rapidamente.

Com stablecoins, porém, o risco de liquidação é menor, porque a variação de preço é insignificante. Isso também significa que a Collateral to Debt Ratio (CDR, ou Razão de Garantia para Dívida) pode ficar proxima aos 100%, permitindo um número maior de loops, e com isso um maior APR.

Perceba que a Impermax cobra taxas quando você toma emprestado e alavanca sua posição. A taxa corresponde a 0.1% da sua posição final. Como exemplo, se eu tenho $100 em MAI/USDC e eu alavanco 50 vezes, minha posição final valerá $5,000 e eu irei pagar uma taxa de $4.90 correspondente aos $4,900 que eu tomei emprestado.&#x20;

O efeito de fazer looping com a combinação emprestar/tomar emprestado permite multiplicar o APY final. Com um APY inicial de 20% para o par MAI/USDC com uma CDR de 110%, operando o loop 50 vezes, e utilizando a fórmula

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
