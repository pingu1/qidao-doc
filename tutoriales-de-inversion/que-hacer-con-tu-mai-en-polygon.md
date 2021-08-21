---
description: >-
  Este tutorial te mostrará las diferentes opciones con las que puedes utilizar
  tus MAI recién acuñados en Polygon.
---

# Qué puedes hacer con tu MAI en Polygon

## Objetivo de este tutorial <a id="goal-of-this-tutorial"></a>

El objetivo de este tutorial no es presentar en detalle lo que puedes hacer con tu moneda estable MAI, sino tener un listado de todos los sitios web y aplicaciones DeFi en Polygon que te permitirán usar tu MAI directamente o en combinación con otras monedas estables. Para obtener más detalles sobre formas específicas de usar MAI, puedes consultar otros tutoriales en este sitio web u obtener ayuda en [Discord](https://discord.gg/AjSSTSy8wv) o [Telegram](https://t.me/QiDaoProtocol).

Ten en cuenta que la lista no está completa y nunca lo estará, ya que cada semana se lanzan nuevas DApps en la red. No podemos revisarlas todas, así que solo presentaremos las opciones principales, o las opciones más famosas / más "seguras".

Si quieres que se incluya un proyecto en particular, únete a la comunidad de QiDao en [Discord](https://discord.gg/mQq55j65xJ).

{% hint style="info" %}
No se mostrarán aquí las granjas de Mai Finance. Este tema merecerá su propio tutorial con información detallada, ya que Qi ofrece mucho más que cualquier otro token nativo que simplemente cosecharías para vender y aumentar tu posición en otras criptomonedas.
{% endhint %}

## Cosecha de forma segura en los mejores proyectos <a id="farming-safely-on-bluechip-projects"></a>

Los proyectos de primera categoría son aplicaciones DeFi que han probado su solidez y presentan un menor riesgo. Por lo general, están auditados y su equipo ha estado trabajando en ellos durante mucho tiempo. Normalmente, no tienen grandes APR \(tasa de porcentaje anual\), pero se puede confiar en ellos.

### Balancer <a id="balancer"></a>

​[Balancer](https://polygon.balancer.fi/#/) es un gestor de cartera automatizado, proveedor de liquidez y sensor de precios. En la plataforma, podrás prestar tus criptos y cobrar comisiones a quienes inviertan, los cuales re-equilibran sus carteras buscando oportunidades de arbitraje. Si quieres más detalles sobre Balancer, lee [la documentación oficial.](https://docs.balancer.fi/)

En la red de Polygon, Balancer propone una reserva de liquidez \(pool\) compuesta por las 4 principales monedas estables: DAI, USDC, USDT y MAI \(miMATIC\). Este pool de monedas estables tiene actualmente un APR bastante constante de ~20%.

![Estado del pool de monedas estables a fecha Agosto de 2021](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-MgpdyV6fL-EQ7Zb-dt9%2F-MgpkCtdM5t47plx80WC%2FScreen%20Shot%202021-08-11%20at%2011.06.59%20AM.png?alt=media&token=8bedd49d-bb7e-4cbb-83d8-d6724489c983)

Lo mejor de Balancer es que no es necesario que poseas las 4 monedas para depositarlas en el pool. Balancer generará automáticamente una combinación equilibrada con cualquier depósito que realices. Esto significa que si tienes $100 en MAI, simplemente puedes depositarlos en el pool de Balancer y dejar que el algoritmo los descomponga correctamente para tener una proporción del 25% para cada moneda, dependiendo de su precio respectivo en el momento del depósito.

Las recompensas del pool se pagan utilizando el token BAL, el cual es distribuido semanalmente. Además del token BAL, se pueden recibir recompensas adicionales según el pool en el que depositaste. Puedes consultar los diferentes [programas de incentivos aquí](https://balancer-incentives.web.app/). En nuestro caso, participar en el pool de estables también te otorgará recompensas en MATIC y Qi.

El flujo completo sería algo así:

![](../.gitbook/assets/granjea-monedas-estables-en-balancer.png)

Si necesitas más detalles sobre cómo puedes usar Mai Finance para prestar tus criptos y pedir prestado MAI \(en lugar de vender tus criptos para comprar MAI\), consulta otras guías en este sitio web. Incluso puedes [incluir AAVE en el ciclo](https://app.gitbook.com/@qidao-qimps/s/mai-finance-tutorials/~/drafts/-MgyckLyKbYJxZD6c6RY/es-tutoriales-de-inversion/apalancamiento-con-tus-tokens-de-aave) para ganar aún más.

### Curve finance <a id="curve-finance"></a>

[Curve](https://polygon.curve.fi/) es otra plataforma en la cual podrás prestar tus activos de criptomonedas en reservas de liquidez \(pool\) que generarán ingresos, aunque no MAI directamente \(¿por ahora?\). Las opciones más interesantes son:

* El pool de AAVE, que generará entre un 5% y un 15% de APR \(el APR varía bastante\) en un trío de monedas estables \(DAI/USDC/USDT\). La reserva funciona exactamente como en Balancer, de forma que puedes entrar en el pool utilizando un solo activo de los tres que serán usados en AAVE por el protocolo. 
* El pool de atricrypto que está compuesto de un trío de monedas estables e incluye wETH y wBTC también para mitigar la pérdida impermanente \(_impermanent loss_\). Este pool tiene un APR que oscila entre un 25% y un 30%. El equipo de Mai Finance está actualmente intentando añadir MAI también a este pool, lo cual significará que podrías ser capaz de entrar en ella directamente con tu MAI acuñado en Mai Finance.

Mientras que esperamos a que el protocolo Curve acepte a MAI como una moneda estable para sus pools, puedes todavía sacar provecho de ellos usando tus criptos favoritas con Curve siguiendo los siguientes pasos \(ejemplo con MATIC\)

* Deposita tus tokens de MATIC en AAVE y recibe amWMATIC
* Deposita tus amWMATIC en Mai Finance y recibe camWMATIC \(las recompensas de AAVE serán auto-compuestas en los tokens de camWMATIC\)
* Usa tus camWMATIC como colateral en Mai Finance y pide prestado MAI usándolo de garantía.
* Utiliza la [página de Anchor](https://app.mai.finance/swap) en Mai Finance para intercambiar todo tu MAI por USDC
* Una vez hecho eso puedes:
  * Entrar en el pool de atricrypto en Curve con tu USDC y conseguir recompensas del 25% al 30%.
  * Entrar en el pool de AAVE en Curve con tu USDC y conseguir recompensas del 5% al 15%.

Las recompensas en Curve se distribuyen de la siguiente forma:

* USDC auto-compuesto que incrementa tu posición en el pool \(será una mezcla entre USDC/USDT/DAI y posiblemente wBTC/wETH para el pool de atricrypto\)
* WMATIC que puedes luego usar para repetir el ciclo mostrado arriba e incrementar tu préstamo y el capital invertido.
* Tokens de CRV, que puedes también usar como colateral en Mai Finance para pedir prestado más MAI e incrementar tu capital invertido.

![](../.gitbook/assets/granjea-monedas-estables-en-curve.png)

### AAVE <a id="aave"></a>

Puedes consultar la guía completa acerca de cómo puedes  [hacer apalancamiento e incrementar las ganancias de tus tokens con AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/es-tutoriales-de-inversion/apalancamiento-con-tus-tokens-de-aave). Este no es un uso directo de la moneda estable MAI, pero podemos imaginar que en el futuro AAVE también tendrá un programa con MAI en el que podrás prestar tus tokens.

### QuickSwap <a id="quickswap"></a>

​[QuickSwap](https://quickswap.exchange/#/) es probablemente uno de los DEX \(**EX**changes **D**escentralizados\) más famosos de Polygon, junto con SushiSwap y 1Inch. Es también un AMM \(_**A**utomated **M**arket **M**aker_\) que permite a los usuarios invertir eficientemente en la red de Polygon utilizando reservas de liquidez \(_liquidity pools\)_. Cualquier operación en un exchange está sujeta a una comisión que es parcialmente redistribuida a los usuarios que depositan su liquidez en la plataforma.

La forma en la que puedes usar MAI en QuickSwap es muy similar a cosechar en una [granja de rendimiento](https://qidao-qimps.gitbook.io/mai-finance-tutorials/en-investment-tutorials/secure-your-yield-farming-profits). Si necesitas ayuda para seguir los pasos exactos y entrar en la reserva de liquidez de MAI/USDC en QuickSwap puedes leer éste artículo \(por el momento sólo disponible en Inglés\).

Actualmente, si entras en el pool de MAI/USDC en QuickSwap obtendrás:

* Comisiones de las operaciones
* Tokens de QUICK

![Detalles de la reserva de MAI/USDC en QuickSwap a fecha de Agosto de 2021](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-Mgq0S-BjgfXOCOq5Gpc%2F-Mgq43bDz3V2cBgKXfJ5%2FScreen%20Shot%202021-08-11%20at%2012.37.56%20PM.png?alt=media&token=9cceebf1-15c7-4112-aa12-afa23a86462a)

## Granjas _degeneradas_ y agregadores <a id="degen-farms-and-aggregators"></a>

### Adamant <a id="adamant"></a>

​[Adamant](https://adamant.finance/home) es un agregador que incluye las "mejores" granjas de Polygon y te permite entrar en ellas directamente desde su sitio web. Al depositar tus activos \(Tokens LP\) en un pool específico de Adamant, el algoritmo cosechará las recompensas otorgadas por éste y compondrá automáticamente parte de las mismas incrementando tu posición de tokens LP. El resto de la recompensa es generalmente convertida en WMATIC, la cual es redistribuida a los poseedores del token ADDY \(token nativo de Adamant\). Finalmente, recibes también una recompensa en forma de tokens de ADDY la cual puedes cosechar y bloquear durante 90 días, recibiendo por ello parte de los dividendos de WMATIC.

En general, Adamant es un buen sitio al que acudir si no te importa demasiado el token que estás granjeando y si no quieres estar pendiente de reinvertir tus recompensas manualmente varias veces al día. También genera más ingresos debido a que recibes una parte de recompensas en ADDY adicionalmente a las recompensas que otorgan los pools.

Adamant actualmente soporta unos cuantos pools que aceptan el par LP de MAI/USDC. Éstos son:

* QuickSwap: La recompensa en QUICK es intercambiada por más tokens LP de MAI/USDC LP y recompensas en WMATIC.
* DinoSwap: La recompensa en Dino es intercambiada por más tokens LP de MAI/USDC LP y recompensas en WMATIC.
* Mai Finance: La recompensa en Qi es intercambiada por más tokens LP de MAI/USDC LP y recompensas en WMATIC.

![Reserva de QuickSwap de MAI/USDC en Adamant](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-Mgq0S-BjgfXOCOq5Gpc%2F-Mgq72u5oC2sKOvq4Z4H%2FScreen%20Shot%202021-08-11%20at%2012.51.12%20PM.png?alt=media&token=3b7ab099-f66c-4bd7-870b-623f600336bd)

{% hint style="info" %}
Estas capturas de pantalla de el pool de QuickSwap en el sitio web de QuickSwap \(ver sección anterior\) y en el de Adamant \(imagen superior\) han sido tomadas el mismo día, pero muestran diferentes APYs \(Porcentaje de Rendimiento Anual o **A**nnual **P**ercentage **Y**ield\).
{% endhint %}

Puedes ver que el APY en Adamant es ligeramente superior al directo en QuickSwap. El desglose de la recompensa es el siguiente:

* 12.88% QUICK Auto-compuesto QUICK \(lo cual significa que la recompensa en QUICK es transformada en más tokens LP\)
* 9.16% Recompensa en ADDY \(no compuesta\)
* 3.40% Dividendo de la cuota de comisiones \(reclamando ADDY diariamente\)

Lo cual significa que, del total de 20.92% otorgado por QuickSwap, sólo un 12.88% es usado para incrementar tu posición como proveedor de liquidez \(LP\) y el resto es intercambiado para obtener dividendo en WMATIC. Tendrás la posibilidad de reclamar tus recompensas en ADDY diariamente \(o cuando decidas\) y volverlas a depositar, lo cual generará a su vez dividendos en WMATIC. En otras palabras, Adamant _parece_ una opción superior porque tiene mejores APYs y compone automáticamente tus recompensas, pero en realidad incluye para ello un montón de acciones manuales que tendrás que ejecutar para alcanzar ese APY teórico.

{% hint style="info" %}
La utilización de Adamant tiene también un impacto significativo en los precios de los tokens nativos. Esto es debido a que Adamant está constantemente vendiendo los tokens cosechados para generar más pares de LP y WMATIC como dividendos para los ****poseedores de ADDY. La presión de venta es muy elevada en dichos tokens de granjas y puede dar explicación al por qué sus precios están consistentemente decayendo. 
{% endhint %}

### Otras granjas que aceptan el par LP de MAI/USDC <a id="other-farms-accepting-mai-usdc-lp-pair"></a>

A medida que MAI consigue una mayor popularidad en Polygon y debido a que QuickSwap ya soporta el par MAI/USDC, un número cada vez más creciente de granjas lo aceptan también. La siguiente lista incluye unos pocos proyectos en los cuales puedes obtener rendimientos utilizando MAI/USDC

* DinoSwap
* Augury
* Polypup
* ...

Otras granjas pueden también aceptar el par MAI/USDC. Si quieres mantenerte informado acerca de nuevas granjas y sus fechas de lanzamiento te recomendamos encarecidamente echarle un vistazo al [Calendario de RugDoc.io](https://rugdoc.io/calendar/) para granjas de Polygon. Este sitio web también ofrece información general acerca de cada proyecto así como de sus potenciales riesgos asociados.

## Impermax <a id="impermax"></a>

### Explicación general <a id="a-little-bit-of-explanation"></a>

​[Impermax](https://polygon.impermax.finance/) es una plataforma que permite a los usuarios apalancarse con sus tokens LP para obtener rendimientos superiores. El objetivo es muy simple: al proveer con tus tokens LP y utilizarlos como colateral, puedes entonces pedir prestados más de los 2 activos subyacentes para generar más tokens LP y repetir el bucle. 

![Esquema explicativo del ciclo de Impermax](../.gitbook/assets/estrategia-con-impermax.png)

Al realizarlo, el usuario está expuesto a la _impermanent loss_ y esa pérdida se ve magnificada por el número de veces que se repita el ciclo. El riesgo de liquidación también se ve multiplicado cuando se ejecutan demasiadas iteraciones del ciclo. Indudablemente, si el APR se multiplica, también la variación de los precios de las dos monedas que conforman el par se ven amplificadas por el efecto del apalancamiento, lo cual puede conducir a ser liquidado más rápidamente.

Con las monedas estables el riesgo el riesgo de liquidación es sin embargo inferior, debido a que la variación de los precios es inapreciable. Esto significa también que el Ratio de Colateral a Deuda \(CDR\) puede ser muy cercano al 100%, posibilitando realizar un alto número de iteraciones del ciclo y por tanto a un alto APR.

Tenga en cuenta que Impermax cobra comisiones cuando tomas prestado y apalancas tu posición. La comisión corresponde al 0,1% de su posición final. Por ejemplo, si tengo $100 en MAI / USDC y apalanco al 50x, mi posición final valdrá $5,000 y pagaré una comisión de $4.90 correspondientes a los $4,900 que pedí prestados.

El efecto de hacer un bucle combinando suministrar liquidez y pedir prestado permite multiplicar el APY final. Partiendo de un APY inicial del 20% para el par MAI / USDC con un CDR del 110%, ejecutando el bucle 50 veces y usando la fórmula siguiente

$$
APR_{Final}=APR_{Inicial} * \sum_{i=0}^{n}{\frac{100}{CDR}^i}
$$

Podemos obtener fácilmente un APR final del 228%. Hay algunos elementos que afectarán al APR, tales como el APR de pedir prestado \(interés del préstamo por tomar prestados más tokens LP\) y la oferta / demanda de ambos activos que componen el par LP \(impactando directamente en el APR\).

Además, debido a que todos los ratios se ven magnificados por el número de veces que se ejecuta el ciclo, el APR variará drásticamente y puede en ocasiones incluso ser negativo durante breves lapsos de tiempo \(tus tokens LP se utilizarán para re-pagar el APR negativo\).

### Posición apalancada de mi par MAI/USDC <a id="leveraged-position-of-my-mai-usdc-pair"></a>

Al final, estás usando el APR base con un valor mucho mayor, lo cual genera intereses mucho mayores, incrementando el APR de tu posición inicial.

![Un ejemplo del panel de Impermax con una inversi&#xF3;n inicial de $70.52 en el par MAI/USDC](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-MgqEQTtpnqlSldZUdgv%2F-MgqIAdeSJZrQoezm26E%2FScreen%20Shot%202021-08-11%20at%201.38.33%20PM.png?alt=media&token=74c40155-257e-4c6c-9229-89a4f6e71ba0)

Puedo ver fácilmente cuánto estoy utilizando como colateral, cuánto he invertido inicialmente, cuál es el ratio de apalancamiento y cuales son los valores de liquidación debido al ratio de liquidación. Al momento de escribir este artículo, la posición anterior me dará los siguientes ratios:

![Estimaci&#xF3;n de ingresos y gastos en un momento determinado](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-MgqEQTtpnqlSldZUdgv%2F-MgqIifDBzLceL5ywne5%2FScreen%20Shot%202021-08-11%20at%201.41.55%20PM.png?alt=media&token=0638d8fa-3787-4e7b-8803-1574d0ce9857)

El APR se otorga en el token IMX, el cual puede ser intercambiado por más MAI/USDC \(utilizando el poder de Mai Finance para pedir prestado al 0% de interés\), o utilizado para proveer de liquidez en reservas específicas que aceptan IMX en Impermax.

### Suministrando liquidez de MAI a prestatarios <a id="supplying-mai-to-borrowers"></a>

De hecho, en la aplicación también puedes proporcionar liquidez a aquellos que quieran aplicar ciclos de apalancamiento en sus posiciones \(necesitarán activos subyacentes para generar más tokens LP\). Prestar activos es una excelente manera de obtener rendimientos y permite que los prestatarios asuman todos los riesgos. Además, cuantos más usuarios pidan prestado, mayor será el APR de suministro.

![Ratios por suministrar y pedir prestado MAI en Impermax en un momento determinado](https://gblobscdn.gitbook.com/assets%2F-MgS6h4h2L6e5O5bUNqY%2F-MgqEQTtpnqlSldZUdgv%2F-MgqK1ePLITqptmdA4rO%2FScreen%20Shot%202021-08-11%20at%201.47.56%20PM.png?alt=media&token=74dc29af-77f3-4a14-930e-a730bf1486f6)

Ésta es una forma genial de optimizar tu préstamo al 0% de interés de Mai Finance. No sólo no tienes que pagar nada por pedir prestado MAI, sino que puedes recibir altos rendimientos simplemente depositándolo en Impermax.

## Descargo de responsabilidad <a id="disclaimer"></a>

Todo lo contenido en este tutorial es puramente educativo. El objetivo es dar luz a proyectos que pensamos que son valiosos para quienes están aprendiendo y evolucionando en el mundo cripto en Polygon. Obviamente no hablamos de Mai Finance como una granja porque dentro de poco habrá un tutorial enteramente dedicado a ello. 

Por último, esta guía EN NINGÚN MODO pretende ser aplicada tal cual, no es un consejo financiero y no deberías seguirla ciegamente punto por punto. Por favor, lee los documentos de los diferentes proyectos mencionados antes de considerar invertir en dichas plataformas.

{% hint style="info" %}
Ten en cuenta que una estrategia que funciona bien en un momento dado puede funcionar mal \(o hacerle perder dinero\) en otro momento. Manténte informado, controla los mercados, controla tus inversiones y, como siempre, haz tu propia investigación.
{% endhint %}

