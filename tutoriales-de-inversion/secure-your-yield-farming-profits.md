---
description: >-
  Esta página describe en detalle una estrategia "segura" que convierte a las
  granjas de rendimiento (yield farming) un poco menos rentables, pero mucho más
  segura.
---

# Farmear utilizando únicamente monedas estables

## Conceptos generales

Cuando accedes a una granja de rendimiento en Polygon, estás exponiendo a tus inversiones al éxito o al fracaso de la granja. Esta guía no explicará detalladamente qué es una granja de rendimiento, o cómo puedes farmear en estas. Si necesitas entender este concepto, existen numerosos tutoriales en internet. Además, puedes obtener ayuda de la comunidad de QiDAO en Discord

El principal problema cuando estas farmeando es que tienes que tomar una decisión entre:

* Vender el token nativo y convertirlo entre activos "seguros" que representarán tus ganancias.
* Reinvertirlos para generar más beneficios \(también conocido como ¿hiper compounding?\)

Esta guía describirá paso a paso cómo usar Mai Finance para asegurar tus ganancias mientras sigues re-invirtiendo una porción de estas en la granja.

{% hint style="info" %}
Para entender con mejor detalle cómo puedes hacerlo, usaré la última granja PolyUp \(poner hipervinculo\). Esta explicación se realizará con propósito educativo y no deberá ser utilizada como consejo financiero. Además, el término "seguro" esta basado en mi opinión personal del equipo. Como siempre, Haz Tu Propia Investigación \(DYOR\). Por último, no recomendamos esta granja.
{% endhint %}

![](../.gitbook/assets/screen-shot-2021-08-09-at-10.20.26-am.png)

## Ciclo de vida del farmeo

### Ponerse manos a la obra

Una vez un humilde granjero me dijo lo siguiente:

> _**No deberías comprar aquello que puedes obtener**_

En esta guía, intentaremos implementar toda la seguridad financiera posible. Para hacerlo posible, farmearemos utilizando solamente monedas estables, para proteger a nuestra inversión de cualquier pérdida permanente. La mayoría de las granjas proponen pares de monedas estables en sus reservas de liquidez \(liquidity pool o LP\), y Mai al ganar cada vez mas visibilidad, podrás encontrar granjas que proponen reservas del par MAI/USDC. Este será el par que trataremos a continuación.

Para poder empezar a farmear con el par MAI/USDC, necesitarás adquirir las monedas estables. Mai Finance te permitirá pedir prestado MAI al depositar tu criptomoneda favorita. En nuestro caso, tenemos algo de MATIC en nuestra cartera, listo para ser utilizado. Al depositar MATIC en la [_bóveda de MATIC_](https://app.mai.finance/vaults/matic) _\(o vault\)_ en Mai Finance, puedo pedir prestado MAI. Si necesitas ayuda haciendo esto, por favor únete al servidor de Discord y pregunta a la comunidad. Además, puedes leer los otros tutoriales de esta página web donde podrás encontrar como hacer esto.

{% hint style="info" %}
Puedes depositar tus tokens de MATIC en tu bóveda de MATIC, pero además puedes depositarlos en AAVE para obtener amWMATIC, depositarlos en Mai Finance en la pestaña de [yield](https://app.mai.finance/yield) para obtener camWMATIC, y usar estos camWMATIC como colateral. Con esto, podrás pedir prestado la misma cantidad de MAI, pero además podras obtener rendimientos superiores en tu MATIC. Para obtener más información sobre esto último, consulte [Apalancamiento con tus tokens de AAVE](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/es/tutoriales-de-inversion/apalancamiento-con-tus-tokens-de-aave).
{% endhint %}

Una vez hayas obtenido el préstamo de MAI, podrás utilizar la página de [Anchor](https://app.mai.finance/anchor) para convertir la mitad de tu préstamo en USDC. Recuerda, que para farmear usando los pares de liquidez, las dos partes tienen que tener un ratio de 1:1.

![Usando la p&#xE1;gina Anchor se podr&#xE1; convertir 30 MAI a USDC](../.gitbook/assets/screen-shot-2021-08-09-at-6.28.28-am.png)

Dependiendo de la granja donde quieras farmear, necesitarás combinar tus 2 monedas estables \(MAI y USDC\) en un par de liquidez válido usando un **DEX** \(**EX**change **D**escentralizado\). Como vamos a utilizar la granja de Polyup, y esa página acepta los pares de liquidez de Quickswap, deberás ir a [QuickSwap](https://quickswap.exchange/#/pool) y generar ahí el par.

![Genera unos tokens de par de liquidez usando MAI y USDC ](../.gitbook/assets/screen-shot-2021-08-09-at-6.29.16-am.png)

Ahora estás listo para entrar en una granja.

### Deposita y recolecta los tokens de la granja

Ahora que tienes algunos tokens del par de liquidez, puedes ir a la granja y depositarlos para empezar a recolectar los tokens nativos de la granja. En este ejemplo, se ha depositado MAI/USDC en la siguiente reserva de liquidez, y se ha empezado a generar tokens BALL.

![Generar BALL en la reserva](../.gitbook/assets/screen-shot-2021-08-09-at-10.58.19-am.png)

Por ahora, cómo se puede observar en la imagen superior, farmeando MAI/USDC se puede una tasa de retorno del 176.99%. Esto se debe a la cantidad de liquidez que hay en la reserva de liquidez, y en el precio del token BALL, por lo que este porcentaje puede variar.

{% hint style="info" %}
Es importante resaltar que cuando depositas los tokens del par de liquidez, muchas granjas cobran alrededor del 2% o 4% en forma de comisión directamente de los tokens depositados. Ten cuidado con esto, y estate seguro de que hay riesgo de que puedas perder todo el valor de la comisión, o no recuperarlo del todo.
{% endhint %}

Ahora que tus monedas estables estan depositadas en la reserva, podrás comenzar a generar los tokens nativos de la granja que podras recolectar siempre que quieras. Cabe destacar, que el precio del token de la granja será muy volátil, por lo que asegúrate de ir recolectando el token periodicamente. Cuanto mayor sea la espera, mayor será el riesgo de que todos esos tokens de la granja se hayan devaluado considerablemente. Para poder recolectar los tokens BALL del ejemplo anterior, bastará con hacer click en el botón de **Harvest.**

### Apalancate con tus tokens de granja

Ahora que tienes unos tokens de una granja, puedes elegir entre lo siguiente:

* Venderlos para comprar algo con mayor valor \(como podría ser tu crypto preferida\).
* Reinvertirlos en la reserva.

Sin embargo, Mai Finance presenta una alternativa que te deja hacer ambas. Una vez que hayas recolectado tus recompensas, podrás ir a tu DEX favorito que tenga soporte de dicho token. Por lo general, puedes encontrar un link al DEX en el menú de la granja directamente. Este link incluirá la dirección del contrato del token, lo que te permitirá operar con ese token de forma más sencilla.

![Cambiando mis recompensas por MATIC](../.gitbook/assets/screen-shot-2021-08-09-at-11.14.29-am.png)

Llegados a este punto, volvemos a tener tokens MATIC en nuestra cartera, listos para ser depositados en MAI Finance como colateral. Si lo hiciera, podría pedir prestado MAI, cambiar una parte por USDC, crear un token del par de la reserva de liquidez y redepositarlos en la granja. Haciendo esta conversión, he "asegurado" el 100% de las recompensas intercambiando el token nativo de la granja por un token mucho mas estable \(en este caso MATIC\) y he vuelto a reinvertir el 50% de mis recompensas en la reserva de liquidez \(para ser exactos, ha sido un 46% debido a la comisión del 4% al depositar el par\).

Dicho de otra manera, el APR \(Tasa de Porcentaje Anual\) ha sido aplicado al 100% en tu cryptomoneda principal. Si estás depositando nuevos tokens del par de liquidez en la reserva, estarás obteniendo el 50% del APY \(Porcentaje de Rendimiento Anual\) de la reserva de liquidez

## Estimación de las ganancias

Antes de comenzar con el análisis de los resultados, hay que considerar lo siguiente:

* Se comenzó con una cantidad de 60 MAI prestados habiendo aportado previamente $120.00 de MATIC.
* El APR de la granja se mantuvo al 176.99%, lo que se traslada a una ganancia diaria del 0.484%.
* El valor de MATIC y BALL se ha mantenido constante.

Obviamente estas consideraciones no se pueden aplicar en la vida real, ya que el APR disminuirá a medida que entre liquidez a la reserva y el precio del token fluctuará con el tiempo.

### Resultados aproximados

| Día | Valor LP | Valor Recompensa | Matic Compuesto | LP Creados |
| :---: | ---: | ---: | ---: | ---: |
| 1 | $57.60 | $0.279 | $0.279 | $0.139 |
| 2 | $57.734 | $0.280 | $0.559 | $0.140 |
| 3 | $57.874 | $0.280 | $0.840 | $0.140 |
| 4 | $58.014 | $0.281 | $1.121 | $0.141 |
| 5 | $58.155 | $0.282 | $1.403 | $0.141 |
| 6 | $58.296 | $0.282 | $1.686 | $0.141 |
| 7 | $58.437 | $0.283 | $1.969 | $0.142 |
| 8 | $58.579 | $0.284 | $2.253 | $0.142 |
| 9 | $58.721 | $0.285 | $2.538 | $0.142 |
| 10 | $58.863 | $0.285 | $2.823 | $0.143 |
| 11 | $59.006 | $0.286 | $3.109 | $0.143 |
| 12 | $59.149 | $0.287 | $3.396 | $0.143 |
| 13 | $59.292 | $0.287 | $3.684 | $0.144 |
| 14 | $59.436 | $0.288 | $3.972 | $0.144 |
| 15 | $59.580 | $0.289 | $4.261 | $0.144 |
| 16 | $59.725 | $0.289 | $4.551 | $0.145 |
| 17 | $59.870 | $0.290 | $4.841 | $0.145 |
| 18 | $60.015 | $0.291 | $5.132 | $0.145 |

* En el día 1, la comisión del 4% ha sido aplicado a los 60$ del par MAI/USDC.
* Al final del día 1, el beneficio generado \($0.279\) ha sido transferido totalmente a la bóveda de MATIC.
* Al final del día 1, como hemos añadido mas MATIC a nuestra bóveda, podemos pedir prestado mas MAI.
* Para mantener el Ratio de Colateral Deuda \(CDR\) al 200%, solo se pedira prestado la mitad del MATIC depositado \($0.139\).
* Al comienzo del día 2, se ha reinvertido $0.139 en la granja \(donde la granja cobrará un 4% de comisión de depósito\).
* Al comienzo del día 2, se ha comenzado con un $0.134 adicional del token del par de liquidez. 

### Estimación de APRs, APYs y crecimiento del beneficio

La estimación fue interrumpida en el dia 18 ya que una vez pasada dicha fecha, se puede observar que se ha vuelto a obtener 60$ del token de la reserva de liquidez. Esto significa que se ha farmeado lo suficiente para volver a obtener el depósito inicial, esto debería ser el mínimo que debería hacer cualquier granjero. 

A partir de ese día, sólo se obtendrían beneficios y al estar en una reserva de liquidez de monedas estables, es imposible que haya pérdida impermanente en la liquidez suministrada. Esto significa, que no habrá ninguna posibilidad de perder dinero al estar en dicha reserva.

Sin embargo, hay que destacar que la comisión del depósito inicial \($2.40\) fue repagada en el dia 9 al tener el suficiente MATIC en la cartera como beneficio. Si se hubiera vendido el token nativo de la granja y no se hubiera reinvertido en la reserva de liquidez, ese hubiera sido el momendo dónde solo generaría beneficios.

En términos de ganancias, la recompensa que se compone en la granja, es solo del 50% del APR. Esto significa que con una granja con un APR del 176.99%, el crecimiento anual sería del 88.495% anual,  o 0.242% diario.

También es posible calcular la ganancia exacta que fue acumulada en cualquier día en la granja, asumiendo que se vuelven a reinvertir diariamente, se puede utilizar la siguiente fórmula para calcular el **ROI** \( Retorno de la Inversión\):

$$
ROI_{DíaN}=Inversión Inicial*(1+APRDiario)^{DiaN}-Inversión Inicial
$$

En el caso de la granja cobre una comisión de depósito 4%, deberás multiplicar el resultado por 96%. En este caso, se puede comprobar que la formula superior funciona comprobando el resultado con la tabla anterior.

Comenzando con $60.00 y generando $81.81 tras 1 año da un APY del 136.34%.

Si comparamos el APY teórico con un APR del 88.495% usando la siguiente fórmula:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Esto da como resultado un APR del 88.495% y  un del N = 365 \(reinvirtiendo diariamente\).

$$
APY = ( 1 + \frac{0.88495}{365})^{365}-1=142.02\%
$$

Destacar que la estimación superior no tienen en cuenta la comisión del 4% del depósito, de ahí a que haya discrepancia en el resultado.

Las ganancias en la cartera de MATIC son simplemente el doble de ganancias de la granja y podremos calcular el ROI de cualquier día usando la formula de arriba y multiplicando el resultado por 2.

Este es el número de MATIC que se generará al mantenerse en la misma granja por un año, con una inversión inicial de 60$ del par MAI/USDC, asumiendo que el APR se mantiene constante. Esto da un APY adicional del 272.69%, que es aproximadamente el mismo APR que la granja publicita \(las granjas por lo general no tienen en consideración el 4% de comisión de depósito en el APR\).

### Resumiendo tras 1 año de farmeo con monedas estables

Al final del año se obtendrá lo siguiente:

* $283.62 MATIC en la bóveda \($120.00 iniciales  + $163.62 generados en la granja\).
* $141.82 de deuda \($60.00 iniciales  + $81.82 prestados y reinvertidos\).
* $141.82 de MAI/USDC tokens en la granja.

## Descargo de responsabilidad

Para realizar esta estrategia se ha asumido lo siguiente:

* La granja mantiene un APR constante durante un año \(cosa que es totalmente errónea\)
* Se puede farmear durante un año entero \(cosa que es imposible, ya que ninguna granja se mantiene activa durante tanto tiempo\)

Además, el APR del par MAI/USDC de la reserva de Polypup tras 24h de farmeo es 128.13%, debido a que el precio de BALL esta disminuyendo ligeramente.

Farmear con monedas estables _**podrá**_. ser la forma más "segura" de obtener ganancias porque no estas expuestos a pérdidas impermanentes.   Sin embargo, no hay ninguna garantía de que puedas obtener el 4% de comisión del depósito inicial. Se pueden encontrar facilmente granjas que tiene reservas de monedas estables con 0% o 1%  de comisión de depósito, incluso en las reservas no nativas \(reservas que aceptan pares de liquidez sin el token de la granja en cuestión\).

Recolectar las recompensas e intercambiarlas por algo valioso es considerado la mejor estrategia cuando se farmea en granjas de rendimiento. Pedir prestado MAI para reinvertir una parte en la reserva de liquidez de tus monedas estables, e incrementar tus beneficios potenciales al farmear expone tus beneficios a la comisión de depósito del 4% que la granja esta cobrando de tu par de liquidez, lo que no sería la mejor solución si estas dudando si los podrás recuperar, por lo que será mejor usar otra estrategia para reinvertir tus ganancias \(invertir en reservas nativas / reservas con un 0% de comisión / reservas con mayores APRs\).

{% hint style="info" %}
Ten en cuenta que una estrategia que en el presente funciona, puede no funcionar en un futuro \(incluso podría hacerte perder dinero\). Por favor, esté informado, monitorea el mercado, échale un ojo a tus inversiones periódicamente y como siempre, _**DYOR.**_
{% endhint %}

