---
description: >-
  Solarbeam tiene un pool de farmeo MAI-MOVR con un bonito APR. Hoy veremos cómo
  aprovecharlo.
---

# Farmeando MAI en SolarBeam

La mayoría de los tutoriales presentados en esta guía utilizan monedas estables como posición de partida. Esto se debe principalmente al hecho de que los pares de monedas estables no se ven afectados por las pérdidas impermanentes ni por la volatilidad de otros activos. Es entonces casi imposible perder su inicial, y usted puede utilizar estrategias más arriesgadas con las ganancias de sus estables para aumentar sus ganancias.&#x20;

Hoy, estamos probando otro enfoque en Moonriver con Solarbeam, actualmente la única aplicación que utiliza MAI. El par LP (Proveedor de Liquidez) allí es MAI-MOVR. MAI es la moneda estable de Mai Finance que se podrá puentear a Moonriver o acuñar desde una bóveda, y MOVR es el token de gas nativo de Moonriver. Como tal, MOVR siempre tendrá algún tipo de utilidad y nunca debería bajar de precio de forma drástica. No es un par estable, pero la única parte variable del token está vinculada a MOVR, lo que lo convierte en un buen punto de partida de todos modos.&#x20;

Vamos a ver cómo podemos generar algunos rendimientos muy altos con un bucle de retroalimentación cerrado en Moonriver sin desechar demasiados tokens de granja sobre la marcha.

![](../../.gitbook/assets/solarbeam-1.png)

## SolarBeam

### Farmeando MAI en Solarbeam

Solarbeam es el primer y principal DEX (EXchange Descentralizado) y AMM (Automatic Market Maker) en Moonriver, y la segunda aplicación en términos de TVL en la cadena. También es el primer socio de Mai Finance en Moonriver y ofrece un pool de MAI-MOVR que se recompensa con parte de su token nativo, el token SOLAR. Este es también el lugar donde encontrarás algo de liquidez para MAI.

![Par MAI-MOVR en Solarbeam a Diciembre de 2021](../../.gitbook/assets/solarbeam-2.png)

El APR (Annual Percentage Rate) del 84% es bastante alto debido al bajo uso del pool, lo que también lo convierte en un punto de partida perfecto para nuestra estrategia. Obtendrás este APR (correspondiente a un 131% APY si quieres comparar con algo como MAI-WMATIC en QuickSwap como referencia) y la recompensa se pagará en tokens SOLAR. A fecha de Diciembre de 2021, 1 SOLAR = 3,78 USDC.

### Haciendo staking de SOLAR

La mayoría de los forks de Uniswap proponen el staking de su token nativo, y Solarbeam también lo está haciendo. Puedes stakear tu SOLAR en un Vault para conseguir más SOLAR, y dependiendo de la duración de tu bloqueo, obtendrás tasas muy interesantes (hasta el 200% APRs para un bloqueo de 30 días), pero nosotros utilizaremos el staking para ganar tokens externos. De hecho, puedes apostar tus tokens SOLAR para recibir un montón de otros tokens de diferentes aplicaciones en Moonriver, y el que estamos buscando es el token ROME.

![Haciendo staking de SOLAR para conseguir ROME en Solarbeam](../../.gitbook/assets/solarbeam-3.png)

Notarás que el pool de ROME es el que tiene el APR más bajo, pero sigue siendo bastante alto, y pronto verás que nuestros tokens de ROME se multiplicarán a un ritmo loco.

## Rome DAO

Rome DAO es otro gran jugador en Moonriver. Es un Ohm-fork (copia de Olympus DAO) que utiliza el token ROME como token nativo. Podrás hacer staking de tus tokens ROME en la aplicación con el fin de obtener rendimientos muy altos. El objetivo de cada Ohm-fork es tener la mayor cantidad de tokens nativos apostados y atraer liquidez para poder sostener la emisión. Si necesita más detalles sobre los proyectos tipo Ohm, puede ver nuestro tutorial sobre [Klima DAO](https://guide.qidao.community/v/espanol/tutoriales/polygon/ohm-forks-on-polygon-the-case-of-klima) en Polygon.

![Haciendo staking de ROME en Rome DAO por un APR del 771% a Diciembre de 2021](../../.gitbook/assets/solarbeam-4.png)

Dado que obtendremos tokens ROME de Solarbeam, deberíamos poder stakearlos en Rome DAO y el sistema de rebase nos permitirá obtener mucho más rápidamente. Para esta estrategia, haremos staking de tokens ROME en Rome DAO y venderemos el 50% de la recompensa diaria, que actualmente corresponde a \~1% del depósito en Rome DAO.

## Mai Finance

Mai Finance es una plataforma de préstamos en la que podrás depositar tus criptoactivos y pedir prestada la moneda estable MAI al 0% de interés. La única comisión que se cobrará en Moonriver es la de reembolso del 0,5% de tu préstamo.

![Bóvedas de MAI Finance disponibles en Moonriver](../../.gitbook/assets/solarbeam-5.png)

Para nuestra estrategia, utilizaremos una bóveda de ETH. El token ROME que se extraerá del pool de staking de ROME DAO se dividirá de la siguiente manera:&#x20;

* El 33% se intercambiará a MOVR utilizando la función de intercambio en Solarbeam&#x20;
* El 66% se intercambiará por ETH utilizando la función de intercambio de Solarbeam&#x20;

A continuación, podrá depositar el ETH en Mai Finance para pedir prestado MAI con una CDR (Ratio de Colateral a Deuda) del 200% para mantenerse en la zona segura e intentar evitar la liquidación. El MAI prestado se utilizará entonces para crear tokens MAI-MOVR LP adicionales que se añadirán a la posición inicial en Solarbeam.&#x20;

Por ejemplo, por cada 1$ de ROME que se extraiga de ROME DAO obtendremos:

* 0,33$ de MOVR 0,66$ de ETH depositados en Mai Finance&#x20;
* 0,33$ de MAI prestados contra nuestro ETH&#x20;
* 0,66$ de token MAI-MOVR LP para añadir a Solarbeam

## Estrategia de Farmeo

La siguiente simulación se hace suponiendo lo siguiente:&#x20;

* Todos los tipos y precios se mantienen iguales durante todo el periodo de la simulación, 1 año en nuestro caso:
  * 84% de APR en el farming de MAI-MOVR en Solarbeam&#x20;
  * 108% de APR al hacer staking de SOLAR para cultivar tokens de ROMA&#x20;
  * 771% APR en Rome DAO al hacer staking de tokens de ROME&#x20;
* Todas las recompensas y protocolos funcionarán de la misma forma durante todo un año
* El 50% de las ganancias de ROME DAO se vende por un 33% de MOVR y un 66% de ETH
* &#x20;La inversión inicial es de 100$ en token MAI-MOVR LP

![](../../.gitbook/assets/solarbeam-6.png)

### Día 1

El día 1, simplemente depositaría sus 100 dólares de MAI-MOVR en Solarbeam y cosecharía sus tokens SOLAR al final del día. Esto le daría el siguiente resultado:

| MAI-MOVR | SOLAR | ROME  | ETH   | LP Adicional |
| -------- | ----- | ----- | ----- | ------------ |
| 100.000  | 0.230 | 0.000 | 0.000 | 0.000        |

### Día 2

En el día 2, mantendrás tu posición de MAI-MOVR para cultivar más SOLAR, pero también stakearas tus primeros tokens SOLAR para empezar a recolectar algunos tokens de ROME. Al final del día 2, obtendrías:

| MAI-MOVR | SOLAR | ROME  | ETH   | LP Adicional |
| -------- | ----- | ----- | ----- | ------------ |
| 100.000  | 0.460 | 0.001 | 0.000 | 0.000        |

### Día 3

Al principio del día 3, deberías poder cosechar tus primeros tokens de ROME de la recompensa de staking diaria del 50%. Probablemente no sea una buena idea hacerlo en el día 3 con sólo una inicial de 100 dólares porque la cantidad es bastante insignificante, pero aun así. Venderás el 33% por MOVR y el 66% por ETH que depositarás en tu bóveda en Mai Finance, y luego pedirás prestado MAI contra tu nueva colateral.

| MAI-MOVR | SOLAR | ROME  | ETH      | LP adicional |
| -------- | ----- | ----- | -------- | ------------ |
| 100.000  | 0.690 | 0.002 | 0.000005 | 0.000005     |

LLegados a este punto, el sistema estará funcionando de forma completa.

## Resultados de Farmeo

### Rutina diaria:

Una vez que el sistema esté completamente preparado, esta es su rutina diaria:

* Recoge SOLAR del pool de MAI-MOVR&#x20;
* Poner en staking los tokens SOLAR que acabas de conseguir.
* &#x20;Recoge los tokens de ROME del pool de staking de SOLAR&#x20;
* Stakea los tokens de ROMA recién adquiridos&#x20;
* Saque del staking el 50% de sus ganancias diarias en la DAO de ROME (corresponde a \~1,5 reajustes)&#x20;
* Venda el 66% de sus fichas ROME por ETH&#x20;
* Venda el 33% de sus tokens ROME por MOVR&#x20;
* Deposite ETH en la bóveda de ETH en Mai Finance&#x20;
* Pida prestado el 50% de su depósito como moneda estable MAI
* &#x20;Empareje el MAI prestado con los tokens MOVR&#x20;
* Deposita tus tokens MAI-MOVR adicionales

### Resultados mensuales aproximados

| day | MAI-MOVR | SOLAR stakeado | ROME stakeado | ETH     |
| --- | -------- | -------------- | ------------- | ------- |
| 30  | 100.021  | 7.135          | 0.352         | 0.023   |
| 60  | 100.190  | 14.045         | 1.550         | 0.200   |
| 90  | 100.713  | 20.978         | 3.911         | 0.740   |
| 120 | 101.872  | 27.968         | 7.869         | 1.925   |
| 150 | 104.052  | 35.072         | 14.023        | 4.148   |
| 180 | 107.788  | 42.378         | 23.204        | 7.947   |
| 210 | 113.814  | 50.019         | 36.559        | 14.065  |
| 240 | 123.142  | 58.178         | 55.580        | 23.525  |
| 270 | 137.175  | 67.158         | 82.767        | 37.745  |
| 300 | 157.848  | 77.321         | 120.875       | 58.681  |
| 330 | 187.841  | 89.226         | 174.234       | 89.041  |
| 360 | 230.861  | 103.358        | 248.711       | 132.575 |

### Día 365

Después de un año completo de farmeo, usted tendría:

* 239,633 dólares de MAI-MOVR en Solarbeam&#x20;
* 106,358 dólares en tokens SOLAR en Solarbeam&#x20;
* 263,708 dólares en tokens ROME stakeados en Rome DAO&#x20;
* 141,450 $ de ETH en Mai Finance
* &#x20;68,817 $ de deuda MAI en Mai Finance&#x20;

El MAI-MOVR adicional no se corresponde totalmente con la deuda, ya que estamos utilizando un tercio de los tokens ROME intercambiados para obtener la mitad de los nuevos tokens LP. Por tanto, este bucle le daría un APY equivalente de 583,15% a partir de una posición inicial relativamente estable.

## Descargo de Responsabilidad

Lo principal que hay que entender de esta estrategia es que Moonriver está actualmente infrautilizado y las tasas de recompensa son muy interesantes. Además, en cuanto se introduce un Ohm-fork en la estrategia para reinvertir una parte de las ganancias, las tasas de recompensa son tan descabelladas que se obtendrá un beneficio muy importante siempre que se mantengan suficientes tokens en el DAO para generar recompensas de staking.&#x20;

Sin embargo, ten en cuenta que los proyectos tendrán tasas de recompensa variables que no estarán garantizadas a lo largo de un año. Por favor, asegúrese de entender todo el proyecto en el que está invirtiendo, haga su propia investigación y asegúrese de invertir sólo lo que puede estar dispuesto a perder. Debido a que esta estrategia está invirtiendo en una inicial relativamente estable, lo único que está en riesgo aquí son los beneficios de otros sistemas. Esta guía no puede tomarse como una promoción de los proyectos que utiliza.
