---
description: >-
  DeFi no tiene por qué ser complicado. Este artículo presenta cómo se puede
  operar en DeFi utilizando Mai Finance con una estrategia de bajo riesgo y
  obteniendo intereses razonables.
---

# Estrategia para novatos usando camDAI

## Introducción

La mayoría de la gente se asusta cuando piensa en DeFi. Siempre hay que tener presente el riesgo cuando se utilizan criptomonedas, la volatilidad de este mercado puede hacer que uno pierda mucho dinero, y hay tantas posibilidades, que encontrar una estrategia adecuada puede ser bastante complejo. Sin embargo, cuando se utilizan las herramientas correctas, algunas estrategias fáciles y de bajo riesgo pueden obtener buenos resultados, y probablemente puedan competir con opciones más complejas y arriesgadas.&#x20;

En esta guía, trataremos de presentar una estrategia de inversión basada en la moneda estable apalancada, con un toque de riesgo para mayores intereses.

## Entendiendo el apalancamiento

![Historia de un Qinero](../../.gitbook/assets/canDAI-farwest.png)

Estas en el lejano oeste, durante la gran fiebre del oro. Los bancos quieren comprar oro para poder prestar dinero a la gente y obtener intereses por estos préstamos, y los mineros quieren hacerse ricos vendiendo su oro a los bancos.&#x20;

Eres un minero, pero no tienes mucha suerte. Sólo has encontrado una pepita. Sin embargo, eres super inteligente y, en lugar de seguir minando y tentar a la suerte, ¡tienes otro plan!

Vas a un banco y le explicas que tienes oro. Puedes depositar el oro en el banco como garantía, lo que significa que dejas que el banco utilice ese oro para la gente que quiera usarlo, y el banco te dará algunos intereses por tu depósito.&#x20;

Además, como has prestado algo de oro, el banco acepta que le pidas dinero prestado, y en caso de que no puedas devolver el préstamo pagando algunos intereses extras. El banco se pagará a sí mismo con el oro que has depositado. Genial, ahora estás ganando intereses por el oro que tienes en el banco, y te han dado algo de dinero.&#x20;

Con eso, decides ir a ver a un compañero minero y comprar su oro con tu dinero. Esto le permite a tu compañero centrarse en la minería y obtener dinero en efectivo por el oro que ha encontrado. Todo el mundo está contento.&#x20;

Vuelves al banco y depositas el oro que has comprado a tu compañero. Esto implica más intereses, y ahora el banco te deja pedir más dinero prestado con el oro extra que has depositado. Tienes más oro expuesto a los intereses del banco, y algo más de efectivo. Es hora de volver a ver si tu amigo ha encontrado más oro, y repetir esto una y otra vez.

Esto es lo que se conoce como apalancamiento. Ahora imagina que puedes encontrar un banco que te permite pedir prestado dinero en efectivo a un interés del 0%, por lo que tienes una sólida máquina de imprimir dinero sólo con los intereses que estás obteniendo con tus operaciones.

## Introduciendo las herramientas

### AAVE

[AAVE](https://app.aave.com) es una plataforma de préstamos y depósitos en la que puedes depositar tus crypto activos. Al prestar en AAVE, tus tokens depositados obtendrán un interés. Para nuestra estrategia, prestaremos DAI, una moneda estable (vinculada al dólar estadounidense). En AAVE, 100 dólares de DAI generarán potencialmente entre un 4% y un 10% de rentabilidad en el plazo de un año.

![Mercados de AAVE en Polygon a fecha de Octubre 2021](../../.gitbook/assets/canDAI-aave.png)

Cuando depositas tus activos en AAVE, recibirás un recibo de depósito. En nuestro ejemplo, como estamos depositando DAI, obtendremos tokens **amDAI** en nuestra cartera (aave market DAI). Es absolutamente necesario que guardes este comprobante porque lo necesitarás para retirar tus DAI de AAVE. Este es el equivalente al banco que aceptará su oro en nuestra comparación del lejano oeste.

### Mai Finance

[Mai Finance](https://app.mai.finance) es una plataforma de préstamos que te permite depositar algunos activos en una bóveda, y pedir un préstamo contra el valor de este depósito. Si volvemos a la analogía del banco, sería un banco que te permite pedir un préstamo, pero el préstamo no proviene de lo que otras personas están prestando. En su lugar, el banco imprime el dinero correspondiente a tu depósito personal, por lo que sólo te prestas contra ti mismo.

Mai finance aceptará tu amDAI en su herramienta de [Yield](https://app.mai.finance/yield). La funcionalidad de Yield es sólo una herramienta intermediaria entre AAVE y Mai Finance. Como puedes ver en la captura de pantalla de AAVE, prestar DAI te hará ganar un 8,75% en DAI (que se compone), pero también un 2,01% de recompensa en MATIC. El instrumento de rendimiento de Mai Finance recogerá esta recompensa en MATIC y la cambiará por más DAI que se añadirá a su depósito de DAI. El **APY** (Porcentaje Anual de Rendimiento) en el sitio de Mai Finance muestra, por tanto, los intereses agregados de AAVE.

![Yield en Mai Finance](../../.gitbook/assets/camDAI-yield.png)

Una vez haya depositado su amDAI en Yield, obtendrá algo de camDAI en su cartera (amDAI compuesto). Se trata de un recibo que indica tu parte del fondo de amDAI en Yield. Como nota adicional, debido a que el camDAI es una representación de tu parte del pool de amDAI, la relación entre el amDAI y el camDAI no es 1:1. Vea este [articulo ](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/tutoriales-de-polygon/apalancamiento-con-tus-tokens-de-aave)para obtener más detalles.

Ahora puedes [depositar tus tokens camDAI](https://app.mai.finance/vaults) en una bóveda en Mai Finance, y podrá pedir un préstamo de MAI (una moneda estable vinculada a 1 dólar) contra su garantía. En nuestra comparación con el lejano oeste, se trata de un segundo banco que le permitirá pedir un préstamo en efectivo basado en la cantidad de oro que ya has depositado en el primer banco. Este segundo banco acepta el recibo del primer banco como garantía en caso de que no puedas devolver el préstamo.

### Zapper

[Zapper](https://zapper.fi/dashboard) es como una navaja suiza de DeFi en Polygon. Esta plataforma te permitirá hacer farming de rendimientos en pools de liquidez, prestar tus activos en AAVE directamente desde su plataforma, presenta una interfaz con tus diferentes inversiones, y te permitirá intercambiar algunas monedas por otras. Esta es la última función que utilizaremos para intercambiar la moneda estable MAI que acabamos de tomar prestada por más DAI.

![Intercambiando MAI por DAI](../../.gitbook/assets/camDAI-zapper.png)

En nuestro ejemplo del lejano oeste, Zapper es el minero de oro que aceptará tu dinero y te venderá su oro.

### Balancer

Como se puede ver en la captura de pantalla anterior, Zapper está utilizando Balancer como el protocolo para realizar el intercambio. [Balancer](https://polygon.balancer.fi/#/) es un gestor de carteras automatizado, proveedor de liquidez y sensor de precios en el que podrás proporcionar liquidez (y obtener comisiones por ello) o intercambiar divisas utilizando los distintos pools de liquidez existentes en la plataforma.&#x20;

Para nuestra guía, utilizaremos Balancer para exponer nuestras inversiones a un poco más de volatilidad y obtener mejores intereses. Sin embargo, esto es 100% opcional.

## Descripción de la estrategia

### Estrategia principal

Aunque hayamos explicado qué es AAVE, nuestra estrategia utilizará una función de Mai Finance para automatizar el depósito del DAI en el AAVE, el depósito del amDAI en Yield y el depósito del camDAI en la bóveda de camDAI.

![](../../.gitbook/assets/camDAI-zapDAI.png) ![](../../.gitbook/assets/camDAI-zapdeposit.png)

El botón `Zap in using DAI` abre una ventana emergente que le permite depositar su DAI en la bóveda y realiza el depósito de AAVE automáticamente. Esto ahorra mucho tiempo, y algo de gas.

Este será nuestro primer paso. Suponiendo que tenemos 100 dólares en DAI, los depositaremos en Mai Finance en una bóveda de DAI. Esto nos permitirá tomar prestados MAI contra este depósito inicial.&#x20;

El ratio de Colateral a deuda, también conocido como CDR para la bóveda de camDAI es del 110%. Esto significa que la relación entre su colateral (los 100 dólares de DAI) y el préstamo que vamos a obtener tiene que ser, cómo mínimo, superior al 110%.

{% hint style="danger" %}
Si este ratio CRD alcanza el valor mínimo del 110%, significa que su colateral está perdiendo valor y su deuda puede llegar a ser mayor que el valor de su colateral. En este punto, su bóveda puede ser parcialmente liquidada: alguien puede pagar una parte de su deuda y obtener una parte de su colateral como recompensa. Sin embargo, dado que tanto DAI como MAI son monedas estables vinculadas al dólar estadounidense, el riesgo de obtener una gran diferencia entre los 2 activos es muy bajo, lo que hace que esta estrategia sea bastante segura.
{% endhint %}

Para mantener el riesgo de liquidación bastante bajo, intentaremos mantener un CDR del 115%. Para saber cuánto MAI podemos pedir prestado para mantenernos en un CDR del 115%, utilizaremos esta fórmula:

$$
MAI_{disponible} = \frac{Valor_{Colateral} - Valor_{Deuda} * CDR_{Objetivo}}{CDR_{Objetivo}}
$$

Con un valor de la garantía de 100 dólares, sin deuda aún, y un objetivo de CDR del 115%, esto es lo que podemos pedir prestado:

$$
MAI_{available}=\frac{100 - 0*1.15}{1.15}=86.95
$$

​A continuación, puedes cambiar el MAI que has tomado prestado por el DAI y repetirlo. Así es como debería quedar tu colateral y tu deuda tras repetir esto varias veces:

| Nº bucles | Colateral | Deuda   | Préstamo Disponible | APY Equivalente | DAI liquidation price |
| --------- | --------- | ------- | ------------------- | --------------- | --------------------- |
| 1         | 100.000   | 0.000   | 86.956              | 10.42%          | 0                     |
| 2         | 189.956   | 86.956  | 75.614              | 19.48%          | 0.512                 |
| 3         | 262.571   | 162.571 | 62.751              | 27.36%          | 0.681                 |
| 4         | 328.323   | 228.323 | 57.175              | 34.21%          | 0.765                 |
| 5         | 385.498   | 285.498 | 49.718              | 40.17%          | 0.815                 |
| 6         | 435.216   | 335.216 | 43.233              | 45.35%          | 0.847                 |
| 7         | 478.449   | 278.448 | 37.593              | 49.85%          | 0.870                 |
| 8         | 516.042   | 416.042 | 32.690              | 53.77%          | 0.887                 |
| 9         | 548.732   | 448.732 | 28.426              | 57.18%          | 0.899                 |
| 10        | 577.158   | 477.158 | 24.718              | 60.14%          | 0.909                 |
| 11        | 601.877   | 501.877 | 21.494              | 62.72%          | 0.917                 |
| 12        | 623.371   | 523.371 | 18.691              | 64.96%          | 0.924                 |
| 13        | 642.062   | 542.062 | 16.253              | 66.90%          | 0.929                 |
| 14        | 658.315   | 558.315 | 14.133              | 68.60%          | 0.933                 |
| 15        | 672.448   | 572.448 | 12.289              | 70.07%          | 0.936                 |
| 16        | 684.737   | 584.737 | 10.686              | 71.35%          | 0.939                 |
| 17        | 695.423   | 595.423 | 9.293               | 72.46%          | 0.942                 |

Nos detenemos en 17 bucles, pero puedes realizar tantos bucles cómo quieras.

Al final de los 17 bucles, tendrías 695,423 dólares de colateral y 595,423 dólares de deuda. Esto corresponde a un CDR del 116,79% que debería ser lo suficientemente seguro como para evitar la liquidación.&#x20;

Si consideramos el 10,42% de APY que otorga la funcionalidad de Yield de Mai Finance, esto generaría:

$$
Interes = Valor_{colateral}*APY=695.423*10.42\%= \$72.463
$$

Si tenemos en cuenta que la inversión inicial fue de sólo 100 dólares, ¡se trata de un APY equivalente del 72,463% haciendo staking con una moneda estable!

## Estrategia Alternativa

Con el fin de obtener un poco de exposición a activos de alta volatilidad, puede utilizar el mismo bucle que el anterior, pero sólo apalancar el 90% del MAI prestado, y utilizar el 10% para comprar otro activo. En este ejemplo, utilizaremos el 10% para comprar Qi (el token nativo de Mai Finance) y utilizaremos el pool Qi-BAL en Balancer que actualmente tiene una APR(Porcentaje Anual Equivalente) del 107,12%.

![Qi-BAL pool state as of October 2021](../../.gitbook/assets/camDAI-balancer.png)

Dado que estamos reinyectando menos DAI en la bóveda de camDAI, también realizaremos menos bucles. La configuración será la siguiente:

| Nº Bucles | Colateral | Deuda   | Qi     | Préstamo Disponible | APY Equivalente | Precio Liquidación DAI |
| --------- | --------- | ------- | ------ | ------------------- | --------------- | ---------------------- |
| 1         | 100.000   | 0.000   | 0.000  | 86.957              | 10.42%          | 0                      |
| 2         | 178.261   | 86.957  | 8.696  | 68.053              | 35.22%          | 0.537                  |
| 3         | 239.509   | 155.009 | 15.501 | 53.259              | 54.63%          | 0.712                  |
| 4         | 287.441   | 208.268 | 20.827 | 41.681              | 69.82%          | 0.797                  |
| 5         | 324.954   | 249.949 | 24.995 | 32.620              | 81.71%          | 0.846                  |
| 6         | 354.312   | 282.569 | 28.257 | 25.529              | 91.01%          | 0.877                  |
| 7         | 377.288   | 308.097 | 30.810 | 19.979              | 98.29%          | 0.898                  |
| 8         | 395.269   | 328.076 | 32.808 | 15.636              | 103.99%         | 0.913                  |
| 9         | 409.341   | 343.712 | 34.371 | 12.237              | 108.45%         | 0.924                  |
| 10        | 420.354   | 355.948 | 35.595 | 9.576               | 111.94%         | 0.931                  |

Al final de los 10 bucles, obtendrías

* 420.354 dólares de DAI como colateral
* $355.948 de deuda
* $35.595 de Qi&#x20;

Los mismos cálculos que en el caso anterior dan los siguientes resultados&#x20;

* Un CDR final del 118,09%, que debería considerarse lo suficientemente seguro para evitar la liquidación
* $43.800 de intereses sobre DAI del 10,42% de APY otorgado por el Yield
* $68.139 de intereses sobre su Qi del pool de Balancer, si se asume que va a componer las recompensas de Qi y BAL en el pool Qi-BAL
* Un APY total del 111,94%&#x20;

Esta estrategia presenta más riesgos en el sentido de que la inversión en el pool Qi-BAL no está garantizada. Sin embargo, obtendrá un poco de exposición a Qi, lo que le permitirá participar en el protocolo QiDAO. Si utilizas la recompensa de BAL en Mai Finance como garantía y pides un préstamo con ella, también podrás reinvertir en la bóveda de camDAI o en el pool Qi-BAL. Si lo haces, también tendrás derecho a recibir recompensas de préstamo pagadas en Qi cada semana.

## Conclusión

Con una inversión mínima y un bajo mantenimiento, puedes obtener unos resultados bastante sólidos simplemente apalancando tu DAI. Dado que DAI es una moneda estable que tiene mucha liquidez a través de múltiples cadenas, el riesgo es relativamente bajo de que DAI se desconecte y que su bóveda sea liquidada. Es el tipo de configuración conocido como "set and forget" que puede ser fácilmente un muy buen punto de partida para cualquier principiante en DeFi, y lo más probable es que esta estrategia funcione de la misma manera en un mercado alcista o en un mercado bajista. Por último, también explicamos cómo se puede utilizar la misma estrategia para hacerse con una parte del préstamo y probar las muchas posibilidades que tiene DeFi en Polygon.

## Descargo de Responsabilidad

Todo lo que se presenta en este tutorial es un contenido educativo realizado para ilustrar la opción de apalancamiento que propone Mai Finance. No hemos hablado del reembolso de la deuda porque hay artículos dedicados a ello en esta página web, pero hay que tener en cuenta que MAI Finance cobra una comisión de reembolso del 0,5% sobre el importe prestado. Como siempre, haz tus propias investigaciones y no dudes en preguntar en el [Servidor Discord de la DAO](https://discord.com/invite/qidaoprotocol).

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su propia cuenta.
{% endhint %}
