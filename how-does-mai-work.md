---
description: >-
  Entender cómo funciona MAI es crucial para cualquier inversor que realmente
  quiera entender cómo funciona Mai Finance, así que en este artículo entenderá
  cómo funciona el MAI.
---

# ¿Cómo funciona MAI?

## ¿Qué es una stablecoin?

Antes de explicar lo que es MAI, tenemos que entender lo que es una moneda estable (o stablecoin), una moneda estable es un tipo de criptodivisa que está diseñada para mantener un precio de mercado estable. La mayoría de las monedas estables están vinculadas al dólar estadounidense (se comportan o intentar comportar como el dólar, es decir, mantendrá un precio cercano a $1), pero puedes encontrar otras monedas estables vinculadas a otras materias primas como el oro (como EGold) o la plata (SilverCoin).

Sin embargo, hay dos categorías principales en las que pueden encajar todas las monedas estables, **colateralizadas** o **no colateralizadas**. Las monedas estables colateralizadas son aquellas que poseen los activos contra los que se vincula su moneda, mientras que las no colateralizadas hacen uso de algoritmos para controlar la oferta de tokens con el fin de mantener el precio fijo en un nivel predeterminado.

## El desastre de IRON Finance

Si llevas algún tiempo en el mundo de las criptomonedas, puede que recuerdes el desastre del token **TITAN** e **IRON**, pero para los que no, este es el resumen. IRON Finance era un proyecto que tenía 2 tokens, la moneda estable _IRON_ y el token _TITAN_, sin embargo la moneda estable IRON **no estaba totalmente respaldada** con monedas estables, la proporción para acuñar o producir IRON era de **75% USDC** y **25% de TITAN**. Así que básicamente era una receta para el desastre.

En junio de 2021 el token TITAN alcanzó un ATH (All-Time-High o precio record) de 65 dólares, lo que provocó que un montón de inversores, que habían invertido cantidades considerables en la moneda, decidieran vender. Esto causó un problema ya que TITAN tiene un precio basado en la oferta y la demanda. Por lo tanto, a medida que la oferta disponible de TITAN aumentaba, el precio comenzó a disminuir. Esto causó una enorme presión de venta, por lo que el precio de TITAN cayó aún más rápido, así que cuando TITAN comenzó a caer rápidamente, IRON perdió su respaldo, por lo que la stablecoin de IRON dejó de valer $1 (esto se conoce como perder el "**peg**").

![Gráfica del precio del token TITAN](.gitbook/assets/iron.jpg)

![Gráfica del precio de IRON](.gitbook/assets/titan.jpg)

La gente comenzó a comprar la moneda estable IRON para venderla por USDC y ganar algo de dinero rápido, en una gran oportunidad de arbitraje (esto es beneficiarse de las variaciones de precio de los tokens). En resumen, se ha llegado a calcular que aproximadamente se perdieron casi 1.750 millones de dólares en este incidente. Ahora, ¿hay alguna diferencia entre la moneda estable IRON y la moneda estable MAI?

## ¿Qué es MAI?

MAI es una moneda estable que está respaldada por tokens que se encuentran bloqueado en la plataforma, la producción de de MAI puede hacerse a través de **depósitos de colaterales aprobados** en bóvedas o a través de **Anchor.**

Al acuñar MAI depositando colaterales aprobados, el **CDR** (Coeficiente de Colateral a Deuda) necesita estar por encima del 150%, esto significa que si depositas $100 de colateral, la cantidad máxima de MAI que puedes pedir prestada es de $66.6667. Más adelante en este artículo veremos el por qué de esto.

Otra forma de acuñar MAI es a través del [Anchor](https://app.mai.finance/anchor), esto significa que cuando cambias una moneda estable (a partir de Septiembre de 2021 puedes acuñar MAI usando **DAI**, **USDC** y **USDT**) por MAI, el nuevo MAI es acuñado por la tesorería y el USDC depositado se mantiene guardado en la tesorería como garantía o colateral. En el caso contrario, cuando quieras obtener de vuelta tu USDC, el MAI que proporciones para el cambio se quemará.

![Monedas estables que pueden ser intercambiadas por MAI](<.gitbook/assets/image (5).png>)

Como se puede ver en la imagen de abajo, el precio de la moneda estable MAI oscila casi siempre en los $ 1, esto se debe a que, tal y cómo dice la [documentación oficial](https://docs.mai.finance/stablecoin-economics), la moneda estable MAI permite a los usuarios participar en oportunidades de arbitraje de bajo riesgo a través de Anchor cuando el precio de MAI cae por debajo de $0,99 o sube por encima de $1,01.

![Gráfica del precio del token MAI en los últimos 90 días](<.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1).png>)

## ¿Por qué se mantiene siempre en $1?

El precio se mantiene cercano al dólar mediante 2 mecanismos, a través de **Anchor** o mediante el depósito de colateral aprobado en las bóvedas (o vaults), en esta sección del artículo, entenderá el por qué

### Anchor

Anchor permite a los usuarios acuñar MAI dando a cambio monedas estables e intercambiar MAI por otras monedas estables. Además, como se puede ver en la imagen de abajo, se aplica una tasa del 1% cuando se cambian las monedas estables por MAI o viceversa, hay dos motivos principales por lo que se aplican estas tasas:

* La comisión del 1% para crear MAI crea un precio techo (price ceiling) de $1.01.
* La comisión del 1% al intercambiar MAI por otras monedas estables establece un precio de suelo de $0.99

![](<.gitbook/assets/image (9).png>)

Tener un precio de techo y suelo ayuda a MAI a no variar demasiado de su "**peg**" (recuerda que este es el término que se utiliza para decir que las monedas estables mantienen el precio de $1) sin embargo, cómo has visto en la imagen superior del gráfico de MAI, hay ocasiones donde puedes participar en oportunidades de arbitraje de bajo riesgo (lo que significa que puedes vender tus monedas estables cuando MAI está por debajo de $1 o vender MAI cuando está por encima de $1 para ganar algo de dinero rápido).

Sobre las causas de la fluctuación del precio de MAI, podría haber dos razones principales para esto:

* Si el mercado está en una **tendencia bajista**: la gente venderá sus activos volátiles y comprará monedas estables para evitar la pérdida de valor de sus activos volátiles. Esto significa que la gente querrá comprar MAI, aumentando su precio.
* Si el mercado está en una **tendencia alcista**: la gente comenzará a comprar activos más volátiles, utilizando sus monedas estables. Esto significa que la gente vende su MAI, haciendo que su precio baje.

### Depositando colateral en bóvedas

Para poder acuñar MAI utilizando las bóvedas de Mai Finance, necesitas depositar algún colateral allí y tener un **CDR** (Collateral to Debt Ratio) por encima de un cierto nivel, en este caso es del 150% (sin embargo este porcentaje puede cambiar en el futuro si la comunidad lo decidiera). Esto significa que las bóvedas estarán siempre **sobre-colateralizadas** (en un 150%) para asegurar que siempre hay más colateral para respaldar el nuevo MAI acuñado.

Recuerda que si una bóveda tiene menos de un 150% de CDR, ésta podría ser parcialmente liquidada por la comunidad, por lo que se podría perder una parte del colateral depositado si un liquidador paga parte de dicha deuda.

A medida que el valor del colateral aumenta, se puede pedir prestado más MAI, ya que un aumento del precio del colateral aumentará el CDR del préstamo. En el caso opuesto, a medida que el valor del colateral disminuye, se podrá pedir prestado menos MAI, esto se hace para evitar que el CDR caiga por debajo de la marca del 150%.

## Conclusión

Como has visto a lo largo de este artículo, la moneda estable MAI es un tipo de moneda estable que está **sobre-colateralizada,** lo que significa que siempre habrá suficiente garantía para respaldar el precio del token MAI. Esto debería dar suficiente alivio a aquellos inversores que dudan sobre invertir en proyectos que acuñan monedas estables. Además, hay que tener en cuenta que cuánto más MAI haya en el mercado, más estable será su precio.

Recientemente, se han introducido los préstamos incentivos en las bóvedas de Mai Finance, si quieres entender en qué consiste, puedes consultar este [artículo](prestamos-mai-depositos-incentivados.md). Esto ayudará aún más a la estabilidad del precio de MAI

## Disclaimer

Puedes encontrar el artículo original hecho por el equipo de Mai Finance sobre MAI [aquí](https://docs.mai.finance/stablecoin-economics).

Esta guía no es consejo financiero y ha sido realizada con un objetivo puramente educativo.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta o **DYOR**.
{% endhint %}
