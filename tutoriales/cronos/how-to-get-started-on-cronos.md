---
description: >-
  En este artículo te explicaremos todo lo que necesitas saber para poder
  utilizar la red de Crono
---

# Cómo comenzar en Cronos

## ¿Qué es Cronos?

Será difícil explicar qué es Cronos sin mencionar a Crypto.com. Crypto.com es uno de los mayores intercambios centralizados (también conocido como CEX) y está construyendo su propio conjunto de cadenas, incluyendo Crypto.org Chain y Cronos. Crypto.org Chain es una cadena con tecnología propia mientras que Cronos es su hermana compatible con EVM (Ethereum Virtual Machine).&#x20;

Es prácticamente lo mismo que la cadena de Binance dedicada a la CEX, y la cadena inteligente de Binance que es compatible con EVM. Entre otras ventajas, Cronos presenta compatibilidad con EVM, lo que significa que la mayoría de las aplicaciones que se lanzaron en otras cadenas EVM también pueden ser desplegadas en Cronos, incluyendo Mai Finance, y Scalability: Cronos es más rápido y más barato que la Mainnet de Ethereum.

## ¿Cómo comenzar a usar Cronos?

Para utilizar la red Cronos, necesitarás una dirección de monedero. Dado que Cronos es una red compatible con EVM, aceptará los mismos monederos que en otras cadenas compatibles con EVM, incluyendo monederos web como Metamask o Nifty, y podrás utilizar tu monedero hardware como Trezor o Ledger.

&#x20;Para este tutorial, nos ceñiremos a Metamask como con el resto de guías de esta página web. Si no tienes Metamask instalado, puedes encontrar instrucciones en [Cómo comenzar en Polygon](https://guide.qidao.community/v/espanol/tutoriales-de-polygon/how-to-get-started-on-polygon).

### Añadiendo Cronos a Metamask

Si has instalado la última versión de Metamask, ya deberías tener acceso a la cadena Cronos y no tienes que hacer nada más que seleccionar Cronos en el menú desplegable de la red en la parte superior de Metamask. También puedes establecer una nueva RPC para acceder a Cronos siguiendo estos pasos. Abre la ventana emergente de Metamask, haz clic en el icono de tu cartera, vaya a `Configuración` ,entonces elija `Redes` y busque `Cronos`. Los datos que deberías obtener son los siguientes:

* **Nombre de la Red:** Cronos
* **URL del RPC:** https://evm-cronos.crypto.org
* **ID de la cadena:** 25
* **Simbolo del activo:** CRO
* **URL del explorador de bloques:** https://cronos.crypto.org/explorer/

Guarde los cambios y Metamask le cambiará automáticamente a la red Cronos:

![¡Felicidades, ya puede utilizar la red de Cronos!](../../.gitbook/assets/Cronos-onboarding-1.png)

## Transfiriendo activos a Cronos

### Faucets

No hay ningún grifo oficial para conseguir tus primeros tokens de CRO para tus primeras transacciones. Sin embargo, alguna aplicación te proporcionará este servicio si haces un puente con algunos fondos a Cronos, o simplemente si necesitas algun token para pagar el gas:

* [Faucet de Crystl Finance](https://cronos.crystl.finance/faucet): Después de conectar tu monedero y completar el captcha, podrás solicitar algún CRO que será enviado a tu monedero.
* [Elk Finance](https://app.elk.finance/#/elknet): Cuando esté pasando sus tokens ELK de una cadena a otra, tendrá la opción de cambiar una pequeña parte de los ELK transferidos al token de gas nativo de la cadena de destino. Esto es especialmente útil si es la primera vez que se transfieren activos a una nueva cadena.

![Usando el puente de ElkNet y convirtiendo $1 para poder pagar el gas](../../.gitbook/assets/Cronos-onboarding-2.png)

* [Crypto.com](https://crypto.com): No olvides que Cronos es una cadena profundamente vinculada a Crypto.com. Puedes crear una cuenta allí, comprar tus tokens CRO directamente vinculando una cuenta bancaria y enviarlos a Cronos.

{% hint style="info" %}
Ten en cuenta que necesitarás algún token de gas para poder realizar transacciones. Esto significa que si haces un puente de activos de otra cadena a Cronos en una cuenta sin tokens CRO, estarás atascado y no podrás hacer nada. Asegúrate de que tu cartera tiene fondos suficientes para realizar al menos una transacción de intercambio de tokens de gas.
{% endhint %}

### Puentes

* [Relay Chain](https://app.relaychain.com/transfer#/) es el socio oficial de Mai Finance si quieres puentear tu MAI a Cronos. RelayChain soporta ahora el puenteo de MAI desde unas cuantas cadenas diferentes, por lo que podrás enviar tus activos desde Polygon, Moonriver, Avalanche o Shiden a Cronos. Simplemente selecciona la cadena de destino como Cronos, y el token a enviar (la mayoría de las veces está denominado como MAI, pero a veces también lo puedes encontrar como miMATIC). Selecciona la cantidad a transferir e inicia la transferencia, ésta no debería tardar más de 10 minutos. No olvide de prestar atención a las tarifas de transferencia. Sin embargo, una cosa buena de RelayChain es que te dará algo de CRO en el lado receptor para que puedas cambiar algo de MAI por CRO.

![Transfiriendo MAI desde Polygon a Cronos usando RelayChain](../../.gitbook/assets/Cronos-onboarding-3.png)

* [AnySwap](https://anyswap.exchange/#/router) es también una posibilidad para la mayoría de las cadenas si quieres transferir algunos activos a Cronos. Como nota adicional, AnySwap también soporta la transferencia de MAI de Polygon a Cronos.
* [ElkNet](https://app.elk.finance/#/elknet) es un caso particular, ya que el puente de Elk Finance le permitirá puentear el token ELK de cualquier cadena compatible con EVM a cualquier otra cadena compatible con EVM en la que estén desplegados con la posibilidad de intercambiar una pequeña porción de la cantidad transferida en token de gas (véase la sección dedicada a los faucets justo arriba).

### Hub de MAI

En el caso de que hagas un puente entre MAI de Polygon y Cronos a través de Relay Chain, obtendrás la versión de MAI de RelayChain en lugar del MAI nativo acuñado por la aplicación en Cronos. Los 2 tokens (el de RelayChain y el de Mai Finance) tienen el mismo valor y el mismo nombre, pero diferentes direcciones de contrato, y el único que será aceptado para cultivar rendimientos en Cronos es el de Mai Finance.

Puedes intercambiar el MAI obtenido de Relay Chain en [el hub de Mai Finance](https://app.mai.finance/hub) con una proporción de 1:1, entonces podrá utilizar su verdadero MAI en otras plataformas.

![Intercambiando MAI(RelayChain) por MAI en Cronos usando el Hub](../../.gitbook/assets/Cronos-onboarding-4.png)

No olvides que tendrás que convertir tus MAI verdaderos en la versión de la cadena de relevo si quieres pasarlos de Cronos a otra cadena.

{% hint style="info" %}
Parece que AnySwap soporta las transferencias de MAI de Polygon a Cronos, pero recibirás la versión AnySwap de MAI que no podrás intercambiar a través del puente. Puede que te quedes con un token inutilizable, así que asegúrate de que estás usando el puente correcto.
{% endhint %}

## DeFi en Cronos

Al estar Cronos vinculado a Crypto.com, una gran cantidad de inversiones están fluyendo en la cadena y las aplicaciones DeFi están ahí para apoyar la liquidez. Como tal, puede ser capaz de farmear rendimientos en las siguientes plataformas:

* [CroDex](https://swap.crodex.app/#/swap): Se trata de uno de los principales DEX (Exchanges descentralizados) y AMM (Automated Market Maker) en Cronos, y es un fork de Uniswap v2 como QuickSwap. Podrás intercambiar tus activos, participar en la minería de liquidez proporcionando pares LP (Liquidity Providing) en granjas, o apostar el token nativo de la plataforma para ganar más recompensas. CroDex es también el primer socio oficial de Mai Finance en Cronos, y el único lugar donde podrás intercambiar MAI por otros activos, así como participar en programas de farmeo de liquidez con los pares MAI-USDC y MAI-CRO.

![Farmeando con MAI en CroDex](../../.gitbook/assets/Cronos-onboarding-5.png)

Cuando cultives en CroDex, obtendrás recompensas en tokens CRX que puedes apostar en una Bóveda para obtener más tokens CRX, pero hay otras opciones (mejores) que serán presentadas en un futuro tutorial.

* [VVS](https://vvs.finance) y [CronaSwap](https://app.cronaswap.org): Estos son otros DEXs/AMMs que son forks de PancakeSwap (otro fork de Uniswap) donde obtendrás las mismas características que en CroDex.
* [Beefy Finance](https://app.beefy.finance/#/cronos), [Adamant](https://adamant.finance) y [Autofarm](https://autofarm.network/cronos/) son famosos agregadores / optimizadores de rendimiento que están presentes en muchas redes, y donde podrás depositar tus tokens LP desde la mayoría de los DEX, y dejar que los algoritmos a cargo de los pools cosechen los tokens de la granja y compongan las recompensas en más tokens LP.
* [Crystl Finance](https://cronos.crystl.finance) es una fork que se lanzó primero en Polygon y ahora también está disponible en Cronos. Los usuarios podrán depositar tokens LP en bóvedas para ganar tokens CRYSTL que pueden ser apostados o cultivados (o intercambiados).
* [Fortune DAO](https://www.fortunedao.com/#/) es el principal fork de Ohm (Olympus) en Cronos que acepta DAI y USDC.

## Mai Finance en Cronos

Actualmente la aplicación aún no se ha lanzado por completo y se está esperando principalmente a que ChainLink acepte esos tokens como colaterales. El Hub ya está presente, por lo que se puede esperar un lanzamiento en el primer trimestre de 2022.

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La mención de un proyecto en esta guía no debe considerarse como una aprobación del mismo.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
