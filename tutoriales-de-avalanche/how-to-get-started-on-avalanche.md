---
description: >-
  En este artículo encontrarás todo lo que necesitas saber para empezar a
  utilizar la red de Avalanche
---

# Cómo comenzar en Avalanche

## ¿Que es Avalanche?

Avalanche es una cadena de bloques de L-1 que funciona como plataforma para aplicaciones descentralizadas y redes de cadenas de bloques personalizadas. La red Avalanche consta de tres cadenas de bloques individuales: la X-Chain, la C-Chain y la P-Chain. Cada cadena tiene un propósito distinto, que difiere radicalmente del enfoque de las demás, es decir, que todos los nodos validen todas las transacciones. Las cadenas de bloques de Avalanche incluso utilizan diferentes mecanismos de consenso en función de sus casos de uso. 

Avalanche es 100% compatible con la cadena de herramientas de Ethereum (o también conocido como EVM), y su cadena C ofrece la misma funcionalidad que Ethereum, pero con un mayor rendimiento, una tiempo de transacción de menos de un segundo y unas tasas de transacción mucho más bajas. AVAX es el token de gas nativo de la red Avalanche.

## ¿Cómo empezar a utilizar Avalanche?

Antes de utilizar la red Avalanche, deberá crear una dirección de cartera. Hay diferentes tipos de monederos que se pueden utilizar, incluyendo **monederos de software** como Metamask o el [monedero nativo de Avalanche](https://wallet.avax.network), así como **monederos de hardware** como [Trezor ](https://trezor.io/coins/)o [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX-?docs=true). 

Para la realización de este tutorial, usaremos Metamask. Si no tienes Metamask instalado, puedes encontrar un tutorial sobre ésto en [cómo empezar en Polygon](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/tutoriales-de-polygon/how-to-get-started-on-polygon)

### Añadiendo Avalanche a Metamask

Para utilizar la red Avalanche, tendrás que añadirla a Metamask. Para ello, haz clic en el menú desplegable de la red (donde te saldrá por defecto Ethereum Mainnet si es la primera vez que la configuras), y luego selecciona RPC personalizado. A continuación, tienes que añadir los siguientes valores en el formulario que aparece:

* **Network Name**: Avalanche Network
* **New RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Symbol**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Guarda los cambios y Metamask te cambiará automáticamente a la red Avalanche.

![¡Felicidades! ¡Ya estás usando Avalanche!](<../.gitbook/assets/image (39).png>)

## Transfiriendo fondos a Avalanche

### Obteniendo Avalanche gratis

Actualmente no hay ninguna forma de obtener de forma gratuita tokens AVAX para usar la red de Avalanche. Si necesitas algunos AVAX para cubrir el coste del de gas, tendrá que enviar AVAX directamente a tu cartera desde un exchange centralizado (también conocido como CEXs), o mediante el puente de tokens a través del puente Elknet. Puedes encontrar más información sobre esta segunda opción en la sección sobre [Puentes](how-to-get-started-on-avalanche.md#bridges).

### Puentes

* [Puente oficial de Avalanche ](https://bridge.avax.network)- Avalanche tiene su propio puente que puede utilizarse para mandar activos desde la red principal de Ethereum a Avalanche. Las tasas de gas se pagan en el token origen pueden ser altas ya que se está puenteando desde Ethereum.
* [Anyswap](https://anyswap.exchange/#/bridge) también permite transferir activos a muchas cadenas diferentes. Hay cantidades mínimas de tokens para transferir que variarán en función del token, pero el coste de esta transacción es fijo.
* [Celer Bridge](https://cbridge.celer.network/#/transfer) ofrece servicios de transferencia de activos para muchas cadenas con una interfaz de usuario muy intuitiva. La comisión al realizar la transferencia es de un 3% para Avalanche.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) ofrece una interfaz fácil de usar e intuitiva con tarifas bajas. Como nota adicional, Relay Chain es la aplicación oficial para [transferir MAI a Avalanche](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/universidade-de-mai/mai-metaverse).
* [Elknet](https://app.elk.finance/#/elknet) es un servicio de transferencia de activos desde una cadena a otra ofrecido por Elk Finance, un exchange descentralizado disponible en múltiples redes, incluyendo Avalanche, Binance, Fantom, Polygon y xDai. Lo que diferencia a Elknet de los otros puentes de esta lista es que no se requiere AVAX para el bridging, pero hay una pega que repasaremos a continuación. El coste del puente es sólo la tasa de gas para la transacción.
  * Para enviar sus tokens a Avalanche a través de Elknet, primero tendrá que convertirlos en Elk, el token nativo de Elk Finance.
  * A continuación, puede utilizar el puente para trasladar su ELK desde las redes soportadas a Avalanche, y si marca la opción "Cambiar $ELK 1 por gas", una parte de su transferencia se convertirá en AVAX. 
  * Una vez que la transferencia se haya completado (normalmente suele tardar menos de 10 minutos), puedes cambiar tu monedero a la red de Avalanche y verás tu ELK y un poco de AVAX listos para desplegar. 
  * Ahora puede cambiar su ELK directamente en esta página a cualquier token que tenga soporte en Avalanche. Lo mismo puede hacerse a la inversa para volver a Polygon o a cualquier otra cadena que tenga soporte en esta DApp.

![Interfaz de Elknet](<../.gitbook/assets/image (37).png>)

## DeFI en Avalanche

Avalanche ha experimentado un gran crecimiento en estos últimos meses, lo que ha llevado no sólo al desarrollo de grandes proyectos nativos, sino que otros proyectos DeFi existentes en otras cadenas están empezando a dar el paso a esta red, incluida Curve, aunque está aún no se ha lanzado.

* [Aave](https://app.aave.com/dashboard) se ha lanzado recientemente en Avalanche y ya se han bloqueado 4.000 millones de dólares en TVL (Total Value Locked). Los tokens que se pueden bloquear como colateral en Aave en la red de Avalanche son Aave, Avalanche, Dai, Tether, USDC, WBTC y WETH. Los tokens camAVAX se aceptarán como colateral para las bóvedas de Mai Finance.
* [Beefy Finance](https://app.beefy.finance/#/avax) es probablemente conocido por la mayoría de los usuarios DeFI, ya que está disponible en otras cadenas como Binance Smart Chain, Fantom, Harmony, Polygon... Beefy es lo que se conoce como un autocompounder, y actualmente proporciona grandes APYs de farming tanto para las granjas de un solo token como para las de dos tokens. Beefy ofrece la funcionalidad de autocompounding para los LPs [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) y [MAI/USDC.e](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e). Para formar estos tokens LPs puedes utilizar la aplicación Trader Joe..
* [Benqi](https://app.benqi.fi/markets) es un protocolo similar a Aave y fue el primero que se lanzó en esta red. Los tokens que se pueden depositar como colateral son Avalanche, Dai, Link, Tether, USDC, WBTC y WETH..

![Interfaz de BenQI](<../.gitbook/assets/image (40).png>)

* [TraderJoe](https://www.traderjoexyz.com/#/home) es un intercambio descentralizado y se ha convertido en uno de los principales proyectos de Avalanche con una interfaz de usuario intuitiva, y una gran función de "zapping" que permite a los usuarios convertir un token directamente en un token de fondo de liquidez. TraderJoe es también el socio oficial con un [par de liquidez MAI-USDC en Avalanche](../mai-metaverse.md#usando-mai-en-avax).

![](<../.gitbook/assets/image (36).png>)

* [YieldYak](https://yieldyak.com/farms) es otro protocolo que autocompone tus tokens que también proporciona altos APYs de farming. Sus granjas de un solo token funcionan en forma conjunta con BenQI para hacer apalancamiento y asi obtener rendimientos más altos y, por lo tanto, debe considerarse una estrategia arriesgada.

![](<../.gitbook/assets/image (38).png>)

## Otros links útiles

* [Página de Avalanche](https://www.avax.network)
* [Links de la comunidad de Avalanche](https://www.avax.network/community)(Discord, Medium, Reddit, Twitter, etc)
* [Debank](https://debank.com)

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La mención de un proyecto en esta guía no debe considerarse como una promoción a dicho proyecto.
