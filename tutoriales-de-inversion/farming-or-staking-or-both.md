---
description: >-
  Esta guía presentará una estrategia que destacará cuales son las interacciones
  principales entre Mai Finance, QuickSwap y Adamant tras el lanzamiento de los
  nuevos LPs en Mai Finance y QuickSwap.
---

# ¿Farmear o hacer staking? ¿O Ambas?

![](../.gitbook/assets/screen-shot-2021-09-03-at-9.24.12-am.png)

## Introducción

Cuando utilizas aplicaciones DeFi (**De**centralize **Fi**nance) , especialmente cuando son granjas de farming, sueles acabar acumulando el token nativo de la granja que hayas utilizado. La mayoría de la gente suele vender dichos tokens para comprar sus cryptos favoritas , por lo que les mostraremos algunas alternativas para mantener los tokens nativos y ponerlos a trabajar, lo que incrementará tus beneficios finales.

Para realizar esto, utilizaremos las nuevas LPs (Proveedor de Liquidez) lanzadas en QuickSwap al inicio de Septiembre de 2021, que utilizan el token Qi de Mai Finance. Si necesitas más información para entender las aplicaciones de  QuickSwap y Adamant, léase el artículo [Stacking DApps guide](acumula-dapps-como-cromos.md).

## Aplicación y presentación de los nuevos pares

### Farming 

Para poder maximizar nuestras ganancias, usaremos 3 aplicaciones diferentes:

* Mai Finance.
* QuickSwap.
* Adamant.

Además utilizaremos los siguientes pares de liquidez:

* Qi/MATIC en Mai Finance para generar Qi.
* Qi/WETH en QuickSwap para generar QUICK y ADDY.
* Qi/QUICK en Adamant para generar ADDY y MATIC.

Puedes observar que cada aplicación esta generando tokens que pueden ser utilizados en las aplicaciones de arriba. La idea principal es usar los tokens Qi generados en Mai Finance en combinación con el token QUICK generado en QuickSwap, donde además estos últimos se pueden usar en Adamant. Adamant generará tokens ADDY que te permitirá reclamar dividendos en forma de WMATIC. El token WMATIC puede bloquearse en Mai Finance en la bóveda WMATIC para pedir prestado MAI, y posteriormente comprar MATIC y WETH. Estos dos tokens pueden ser usados juntos a Qi para incrementar tu posiciones tanto en Mai Finance como en QuickSwap.

### Staking

Cabe destacar que los tokens generados en Mai Finance y Quickswap pueden ser usados en:

* Qi en Mai Finance **Y **en QuickSwap pueden ser usados en **QIP** (Propuestas de mejora de QiDao). Puedes ver las QIPs actuales y anteriores [aquí](https://snapshot.org/#/qidao.eth).
* Qi en Mai Finance puede ser bloqueado. Si bloqueas tus Qi empezarás a recibir los dividendos del protocolo que son pagados en Qi cada Miércoles. Más detalles acerca del staking de Qi próximamente.
* QUICK en QuickSwap puede ser stakeado para generar tokens QUICK en "_Dragon's Lair_".
* QUICK bloqueado (dQUICK) puede ser utilizado en QuickSwap para generar otros tokens en "_Dragon's Syrup_", los que se utilizarán en este caso generan tokens ADDY .
* ADDY en Adamant son generados automáticamente, pero están bloquados 90 días), pero generarán dividendos en WMATIC.
* ADDY en Adamant puede ser bloqueado para aumentar tu APRs/APYs (**P**orcentaje de **R**ecompensas **A**nuales / **P**orcentaje de **R**endimiento **A**nual) en los pares que estés utilizando en la página, así cómo generando más ADDYs, e incrementando tus diviendos de MATIC.

## Realizando Bootstrapping

![](../.gitbook/assets/screen-shot-2021-09-08-at-6.54.08-am.png)

A continuación, se va a realizar una simulación con una inversión inicial de $1,000 en los pares de liquidez (LPs) Qi/MATIC y Qi/WETH , teniendo en cuenta que los APRs / APYs utilizados son los que habían el **9 de Septiembre de 2021**. Cabe destacar que los porcentajes variarán, el precio de los tokens no será constante o que algunos programas pueden dejar de estar operativos. Por lo que los resultados son sólo una estimación de lo que podrías obtener si todo se mantuviera tal y cómo estaba el **9 de Septiembre de 2021,** cosa que nunca se producirá, así que este ejemplo se debe tomar como un recurso educativo.

### Día 1

{% hint style="info" %}
**ATENCIÓN: **Los porcentajes de los pares de liquidez utilizados a continuación son aquellos que estuvieron disponibles unas horas más tarde de la primera implementación de éstos, por lo que los APRs y APYs no van a ser los mismos a la hora de la lectura, donde además se realizarán revisiones continuas. Por favor, **DYOR **y utiliza esta guía con precaución.
{% endhint %}

Ya que tenemos $500 del par de liquidez Qi/MATIC y $500 del par de liquidez Qi/WETH,  los depositaremos en Mai Finance y Quickswap respectivamente. Por otro lado, si prefieres acumular Qi o Quick, puedes aumentar los tokens del par de liquidez que prefieras, ya que así se te generarán más de tus tokens favoritos, por lo que así tendrás más para poder realizar staking de éste. En este ejemplo, se utilizará una división del 50% del capital inicial.

* $500 de Qi/MATIC estarán en Mai Finance, con un APR del 1160.65%.
* $500 de Qi/WETH estarán en QuickSwap, con un APR del 1817.44%.

Además utilizaremos los siguientes APRs para el resto de la simulación:

* APR de dQUICK del "_Dragon's Lair _" es el 17.28%.
* APR de ADYY del "_Dragon's Syrup_" es el 17.08%.
* APR de Qi/QUICK en Adamant para los pares autocompuestos es del 133%.
* APR de Qi/QUICK en Adamant para los tokens es del 131%.
* APR de WMATIC en Adamant es el 35% de tus tokens ADDY bloqueados.

Ya que el APR generado en Mai Finance es inferior al de Quickswap, utilizaremos el 100% del Qi generado en Mai Finance para obtener más tokens del par Qi/QUICK, es decir, el Qi no se venderá directamente, sino que se combinará con el token QUICK recibido en Quickswap. Esto supondrá que al final de esta operación tendremos 0 Qi. Sin embargo, si decides dividir tu inversión inicial de forma diferente, podrás tener 0 QUICK y algo de Qi.

Por lo que al final del Día 1 tendremos en nuestro portafolio lo siguiente:

| Tipo de Recompensa  | Valor en Dólares |
| ------------------- | ---------------- |
| dQUICK en QuickSwap | 8.997            |
| ADDY en QuickSwap   | 0                |
| Qi/QUICK en Adamant | 31.799           |
| ADDY en Adamant     | 0                |
| WMATIC en Adamant   | 0                |

### Día 2

En el 2º día, el dQUICK depositado en el "_Dragon's Syrup_" de QuickSwap comienza a generar tokens ADDY, así cómo el par Qi/QUICK en Adamant. Al final del día 2 se obtendrá lo siguiente: 

| Tipo de Recompensa  | Valor en Dólares |
| ------------------- | ---------------- |
| dQUICK en QuickSwap | 17.998           |
| ADDY en QuickSwap   | 0.0042           |
| Qi/QUICK en Adamant | 63.713           |
| ADDY en Adamant     | 0.114            |
| WMATIC en Adamant   | 0                |

Es importante no olvidar que hay que reclamar las recomensas diarias de Adamant, para así generar mas dividendos en forma de WMATIC.

### Día 3

En el Día 3, los tokens ADDY reclamados en Adamant comenzarán a generar diviendos en forma de WMATIC. Al final del día 3 se obtendrá lo siguiente: 

| Tipo de Recompensa  | Valor en Dólares |
| ------------------- | ---------------- |
| dQUICK en QuickSwap | 27.004           |
| ADDY en QuickSwap   | 0.025            |
| Qi/QUICK en Adamant | 95.743           |
| ADDY en Adamant     | 0.343            |
| WMATIC en Adamant   | 0.0001           |

A partir del día 4 podremos realizar lo siguiente:

* Recoger los dividendos en forma de WMATIC.
* Depositar una parte del WMATIC en Mai Finance y pedir prestado MAI gracias al colateral aportado.
* Vender MAI para comprar más WETH.
* Crear el par de liquidez de MATIC con Qi, y el WETH con Qi generado en Mai Finance.
* Deposit el par Qi/WMATIC adicional en Mai Finance y el par Qi/WETH en QuickSwap.

Llegados a este punto, el sistema de farmeo está completado, por lo que podemos empezar a calcular los beneficios.

## Resultados del Farmeo

### Rutina Diaria

La rutina diaria de esta estrategia está formada por las siguientes transacciones:

* Recolectar el Qi en Mai Finance.
* Recolectar el WMATIC en Adamant.
* Depositar el 66% del WMATIC en Mai Finance.
* Pedir prestado MAI por el 50% del depósito.
* Cambiar MAI por WETH.
* Crear el par Qi/WMATIC en QuickSwap.
* Depositar el par Qi/WMATIC en Mai Finance.
* Crear el par Qi/WETH en QuickSwap.
* Depositar el par Qi/WETH en QuickSwap.
* Recoger el token Quick en QuickSwap.
* Crear el par Qi/QUICK en QuickSwap.
* Depositar el QUICK restante en "_Dragon's Lair"_.
* Depositar dQUICK en_ "Dragon's Syrup"_.
* Recoger el token ADDY de _"Dragon's Syrup"._
* Recoger el token ADDY de Adamant.
* Depositar el nuevo par Qi/QUICK en Adamant.
* Depositar el ADDY recogido en Adamant (éste será bloqueado por 90 días).

### Estimación de Resultados Mensuales

| Mes | dQUICK    | Qi/QUICK   | ADDY       | <p>Qi/MATIC <br>Qi/WETH</p> |
| --- | --------- | ---------- | ---------- | --------------------------- |
| 1   | $280.96   | $1,040.78  | $54.97     | $0.91                       |
| 2   | $557.79   | $2,162.98  | $224.36    | $7.89                       |
| 3   | $842.08   | $3,413.73  | $521.09    | $27.85                      |
| 4   | $1,138.60 | $4,816.62  | $960.17    | $68.48                      |
| 5   | $1,454.30 | $6,405.18  | $1,559.60  | $138.44                     |
| 6   | $1,798.77 | $8,224.86  | $2,341.64  | $247.49                     |
| 7   | $2,184.58 | $10,335.38 | $3,334.13  | $406.84                     |
| 8   | $2,627.76 | $12,813.60 | $4,572.23  | $629.47                     |
| 9   | $3,148.40 | $15,757.01 | $6,100.39  | $930.60                     |
| 10  | $3,771.42 | $19,288.05 | $7,974.83  | $1,328.32                   |
| 11  | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31                   |
| 12  | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79                   |

### Día 365

Tras realizar esta estrategia por un año, hemos obtenido los siguientes resultados:

| Tipo de recompensa           | Valor en Dólares |
| ---------------------------- | ---------------- |
| dQUICK en QuickSwap          | 5,628.29         |
| ADDY en QuickSwap            | 365.25           |
| Qi/QUICK en Adamant          | 29,733.58        |
| ADDY en Adamant              | 13,587.56        |
| Qi/MATIC y Qi/WETH Adicional | 2,631.07         |

Cabe destacar que el ADDY que se generaba diariamente en la granja de QuickSwap no se ha recogido de forma diaria y añadido a Adamant para incrementar las recompensas en esta simulación, para simplificar los cálculos.  Además una vez pasado los 90 días del bloqueo del ADDY, no se volvió a bloquear el ADDY de nuevo, por lo que se podría obtener más recompensas en Adamant, así cómo obtener mas WMATIC.

Finalmente, tras un año el beneficio generado es de $51,580.50. Si consideramos que la inversión inicial fue de $1,000 de Qi/MATIC y Qi/WETH, esto significa un APY del 5 087.39%.

## Descargo de Responsabilidad

Esta guía no ha sido diseñada como consejo financiero, sino como guía educativa. Debes tener cuidado con las fluctuaciones del precio, con la oferta y demanda, las variaciones de los APRs en las distintas aplicaciones, pérdida impermanente, etc. El propósito de esta guía no ha sido para que ésta sea llevada al pie de la letra, así que por favor, tenga cuidado y sólo invierta aquello que está dispuesto a perder.

{% hint style="info" %}
Ten en cuenta que una estrategia que funciona bien en un momento dado puede funcionar mal (o hacerle perder dinero) en otro momento. Mantente informado, controla los mercados, controla tus inversiones y, como siempre, haz tu propia investigación.
{% endhint %}
