---
description: >-
  Este artículo es una explicación detallada acerca de cómo puedes usar Mai
  Finance para pedir prestado MAI al 0% de interés, donde te pagarán por
  hacerlo, haciendo el interés del préstamo negativo.
---

# Préstamos de MAI y Depósitos Incentivados

## Introducción

El negocio principal de Mai Finance es ser una plataforma de préstamos. En vez de vender sus crypto para comprar otros activos, la gente será capaz de bloquear sus activos en Mai Finance y pedir prestado gracias a éste. Esto presenta una oportunidad de mantener tus activos valiosos (WBTC, WETH …) mientras puedes obtener otros activos y participar en granjas de rendimiento. En ese caso, el préstamo es usado para generar beneficios adicionales mientras que el colateral gana valor.

Otra de las ventajas principales al usar Mai Finance es que no hay ninguna fecha para realizar el pago de la deuda. Dicho de otra manera, puedes pedir prestado la stablecoin MAI gracias al colateral depositado, no tienes que pagar ningún interés y puedes saldar tu deuda cuando lo creas conveniente. Véase los artículos sobre el [pago de la deuda](debt-repayment-why-and-when.md) para saber los detalles. La única comisión que tendrás que pagar es la cuota de pago correspondiente al **0.5%** del dinero que has pedido prestado cuando pagas tu préstamo, esto será cogido directamente del colateral que hayas depositado

Por ejemplo, si has depositado $200 de WETH para pedir prestado $100 de MAI, cuando vayas a pagar tu préstamo tendrías que pagar $0.50 que serán tomados de tu depósito de WETH .

Además de esta increíble oportunidad, el equipo de Mai Finance introdujo en Septiembre de 2021 incentivos en los préstamos  pagados en Qi, el token nativo de Mai Finance. Es decir, al depositar tus activos en Mai Finance en una bóveda (vaults) para pedir prestado MAI, recibirás dinero extra al hacerlo. Este artículo explica de forma detallada cómo funciona esta funcionalidad.

## Bóveda - ¿Qué son y cómo funcionan?

### Creación de la bóveda

En Mai Finance, las bóvedas (vaults) son un tipo de almacenamiento especial donde puedes depositar tus activos. Actualmente, hay 10 tipos de bóvedas:

![Los distintos tipos de bóvedas que puedes crear en Mai Finance](<.gitbook/assets/image (8).png>)

Hay 2 tipos diferentes de bóvedas:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

y

* camWETH
* camWBTC
* camWMATIC
* camAAVE

Las 6 primeras bóvedas son para activos "simples"  mientras que los 4 últimos son camTokens. Los camTokens son los encargados de hacer compounding con los tokens de mercado de  AAVE, es decir, es la representación de un depósito que se hace en AAVE, y luego éste es depositado en las granjas de rendimientos (yield pools) de Mai Finance. Mientras tus activos están generando rendimiento en AAVE (y éstos son automáticamente compuestos ), puedes pedir prestado MAI al depositar estos tokens.

Cabe destacar, en la imagen superior se puede observar una información importante respecto a la creación de las bóvedas

* **MAI disponible**: corresponde al techo máximo de deuda, el número máximo de MAI que puede ser creado en el deposito de las bóvedas.
* **Min Coll. ratio**: El Ratio de Colateral a Deuda(CDR) mínimo para esa bóveda.
* **Vault incentives APR** (esto será tratado más tarde en el artículo).

### Entendiendo el techo de deuda

El número máximo de MAI que uno puede crear en una bóveda depende de la cantidad de activo que haya sido depositado en ésta. El techo de deuda ha sido implementado para asegurarse de que el mercado no se encuentra inundado con MAI en un periodo corto de tiempo, lo que podría afectar al precio de la stablecoin.

Por ejemplo, si una gran institución financiera depositara 5,000 WBTC de una sola vez y pidiera prestado $100,000,000 de MAI, intercambiando ese MAI por más WBTC, esto podría afectar al precio de MAI haciendo que peligre la estabilidad del precio de $1 de MAI, poniendo en riesgo a toda la plataforma. El techo de deuda es el mecanismo que previene que esto ocurra: hay una cantidad máxima de MAI que puede ser creado en cada tipo de bóveda-

Cuando el techo de deuda es alcanzado (ya no se puede crear mas MAI), el tiempo en el cual ha ocurrido esto es guardado, y el sistema incrementará automáticamente el techo de deuda pasadas unas 48 horas. Esto es tiempo suficiente para que el precio de MAI se estabilice (en caso de que haya una gran presión de venta siguiendo una gran venta de MAI).&#x20;

Esto significa que en 48 horas, nadie podrá pedir prestado mas MAI en una bóveda que ha alcanzado el techo de deuda, a no ser de que se pague una deuda en ese tiempo.

Además, cuanto más MAI haya en el mercado, su precio será mas estable. Ya que, si hubiera una gran venta de MAI ésta sería menos "invasiva" cuanto más  MAI haya en circulación.  Esto se entiende mejor así:

* Si alguien vendiera 1,000 MAI cuando hay 10,000 MAI en circulación, la venta supondría el 10% del MAI circulante.
* Si alguien vendiera 1,000 MAI cuando hay 10,000,000 MAI en circulación, la venta supondría el 0.01% del MAI circulante

Esto hace que el techo de la deuda no sea aumentado incrementalmente, sino exponencial: cuanto más MAI haya en circulación, menor será el impacto que una gran venta pueda tener,  así que el techo de venta puede ser incrementado incluso más.

{% hint style="info" %}
Cuando pides prestado MAI,  puede ocurrir que la cantidad de MAI que puedes pedir se encuentre limitado por el techo de deuda, independientemente del valor del colateral depositado y la cantidad de MAI que ya hayas pedido prestado. Cuando ese sea el caso, sería recomendable esperar 48h antes de que puedas pedir prestado más MAI.
{% endhint %}

### Entendiendo el Ratio de Colateral a Deuda

El **CDR**, o **R**atio **** de **C**olatera**l** a **D**euda **** es el ratio entre el valor que has depositado en Mai Finance y la cantidad de MAI que has pedido prestado.

Por ejemplo, si has depositado $200 de WETH para pedir prestado $100 de MAI, tu **CDR** sería de:

$$
CDR=\frac{ValorColateral}{ValorDeuda}=\frac{200}{100}=200\%
$$

Manteniendo un CDR superior al 100% significa que hay mas colateral que deuda. Esto es obligatorio para así asegurarse que MAI está **sobre-colateralizado**, esto es uno de los principios de los tokenomics de Mai Finance. Puedes obtener más detalles acerca de esto en la [documentación de Mai Finance](https://docs.mai.finance/stablecoin-economics).

Cada tipo de bóveda tiene un CDR determinado, esto es una marca que sirve de referencia para considerar si una bóveda se encuentra en riesgo ya que la cantidad de MAI prestada podría no ser respaldada por la suficiente cantidad de colateral. Llegados a ese punto, cualquiera podría liquidar la bóveda, haciendo que parte de esa deuda sea pagada por un liquidador, obteniendo como recompensa parte del colateral. Lo dicho, puedes obtener más información acerca del proceso de liquidación en la documentación oficial.

Cuando pides prestado MAI en contra de un colateral depositado, podrás obtener cual es la cantidad máxima de MAI que puedes pedir prestada, y cuál sería el impacto en tu ratio de "salud" dependiendo de la cantidad prestada, tal y cómo se puede ver en la imagen inferior:

![Variación de la "salud" del préstamo dependiendo de la cantidad prestada](<.gitbook/assets/image (2).png>)

Es muy importante echarle un ojo a tu **CDR** y mantener un ratio saludable para:

* Evitar ser liquidado
* Incrementar la "salud" de toda la plataforma de Mai Finance al asegurarte de que la cantidad de MAI circulante tiene colateral que lo respalde.

Un CDR "sano", definido por el equipo de Mai Finance , es entre el 25% y el 270% sobre el valor mínimo del CDR. Además, puedes ver nuestras guías sobre estrategias sobre como puedes usar CDRs agresivos/conservadores para [invertir](tutoriales/polygon/apalancamiento-con-tus-tokens-de-aave.md#examples-with-numbers) en otros proyectos, o [pagar tu deuda](debt-repayment-how.md) usando tu deuda.

## Préstamos incentivados

### Entendiendo los APRs de los prestamos incentivados

En Septiembre de 2021, Mai Finance introdujo los préstamos incentivados. Esta es una recompensa distribuida por el equipo de Mai Finance para cualquiera que pida prestado MAI y participe en el crecimiento de la plataforma

Cada tipo de bóveda (entre los 10 tipos existentes) reciben 0.05 Qi por bloque, que es distribuido a aquellos usuarios que tengan un CDR sano. El APR de la bóveda es definido por la cantidad de MAI que hayan pedido prestada.

Por ejemplo, Ben y Kila son 2 amigos que han depositado su ETH en la bóveda de  WETH en Mai Finance.

* Ben ha depositado el equivalente de $2,000 de ETH y ha pedido prestado 1,000 MAI.
* Kila ha depositado el equivalente de $10,000 de ETH y ha pedido prestado 6,000 MAI.

La cantidad actual de MAI prestado en la bóveda de WETH asciende a 1,000,000 MAI.

Ben y Kila están cualificados para acceder a esas recompensas ya que Ben tiene un CDR del 200%y Kila un CDR del 166.67%. Ben, con su préstamo, tiene el 0.1% de la cantidad total prestada, mientras Kila tiene el 0.6%.

La cantidad total de Qi distribuida a la bóveda de WETH (o cualquier otra) es:

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86 400 es el número de segundos que tiene un día, y en Polygon, el tiempo de bloque es de 2 segundos, lo que significa que la cantidad total de bloques que se producirán en Polygon en un día será 86,400 / 2 = 43,200. Por lo que la emisión de cada tipo de bóveda es 2160 Qi /día

**Nota:** El tiempo de bloque se ha incrementado últimamente a 2.6 segundos. Sin embargo, todos los APRs y APYs mostrado en las apps suponen un tiempo de bloque de 2 segundos. Por favor haga su propia investigación y vea el tiempo de bloque actual [PolygonScan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Si el estado de la bóveda se mantuviera constante, Ben obtendría el 0.1% de los 2160 Qi distribuidos, mientras que Kila obtendría el 0.6%.

* Ben obtendría 2.16 Qi cada día, lo que es una recompensa diaria del 0.0216%, o un APR del 78.84%
* Kila obtendría 12.96 Qi cada día, lo que es una recompensa diaria del 0.0216%, o un APR del 78.84%

Cabe destacar que, 2160 Qi de 10,000,000 MAI, hace que la recompensa diaria sea del 0.216%, o 78.84%, el cual es el APR de la bóveda.

{% hint style="info" %}
Es fácil de ver que el APR de la bóveda esta relacionado con la cantidad de MAI prestada. Cuanto más MAI sea prestado, menor será el APR. Recuerda, que la cantidad de MAI que puede ser prestada esta limitada por el techo de deuda, el cual se incrementado dependiendo de la demanda de MAI.
{% endhint %}

Para verificarlo, podemos calcular el APR teórico para la bóveda de MATIC usando los números que nos proporciona las [estadísticas ](https://app.mai.finance/analytics)de Mai Finance. La cantidad de MAI prestada en la bóveda de MATIC es 785 328. La recompensa es de 2160 Qi por día en esa bóveda. Eso corresponde a un APR del:

$$
APR=\frac{RecompensaQi * PrecioQi}{MAI_{prestado}}*365=\frac{2160 *0.441}{785328 }*365=44.29\%
$$

Esto da como resultado aproximadamente el APR existente al crear una bóveda en Mai Finance, ten en cuenta que la cantidad de MAI prestado y el precio de Qi variarán con el tiempo por lo que el APR no sera siempre el mismo.

![APR de la bóveda de MAI en el lanzamiento de los préstamos incentivados](<.gitbook/assets/image (23) (2) (3) (2).png>)

### Calculando los APRs iniciales

Usando los mismos datos que en el ejemplo anterior, podemos calcular el APR inicial de cada tipo de bóveda:

| Tipo de bóveda | APR Inicial |
| -------------- | ----------- |
| MATIC          | 44.29%      |
| WETH           | 24.03%      |
| LINK           | 27.41%      |
| AAVE           | 164.14%     |
| CRV            | 159.96%     |
| WBTC           | 36.92%      |
| camWETH        | 25.46%      |
| camWMATIC      | 44.33%      |
| camAAVE        | 167.23%     |
| camWBTC        | 47.38%      |

{% hint style="info" %}
Como puedes ver, algunas bóvedas generarán mas recompensas que otras. Además, puedes observar que es muy importante depositar tus activos lo antes posible para así poder beneficiarte de estos jugosos APRs antes de que el techo de deuda se incremente, bajando consecuentemente el APR.

Además si decidieras mantener tu préstamo por más de un año, la cuota del 0.5% será compensada totalmente por el programa de recompensas.&#x20;
{% endhint %}

### Distribución de los incentivos

Las recompensas de los prestamos incentivados serán distribuidas de la misma forma que las recompensas al hacer staking de Qi. Cada miércoles, el Qi será distribuido de forma automática a tu cartera.

## FAQs de los préstamos incentivados

* &#x20;**¿Cuáles son las bóvedas que recibirán recompensas?**

A día de hoy, todos los tipos de bóvedas recibirán recompensas en forma de Qi

* &#x20;**¿Cuántas recompensas serán entregadas a los prestamos incentivados?**

0.05 Qi/ bloque para todas las bóvedas

* **¿Cuánto MAI tengo que pedir prestado para poder recibir las recompensas?**

&#x20;Para los prestamos incentivados, deberás mantenerte por encima del 25% hasta 270% del ratio de liquidación para poder recibir el airdrop de QI token. Esto significa:

* &#x20;_Matic_ - Ratio de liquidación 150% - Para poder recibir recompensas deberás estar entre 175% y 420%&#x20;
* _Tokens_: - Ratio de liquidación 130% - Para poder recibir recompensas deberás estar entre 155% y 400%&#x20;
* _CamTokens_: - Ratio de liquidación  135% - Para poder recibir recompensas deberás estar entre 160% y 405%



* &#x20;**¿Cómo puedo comprobar si mi bóveda recibirá las recompensas?**

Si ves el emoticono del fuego en el overview de tu bóveda, ésta estará generando recompensas

* &#x20;**¿Cuántas recompensas recibiré?**

Tus recompensas finales están basadas en la cantidad de MAI que hayas pedido prestada en comparación con la cantidad total de MAI que se haya pedido prestada en cada tipo de bóveda&#x20;

* &#x20;**¿Cuánto tiempo duraran los prestamos incentivados?**

La duración del programa de incentivos es de 3 meses, sin embargo, la DAO puede proponer una votación o para terminar este programa de incentivos antes de tiempo o extender el programa

* **¿Cómo recibiré las recompensas?**

Qi será enviado a tu cartera automáticamente (airdrop)

* **¿Cómo se comprueba en que bloques tendré recompensas?**

Podrás recibir las recompensas dependiendo del bloque en el que hayas bloqueado, ya que recibirás recompensas acorde a los bloques en los que hayas participado.&#x20;

* **¿Cuándo empiezan a calcularse las recompensas semanales?**

Seguiremos el mismo calendario que eQi. Puedes comprobar el numero de bloque en la pagina **boost**

## Descargo de responsabilidad

Los APRs mostrados a lo largo de este articulo están sujetos a cambios por lo que dependiendo de cuando leas el documento, éstos pueden ser distintos. Recuerda que la cantidad de MAI prestada, el techo de deuda y el valor del token Qi pueden afectar a los APRs de las distintas bóvedas. Por favor, asegúrese de que invierte responsablemente.

{% hint style="info" %}
Ten en cuenta que una estrategia que funciona bien en un momento dado puede funcionar mal (o hacerle perder dinero) en otro momento. Mantente informado, controla los mercados, controla tus inversiones y, como siempre, haz tu propia investigación.
{% endhint %}
