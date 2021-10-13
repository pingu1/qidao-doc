---
description: >-
  Este artículo presenta como puedes combinar el farmeo en las granjas de
  rendimiento con los préstamos incentivados para incrementar los intereses que
  puedes obtener en tus operaciones.
---

# ¿Cómo combinar el farmeo con los préstamos incentivados?

## Intro

En Septiembre de 2021, Mai Finance introdujo los préstamos incentivados con el fin de promocionar su negocio de préstamos y hacer que la gente use sus tokens como colateral para pedir prestado MAI. No se trata sólo de obtenerun préstamo al 0% de interés con una pequeña cuota de repago, ahora la gente también puede recibir pagos por pedir dinero prestado. Esta guía propondrá una estrategia basada en el farmeo de monedas estables utilizando **Augury Finance **como fuente de tokens que alimentarán las bóvedas de Mai Finance, lo que supondrá un incentivo superior al préstamo, y MAI adicional que se reinyectará en la granja.

![](<../.gitbook/assets/image (29).png>)

## Estrategia y presentación de aplicaciones

### Augury Finance

Augury Finance es un agregador de rendimientos que no se centra en auto-componer tus tokens **LP** (Liquidity Pool). En su lugar, Augury venderá automáticamente los tokens de las granjas que utiliza para comprar otros tokens en sus _Infusiones_.

Por ejemplo, puedes hacer farming del par DFYN-WETH en Augury

![Ejemplo de la piscina de liquidez del par DFYN-WETH en Augury Finance](<../.gitbook/assets/image (30).png>)

Esta _Infusion _utiliza **DinoSwap **como granja subyacente, y un token LP que se puede conseguir usando DFYN. Con un APR del 123.43%, los usuarios que depositen liquidez en este pool serán recompensados con

* 30% de WETH
* 20% de LINK
* 20% de WBTC
* 15% de USDT
* 15% de WMATIC

Si cultivas en DinoSwap, te pagarán con tokens DINO, cuyo precio es muy volátil. En otros agregadores como Adamant o Beefy, aumentarías tu posición en LP (tendrías mas tokens LP), pero con Augury "aseguras" tu beneficio obteniendo tokens que tienen menos probabilidad de tener una volatilidad muy alta. El único inconveniente es que tu posición inicial no crecerá con el tiempo ya que el 100% de la cosecha DINO se convierte en el conjunto de tokens que componen la recompensa en Augury.

{% hint style="info" %}
Augury finance utiliza 3 "tiers" diferentes de infusion que tienen diferentes comisiones de depósito y de rendimiento. Por favor, lea sobre los tipos de niveles que desea utilizar y asegúrese de que entiende su impacto para su estrategia de farming.
{% endhint %}

En nuestra estrategia, utilizaremos la granja USDT-UST (TIER 2) que recompensa a los usuarios con una mezcla de WETH/WBTC/LINK/WMATIC/USDC, ya que Mai Finance propone 4 bóvedas para 4 de los 5 tokens que obtendremos como recompensa. Para maximizar nuestros beneficios, añadiremos AAVE entre la salida de Augury y el depósito en las bóvedas de Mai Finance, ya que 3 de los 5 tokens que cosecharemos se pueden depositar en AAVE.

![Estrategia de farming con las stablecoins USDT-UST ](<../.gitbook/assets/image (31).png>)

### Curve

Curve es un proyecto "blue-chip" que recompensará a los usuarios que presten tokens "blue-chip". La recompensa se compone de tokens auto-compuestos (añadidos automáticamente a la inversión inicial), tokens WMATIC y tokens CRV, que son 2 tokens que también se aceptan como colateral en Mai Finance.

Una de las cosas más interesantes de Curve y sus pools es que no hay que depositar una cantidad exacta de cada token para un determinado pool. En su lugar, se puede proporcionar un único token y el algoritmo que gestiona el pool ajustará automáticamente los otros tokens vendiendo una parte del depósito y comprando los otros tokens para mantener un ratio correcto en el pool. 

Utilizaremos el pool _atricrypto3 _que acepta cualquier combinación de WBTC/WETH/USDC/USDT/DAI y añadiremos a este pool los USDC que serán generados por el pool en Augury.

![Detalles del pool atricrypto3 en Curve en Septiembre de 2021](<../.gitbook/assets/image (32).png>)

### AAVE

Como se menciona en el apartado sobre Augury, AAVE se utiliza para añadir una pequeña recompensa adicional a los tokens producidos en Augury antes de que los utilicemos en Mai Finance. En lugar de depositar nuestros WBTC, WETH y WMATIC directamente en Mai Finance, depositaremos estos tokens en AAVE y utilizaremos la funcionalidad de [Yield ](https://app.mai.finance/yield)de Mai Finance para auto-componer las recompensas de AAVE en los pools de amToken, y utilizaremos los camToken como colateral en las bóvedas de Mai Finance. Puedes obtener más detalles sobre esta parte leyendo el [tutorial sobre los tokens AAVE](apalancamiento-con-tus-tokens-de-aave.md).

![Las recompensas al depositar en AAVE en Septiembre de 2021](<../.gitbook/assets/image (33).png>)

### Balancer

Balancer es otro proyecto "blue-chip" como Curve. Podrás depositar determinados tokens en pools compuestos por más de 2 tokens, donde podrás depositar un único token. El pool se equilibrará automáticamente para obtener una proporción igual de cada token que compone el pool. 

Para nuestra estrategia, utilizaremos el pool WETH/BAL/Qi/MAI/USDC. Este pool aceptará el token Qi que se generará en las bóvedas de Mai Finance, y nos recompensará con Qi adicional, y tokens BAL que podremos depositar en Mai Finance en la bóveda BAL, permitiéndonos generar más MAI y aumentar nuestra posición al hacer farming en Augury.

![Estadísticas del pool de Balancer en Septiembre de 2021](<../.gitbook/assets/image (34).png>)

## Poniendo en marcha el sistema

![](<../.gitbook/assets/image (35).png>)

Lo que viene a continuación es una simulación realizada con una inversión inicial de 1.000 dólares de ETH que se deposita en la bóveda de camWETH para pedir prestados 500 dólares en forma de MAI, convertidos posteriormente en 500 dólares del par USDT-UST. Para poder realizar la simulación de este sistema se han tenido en cuenta los siguientes APRs:

* APR del par USDT-UST 22.53%
* APR de amWBTC de 0.39%
* APR de amWETH de 1.71%
* APR de amWMATIC del 3.80%
* APR de atricrypto3 del 3.86% con tokens LP auto-compuestos, 13.09% de WMATIC y 17.63% de CRV
* APR del pool de 5-tokens de Balancer del 43.46% con un ratio BAL:Qi de 1:6
* APRs de los préstamos incentivados
  * 23.28% de camWBTC
  * 21.52% de camWETH
  * 32.93% de camWMATIC
  * 24.51% de LINK
  * 116.71% de CRV
  * 62.38% de BAL

Todas estos APRs están sujetos a cambios en las diferentes plataformas, y no hay garantía de que se mantengan durante todo un año, sin embargo, las supondremos como constantes para esta simulación con el fin de hacernos una idea del APR global del sistema. Para "simplificar" aún más la simulación, no tendremos en cuenta las variaciones de precios ni las comisiones por transacción. También hay que tener en cuenta que esta simulación tiene en cuenta que las recompensas de los préstamos incentivados de Mai Finance y las recompensas de Balancer se componen diariamente en lugar de semanalmente, pero estas recompensas actualmente se envían semanalmente a la cartera de los usuarios. Por último, para esta simulación, supondremos que el **CDR **(Collateral to Debt Ratio) es siempre del 200%, lo que significa que sólo pedimos prestado la mitad de lo que depositamos para seguir recibiendo las recompensas, para así reducir el riesgo de ser liquidado fácilmente.

### Día 1

Si todavía tienes tus 1.000 dólares en WETH, deposítalos en AAVE para obtener amWETH, luego deposita tus amWETH en[ Mai Finance](https://app.mai.finance/yield) para obtener camWETH, y finalmente deposita tus camWETH en la bóveda correspondiente para poder pedir prestados 500 MAI. 

Utiliza [Anchor ](https://app.mai.finance/anchor)para convertir tus MAI en USDT (o puedes utilizar otro DEX como [QuickSwap ](https://www.quickswap.org/#/swap)si no hay liquidez en Anchor), luego puedes utilizar [DFYN ](https://exchange.dfyn.network/#/swap)para intercambiar el 50% de tus USDT en UST y formar un par USDT-UST que luego podrás depositar en [Augury](how-to-combine-farming-and-borrowing-rewards.md#intro). Tenga en cuenta que también necesitará algunos OMEN que también puede comprar en QuickSwap.

 Por lo tanto, al final del Día 1, obtendremos las siguientes recompensas:

| Tipo de Recompensa | Valor en dólares |
| ------------------ | ---------------- |
| WBTC del farming   | 0.123            |
| WETH del farming   | 0.031            |
| WMATIC del farming | 0.031            |
| LINK del farming   | 0.031            |
| USDC del farming   | 0.092            |
| Qi de las bóvedas  | 0.295            |

Estas serán las recompensas que obtendremos al hacer farming y pedir prestado en el 1º Dia

### Día 2

Las recompensas se cosechan, WBTC, WETH y WMATIC es enviado a las bóvedas correspondientes en Mai Finance después de pasar por AAVE y la funcionalidad de Yield de Mai Finance. LINK es depositado directamente en la bóveda de LINK, y el USDC es enviado a Curve en el pool de atricrypto3. La recompensa en forma de Qi es enviada a Balancer. En este punto, podremos pedir prestado más MAI en las 3 bóvedas de camTokens y en la bóveda de LINK (0,13 dólares de MAI para ser exactos) y podremos crear más pares USDT-UST a partir del MAI que hemos pedido prestado. 

Por lo tanto, al final del Día 2, obtendremos las siguientes recompensas

| Tipo de Recompensa            | Valor en dólares |
| ----------------------------- | ---------------- |
| WBTC del farming              | 0.123            |
| WETH del farming              | 0.031            |
| WMATIC del farming + Curve    | 0.031            |
| LINK del farming              | 0.031            |
| USDC del farming              | 0.093            |
| Recompensas de CRV en Curve   | 0.00004          |
| Recompensas BAL               | 0.00005          |
| Recompensas Qi de las bóvedas | 0.296            |

Llegados a este punto, el sistema está listo y las recompensas fluyen de manera que cada paso alimenta al siguiente, creando así un bonito bucle.

## Resultados del Farming

### Rutina Diaria

La rutina diaria estará compuesta por los siguientes pasos:

* Cosechar recompensas en Augury
* Depositar WBTC, WETH y WMATIC en AAVE
* Depositar amWBTC, amWETH y amWMATIC en Mai Finance en la funcionalidad de Yield
* Depositar camWBTC, camWETH ycamWMATIC en sus respectivas bóvedas en Mai Finance
* Depositar LINK en la bóveda de LINK en Mai Finance
* Depositar USDC en el pool atricrypto3 de Curve
* Cosechar WMATIC de Curve y depositarlos en la bóveda de camWMATIC 
* Cosechar CRV de Curve y usarlos en la bóveda de CRV
* Pedir prestado MAI en las distintas bóvedas
* Convertir MAI a USDT en Mai Finance usando Anchor
* Convertir el 50% del USDT a UST usando DFYN
* Crear el nuevo par LP USDT-UST en DFYN
* Depositar los nuevos tokens LP en Augury

### Rutina Semanal

Además, obtendrás recompensas semanales en BAL (de tu depósito de Qi en Balancer) y tokens de Qi (de los préstamos incentivados). Por lo que tendrás que:

* Depositar el token Qi en Balancer
* Depositar el token BAL en la bóveda BAL de Mai Finance
* Pedir prestado MAI gracias al nuevo BAL depositado y convertirlos al par USDT-UST para hacer farming en Augury

### Resultados mensuales aproximados

| Mes | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
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

Cabe destacar:

* El crecimiento en la posición del USDT-UST es el resultado de los MAI que se han pedido prestados gracias a las bóvedas
* El pool de CRV es casi inexistente debido a la muy baja cantidad de USDC depositados en Curve
* La bóveda de BAL no es importante debido a que el 14,28% de la recompensas de Balancer se pagan en tokens BAL, el resto se paga en tokens Qi
* La cantidad en el pool de Balancer es la mayor ganancia, y es sólo el resultado de las recompensas de las bóvedas y de Balancer

### Día 365

Tras haber transcurrido un año, el estado final de nuestra inversión es el siguiente:

| Posición    | Valor en dólares |
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

La deuda total es el total de la posición del par USDT-UST, que son $553.24, y la recompensa final generada es de $280.63, lo que es aproximadamente un APY del 28.06%.

### Comparación con otras estrategias

Obtener un APY del 28% usando estrategias de farmeo con monedas estables no está nada mal, pero ¿Cómo se compara esto con otras estrategias más fáciles que podríamos aplicar con el valor inicial de 1.000 dólares de ETH? Comprobemos el APY final de las siguientes estrategias: 

* Apalancamiento de x8 de amWETH a través de AAVE: para ello, utilizaremos el flujo exacto descrito en el[ artículo de tokens de AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/es/tutoriales-de-inversion/apalancamiento-con-tus-tokens-de-aave).
* Farming de monedas estables en Augury: para esta estrategia, vendemos el WETH y cultivamos con 1.000 $ de USDT-UST en la misma Infusion en Augury
* Farming de monedas estables en QuickSwap: para esta estrategia, utilizaremos la bóveda de camWETH para beneficiarnos de la recompensa de la bóveda, y haremos farming con 500 $ de MAI en QuickSwap (MAI-DAI al 19. 78% APY), utilizando la bóveda de dQUICK en Mai Finance para pedir prestado MAI adicional y reinvertirlo en la granja de rendimiento (las bóvedas de dQUICK tienen un APR del 55,72%)

| Estrategia                            | APY Final |
| ------------------------------------- | --------- |
| Estrategia presentada en esta guía    | 28.06%    |
| Incrementa tus AAVE tokens x8         | 46.46%    |
| Farming de stables en Augury          | 22.53%    |
| Farming en Quickswap + bóveda dQUICK  | 35.96%    |

## Descargo de Responsabilidad

Esta estrategia es realmente interesante y utiliza la mayoría de las bóvedas de Mai Finance, y esta guía se ha escrito principalmente para mostrar que, a partir de Septiembre de 2021, esta es la parte que generaría más recompensas al famear monedas estables. Sin embargo, esta estrategia puede ser la más tediosa, ya que implica muchas operaciones en varias plataformas. Por último, Augury es una herramienta fantástica que genera tokens específicos que pueden incluirse en varias estrategias, pero probablemente no en el farming con stablecoins. Y como nota adicional, no se han tenido en cuenta las comisiones de depósito ni de rendimiento a la hora de calcular el APY final.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta o DYOR
{% endhint %}
