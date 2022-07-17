---
description: >-
  Este artículo explica en detalles que puedes hacer con tu Qi, el token nativo
  de Mai Finance, en Polygon. Además analizaremos si Qi es una buena oportunidad
  de inversión y qué afecta al precio.
---

# ¿Qué hacer con Qi en Polygon?

## Introducción

Qi (o chi), es el token nativo de Mai Finance. Algunos lo usan para votar en QIP (Propuestas de Mejora de **Q**iDAO), algunos hacen staking para poder acumular más Qi, mientras que otros lo usan para hacer farming. Puedes encontrar información acerca de como usar Qi en Mai Finance en este [artículo](../../earning-passive-income-with-qidao.md).

Este artículo, como en la mayoría de artículos sobre inversión existentes en esta guía, estará centrada en como farmear y recolectar rendimientos, pero usando el token Qi. Además, veremos como podemos generar mucho Qi, y como puedes usarlo en distintas aplicaciones en Polygon.

Los granjeros humildes te dirán que tienes que mantenerte humilde, vender lo que recolectas y tomar beneficios. Sin embargo, prefiero decir lo siguiente:

> Dale a un hombre un pescado y podrá alimentarse por un día. Enséñale a pescar y se alimentará toda su vida.

Así qué preparen sus cañas de pescar, y sigan la guía.

## ¿Qué hacer con Qi en Polygon?

### Staking

No nos detendremos mucho en este apartado puesto a que ya hay una guía sobre este concepto. Sin embargo, me gustaría destacar que Mai Finance al recoger beneficios, estos son redistribuidos en gran parte a los stakers de Qi. Hacer staking de tu Qi en Mai Finance es una de las mejores estrategias para usar Qi, además a fecha de Septiembre de 2021, aproximadamente el 23% de todo el Qi circulante esta bloqueado en una media de 2 años.

### Farming de Pares de Proveedor de Liquidez

De nuevo, ya hay varias guías acerca de como puedes incluir el token Qi en tus estrategias de farmeo para generar rendimientos y nunca vender tus token de la granja. Si quiere obtener mas información acerca de esto, véase [Acumula Dapps como si fueran cromos](acumula-dapps-como-cromos.md) y [¿Farmear o hacer staking?](farming-or-staking-or-both.md)

Recuerda que aquí, Qi se junta con otro token para poder formar un par LP (**P**roveedor de **L**iquidez) en [QuickSwap](https://quickswap.exchange/#/quick) para que puedas hacer farming de lo siguiente:

* Qi-WMATIC en Mai Finance y obtener tokens Qi como recompensa
* Qi-WETH en QuickSwap y obtener tokens Quick como recompensa
* Qi-QUICK en QuickSwap y obtener tokens Quick como recompensa

![LP pool on QuickSwap for the Qi-WETH pair](<../../.gitbook/assets/image (19) (2) (1) (1) (1) (1).png>)

### Farming solo con Qi

Qi puede ser utilizado únicamente en [Impermax](https://polygon.impermax.finance). Impermax es una plataforma donde podrás apalancar un token LP varias veces para aumentar tus ganancias en QuickSwap.

Funciona de la siguiente manera, pedirás prestado los 2 tokens que forman el par LP, los combinarás para tener mas tokens LP, obteniendo así una mayor posición. En la mayoría de casos, los interés del préstamo son compensados por el APR del farming, obteniendo así resultados netos positivos

![Posicion apalancada en Qi-WETH en Impermax](<../../.gitbook/assets/image (10).png>)

Podemos ver que el APR al apalancarnos x5 es de 393.88%, basado en el APY del 239.68% en QuickSwap.

{% hint style="info" %}
Destacar que Impermax da APRs (**P**orcentaje de **R**ecompensas **A**nual) aproximado mientras que QuickSwap da APYs (**P**orcentaje de **R**endimiento **A**nual) aproximado, es decir, que QuickSwap supone que compones tus recompensas diariamente. El APY del 239.68% en QuickSwap corresponde aproximadamente a un APR del 122.49%.
{% endhint %}

En Impermax, para pedir prestado Qi y WETH para poder apalancar tu posición, los necesitas obtener de algún sitio. Esto es posible gracias a que otros usuarios (o tu mismo) suministran ambos tokens por separado. Cuánto más veces se pida prestado un token, mayor será el interés al pedir prestado, lo que hará que el APR final sea inferior, incluso haciendo que a veces se convierta en negativo.

![Las estadisticas de Qi y WETH en Impermax para formar el par Qi-WETH](<../../.gitbook/assets/image (11).png>)

En este ejemplo, nos centraremos únicamente en Qi. Como se puede observar en la imagen superior, el suministro total de Qi es de $427.21 y la cantidad usada para apalancar tu posición es de $321.44, obteniéndose así un porcentaje de uso del 75.24%. Impermax tiene un mecanismo interno que calcula automáticamente el APR de suministro (APR que la gente que preste Qi obtendrá) y el APR de préstamo (porcentaje de la recompensa farmeada que será deducida para pagar el préstamo).

Esto significa que puedes suministrar Qi a Impermax y obtener, en nuestro ejemplo, un APR del 43.73% , en el momento que ha sido escrito el artículo. Ya que la oferta y demanda variará, el APR de suministro se incrementará / disminuirá. Cuando suministras tokens a Impermax, obtendrás como recompensa el token que hayas suministrado, lo que significa que esta estrategia te hará acumular mas Qi con el tiempo.

Mientras uses Impermax, puedes usar la opción de apalancamiento para obtener tokens IMX. Por favor, léase el artículo de [Acumula Dapps como si fueran cromos](acumula-dapps-como-cromos.md) para obtener mas información acerca de cómo usar Impermax en tu estrategia de farmeo.

### Balancer

Balancer es una buena herramienta para cualquier estrategia, especialmente en aquellas que incluyan Qi y/o MAI. Balancer propone un un equivalente al farmeo con par LP, pero con más de un token suministrado en un ratio de 1:1. La piscina puede tener 3, 4 o 5 tokens (algunas veces incluso más) con diferente peso, y el algoritmo del programa se encargará de que el ratio de cada token se respete, vendiendo algunos tokens y comprando otros para mantener el equilibrio.

La piscina que vamos a usar en este ejemplo tiene Qi, WMATIC, BAL, USDC y MAI. Esta piscina te dará recompensas en forma de tokens Qi y BAL , y como se puede ver en la imagen, podrás componer ambas en la piscina. Porque otras de las grandes ventajas de Balancer, es que no necesitas suministrar todos los token en su respectivo ratio, ya que el algoritmo lo hará por ti. Es decir, podrías suministrar únicamente Qi en la piscina, y el algoritmo se encargará de reequilibrar el resto.

![Detalles de la piscina a fecha de Septiembre de 2021](<../../.gitbook/assets/image (12).png>)

Además, los tokens BAL pueden (o dentro de poco podrán) ser usados como colateral en Mai Finance, lo que significa que podrás guardar tus tokens BAL en la bóveda de BAL en Mai Finance, y pedir prestado MAI con ellos de colateral. Incluso, al pedir prestado MAI en gracias a tus tokens BAL depositados, podrás recibir recompensas de Qi que podrán ser suministradas a la piscina de Balancer.

![Bucle cerrado usando Mai Finance y Balancer](<../../.gitbook/assets/image (13).png>)

El APR de las bóvedas de BAL dictará si es interesante incluir la bóveda en el bucle, o si es mejor depositar tu Qi directamente en Balancer .

## Entendiendo el precio de Qi

Obtener muchos Qi es una cosa, sin embargo, si el precio de este token de devalúa con el tiempo, ¿es buena estrategia mantenerlo? En esta parte del artículo, veremos cuáles son los diferentes factores que afectan al precio de Qi, para que cuando empieces a invertir tus Qis, puedas tener una idea de cómo puede variar el precio y que impacto puede tener en el ecosistema de Qi.

### Emisión de Qi

Uno de los principales factores que afectan al precio de Qi, es el ritmo en el que éste es creado. Ya que, el precio viene dictado por la relación entre la oferta y demanda. Si hay mucha oferta pero muy poca demanda, el precio naturalmente bajará. De ahí, la importancia de saber cómo se genera Qi para estimar su valor con el paso del tiempo.

Actualmente hay 2 fuentes de emisión de Qi: las recompensas al hacer farming y los préstamos incentivados.

![Las granjas de LP en Mai Finance en September de 2021](<../../.gitbook/assets/image (16).png>)

Si estas farmeando rendimientos en MAI Finance, tienes la opción de elegir o el par MAI/USDC o el par Qi/WMATIC (a fecha de Septiembre de 2021).

* El par MAI/USDC es recompensado por 0.5 Qi / bloque
* El par Qi/WMATIC es recompensado por 1 Qi / bloque

En Polygon, el tiempo en el que se generan cada bloque es de 2 segundos, y al haber 86 400 segundos en un día, significa que el par MAI/USDC es recompensado con 21,600 Qi cada día, y el par Qi/WMATIC con 43,200 Qi.

Las piscinas de Mai Finance son responsables de la creación de 64,800 Qi cada día.

Respecto a las bóvedas, cada una de ellas genera 0.05 Qi / bloque, con una emisión diaria de 2 160 Qi, y al haber actualmente 10 bóvedas, se obtiene un total de 21 600 Qi distribuidos como recompensa para los préstamos incentivados

Esto significa que cada día, 86 400 Qi son creados y distribuidos a sus usarios.

### Optimizadores de rendimiento

Los optimizadores de rendimiento son plataformas que compondrán automáticamente las recompensas con unas estrategias predefinidas, y te dan recompensas adicionales por usar la plataforma. Sin embargo, una gran parte de las recompensas recogidas son vendidas directamente, y reusadas por la plataforma de otra forma.

Por ejemplo, Adamant ofrece farmear el token LP del par Qi/WMATIC LP en su plataforma, con la siguiente distribución de recompensas:

![El par Qi-WMATIC en Adamant](<../../.gitbook/assets/image (15).png>)

![Detalles del APR del 179.23% garantizado por Adamant](<../../.gitbook/assets/image (14).png>)

Puedes observar que el APR ofrecido en Adamant es superior al de Mai Finance, esto se debe a que Adamant está distribuyendo tokens ADDY a los granjeros. La cantidad de Qi que es distribuida al granjero es del 98.45% comparado al 134.42% que puedes obtener en Mai Finance.

De esta recompensa del 98.45%, la mitad de esta es vendida para comprar WMATIC y formar tokens LP adicionales que son distribuidos al granjero directamente.

Con 100$ de LP, asumiendo que el APR y el precio de los tokens se mantienen constante por un año, y asumiendo de que no compones tus recompensas, obtendrías esto tras un año de farming:

* $134.42 de Qi adicional en Mai Finance
* $98.45 de Qi/WMATIC, o $49.23 de Qi adicional en Adamant

Esto significa que, $85.20 en forma de Qi es vendido directamente al mercado, lo que es mas del 60% de la emisión generada por la piscina de Adamant .

Sin embargo, Adamant no es la única plataforma que ofrece esto. Otros plataformas que hacen lo mismo son Beefy Finance o Kogecoin. De los $4.9M **TVL** (Valor Total Bloqueado) en la granja de Qi/WMATIC en Mai Finance, $2.3M vienen directamente de Adamant, $41k de Beefy y $12k de Kogecoin, haciendo que estas 3 plataformas representen mas del 50% del TVL del par en Mai Finance. Se podría llegar a la estimación de que aproximadamente el 30% de la emisión total de Qi es vendida por estas plataformas, creando así una gran presión de venta, disminuyendo su precio, lo que podría explicar por qué Qi tiene algunas dificultades para mantener un precio elevado.

### Entendiendo los pares LP

Cuando haces farming de rendimientos usando pares LP , el token LP es usado para suministrar liquidez a aquellos usuarios que están intercambiando un token por otro. En nuestro ejemplo de Qi/WETH, cuando alguien esta comprando WETH, parte del token puede ser quitado del par LP y vendido al usuario que lo haya solicitado.

Llegados a este punto, ya que parte del WETH ha sido quitado, hay un desequilibrio en el par: hay menos WETH para la misma cantidad de Qi. El algoritmo encargado de mantener el ratio a 1:1 venderá Qi de la piscina, para poder recomprar WETH y volver a obtener un ratio 1:1. Lo contrario pasa cuando hay gente que vende Qi (WETH es vendido para recomprar Qi).

Este fenómeno ocurre también cuando los 2 tokens que componen el par aumentan o bajan de precio. Por ejemplo, asumamos que el precio de Qi es de $1, el precio de ETH es $1,000, y hay una piscina con $100 en forma de Qi y $100 en forma de WETH. Esto supondría que hay 100 Qi y 0.1 WETH.

Ahora, si el precio de ETH aumenta hasta $2,000, y la piscina no cambia el numero de tokens, tendríamos $100 en forma de Qi pero $200 en forma de WETH, por lo que el equilibrio se habría perdido. Por lo que, el algoritmo encargado del par venderá una parte del ETH para poder comprar más Qi. En nuestro ejemplo, $50 en forma de ETH serán vendidos para comprar $50 de Qi, obteniéndose un resultado final de:

* 150 Qi con un valor de $150$
* 0.075 ETH con un valor $150

Esto significa que cuando el precio de uno de estos 2 token aumenta, la piscina crea una demanda de compra del otro token, haciendo que aumente el precio de este último. También ocurrirá lo contrario: si un token pierde valor, el otro será vendido para mantener el ratio de 1:1, haciendo que baje el precio del otro consecuentemente. Esto podría explicar parcialmente el comportamiento del precio de Qi comparado con la fluctuación de precio de WETH and WMATIC (los 2 tokens principales con los que Qi esta emparejado).

![Price of Qi (left) VS Price of WMATIC (right)](<../../.gitbook/assets/image (17).png>)

### Falta de utilidad

Finalmente, la falta de utilidad de Qi, o el desconocimiento de ésta, puede explicar por qué el precio de Qi disminuye. La gente que obtiene Qi gracias a los préstamos incentivados y/o farmeando en Mai Finance los venderán mientras tengan "algo" de valor para poder obtener un beneficio, sin ninguna visión a largo plazo, lo que es también una decisión respetable. Este artículo fue escrito con la intención de publicitar las distintas formas en las que puedes usar Qi sin que tengas que venderlos, pero si el precio no aumenta, o no puedes generar beneficios en otros activos, no hay muchos motivos para acumular estos tokens.

### ¿Cómo podemos hacer que el precio suba?

Si quisiéramos que el precio de Qi aumentase, podríamos hacer lo siguiente: .

* **Reducir la emisión**: Con 86 400 Qi creados cada día, el suministro es bastante elevado. Si la emisión disminuyera, el suministro sería inferior, y con menor suministro, el precio debería aumentar teóricamente. Sin embargo, la emisión actual de las granjas debe mantenerse igual porque son parte de la colaboración existente con QuickSwap. Los préstamos incentivados se acaban de lanzar, lo que es una buena forma de dar a conocer la plataforma, empujando a la gente a pedir préstamos, por lo que reducir la emisión puede ser una mala idea.
* **Farmear responsablemente**: No estoy diciendo que Adamant sea el principal culpable, o si es una mala herramienta. Ya que, cómo podéis ver en otros artículos, incluyo muchas veces a Adamant en las estrategias de inversión. Sin embargo, suelo farmear en granjas donde no me importa el precio del token en un futuro. Si quieres farmear rendimientos en Adamant que usa una piscina que se encuentra en Mai Finance, recuerda que estás participando en una herramienta que deprecia el precio de Qi. Si esto te da igual, pues sigue adelante..
* **Entiende cómo funciona el mercado**: el precio de todas las cryptomonedas son muy volátiles ,donde el precio de BTC y de ETH dictarán el movimiento del resto del mercado. Además, recuerda que para que una persona gane dinero, otra tiene que perderlo. No hay dinero "gratis".
* **Encuentra nuevas formas de usar tus Qi**. Este artículo ha presentado algunas estrategias para poder aumentar el número de tokens de tu portfolio. Los bucles cerrados son una gran estrategia ya que el resultado de un producto alimenta el siguiente, creando así un número de interacciones que sólo aumentarán con el paso del tiempo.

Recuerda además que:

$$
Valor = Cantidad * Precio
$$

Cuando el precio de cualquier activo disminuye, pero tu cantidad aumenta, tu valor final podría ser incluso mayor, o al menos no disminuirá tan rápidamente.

## Descargo de responsabilidad

Este artículo ha sido escrito como resultado de numerosas discusiones acerca del precio de Qi en el servidor de Discord. Mucha gente se estaba quejando acerca de la depreciación del precio de Qi, sin llegar a entender los motivos por el cual sucedía eso. Esto lleva a desilusión y frustración, lo que afecta a la comunidad de Qi, de Mai Finance, y al ecosistema DeFi en general. Ten en cuenta, que no hay ninguna garantía que haga que el precio de Qi aumente, por lo que si quieres mantener tus Qis e invertirlos, haga su propia investigación y sea consciente del riesgo.

{% hint style="info" %}
Ten en cuenta que una estrategia que en el presente funciona, puede no funcionar en un futuro (incluso podría hacerte perder dinero). Por favor, esté informado, monitorea el mercado, échale un ojo a tus inversiones periódicamente y como siempre, _**DYOR.**_
{% endhint %}
