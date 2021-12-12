---
description: >-
  En este artículo encontrarás toda la información necesaria para comenzar a
  operar en la blockchain Moonriver
---

# Cómo comenzar en Moonriver

## ¿Qué es Moonriver?

Va a ser complicado explicar qué es Moonriver sin hablar también de otras cadenas, como MoonBeam, Kusama y Polkadot.

Polkadot es una cadena de bloques L1 que compite directamente con Ethereum, Cosmos o Eos, y el objetivo de la cadena es hacer crecer un ecosistema completo de criptomonedas y aplicaciones. Uno de los puntos principales que diferencia a Polkadot de otras L1 es su separación en una cadena principal (la cadena de relevo) y redes creadas por los usuarios (parachains). La cadena de relevo se beneficia de los bajos requisitos en términos de recursos informáticos, ya que la mayoría de los desarrollos y pruebas se realizan en las parachains. Por otro lado, las parachains heredan la misma seguridad que la cadena de relevo. Esto también crea entornos aislados que pueden trabajar de forma autónoma y no revelan los datos del usuario a la cadena principal.&#x20;

Kusama es un entorno de preproducción para Polkadot, una cadena separada que imita a la cadena de relevo principal de Polkadot, y donde se prueban primero todos los desarrollos y actualizaciones para la cadena principal. Sin embargo, como entorno de preproducción, Kusama opera con criptomonedas reales y transacciones reales, pero con reglas más laxas que en Polkadot. Sin embargo, el objetivo de las aplicaciones y cadenas laterales desarrolladas en Kusama es migrar a Polkadot en algún momento. Debido a las reglas más laxas, es más fácil para un proyecto probar cosas y hacer crecer una comunidad mientras se desarrolla el protocolo. Una vez que el producto final está listo, todo puede migrar al entorno de producción.&#x20;

Moonriver es, en realidad, una parachainde Kusama. El código que se despliega en Moonriver es una versión de prueba del código que puede desplegarse en Moonbeam, la versión de producción de Moonriver en Polkadot. Una vez que el código es validado en Moonriver, puede ser enviado a Moonbeam. Moonbeam y Moonriver son dos cadenas compatibles con EVM, lo que significa que aceptan los mismos contratos inteligentes que otras cadenas compatibles con la red Ethereum. Debido a esto, Moonriver se convirtió rápidamente en el punto de entrada de muchas DApps (Aplicaciones Descentralizadas) que querían expandirse desde la red Ethereum (Mainnet Ethereum, Polygon, Avalanche, Fantom...) a la red Polkadot.&#x20;

Al igual que otras cadenas compatibles con EVM, Moonriver utiliza un token de gas para verificar las transacciones: el token MOVR.

## ¿Cómo comenzar en Moonriver?

Antes de utilizar la red Moonriver, necesitarás una dirección de monedero. Dado que Moonriver es una red EVM, aceptará los mismos monederos que en otras cadenas EVM, incluyendo monederos web como Metamask o Nifty, y podrás utilizar tu monedero hardware como Trezor o Ledger, pero puede que tengas que seguir pasos adicionales para poder conectar tu monedero frío a la red. Puedes encontrar una guía paso a paso muy clara en la [ documentación oficial de Moonbeam](https://moonbeam.foundation/tutorials/how-to-create-moonriver-ethereum-address/).

Para este tutorial, nos ceñiremos a Metamask como para todas las demás guías de este sitio. Si no tiene Metamask instalado, puede encontrar instrucciones en [Cómo comenzar en Polygon.](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/tutoriales-de-polygon/how-to-get-started-on-polygon)

### Añadiendo Moonriver a Metamask

En teoría, Moonriver viene preinstalado con MetaMask, lo que significa que no deberías tener que añadir la información de la cadena para que Metamask funcione. Sin embargo, puede ser una buena idea verificar que tu configuración es correcta comprobando dos veces los valores guardados en tu monedero local. Abre la ventana emergente de Metamask, haz clic en el icono de tu monedero, vaya a `Configuración`, luego elija `Redes` y encuentra `Moonriver`. Los datos que deberías encontrar son los siguientes&#x20;

* **Nombre de la Red:** Moonriver
* **Nuevo URL RPC:** https://rpc.moonriver.moonbeam.network
* **ID de Cadena:** 1285
* **Simbolo de Moneda:** MOVR
* **URL de explorador de bloques:** https://blockscout.moonriver.moonbeam.network/

Guarde los cambios y Metamask le cambiará automáticamente a la red Moonriver:

![¡Felicidades, ya puedes usar la red Moonriver!](../.gitbook/assets/Moonriver-setup-MM.png)

## Transfieriendo activos a Moonriver

### Faucets

Uno de los mayores DEX en Moonriver, SolarBeam, ofrece [una transaccion sin coste de gas](https://app.solarbeam.io/bridge/gas-swap) en caso de que te quedes sin gasolina. Esto también supone que tienes algunos fondos en Moonriver, pero no puedes hacer nada porque tienes 0 MOVR en tu cartera.

![Transacción sin comisión en Moonriver](../.gitbook/assets/Moonriver-faucet.png)

Tenga en cuenta que sólo se aceptan ciertos activos para esta transacción sin gas, y MAI no forma parte de las monedas admitidas.

### Puentes&#x20;

* [Relay Chain](https://app.relaychain.com/transfer#/) es el socio oficial de Mai Finance si quieres transferir tu MAI a Moonriver desde Polygon. Cuando esté conectado a Polygon, sólo tiene que elegir la cadena de destino (Moonriver) y el activo que desea enviar (MAI o miMATIC) con la cantidad correcta, y hacer clic en el botón `Transfer` .Preste atención a las comisiones de transacción.

![Transfieriendo MAI de Polygon a Moonriver usando Relay Chain](../.gitbook/assets/Moonriver-relaychain.png)

* Si necesita hacer un puente con otros activos de otra red, puede utilizar la Relay Chain (véase más arriba), [AnySwap](https://anyswap.exchange/#/bridge) funcionará si quieres transferir desde Eth Mainnet a Moonriver, y por supuesto también puedes usar la función de puente desde [Solarbeam](https://app.solarbeam.io/bridge).
* Por último, cabe destacar que [Elknet](https://app.elk.finance/#/elknet) actuará tanto de puente como de grifo (faucet) cuando transfieras el token ELK entre 2 redes. Podrás hacer un puente con tu ELK y en el extremo receptor, podrás tener una pequeña porción de tu ELK directamente disponible como el token de gas, MOVR en nuestro caso.

### Hub

En el caso de que hagas un puente entre MAI de Polygon y Moonriver a través de Relay Chain, obtendrás la versión de MAI de RelayChain en lugar del MAI nativo acuñado por la aplicación en Moonriver. Los 2 tokens (el de RelayChain y el de Mai Finance) tienen el mismo valor y el mismo nombre, pero diferentes direcciones de contrato, y el único que será aceptado para cultivar rendimientos en Moonriver es el de Mai Finance.

Puedes cambiar tu MAI de Relay Chain usando el [hub en Mai Finance](https://app.mai.finance/hub) con una proporción de 1:1, entonces podrá utilizar verdadero MAI en otras plataformas.

![Usando el hub para intercambiar el MAI de Relay Chain por MAI nativo](../.gitbook/assets/Moonriver-hub.png)

{% hint style="info" %}
Como nota al margen, si quieres pasar tu MAI de Moonriver a Polygon u otras cadenas, tendrás que convertirlas primero en su versión RelayChain.
{% endhint %}

## DeFi en Moonriver

Moonriver está consiguiendo mucha tracción y cada vez más aplicaciones se están moviendo a esta nueva cadena, con un potencial para migrar completamente a Polkadot. Así, podrá farmear rendimientos en la siguiente plataforma (la lista no está completa):

* [Solarbeam](https://app.solarbeam.io): Esta es el principal DEX y AMM en Moonriver. Podrás intercambiar tus activos, participar en la minería de liquidez proporcionando pares LP (Liquidity Providing) en granjas, o stakear el token nativo de la plataforma. Solarbeam es también uno de los primeros socios de Mai Finance en Moonriver, y podrás hacer farming con el par MAI-MOVR. También encontrarás un pool de MAI-USDC que no recibe recompensas, pero que puede obtener algunas comisiones de operación.

![Pares LP que incluyen MAI en solarbeam en Diciembre de 2021](../.gitbook/assets/Moonriver-solarbeam.png)

Cuando farmees en Solarbeam, serás recompensado en tokens SOLAR que luego podrás stakear en una Bóveda durante un determinado periodo de carencia y ganar tokens SOLAR adicionales, o stakear para ganar otros tokens exóticos para la plataforma.

* [Huckleberry Finance](https://www.huckleberry.finance): Este es otro DEX/AMM en Moonriver donde podrás cultivar yieles, y posiblemente usar a Beefy para aumentar tus ganancias.
* [Beefy Finance](https://app.beefy.finance/#/moonriver): El famoso autocompensador también está en Moonriver y te ayudará a componer tus ganancias tanto de Solarbeam como de Huckleberry. Como nota al margen, Beefy no propone el par MAI-MOVR en el momento de escribir este artículo, pero es posible que pronto puedas usar a Beefy para cosechar los tokens SOLAR y obtener más MAI-MOVR del compounder.
* [Sushiswap](https://app.sushi.com): ¡No es necesario presentar SushiSwap! Podrás intercambiar tus activos y los rendimientos de las granjas por ciertos tokens de LP como lo harías en cualquier otra cadena. Las recompensas se conceden en SUSHI y MOVR.
* [Rome DAO](https://romedao.finance): Este es el primer tenedor OHM en Moonriver. Vincula tus activos para obtener tokens de ROMA con descuento que puedes apostar para ganar un APY muy alto. En el momento de escribir este artículo, el ROI de 5 días es de alrededor del 10,6%. RomeDAO acepta actualmente FRAX y MIM en su tesorería, pero pronto podría aceptar también MAIe

## Mai Finance en Moonriver

La plataforma de préstamos ya está disponible en Moonriver, donde podrás poner tus tokens mooSolarETH-USDC en una cámara acorazada y tomar prestados MAI contra ella. Para ello:

* Crear un par ETH-USDC en Solarbeam
* Depositar el ETH-USDC en Beefy y obtén el token mooSolarETH-USDC como recibo
* Deposita tu mooToken en Mai Finance en [su vault correspondiente](https://app.mai.finance/vaults/create)

![Mai Finance vaults on Moonriver as of December 2021](../.gitbook/assets/Moonriver-vaults.png)

La bóveda de ETH simple también es una opción. Mientras que su colateral está ganando 44,08% APY de Beefy Finance (en el momento de escribir), usted será capaz de pedir prestado MAI y hacer farming con el par MAI-MOVR y obtener 128% APRs en Solarbeam, o pronto 158,058% APY en RomeDAO.al&#x20;

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como un respaldo al proyecto.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
