---
description: Usando MAI en Moonbeam para ganar rendimiento con StellaSwap.
---

# Utilizando MAI como Legos en StellaSwap

Aunque Mai Finance no ofrece bóvedas en Moonbeam, es posible utilizar algunos de tus tokens favoritos en la cadena para acuñar MAI utilizando las nuevas bóvedas MAI de StellaSwap. Aprovechando tus tokens de garantía y pidiendo prestado MAI contra ellos, puedes ganar un gran rendimiento a través de una estrategia de bucle que involucra a xSTELLA y MAI.&#x20;

NOTA: Esta guía no pretende ser un consejo financiero. Fue creada con un objetivo educativo en mente. El objetivo de esta guía no es proponer una estrategia a seguir ciegamente, así que por favor haga sus deberes y su propia simulación, y sólo invierta lo que esté dispuesto a perder posiblemente.

[StellaSwap](https://stellaswap.com/) es el principal DEX (intercambio descentralizado) en Moonbeam. Como DEX con todas las funciones, StellaSwap ofrece a los usuarios la posibilidad de intercambiar tokens, ganar rendimiento en las granjas y participar en el gobierno del protocolo. Lo que diferencia a StellaSwap es que es el primer protocolo de este tipo que permite a los usuarios acuñar MAI de forma nativa directamente desde su interfaz a través de una asociación con Mai Finance.

![Minteando MAI usando StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### Minteando MAI en StellaSwap

A diferencia de las cajas fuertes de MAI en Mai Finance, las cajas fuertes de MAI de StellaSwap cobran intereses por pedir prestado contra sus activos. Actualmente, los usuarios pueden pedir prestado MAI contra xStella, el token de reparto de ingresos de StellaSwap, a un interés del 12%, o contra wGLMR, una versión "envuelta" del token de gas nativo de Moonbeam, a un interés del 8%. Aunque los usuarios familiarizados con las cajas fuertes de Mai Finance con un interés del 0% podrían sorprenderse por los tipos de interés más elevados, en esta guía veremos una estrategia de bucle que le permitirá obtener altos rendimientos de sus stablecoins prestadas sin tener que salir de StellaSwap.

![Vaults en StellSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. Primero, vaya a la pagina que permite mintear [MAI.](https://app.stellaswap.com/mai)
2. Desde aquí podrá crear una bóveda xStella o wGLMR para tomar prestado el MAI. Para crear nuestra estrategia de bucle, crearemos una bóveda xStella.
3. Ahora entre en su bóveda recién creada y deposite xStella. Tenga en cuenta que los depósitos de xStella tienen un 40% de LTV (relación préstamo-valor), lo que significa que por cada 100 dólares de xStella, podrá pedir prestados 40 dólares de MAI.&#x20;
4. A continuación, deberás dirigirte a la sección de préstamos, y tomar prestados MAI. Ten en cuenta tu LTV para evitar que te liquiden.

![Vault de xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### Poniendo el sistema en marcha

Ahora que has tomado prestado MAI con éxito, ¡es el momento de ponerlo en práctica! Aprovecharemos nuestro MAI depositándolo en la granja de stablecoins MAI-Base4Pool de StellaSwap y utilizaremos los rendimientos para ganar más tokens de Stella apostando por ellos. ¡Recuerda siempre que si entras en esta estrategia lo haces bajo tu propio riesgo y tu bóveda puede ser liquidada si no haces tu debido estudio!

Primero encontremos el MAI-Base4Pool en la pagina de [Granjas](https://app.stellaswap.com/farm) de StellaSwap.

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Esta granja ofrece actualmente un rendimiento muy atractivo del 26% en monedas estables con un pool compuesto por MAI, FRAX, USDT, USDC y DAI con un rendimiento pagado en tokens de Stella. Tenga en cuenta que este rendimiento compensa en gran medida el interés que estamos pagando actualmente por nuestro MAI prestado (12%). Podemos echar un vistazo a nuestro rendimiento hasta ahora:

$$interes real = (colateral * interes del prestamo)-(mai*rendimiento del farming)$$

Esto nos da un rendimiento efectivo del 1,6% al pedir prestado MAI - no está mal, pero podemos hacerlo mejor. Ahora podemos tomar los tokens de Stella que estamos ganando por estar en el MAI-Base4Pool y [hacer staking para recbir xStella](https://app.stellaswap.com/xstella).

![Staking de xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

Stakear xStella tiene dos beneficios adicionales. En primer lugar, proporciona un APR de staking del 70%, con lo que aumentan nuestros rendimientos, pero lo más importante es que xStella aumenta su valor con el tiempo, ya que los ingresos por intercambio del protocolo se reparten entre los usuarios que hacen staking. Esto significa que los rendimientos que obtenemos de nuestra posición relativamente segura en una granja de stablecoin, aumentan continuamente. Podemos entonces utilizar estos rendimientos adicionales para depositar xStella adicional en nuestra bóveda para aumentar nuestra LTV, o para pedir prestado MAI adicional contra ella.

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como un respaldo al proyecto..

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
