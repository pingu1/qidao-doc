---
description: >-
  En esta guía te explicaremos todo lo que necesitas saber para empezar a
  utilizar las diferentes DApps que ofrece Arbitrum.
---

# Cómo comenzar en Arbitrum

## ¿Qué es Arbitrum?

Arbitrum es una solución de escalado  que permite a los usuarios enviar transacciones en la red Ethereum y conseguir que se ejecuten más rápido por un coste de gas mucho menor. Por esta razón, Arbitrum se conoce como una capa 2 de Ethereum (L2 para abreviar). Al igual que su red hermana, Optimism, Arbitrum utiliza la tecnología optimistic rollup, que se refiere al tipo de pruebas que la red utiliza para trabajar en conjunto con la cadena principal de Ethereum (capa 1, o L1). Para más información sobre los rollups optimistas y otras soluciones de rollups como ZK (zero knowledge), visite [este link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Al tratarse de una tecnología de rollup, Arbitrum no produce sus propios bloques y, por lo tanto, no es un verdadero blockchain. Offchain Labs, los desarrolladores detrás de Arbitrum, tienen como objetivo hacer que la red sea equivalente a EVM (Ethereum Virtual Machine) con futuras actualizaciones.

Tenga en cuenta que debido a esto, Arbitrum no utiliza su propio tokens de gas, sino que utiliza Ether como gas para pagar las transacciones.

## Empezando en Arbitrum

Antes de utilizar Arbitrum, necesitarás una dirección de monedero. Dado que Arbitrum es una red EVM, aceptará los mismos monederos que en otras cadenas EVM, incluyendo monederos web como Metamask o Nifty, y podrás utilizar tu monedero hardware como Trezor o Ledger, pero puede que tengas que seguir pasos adicionales para poder conectar tu monedero frío a la red.

Para este tutorial, nos ceñiremos a Metamask tal y como hemos hecho en todas las demás guías de este sitio. Si no tienes Metamask instalado, puedes encontrar instrucciones en [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Añadiendo Arbitrum to Metamask

Abra la extension de Metamask, y vaya a `Configuracion` , luego escoja `Redes` y busque `Añadir Redes`. Utilizaras la siguiente informacion para añadir la red:

* **Nombre de la red:** Arbitrum
* **URL del RPC:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **ID de la cadena:** 4216
* **Simbolo de la moneda:** ETH
* **URL del explorador de bloques:** [https://arbiscan.io/](https://arbiscan.io/)

Guarde los cambios y Metamask le cambiará automáticamente a Arbitrum:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## Enviando fondos a Arbitrum

### Faucets

No hay faucets para el gas en Arbitrum, pero si usas una DApp como [ElkNet](https://app.elk.finance/#/elknet), puedes optar por intercambiar algunos de tus tokens de Elk como gas cuando hagas el puente desde cualquiera de las redes soportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### Puentes

* [Multi Chain](https://app.multichain.org/#/router) es el socio oficial de Mai Finance si quieres transferir tus MAI o QI a Arbitrum desde cualquier otra red. Desde la red seleccionada, sólo tiene que elegir la cadena de destino (Arbitrum) y el activo que desea enviar (MAI o ETH) con la cantidad que quieras enviar, y hacer clic en el botón Transferir. Preste atención a las tasas de transferencia que se toman directamente en el activo que está transfiriendo.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) es un puente muy popular y permite transferir tokens de unas quince redes diferentes a Arbitrum.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) es otro puente popular. Sólo hay un pequeño número de tokens compatibles, incluyendo ETH, y varias stablecoins como USDC, DAI y USDT, pero ofrece tarifas de puente más bajas que la mayoría de las otras soluciones.
* [Hashflow](https://app.hashflow.com/) es una tecnología puente más reciente que funciona esencialmente como un DEX (intercambio descentralizado) crosschain para cualquier token con suficiente liquidez. Además, los usuarios de Hashflow pueden ganar HFT (tokens de Hashflow) por intercambiar o proporcionar liquidez a los tokens. Las cadenas están actualmente limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon y BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) actuará tanto como bridge y como faucets cuando transfieras el token ELK entre 2 redes. Podrás hacer un puente con tu ELK y en el extremo receptor, podrás tener una pequeña porción de tu ELK directamente disponible como token de gas, ETH en nuestro caso, como se explica en la sección anterior.

## DeFi en Arbitrum

* [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) tiene actualmente el único pool en Arbitrum con liquidez MAI. Al depositar su MAI en el pool MAI/USDC/USDT, los usuarios pueden ganar aproximadamente un 13% de rendimiento en sus stablecoins. Por favor, ten en cuenta que este pool será migrado en breve, lo que soluciona un error de liquidez existente..

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## Mai Finance en Arbitrum

La plataforma de préstamos ya está disponible en Arbitrum, donde podrá depositar sus tokens WETH (Wrapped Ether) o WBTC (Wrapped Bitcoin) en un vault y tomar prestados MAI contra ellos. A continuación, podrá depositar sus MAI prestados en Balancer para obtener rendimientos.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como un respaldo al proyecto.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
