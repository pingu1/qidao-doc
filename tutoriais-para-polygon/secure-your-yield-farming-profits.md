---
description: >-
  Esta pagina ensina, em detalhes, como modificar de maneira "segura" a yield
  farming, uma estratégia DeFi, em uma estratégia um pouco menos rentável mas
  muito mais segura.
---

# Farming utilizando apenas stablecoins

## Ideia Geral

Ao entrar em uma y_ield farm,_ fazenda em inglês, você passa a expor seus investimentos ao sucesso ou fracasso da farm. Este guia não tem como objetivo explicar em detalhes **o que é** uma yield farm, ou como você deve trabalhar com elas. Se você precisa de ajuda sobre isso, há tutoriais disponíveis em todos os lugares da internet. Você também pode conseguir ajudar pela comunidade da QiDAO no [Discord](https://discord.gg/mQq55j65xJ).

O problema principal ao fazer farming é ter de escolher entre:

* vender o token nativo e convertê-lo em ativos "assegurados" que representaram o seu lucro&#x20;
* reinvestí-los para gerar ainda mais lucro (também conhecido como juros hipercompostos)

Este guia irá te apresentar, passo a passo, como utilizar a Mai Finance para assegurar os teus lucros, e ao mesmo tempo reinveistir uma porção deles na farm.&#x20;

{% hint style="info" %}
Para ilustrar em mais detalhes como você pode fazer isso, utilizaremos a ultima farm da[ PolyPup](https://ball.polypup.finance). Isso será feito com objetivo meramente educacional, e não deve ser visto como conselho financeiro. A propósito, o termo "seguro" aqui utilizado é baseado em minha própria avaliação. Como sempre, faça a sua propria pesquisa. Por ultimo, eu particularmente não recomendo esta farm.&#x20;
{% endhint %}

![](../.gitbook/assets/screen-shot-2021-08-09-at-10.20.26-am.png)

## Ciclo de vida do farming

### Preparando-se para a farm

Um fazendeiro humilde uma vez me disse:

> _**Você nunca deve comprar o que pode ganhar**_

Neste tutorial, nos tentaremos aplicar o máximo de segurança financeira possível. Para fazer isso, nós faremos farming utilizando apenas stablecoins, para proteger nosso investimento de qualquer _impermanent loss, ou_ prejuizo impermanente. A maioria das farms dispōe de pares de stablecoins para suas pools de liquidez (LP), e como a MAI tem ganhado mais e mais visibilidade, você pode encontrar farms contendo pools de MAI/USDC. Este é o par de stablecoins que nós focaremos a nossa atenção.

Para começar o _farming_ utilizando par de MAI/USDC, você precisa adquirir algumas stablecoins. A Mai Finance permite a você tomar emprestado a stablecoin MAI de acordo com o depósito da sua criptomoeda favorita. No nosso caso, nós temos algumas MATIC na nossa carteira, prontas para serem usadas. Ao depositar meu MATIC dentro do [cofre da MATIC](https://app.mai.finance/vaults/matic) na Mai Finance, eu posso tomar emprestado MAI. Se você precisar de ajuda para fazer isso, por favor entre no servidor do Discord e pergunte à comunidade. Você também pode aprender a fazer isto lendo outros tutoriais neste site.

{% hint style="info" %}
Você pode depositar seus tokens MATIC no cofre de MATIC, mas você também pode depositá-los na AAVE para obter amWMATIC, depositá-los na Mai Finance na página de rendimento para obter camWMATIC, e utilizar esse camWMATIC como garantia. Você poderá tomar emprestado a mesma quantia de MAI, mas você também ganhará rendimento adicional no seu matic. Veja aqui [como alavancar seus tokens AAVE](../investment-tutorials/leverage-aave-tokens.md) para obter mais detalhes sobre o assunto.
{% endhint %}

Após você tomar emprestado MAI, você pode usar a pagina [página ancora](https://app.mai.finance/anchor) na Mai Finance para converter metade do seu empréstimo a USDC. De fato, quando você faz farm utilizando pares de liquidez (LP), as duas partes do par precisam ser providenciado em uma razão de 1:1.&#x20;

![Utilizando a página de swap para converter 30 MAI em USDC](../.gitbook/assets/screen-shot-2021-08-09-at-6.28.28-am.png)

Agora, dependendo da farm que você pretende utilizar, você precisa combinar as suas duas stable coins (MAI e USDC) em um par LP válido na plataforma da DEX. Como o meu plano é entrar na Polyup, e esta farm aceita LP's da QuickSwap, eu preciso ir a [QuickSwap](https://quickswap.exchange/#/) e gerar o meu par lá dentro.

![Gerando alguns tokens LP utilizando MAI e USDC](../.gitbook/assets/screen-shot-2021-08-09-at-6.29.16-am.png)

Eu estou pronto para entrar na farm agora.

### Depositando e colhendo tokens de farm

Agora que você possui alguns tokens da LP, você pode ir ao site da farm e depositá-los para começar a coletar os tokens da farm. No nosso exemplo, eu depositei meus tokens MAI/USDC dentro da pool respectiva, e comecei a coletar os meus tokens BALL.&#x20;

![Recebendo tokens BALLs na pool](../.gitbook/assets/screen-shot-2021-08-09-at-10.58.19-am.png)

No momento, você pode ver que o farming de MAI/USDC está me gerando um APR de 176.99%. Dependendo da liquidez presente na pool, e do preço do token BALL, este APR pode mudar com o passar do tempo.

{% hint style="info" %}
É muito importante entender que ao depositar seus tokens LP, a maioria das farms irá te cobrar uma taxa entre 2% a 4%, tomada diretamente do valor do seu depósito. Esteja atento a isso, e tenha certeza que você está confortavel em perder esta taxa, e que não irá consegui-la de volta.&#x20;
{% endhint %}

Agora que suas stablecoins foram depositadas na pool, você receberá alguns tokens de farm, que você pode colher quando quiser. Saiba porém que o preço to token da farm será provavelmente muito volátil, então faça questão de colher regularmente, quando o token tiver mais valor. Quanto mais você esperar, maior o risco de você ter uma porção de tokens que valem absolutamente nada. Na foto acima, você pode ver a opção Harvest, que deve ser clicada para obter os seus BALLs.&#x20;

### Alavanque os seus tokens de farm

Tendo em conta que agora você possui alguns tokens de farm, geralmente você pode escolher entre:

* vendê-los para comprar algo de maior valor (sua criptomoeda favorita é um bom exemplo)
* reinvesti-los na pool&#x20;

A Mai Finance te apresenta uma terceira opção que ter permite fazer ambos. Após você ter colhido sua recompensa, simplesmente visite a sua DEX favorita, desde que ela suporte o token da farm. Geralmente, você pode encontrar um link para uma DEX no menu da farm. Este link incluirá o endereço do token, o que te ajudará a trocá-lo facilmente.&#x20;

![Trocando minha recompensa para mais MATIC](../.gitbook/assets/screen-shot-2021-08-09-at-11.14.29-am.png)

Neste momento, eu volto para a etapa em que nós temos tokens MATIC em nossa carteira, prontos para serem depositados na Mai Finance como garantia. Se eu assim fizer, eu posso tomar emprestado MAI, trocar uma parte por USDC, criar um par LP e redepositá-los na farm. Fazendo esta conversão, eu "asseguro" 100% das minhas recompensas ao trocá-los por uma criptomoeda mais estavel (MATIC, no caso). Eu reinvesto, então, 50% da minha recompensa na pool de liquidez (ou na verdade, neste exemplo, 46%, devido as taxas de deposito de 4%).

Se você pensar por uma outra perspectiva, o APR é aplicado totalmente sobre sua criptomoeda principal. Se você está depositando novos tokens lP na pool (com juros compostos), você terá 50% do APY anunciado pela pool.

## Estimativa de ganhos

Todos os resultados apresentados abaixo dependem de assumirmos algumas coisas:

* Nós começamos com o equivalente de 60 MAI, que tomamos emprestado com garantia de $120.00 de MATIC
* O APR da farm permanece constante em 176.99%, o que resulta em um ganho diario de 0.484%
* O valor de MATIC e BALL permanecem os mesmos durante o mesmo período

Essas suposiçōes obviamente não são aplicaveis na vida real ja que o APR deve cair lentamente conforme mais liquidez é injetada na pool, e que os tokens da farm variam em preço

### Resultado bruto estimado

| Dia | Valor da LP | Valor da recompensa | MATIC acumulados | Nova LP criada |
| :-: | ----------: | ------------------: | ---------------: | -------------: |
|  1  |      $57.60 |              $0.279 |           $0.279 |         $0.139 |
|  2  |     $57.734 |              $0.280 |           $0.559 |         $0.140 |
|  3  |     $57.874 |              $0.280 |           $0.840 |         $0.140 |
|  4  |     $58.014 |              $0.281 |           $1.121 |         $0.141 |
|  5  |     $58.155 |              $0.282 |           $1.403 |         $0.141 |
|  6  |     $58.296 |              $0.282 |           $1.686 |         $0.141 |
|  7  |     $58.437 |              $0.283 |           $1.969 |         $0.142 |
|  8  |     $58.579 |              $0.284 |           $2.253 |         $0.142 |
|  9  |     $58.721 |              $0.285 |           $2.538 |         $0.142 |
|  10 |     $58.863 |              $0.285 |           $2.823 |         $0.143 |
|  11 |     $59.006 |              $0.286 |           $3.109 |         $0.143 |
|  12 |     $59.149 |              $0.287 |           $3.396 |         $0.143 |
|  13 |     $59.292 |              $0.287 |           $3.684 |         $0.144 |
|  14 |     $59.436 |              $0.288 |           $3.972 |         $0.144 |
|  15 |     $59.580 |              $0.289 |           $4.261 |         $0.144 |
|  16 |     $59.725 |              $0.289 |           $4.551 |         $0.145 |
|  17 |     $59.870 |              $0.290 |           $4.841 |         $0.145 |
|  18 |     $60.015 |              $0.291 |           $5.132 |         $0.145 |

* No dia 1, a taxa de 4% é aplicada no nosso investimento inicial de 60$ do par MAI/USDC
* No final do dia 1, a receita gerada ($0.279) é totalmente transferida no cofre de MATIC
* No final do dia 1, como nos adicionamos mais fundos ao cofre, nós podemos tomar emprestado mais MAI
* Para manter uma razão Garantia / Divida de 200%, nós apenas pegaremos emprestado 50% do nosso MATIC depositado ($0.139)
* No inicio do dia 2, nós reinvestimos $0.139 na farm (e a farm detem 4% de taxas de deposito)&#x20;
* No inicio do dia 2, nós começamos novamente, com um valor adicional de $0.134 de tokens LP&#x20;

### Estimando o APR, APY e o crescimento da receita

A estimativa parou após 18 dias, porque passado esta data, você pode ver voltamos ao valor de 60$ em tokens LP. Isto significa que eu produzi o suficiente para reembolsar as taxas de deposito iniciais, o que seria o minimo que um fazendeiro deve pretender obter.&#x20;

Passado esta data, permanecer na farm gerará apenas beneficios. E porque nós estamos utilizando stablecoins, ha literalmente um rsico de 0% de impermaent loss na liquidez que eu providenciei, significado que nao ha risco de perder dinheiro ao permanecer na pool.&#x20;

Entretanto, eu tambem posso considar que eu reembolsei a taxa de deposito inicial de $2.40 no dia 9, pois foi o momento que o lucro da minha carteira MATIC alcancou esta quantidade. Se eu apenas estivesse vendendo o token da farm para obter lucro, e não re-investi-lo na pool, este seria o momento, de fato, a partir de que eu geraria apenas beneficios.&#x20;

Se tratando de ganhso, a recompenda que se torna acumulada na farm é apenas 50% do APR da farm. Isto significa que com um APR de 176.99%, a verdadeira taxa de crescimento anual é de apeans 88.495% anualmente, ou 0.242% diariamente.

Também é possivel calcular o ganho exato que foi acumulado em um dia especificod a farm, assumindo que você esta acumulando diariamente, utilizando a seguinte formula para obter o **ROI**, sigla em inglês para **Retorno Sobre Investimento**,&#x20;

$$
ROI_{DayN}=InitialInvestment*(1+DailyAPR)^{DayN}-InitialInvestment
$$

In the case of a farm that takes 4% deposit fee, you need to multiply the above result by 96%. In our case, we can quickly verify that the formula works by comparing its result to the table above

$$
ROI_{Day1} = [60 * (1+0.00242)^{1}-60]*0.96=$0.1396523836
$$

$$
ROI_{Day365}=[60*(1+0.00242)^{365}-60]*0.96=$81.80752927
$$

Starting from $60.00 and generating $81.81 after 1 year gives an APY of 136.34%.

If we compare this to the theoretical APY given by a 88.495% APR using the formula

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

This gives with an APR of 88.495% and N = 365 (compounding daily)

$$
APY = ( 1 + \frac{0.88495}{365})^{365}-1=142.02\%
$$

Note that the estimation above doesn't take into consideration the 4% deposit fee, hence the small discrepancy.

The gains in the MATIC wallet are simply twice the gains from the farm and we can calculate the ROI on a given day using the same formula as above and multiply the result by 2.

$$
ROI_{Day365} = [60 * (1 + 0.00242)^{365} - 60]*0.96*2=$163.6150585
$$

This is the number of MATIC that we would generate by staying into the farm for one year, with an initial investment of 60$ worth of MAI/USDC, assuming the APR of the farm remains the same. This also gives an APY of 272.69%, which is roughly the APR that the farm advertised (the farm usually don't take into consideration the 4% deposit fee in the displayed APR).

### Recap after 1 year farming with stable coins

At the end of the year we would get

* $283.62 MATIC in the Vault (initial $120.00 + $163.62 generated by the farm)
* $141.82 of debt (initial $60.00 + $81.82 borrowed and re-invested)
* $141.82 of MAI/USDC tokens on the farm

## Disclaimer

Everything presented in this strategy is assuming that

* The farm is keeping a constant APR on your pool (which is totally wrong)
* It is possible to farm for a whole year (which is not possible, all farms are ending their farming session sooner or later)

As a side note, the APR of the MAI/USDC pool on Polypup after 24h of farming is 128.13%, mostly because of the price of BALL slowly decaying.

Also, farming with stable coins _**may**_ be the most "secured" way to earn yields because you're not exposed to impermanent loss. However, there is absolutely no guarantee that you will be able to get your 4% deposit back. You can find some websites that have stable coin pools with 0% to 1% deposit fees, even on the non-native pools (pools that accept LP pairs without the native farm token).

Harvesting the rewards and swapping them for something valuable is considered the best strategy when farming yields. Borrowing MAI to re-inject a portion of stable coin in the pool and increase your farming revenues exposes your benefits to the 4% deposit fee that the farm is taking off your LP pair, which may not be the best thing to do if you are unsure to get it back, and it's probably better to use another strategy to re-invest your earnings (invest in native pools / pools with 0% interest / pools with high APRs).

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
