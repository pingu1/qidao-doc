---
description: >-
  En esta guía te explicaremos todo lo que necesitas saber para empezar a
  utilizar las diferentes DApps que ofrece Optimism
---

# Cómo comenzar en Optimism

## ¿Qué es Optimism?

Optimism, u Optimistic Ethereum, como se le llama a veces, es una solución de escalado rollup que permite a los usuarios enviar transacciones en la red Ethereum y conseguir que se ejecuten más rápidamente por un coste de gas mucho menor. Por esta razón, Optimism se conoce como una capa 2 de Ethereum (L2 para abreviar). El nombre Optimism proviene de su uso de la tecnología optimistic rollup, que se refiere al tipo de pruebas que la red utiliza para trabajar en tándem con la cadena principal de Ethereum (capa 1, o L1). Para más información sobre los rollups y otras soluciones de rollups como ZK (Zero Knowledge), puede usar este [ link](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Al ser una tecnología de rollup, Optimism no produce sus propios bloques y, por lo tanto, no es un blockchain. Además, la API de la red de Optimism utiliza en gran medida la misma especificación JSON-RPC que Ethereum y, por lo tanto, es esencialmente equivalente a la EVM (máquina virtual de Ethereum), lo que permite que las aplicaciones creadas para la red principal de Ethereum se ejecuten en Optimism sin cambiar esencialmente su código base.

Tenga en cuenta que debido a esto, Optimism no utiliza su propio token de gas, sino que utiliza Ether como gas para pagar las transacciones.

## Empenzando en Optimism

Antes de usar Optimism, necesitarás una dirección de monedero. Debido a que Optimism es una red EVM, aceptará los mismos monederos que en otras cadenas EVM, incluyendo monederos web como Metamask o Nifty, y podrás usar tu monedero hardware como Trezor o Ledger, pero puede que tengas que seguir pasos extra para poder conectar tu monedero frío a la red.&#x20;

Para este tutorial, nos ceñiremos a Metamask tal y como hemos hecho en todas las demás guías de este sitio. Si no tienes Metamask instalado, puedes encontrar instrucciones en [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Añadiendo Optimism a Metamask

Abra la ventana emergente de Metamask, haga clic en el icono de su cartera, navegue hasta`Configuracion` , elija `Redes` y busque `Añadir Redes`. Utilizará la siguiente información en los campos de texto correspondientes:

* **Nombre de la red:** Optimism
* **URL del RPC:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **Simbolo del token:** ETH
* **URL del explorador de bloques:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

Guarde los cambios y Metamask le cambiará automáticamente al Optimism::

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## Enviando fondos a Optimism

### Faucets

No hay faucets para el gas en Optimism, pero si se utiliza una DApp como [ElkNet](https://app.elk.finance/#/elknet), puedes intercambiar algunas de sus tokens Elk como gas al hacer el puente desde cualquiera de las redes soportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Puentes

* [Multi Chain](https://app.multichain.org/#/router) es el socio oficial de Mai Finance si quieres transferir tus MAI o QI a Optimism desde cualquier otra red. Desde la red seleccionada, sólo tiene que elegir la cadena de destino (Optimism) y el activo que desea enviar (MAI o ETH con la cantidad correcta, y hacer clic en el botón Transferir. Preste atención a las tasas de transferencia tomadas directamente en el activo que está transfiriendo.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) es un puente popular y uno de los socios oficiales de la red Optimism.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) es otro puente popular que también es socio oficial de la red Optimism. Sólo hay un pequeño número de tokens compatibles, incluyendo ETH, y varias stablecoins como USDC, DAI y USDT, pero ofrece tarifas de puente más bajas que la mayoría de las otras soluciones.
* [Hashflow](https://app.hashflow.com/) es una tecnología puente más reciente que funciona esencialmente como un DEX (intercambio descentralizado) crosschain para cualquier token con suficiente liquidez. Además, los usuarios de Hashflow pueden ganar HFT (tokens de Hashflow) por intercambiar o proporcionar liquidez a los tokens. Las cadenas están actualmente limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon y BNB..

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) actuará tanto como bridge como faucets cuando transfieras el token ELK entre 2 redes. Podrás hacer un puente con tu ELK y en el extremo receptor, podrás tener una pequeña porción de tu ELK directamente disponible como token de gas, ETH en nuestro caso, como se explica en la sección anterior.

## DeFi en Optimism

Para empezar con el optimismo, aquí tienes algunas DApps que te pueden resultar útiles para poner en práctica tu MAI y QI, entre ellas:

* [Curve](https://optimism.curve.fi/factory/4/deposit): Aquí es donde existe actualmente la mayor parte de la liquidez de MAI en Optimism, ya que Curve es extremadamente eficiente a la hora de realizar intercambios de stablecoin

Al depositar MAI en el LP de Curve, recibirá tokens de LP que pueden depositarse en la granja de Curve en el sitio web de Mai Finance para generar rendimientos en tokens QI.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) se ha lanzado recientemente en Optimism, y aquí es donde encontrarás el fondo de liquidez QI/WETH. Actualmente, el protocolo no tiene semillas, pero debería proporcionar un caso de uso adicional para QI hasta que se lance el staking de QI en la red. Ten en cuenta que Arrakis utiliza pools Uniswap, por lo que tendrás que depositar tanto QI como WETH en las proporciones especificadas para poder entrar en el LP.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019), una bifurcación de Balancer sancionada oficialmente, se lanzó en Optimism en junio de 2022 y ofrece un nuevo grupo de stablecoin de alta liquidez apodado "Come Together" que se compone de FRAX, USDC y MAI. Debido a sus grandes recompensas, que incluyen tokens QI, BEETS y BAL, es seguro que se convertirá en el grupo de stablecoin de facto para MAI en Optimism.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Mai Finance en Optimism

La plataforma de préstamos ya está disponible en Optimism, donde podrás depositar tus tokens WETH (Wrapped Ether) o WBTC (Wrapped Bitcoin) en una cámara acorazada y tomar prestados MAI contra ellos. Los MAI se pueden depositar en la granja Curve para ganar QI, o en el nuevo pool estable FRAX/USDC/MAI en la recientemente lanzada BeethovenX que gana recompensas en tokens QI, BEETS y BAL.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como un respaldo al proyecto..

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
