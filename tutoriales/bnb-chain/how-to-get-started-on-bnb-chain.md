---
description: >-
  En esta guía te explicaremos todo lo que necesitas saber para empezar a
  utilizar las diferentes DApps que ofrece la cadena BNB
---

# Cómo comenzar en la red BNB

## ¿Qué es la red BNB ?

BNB Chain es una red compatible con EVM (Ethereum Virtual Machine) que es una versión mejorada de la cadena inteligente original de Binance que proporciona bajas tasas de transacción, y tiempos de bloque mucho más rápidos que Ethereum, la cadena en la que se basa.

Por ello, la cadena BNB es una de las más populares del mundo, con más de 4.500 millones de transacciones anuales y una red extremadamente vibrante y madura, en este link puede ver su ecosistema de [DApps](https://dappbay.bnbchain.org/)

La cadena BNB utiliza el token BNB de Binance para pagar los gastos de gas, así que asegúrate de tener algunos en tu cartera para poder realizar transacciones. Binance proporciona las siguientes [guias](https://www.binance.com/en/support/faq/85a1c394ac1d489fb0bfac0ef2fceafd) sobre cómo conseguir comprar o transferir tokens a su cadena BNB.

## Empezando en la red BNB

Antes de utilizar BNB Chain, necesitará una dirección de monedero. Debido a que BNB Chain es una red EVM, aceptará los mismos monederos que en otras cadenas EVM, incluyendo monederos web como Metamask o Nifty, y podrá utilizar su monedero hardware como Trezor o Ledger, pero es posible que tenga que seguir pasos adicionales para poder conectar su monedero frío a la red.

Para este tutorial, nos ceñiremos a Metamask tal y como hemos hecho en todas las demás guías de este sitio. Si no tienes Metamask instalado, puedes encontrar instrucciones en [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

Además, puedes utilizar la propia Binance Wallet para empezar a trabajar en la red de forma más sencilla.

### Añadiendo la red BNB a Metamask

Abra la ventana emergente de Metamask, haga clic en el icono de su cartera, navegue hasta `Configuracion` , elija `Redes` y luego `Añadir Red`. En los campos de texto correspondientes utilizará la siguiente información

* **Nombre de la red:** BNB Chain
* **URL del RPC:** [https://docs.binance.org/smart-chain/developer/rpc.html](https://docs.binance.org/smart-chain/developer/rpc.html)
* **ID de la cadena:** 0x38
* **Simbolo del token:** BNB
* **URL del explorador de bloques:** [**https://bscscan.com/**](https://bscscan.com/)\*\*\*\*

Guarde los cambios y Metamask le cambiará automáticamente a BNB:

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.28.44 AM.png>)

Si desea buscar otras RPC con menor latencia, eche un vistazo a [ChainList](https://chainlist.org/) para ver RPC adicionales.

## Enviando fondos a la red BNB

### Faucets

Hay faucets disponibles de forma gratuita en la cadena BNB, pero es la opinión del autor que será más seguro usar algo como ElkNet para conseguir tokens de gas gratis. Si decide utilizar un faucets que haya encontrado en Internet, hágalo bajo su propia responsabilidad. Con [ElkNet](https://app.elk.finance/#/elknet), puedes optar por intercambiar algunos de tus tokens de Elk como gas cuando hagas el puente desde cualquiera de las redes soportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.29.50 AM.png>)

### Puentes

* [Multi Chain](https://app.multichain.org/#/router) es el socio oficial de Mai Finance si quieres transferir tu MAI o QI a BNB Chain desde cualquier otra red. Desde la red seleccionada, sólo tiene que elegir la cadena de destino (BNB Chain) y el activo que desea enviar (MAI o QI, por ejemplo) con la cantidad correcta, y hacer clic en el botón Transferir. Preste atención a las tasas de transferencia que se cobran directamente sobre el activo que está transfiriendo.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.32.07 AM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) es un puente popular y permite transferir tokens de unas quince redes diferentes a BNB Chain..

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.31.15 AM.png>)

* [Hashflow](https://app.hashflow.com/) es una tecnología puente más reciente que funciona esencialmente como un DEX (intercambio descentralizado) crosschain para cualquier token con suficiente liquidez. Además, los usuarios de Hashflow pueden ganar HFT (tokens de Hashflow) por intercambiar o proporcionar liquidez a los tokens. Las cadenas están actualmente limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon y BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.33.51 AM.png>)

* [Elknet](https://app.elk.finance/#/elknet) actuará tanto como bridge como faucets cuando transfieras el token ELK entre 2 redes. Podrás hacer un puente con tu ELK y, en el extremo receptor, podrás disponer de una pequeña parte de tu ELK directamente como token de gas, BNB en nuestro caso, como se explica en la sección anterior.

## DeFi en la red BNB

* [Ellipsis Finance](https://ellipsis.finance/pool/0x68354c6E8Bbd020F9dE81EAf57ea5424ba9ef322) es el lugar para la liquidez de MAI en la cadena BNB. El pool de MAI en Ellipsis (MAI+val3EPS) se compone de cuatro stablecoins incluyendo BUSD (Binance USD), USDC, USDT (Tether), y MAI. Al depositar stablecoins, y luego apostar el LP en Ellipsis, los usuarios pueden ganar un rendimiento variable entre el 6 y el 15% pagado en el token EPS de Ellipsis, el token VAL de Vallas, así como las comisiones generadas por el pool.

![MAI+val3EPS pool on Ellipsis](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.07.42 AM.png>)

## Mai Finance en la red BNB

La plataforma de préstamos ya está disponible en BNB Chain, donde podrás depositar tus tokens WBNB (Wrapped BNB) y CAKE (PancakeSwap) en un vault y tomar prestados MAI contra ellos. A continuación, puedes depositar tus MAI prestados en Ellipsis para obtener un rendimiento de tus MAI.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.11.26 AM.png>)

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como un respaldo al proyecto.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
