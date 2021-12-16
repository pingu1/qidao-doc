---
description: >-
  Este guia ensina como combinar rendimentos de farming com juros de empréstimos
  fornecidos pela Mai Finance para aumentar sua receita total.
---

# Como combinar recompensas de farming e empréstimos

## Introdução

Em Setembro de 2021, a Mai Finance introduziu o sistema de recompensas em Vaults para promover seu negócio de empréstimos, e atrair pessoas a depositarem seus tokens para tomar MAI emprestado. Não se trata apenas de tomar um empréstimo a 0% de juros, agora pessoas também podem ser pagas para tomar dinheiro emprestado. Este guia irá propor uma estratégia baseada em farming de stablecoins usando a Augury Finance como uma fonte de tokens que irá alimentar os cofres na Mai Finance, incentivando empréstimos maiores, e mais MAI que será então reinvestido na farm.

![](<../.gitbook/assets/image (7).png>)

## Apresentação das pools e das aplicaçōes

### Augury Finance

Augury Finance é um agregador de rendimento que não foca em reacumular automaticamente seus tokens LP (**L**iquidity **P**ool). Ao invés, Augury irá automaticemente vender os tokens da farm que são usados para comprar outros tokens em suas infusions (infusōes)_._

Por exemplo, você pode fazer farming com o par DFYN-WETH na Augury:

![Exemplo da pool de mineração de DFYN-WETH na Augury Finance](<../.gitbook/assets/image (32).png>)

Essa infusão usa a DinoSwap como a farm subjacente, e um token LP que pode ser obtido na DFYN. Com um APR de 123.43%, usuários que fornecerem liquidez a essa pool serão recompensados com:

* 30% de WETH
* 20% de LINK
* 20% de WBTC
* 15% de USDT
* 15% de WMATIC

Se você fizer farming na DinoSwap, você será pago em tokens DINO, cujo preço é muito volátil. Em outros agregadores como a Adamant ou Beefy, você aumentaria sua posição LP, mas com a Augury você protege sua posição ao obter tokens que, provavelmente, terão volatilidade reduzida. A desvantagem é que sua posição inicial não irá crescer ao longo do tempo já que 100% do DINO colhido é convertido a configuracao dos tokes que compoem a recompensa na Augury.

{% hint style="info" %}
A Augury Finance usa 3 diferentes tiers (niveis) de infusão que possuem taxas de deposito e de performance diferentes. Por favor leia sobre os tipos de tiers que quer usar e tenha certeza que entende o seu impacto na sua estratégia de farming.
{% endhint %}

Em nossa estratégia, nós usaremos a farm de tier 2 USDT-UST que recompensa os usuários com uma mistura de WETH/WBTC/LINK/WMATIC/USDC, porque a Mai Finance oferece 4 Vaults para 4 dos 5 tokens que nós receberemos como recompensa. Para maximizar nossos lucros, nós adicionaremos AAVE entre o output (saída) da Augury e os Vaults da Mai Finance, já que 3 dos 5 tokens que nós iremos colher podem ser emprestados na AAVE.&#x20;

![Farming de stablecoins USDT-UST para a nossa estratégia](<../.gitbook/assets/image (31).png>)

### Curve

Curve é um projeto blue chip que recompensa seus usuários emprestando tokens blue chip. A recompensa é composta de tokens reacumulados automaticamente (adicionados de volta ao investimento), tokens WMATIC e CRV, 2 tokens que também são aceitados como garantia na Mai Finance.

Algo interessante a se notar sobre o Curve e suas pools é que não é necessario depositar a quantidade exata de cada token em uma determinada pool. Ao invés disso, um único token pode ser fornecido, e o algoritmo que administra a pool irá automaticamente ajustar os outros tokens, vendendo uma porção do depósito original para comprar os outros tokens, mantendo a propocao correta na pool.

Nós usaremos a pool atricrypto3 que aceita qualquer combinação de WBTC/WETH/USDC/USDT/DAI e nós adicionaremos a essa pool o USDC que será gerado pela pool na Augury.&#x20;

![Detalhes da pool atricrypto3 na Curve em Setembro de 2021](<../.gitbook/assets/image (30).png>)

### AAVE

Como mencionado no parágrafo sobre a Augury, a AAVE é usada para adicionar uma pequena recompensa aos tokens de farming na Augury antes de usá-los na Mai Finance. Ao invés de depositar nosso WBTC, WETH e WMATIC diretamente na Mai Finance, nós iremos depositar estes tokens na AAVE e usar o instrumento de rendimento na Mai Finane para reacumular automaticamente as recompensas da AAVE nas pools amToken, e usar o camToken como garantia nos Vaults. Você pode obter mais detalhes sobre esta parte lendo o [tutorial sobre tokens AAVE](leverage-aave-tokens.md).

![Recompensas de empréstimsos da AAVE em Setembro de 2021](<../.gitbook/assets/image (29).png>)

### Balancer

A Balancer é outro projeto blue chip como a Curve. Nele, você é capaz de participar de pools compostas de mais de dois tokens, apenas depositando um. A pool irá automaticamente ser equilibrada para obter a mesma proporção para cade token que compōe a pool.&#x20;

Para nossa estratégia, nós usaremos a pool WETH/BAL/Qi/MAI/USDC. Esta pool aceitará o token Qi que será coletado dos Vaults na Mai Finance, e nos recompensará com mais Qi e tokens BAL que nós poderemos depositar na Mai Finance no Vault BAL, nos permitindo cunhar mais MAI e aumentar nossa posição de farming na Augury.

![5-pool da Balancer em Setembro de 2021](<../.gitbook/assets/image (23).png>)

## Bootstrapping

![](<../.gitbook/assets/image (19).png>)

Em seguir veremos uma simulação feita com um investimento inicial de $1,000 de ETH que são depositados no Vault camWETH para tomar emprestado $500 de MAI, convertidos em $500 de USDT-UST. Esta simulação assume as seguintes recompensas para os diferentes sistemas:

* APR em farming de USDT-UST de 22.53%
* APR em amWBTC de 0.39%
* APR em amWETH APR de 1.71%
* APR em amWMATIC de 3.80%
* APR em atricrypto3 de 3.86% para o LP token reacumulado automaticamente, 13.09% de WMATIC e 17.63% de CRV
* Pool "5-tokens" na Balancer com APR de 43.46% com uma proporção de 1:6 sobre BAL:Qi
* APRs das recompensas em Vault de
  * 23.28% em camWBTC
  * 21.52% em camWETH
  * 32.93% em camWMATIC
  * 24.51% em LINK
  * 116.71% em CRV
  * 62.38% em BAL

Todos estes APRs estão sujeitos a mudar nas diferentes plataformas, e não há garantia que eles continuarão assim durante o ano todo, entretanto nós os consideraremos estáticos nesta simulação, para conseguirmos uma ideia do possível APR geral do sistema. Para simplificar a simulação, nós não levaremos em consideração as variaçōes de preço, nem as taxas de transaçōes. Também perceba que esta simulação leva em consideração que as recompensas do Vault na Mai Finance e na Balancer são reacumuladas diariamente ao invés de semanalmente, mas, atualmente, estas recompensas são depositadas nas carteiras dos usuários semanalmente por meio de _Airdrops_. Por último, para o funcionamento desta simulação, nós assumiremos que a taxa CDR (_**C**ollateral to **D**ebt **R**atio_, ou Proporção de Garantia para Dívida) é sempre de 200%, o que significa que nós estamos apenas tomando emprestado metade do que nós depositamos para continuar recebendo as recompensas, mas prevenindo de sermos liquidados facilmente.

### 1.º Dia

Se você ainda tiver seus $1,000 de WETH, deposite-os na AAVE para obter amWETH, então deposite seus amWETH na [Mai Finance](https://app.mai.finance/yield) para obter camWETH, e por último deposite seu camWETH dentro do Vault correspondente para poder tomar emprestado 500 MAI.

Use a [anchor](https://app.mai.finance/anchor) para converter seu MAI em USDT (ou você pode usar outra DEX como a QuickSwap se não houve liquidez na Anchor), então você pode usar a [DFYN](https://exchange.dfyn.network/#/) para trocar 50% de seu USDT em UST e formar um par USDT-UST que você pode então depositar na [Augury](https://augury.finance/infusions/). Perceba que você também precisará de um pouco de OMEN, que pode ser comprado na QuickSwap.

Portanto, no final do primeiro dia, nós colheremos as seguintes recompensas:

| Tipo de recompensa        | Valor em dólares |
| ------------------------- | ---------------- |
| WBTC de farming           | 0.123            |
| WETH de farming           | 0.031            |
| WMATIC de farming         | 0.031            |
| LINK de farming           | 0.031            |
| USDC de farming           | 0.092            |
| Recompensas Qi dos Vaults | 0.295            |

Estas são apenas as recompensas que nós conseguimos do farming e empréstimos no fim do primeiro dia.

### 2.º Dia

Recompensas são colhidas, WBTC, WETH e WMATIC são enviados aos Vaults respectivos na Mai Finance após eles passarem pela AAVE e o instrumento de rendimento na Mai. LINK é depositado diretamente no Vault LINK, e USDC enviado a Curve na pool atricrypto3. A recompensa Qi é enviada a Balancer. Neste ponto, nós podemos tomar mais MAI emprestado dos 3 Vaults camToken e do Vault LINK ($0.13 de MAI para ser preciso) e criar mais pares USDT-UST com o MAI emprestado.

Portanto, no final do segundo dia, nós colheremos as seguintes recompensas:

| Tipo de recompensa        | Valor em dólares |
| ------------------------- | ---------------- |
| WBTC de farming           | 0.123            |
| WETH de farming           | 0.031            |
| WMATIC de farming + Curve | 0.031            |
| LINK de farming           | 0.031            |
| USDC de farming           | 0.093            |
| Recompensas CRV na Curve  | 0.00004          |
| Recompensas BAL           | 0.00005          |
| Recompensas Qi dos Vaults | 0.296            |

A partir deste ponto, o sistema está armado e as recompensas estão fluindo de uma maneira que cada etapa alimenta a próxima, o que acaba criando um pequeno loop bem legal.

## Resultados do Farming

### Rotina diária

A rotina diária é composta pelas seguintes transaçōes:

* Colher as recompensas na Augury
* Depositar WBTC, WETH e WMATIC na AAVE
* Depositar amWBTC, amWETH e amWMATIC na Mai Finance no instrumento de rendimento
* Depositar camWBTC, camWETH e camWMATIC nos respectivos Vaults na Mai Finance
* Depositar LINK no Vault de LINK na Mai Finance
* Depositar USDC na pool atricrypto3 na Curve
* Colher WMATIC da Curve e usá-lo no Vault da camWMATIC
* Colher CRV da Curve e usá-lo no Vault CRV
* Tomar MAI emprestado dos diferentes Vaults
* Converter MAI em USDT na Mai Finance pela Anchor
* Converter 50% do USDT em UST na DFYN
* Criar um novo par LP de USDT-UST na DFYN
* Depositar os novos LP tokens na Augury

### Rotina semanal

Além disso, você irá obter recompensas semanais em BAL (do seu deposito em Qi na Balancer) e tokens Qi (das recompensas dos Vaults). Você precisará:

* Depositar o token Qi na Balancer
* Depositar o token BAL na Mai Finance no Vault BAL
* Tomar MAI emprestado do seu depósito adicional de BAL e o converter em um par USDT-UST para fazer farming na Augury

### Resultados mensais brutos

| Mês | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| --- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1   | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2   | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3   | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4   | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5   | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6   | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7   | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8   | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9   | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10  | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11  | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12  | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

A few notes:

* The growth of the USDT-UST pool is the only result of additional MAI borrowed from vaults
* The CRV pool is almost inexistant due to the very low amount of USDC deposited on Curve
* The BAL vault is not important due to the fact that 14.28% of the Balancer reward is paid in BAL tokens, the rest being paid in Qi tokens
* The amount in the Balancer pool is the biggest gain, and is only the result of Vault rewards and Balancer rewards

### Day 365

After a complete year, the final state of our investment would be

| Position    | Value in dollars |
| ----------- | ---------------- |
| USDT-UST    | 553.24           |
| atricrypto3 | 36.20            |
| Balancer    | 137.62           |
| camWBTC     | 47.45            |
| camWETH     | 1,029.19         |
| camWMATIC   | 14.39            |
| LINK        | 11.84            |
| CRV         | 0.017            |
| BAL         | 3.93             |

The total debt is actually the entire USDT-UST position, so $553.24, and the total reward generated is $280.63, corresponding to a final APY of 28.06%.

### Comparison with other strategies

Getting a 28% APY on stable coin farming isn't too bad, but how does this compare to other easier strategies we could apply with the initial $1,000 worth of ETH? Let's check the final APY fo the following strategies

* Leverage amWETH 8 times via AAVE: for this, we will use the exact flow described in the [AAVE token guide](broken-reference).
* Full stable farming on Augury: for this strategy, we sell the WETH and farm with $1,000 worth of USDT-UST on the same infusion on Augury
* Full stable farming on QuickSwap: for this strategy, we will use the camWETH vault to benefit from the vault reward, and farm with $500 worth of MAI on QuickSwap (MAI-DAI at 19.78% APY), using the dQUICK vault on Mai Finance to borrow additional MAI and re-invest into the farming pool (dQUICK vaults with an APR of 55.72%)

| Strategy                         | Final APY |
| -------------------------------- | --------- |
| Strategy presented in this guide | 28.06%    |
| Leverage AAVE token 8x           | 46.46%    |
| Only stable farming on Augury    | 22.53%    |
| Quickswap farming + dQUICK vault | 35.96%    |

## Disclaimer

This strategy is really interesting and uses most vaults from Mai Finance, and this guide has been written mostly to showcase that, as of September 2021, this is the part that would generate the more rewards when faming stable coins. However, this strategy may not be the most interesting one, and involves a lot of manipulations of several platforms. Finally, Augury is a fantastic tool that generates specific tokens that can be included in several strategies, but probably not stable farming solely. And as a side note, no deposit fees nor performance fees have been taken in consideration when calculating the final APY.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}

