---
description: >-
  En esta guía, utilizaremos el concepto de bonos para obtener activos a un
  precio inferior al del mercado, y utilizaremos protocolos que ofrecen altas
  recompensas para aumentar las ganancias.
---

# Combo Exodia en Fantom

## Introducción

Una de las cosas más importantes que hay que tener en cuenta cuando se invierte en cripto es asegurarse de que su inversión inicial está protegida. Si tiene en cuenta este aspecto fundamental, sólo puede poner en riesgo sus ganancias. Sin embargo, hay otra opción si quieres invertir en un token que representa cierta incertidumbre: comprarlo con un descuento, y asegurarte de que las recompensas son lo suficientemente altas como para cubrir tu inversión inicial lo más rápido posible.&#x20;

Desde hace unos meses, esto es posible con la introducción de los bonos, y las tasas de recompensa muy altas que proponen algunos proyectos. Así que hoy, exploramos dos proyectos en Fantom que están utilizando el concepto de bonos con el fin de lograr 2 objetivos muy diferentes.

![](../../.gitbook/assets/exodia-tomb-0.png)

## Exodia

### Presentación del proyecto

[Exodia](https://app.exodia.fi/dashboard) es un pequeño proyecto en Fantom que tiene un potencial gigantesco. Se trata de un fork de Ohm basado en el token EXOD que es una moneda de reserva respaldada por diferentes activos. Los activos de respaldo iniciales añadidos a la tesorería de Exodia eran DAI y FTM, pero el equipo y el DAO a cargo del protocolo decidieron desarrollar vínculos con la comunidad de Olympus y destinar el 33% de sus reservas excedentes a la compra de activos denominados en OHM. Por ello, una pequeña parte de la tesorería está denominada en tokens gOHM.

![Desglose de la tesorería de Exodia en Enero de 2022](../../.gitbook/assets/exodia-tomb-1.png)

### Haciendo bonding con el token LP&#x20;

Para reforzar los lazos, Exodia votó recientemente para aumentar la cantidad de tokens relacionados con OHM en su tesorería, y pronto aceptará un nuevo token como parte de su programa de bonos. El nuevo token es un token LP (Liquidity Providing) que se puede crear en BeethovenX. Una de las mejores cosas de los tokens de BeethovenX es que se pueden crear incluso si sólo se posee un único activo de la selección en el pool, lo que lo hace fácilmente accesible. El token LP se compone de:

* 20% wFTM&#x20;
* 20% EXOD&#x20;
* 20% wsEXOD
* 20% gOHM&#x20;
* 20% MAI

![El Monolith pool en BeethovenX en Enero de 2022](../../.gitbook/assets/exodia-tomb-2.png)

Esta es probablemente el primer fork de Ohm que utiliza un token de LP del fork Balancer para hacer bonos. Esto es particularmente interesante en el sentido de que ahora puede comprar nuevos bonos utilizando sólo sus tokens EXOD. Los pasos serían los siguientes:

* deposite su token EXOD en `The Monolith` en BeethovenX para obtener el token LP
* Vender su token LP en la aplicación Exodia para comprar nuevos EXOD con un descuento&#x20;
* Espere el periodo de adquisición de derechos y recoja sus tokens EXOD
* &#x20;Repetir&#x20;

Esto reduce drásticamente la presión de venta de tokens EXOD, lo que sólo puede beneficiar al protocolo. Anteriormente los "flippers" de bonos tendrían que vender sus EXOD para DAI para comprar bonos adicionales, lo que es parcialmente perjudicial al reducir el precio de los tokens, y tiene un efecto en cascada en la tesorería.

{% hint style="info" %}
Si no está familiarizado con los proyectos de Ohm, le recomiendo encarecidamente que lea algo más sobre el tema. Puede consultar nuestra guía sobre Klima (véase la sección Polígono) o ir directamente a la[ documentacion oficial de Exodia](https://docs.exodia.finance). Además, puedes unirte a su discordia e inscribirte en su plan de educación.
{% endhint %}

También se ve que el token LP acepta MAI, la moneda estable que se puede acuñar en Mai Finance. Esta será en realidad nuestra principal fuente para el LP (ver más adelante). Una vez que hayas comprado tus bonos con un descuento decente, obtendrás tus tokens EXOD al final del período de adquisición de derechos.&#x20;

También puedes stakear este token a un decente APY (Annual Percentage Yield) del 38,787%, que equivale a un APR (Annual Percentage Rate) del 601%, o una ganancia diaria del 1,65%. Utilizaremos el sistema de bonos para comprar tokens EXOD con un descuento, y nos beneficiaremos del altísimo APY para recoger las ganancias de las recompensas de los rebases.

## Tomb Finance

[Tomb Finance](https://tomb.finance) es un proyecto muy particular, original en muchos sentidos. El token TOMB es una moneda estable algorítmica vinculada al token FTM, y diseñada para ser un medio de intercambio y añadir liquidez adicional a FTM, el token de gas de la cadena Fantom. El ecosistema de Tomb Finance propone 2 tokens más:

* TSHARE: es el token de gobernanza de Tomb Finance. Los titulares de TSHARE tienen poder de voto. Los poseedores de TSHARE también recibirán TOMBs adicionales. La emisión de tokens TOMB adicionales a los poseedores de TSHARE sigue la misma mecánica que las bifurcaciones de Ohm, acuñándose nuevos tokens al final de cada época con un APY muy alto.&#x20;
* TBOND: se trata de un token especial que se utiliza principalmente para mantener el peg a 1 FTM. Cuando el precio de TOMB cae por debajo de 1 FTM, los usuarios pueden comprar TBOND al precio actual de los tokens TOMB. Pueden hacerlo vendiendo tokens TOMB al protocolo, y estos tokens se queman, lo que aumenta el valor de TOMB de nuevo a 1 FTM. Comprar TBOND con descuento y poder canjear tokens TOMB dio el nombre al token TBOND. Cuando el token TOMB está por encima de la clavija, las personas pueden canjear sus TBOND por TOMB. Se acuñan nuevos TOMB, lo que reduce el valor del token. En otras palabras, ¡se trata de un token de arbitraje!

![TOMB, TBOND and TSHARE values as of January 2022](../../.gitbook/assets/exodia-tomb-3.png)

Tomb Finance también propone 2 LP pools que le harán ganar tokens TSHARE. Esto es especialmente importante para que Tomb Finance tenga una profundidad de liquidez muy importante. Sin embargo, para lograr el objetivo convertir a TOMB como una solución alternativa a FTM, es importante que el protocolo tenga usuarios que usen TOMB, y por lo tanto sean dueños de la liquidez. Cuando cultivas los pools TOMB-FTM y TSHARE-FTM, eres recompensado con tokens TSHARE que te permitirán ganar más tokens TOMB, lo que supone un pequeño y agradable bucle cerrado dentro de una única aplicación.

## Piezas adicionales para cerrar el bucle

Ahora que presentamos las 2 grandes piezas para nuestra estrategia, veamos rápidamente las otras piezas del rompecabezas del día.

### Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) es un optimizador de rendimientos que aceptará tokens de LP de DEX (Exchanges Descentralizados) particulares, cosechará tokens de recompensa, y dejará que sus algoritmos vendan la recompensa por LP adicionales. Como tal, puede obtener una posición de inversión creciente que compondrá sólo los tokens del LP y capturará el valor del token de recompensa en el momento en que el token sea cosechado. Para nuestra estrategia, utilizaremos el token TOMB-FTM LP. Las razones son múltiples:&#x20;

* TOMB al estar ligado al token FTM, no hay IL (Pérdida Impermanente) en este par, por lo que la única variación estará ligada a la variación del precio del FTM
* TOMB-FTM se recompensa con TSHARE, por lo que la venta de TSHARE no afectará a los 2 tokens del par TOMB-FTM&#x20;
* Tiene un APY bastante alto que para un token LP sin IL utilizando el token LP en beefy le permitirá obtener el recibo`mooTombTOMB-FTM`&#x20;

![Pares LP de Tomb en Beefy Finance en Enero de 2022](../../.gitbook/assets/exodia-tomb-4.png)

{% hint style="info" %}
Para el propósito de esta guía, estamos utilizando TOMB-FTM token porque presenta menos riesgo debido a la ausencia de pérdida impermanente en el par. Sin embargo, usted puede utilizar totalmente el par TSHARE-FTM para obtener mayores recompensas. Asegúrese de entender los riesgos y DYOR primero.
{% endhint %}

### Mercado de préstamos Market XYZ

[Market.XYZ](https://fantom.market.xyz/pool/3) es un protocolo de préstamo en el que podrá depositar algunos activos particulares y pedir préstamos contra ellos. Cuando presta su activo, puede obtener algunos incentivos de préstamo pagados en el activo que presta. Cuando pides un préstamo, tendrás que pagar algunos intereses en el momento de la devolución en el mismo activo que pediste prestado.

Market XYZ inició una asociación con Mai Finance en 2021 con el fin de permitir que se utilicen clases adicionales de activos como garantía para tomar prestada la stablecoin MAI. Estos activos se consideran más arriesgados que los que actualmente se aceptan directamente en Mai Finance, o simplemente están a la espera de un oráculo de ChainLink y no se aceptan directamente en la app principal. Esto aporta beneficios adicionales: el protocolo QiDAO está ganando comisiones de los MAI prestados, los prestatarios están obteniendo MAI a bajos tipos de interés (Mai Finance está añadiendo más MAI de la tesorería regularmente en base a la demanda) y es un caso de uso muy interesante para la moneda estable, impulsando su uso. Por otro lado, los mercados de préstamos son una gran manera de iniciar relaciones sólidas con diferentes socios mientras esperan que sus activos sean aceptados en Mai Finance directamente.

![TOMB Beefy Locker en Market XYZ  en Enero de 2022](../../.gitbook/assets/exodia-tomb-5.png)

El mercado de préstamos que nos interesa para esta estrategia es el locker TOMB Beefy. Después de depositar nuestros tokens TOMB-FTM en Beefy, recibimos un token de recepción mooTombTOMB-FTM que es una "prueba de propiedad" para el token que está componiendo las recompensas en Beefy. Este token de recibo se puede utilizar como garantía en MarketXYZ para pedir préstamos adicionales de MAI.

{% hint style="danger" %}
Market.XYZ sólo permite préstamos con un valor mínimo de 0,05 ETH (\~$170,00 en el momento de escribir este artículo). Asegúrate de depositar suficientes garantías si quieres pedir un préstamo en las diferentes taquillas.
{% endhint %}

En la captura de pantalla anterior, se puede ver que:

* Podemos depositar el token mooTombTOMB-FTM como garantía y obtener un 355,4% de APY, proporcionado por Beefy&#x20;
* Pedir prestado MAI contra nuestra garantía con un 15,02% de tasa de interés (APR)&#x20;

Es fácil ver que las ganancias que obtenemos del cultivo de LP superan con creces los intereses del préstamo, lo que hace que esta estrategia sea viable. Sin embargo, asegúrate de vigilar adecuadamente el precio de FTM y TOMB para evitar su liquidación y asegúrate de pedir un préstamo con un CDR (Collateral to Debt Ratio) muy alto, lo que te permitirá tener tiempo suficiente para devolver el préstamo en caso de una caída masiva del precio.

{% hint style="info" %}
Si no te interesa esta estrategia pero eres usuario de Mai Finance, Market XYZ es una aplicación increíble para prestar tu MAI. Se le pagará en MAI adicional que se compone en su posición.
{% endhint %}

## Estrategia de Farmeo

Para completar nuestro bucle de inversión, comenzaremos con la compra de bonos EXOD utilizando MAI. Las recompensas de EXOD se utilizarán para comprar tokens TOMB-FTM LP. Los tokens se utilizarán en Beefy para componer las recompensas de TSHARE. Además, el recibo de tokens LP se utilizará como garantía en el Mercado XYZ para pedir más MAI, lo que nos devuelve a nuestro paso inicial.&#x20;

Simularemos con algunas suposiciones todas las tasas y precios de las recompensas permanecen iguales durante un año:

* El APY de Exodia es del 38,787%.&#x20;
* El APY de TOMB-FTM mediante beefy es del 318,51%.&#x20;
* El interés de préstamo en Market XYZ es del 15,02% APRs (el interés no se compone, por lo que utilizamos APRs cuando nos referimos a las tasas de préstamo)&#x20;

Además, vamos a suponer que usted está cosechando sus bonos y tokens EXOD extra diariamente y stakea el 50% para beneficiarse de los reembolsos tan pronto como sea posible. Los bonos se comprarán con un descuento medio del 0% para simplificar, pero es de esperar que los consigas con un descuento mejor, y asumiremos que podemos comprar nuevos bonos cada 5 días.

![](../../.gitbook/assets/exodia-tomb-6.png)

### Día 1

Primero tenemos que averiguar qué punto de entrada presenta menos riesgo. El LP TOMB-FTM parece ajustarse exactamente a esto (ver las razones detalladas en la descripción del par LP), así que comenzaremos el bucle en este punto con 1.000 dólares en tokens TOMB-FTM. Una vez que el token LP ha sido creado en SpookySwap, puede depositarlo en Beefy Finance y empezar a pedir prestado de inmediato. Para esta estrategia, intentaremos ceñirnos a un CDR del 300%.

Esto significa que podremos pedir prestados 333 dólares de MAI en la taquilla con un tipo de interés del 15,02%. El MAI prestado se utilizará en BeethovenX para obtener un token wFTM-EXOD-gOHM-wsEXOD-MAI LP. Finalmente, compraremos un bono EXOD con el LP. Tenga en cuenta que toda la configuración se puede hacer en el Día 1. Al final del primer día (suponiendo 3 rebases) obtendremos:

| Posición           | Valor ($) |
| ------------------ | --------- |
| TOMB-FTM           | 1,000.000 |
| Préstamo de MAI    | 333.333   |
| EXOD               | 66.667    |
| TOMB-FTM adicional | 3.930     |
| EXOD adicional     | 1.098     |

### Día 2, 3, 4 y 5

Los próximos días, es inútil hacer nada por la cosecha y la composición de las recompensas EXOD ya que el bono que compramos en el día es todavía vesting. Así que podemos dejar que el token TOMB-FTM LP crezca en precio sin pedir más y centrarnos en las recompensas EXOD. El 50% de la recompensa se convertirá en más EXOD, y el otro 50% se añadirá al TOMB-FTM LP. Al final del Día 5, cuando el bono esté totalmente consolidado, tendríamos:

| Posicion           | Valor ($) |
| ------------------ | --------- |
| TOMB-FTM           | 1,021.369 |
| Préstamo de MAI    | 333.333   |
| EXOD               | 338.869   |
| TOMB-FTM adicional | 4.014     |
| EXOD adicional     | 5.582     |

{% hint style="info" %}
El TOMB-FTM y el EXOD adicionales son sólo lo que se produce en el día 5 y se compone al principio del día 6.
{% endhint %}

### Día 6

El TOMB-FTM compuesto en el día 5, así como el 50% de EXOD cosechado, le dan un total de 1.028,173 $ de TOMB-FTM al comienzo del día 6. Esto significa que su posible préstamo es de 342,724 $, lo que le permite pedir prestados 9,391 $ adicionales de MAI que se utilizarán para comprar un nuevo bono en Exodia. En este punto, el sistema está preparado y puede simplemente gestionar su inversión a través de una rutina diaria ligera.

### Rutina Diaria

La rutina se divide en 2 partes: la verdadera rutina diaria que tendrás que operar diariamente, y una que tendrás que operar cada 5 días.

&#x20;Diariamente, tendrás que:

* Reclamar tokens EXOD adquiridos en Exodia
* Stakear el 50% de los tokens EXOD en Exodia&#x20;
* Vender el 25% de los tokens EXOD por FTM en SpookySwap&#x20;
* Vender el 25% de los tokens EXOD por TOMB en SpookySwap
* Crear un token TOMB-FTM LP en SpookySwap&#x20;
* Depositar el token TOMB-FTM LP en Beefy Finance&#x20;
* Depositar el token de recepción mooTombTOMB-FTM en Market.xyz&#x20;

Además, cada 5 días, tendrás que:

* Pedir prestado MAI adicional en Market.xyz para mantener un CDR del 300%.
* Depositar el MAI prestado en BeethovenX en el pool del Monolith&#x20;
* Intercambiar su token Beethoven LP por un bono EXOD en Exodia

### Resultados mensuales aproximados

Estos serían los resultados aproximados:

| Día | TOMB-FTM   | EXOD       | Deuda Mai  |
| --- | ---------- | ---------- | ---------- |
| 30  | 1,222.088  | 488.438    | 407.363    |
| 60  | 1,531.135  | 735.586    | 510.378    |
| 90  | 1,956.250  | 1,093.089  | 652.083    |
| 120 | 2,546.404  | 1,609.179  | 848.801    |
| 150 | 3,371.740  | 2,353.088  | 1,123.913  |
| 180 | 4,532.773  | 3,424.178  | 1,510.924  |
| 210 | 6,173.591  | 4,965.049  | 2,057.864  |
| 240 | 8,500.790  | 7,180.350  | 2,833.597  |
| 270 | 11,810.653 | 10,363.762 | 3,936.884  |
| 300 | 16,528.139 | 14,936.728 | 5,509.380  |
| 330 | 23,262.834 | 21,504.023 | 7,754.278  |
| 360 | 32,889.239 | 30,933.491 | 10,963.080 |

### Día 365

Después de un año completo de cultivar este sistema, y asumiendo que todo es igual que el día 1 (precios, tarifas y todo lo demás...), tendrías:&#x20;

* 34.855,954 dólares en tokens TOMB-FTM LP en Beefy&#x20;
* 32.863,908 $ de tokens EXOD&#x20;
* Una deuda de 11.618,651 dólares de MAI en Market.xyz, con algunos intereses adicionales que hay que pagar (lo que corresponde a una deuda total de 13.363,772 dólares)

&#x20;Es muy importante tener en cuenta que su Ratio de Colateral a Deuda se mantiene cerca o por encima del 300% en cualquier momento del ejercicio, por lo que es totalmente posible que venda una parte de su TOMB-FTM o EXOD para amortizarlo y bajar los inteses. También es posible ajustar la parte de EXOD que vendes diariamente para simplemente amortizar tu préstamo inicial y comprar nuevos bonos EXOD vendiendo TOMB-FTM. Las variaciones son infinitas, así que siéntase libre de ajustar según lo que más le guste. Al final, a partir de una inversión inicial de 1.000 dólares, usted terminaría con 67.719,862 dólares y una deuda de 13.363,772 dólares, lo que corresponde a un APY global de 5.335,56%.

## Descargo de Responsabilidad

Esta es una guía experimental que está destacando cómo puede aumentar sus ganancias mediante la adición de forks de Ohm en sus bucles de inversión. La simulación se hizo en un momento en el que Exodia tenía un APY muy alto en los tokens EXOD apostados. Lo mismo puede decirse de TOMB-FTM. Estos ratios tan elevados suelen variar mucho, por lo que se pueden esperar muchos menos beneficios a lo largo de un año completo. De hecho, la mayoría de los forks de Ohm no están diseñados para mantener unos rendimientos tan altos durante más de unos meses, y generalmente reducen drásticamente su emisión para seguir emitiendo tokens.&#x20;

Mantente informado sobre los proyectos que utilizas, no dudes en hacer preguntas y, como siempre, haz tus propias investigaciones.

{% hint style="info" %}
Esta guía no es en absoluto un consejo financiero, sino que se ha realizado con un objetivo educativo. Es necesario prestar atención a las variaciones de precios, la oferta y la demanda, las fechas de finalización de los programas de recompensa, las pérdidas impermanentes, etc ... El objetivo no era proponer recetas que se puedan seguir a ciegas, así que por favor haga sus deberes y su propia simulación, y sólo invierta lo que esté dispuesto a perder posiblemente.
{% endhint %}
