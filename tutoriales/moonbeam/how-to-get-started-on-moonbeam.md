---
description: En esta guía, explicaremos cómo empezar a utilizar Moonbeam.
---

# Cómo comenzar en Moonbeam

## ¿Qué es Moonbean?

Lanzado en enero de 2020, Moonbeam es una plataforma de contratos inteligentes compatible con EVM (máquina virtual de Ethereum) que se ejecuta en la red Polkadot, lo que la convierte en lo que se denomina una paracadena Polkadot. Las parachains son conjuntos interconectados de cadenas que se benefician de la cadena principal de Polkadot sin dejar de ser interoperables, por lo que participan en los beneficios y la seguridad de la cadena principal mientras se ejecutan en paralelo a ella.

Polkadot describe los beneficios de las parachains de la siguiente manera: "Las parachains ponen fin a la era de las blockchains en silos, creando una internet descentralizada y conectada de blockchains donde antes sólo existían redes aisladas con sus propias comunidades tribalistas."

![](<../../.gitbook/assets/moonbeam (1).jpg>)

Gracias a su capa de compatibilidad con EVM, Moonbeam facilita que los desarrolladores de Solidity puedan portar sus aplicaciones existentes de otras redes compatibles con EVM a Moonbeam con pocos cambios de código. Moonbeam tiene actualmente un TVL de 130 millones de dólares- Si quiere comprobar cuales son las aplicaciones existentes en esta red, puede visitar el siguiente [link](https://defillama.com/chain/Moonbeam).&#x20;

Moonbeam también ofrece compatibilidad con Substrate. Substrate es un marco modular de blockchain utilizado por los desarrolladores para construir blockchains a la medida de sus necesidades utilizando componentes reutilizables llamados pallets. Utiliza el lenguaje de programación Rust y es el marco que la mayoría de los desarrolladores utilizan cuando construyen parachains para la red Polkadot.

Como Moonbeam es una blockchain basada en Substrate, las aplicaciones integradas en su red se benefician de la interoperabilidad entre las cadenas Polkadot y Ethereum, además de otras como Bitcoin. Los desarrolladores también pueden utilizar las herramientas del ecosistema compatibles con Substrate que se utilizan habitualmente en Ethereum, incluidos los exploradores de bloques, las bibliotecas de desarrollo front-end y los monederos, así como las herramientas de desarrollo como Truffle y Remix.

El token de gas nativo de Moonbeam es GLMR.

## Empezando en Moonbeam

Antes de utilizar Moonbeam, necesitarás una dirección de monedero. Dado que Moonbeam es una red EVM, aceptará los mismos monederos que en otras cadenas EVM, incluyendo monederos web como Metamask o Nifty, y podrás utilizar tu monedero hardware como Trezor o Ledger, pero puede que tengas que seguir pasos adicionales para poder conectar tu monedero frío a la red.&#x20;

Para este tutorial, nos ceñiremos a Metamask tal y como hemos hecho en todas las demás guías de este sitio. Si no tienes Metamask instalado, puedes encontrar instrucciones en [How to get started on Polygon](../polygon/how-to-get-started-on-polygon.md).

### Añadiendo Moonbeam a Metamask

Abra la ventana emergente de Metamask, haga clic en el icono de su monedero, vaya a Configuración, elija Redes y busque Añadir red. Utilizarás la siguiente información en los campos de texto correspondientes:

* **Nombre de la red:** Moonbeam
* **URL del RPC:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **ID de la red:** 128
* **Simbolo del token:** GLMR
* **URL del explorador de bloques:** [https://moonscan.io/](https://moonscan.io/)

Guarde los cambios y Metamask le cambiará automáticamente a Moonbeam:

![Moonbeam en Metamask](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## Enviando fondos a Moonbeam

### Faucets

GLMR es el token de gas nativo de Moonbeam, por lo que necesitarás tener un poco en tu cartera para realizar transacciones en la cadena. Afortunadamente, el faucets oficial de Moonbeam te ayudará a empezar con una pequeña cantidad de GLMR, aunque ten en cuenta que la cantidad dispersada por el tokens a veces puede no ser suficiente para completar una transacción si la red está congestionada.

Para recibir un poco de GLMR gratis, tendrás que verificar que eres un humano a través del bot captcha, y conectar tu monedero Metamask al sitio. Una pequeña cantidad (0,007 GLMR) se enviará inmediatamente a su cartera.

![GLMR.Supply Faucet](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

Además, los usuarios pueden utilizar la herramienta de Solarflare "[Intercambiar por gas](https://app.solarflare.io/bridge/gas-swap)". Esto permite a los usuarios intercambiar otros tokens como WETH, WBTC, USDC, DAI, USDT, BUSD, FLARE y BNB en GLMR, el token de gas nativo de Moonbeam.

![La utilidad de Intercambiar por gas de Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### Puentes

* [Multichain](https://app.multichain.org/#/router) es el puente oficial para MAI a través de su asociación con MAI finance, y puedes enviar fácilmente tu MAI a Moonbeam utilizándolo.

![Multichain en Moonbeam](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) es un AMM (creador de mercado automatizado) con todas las funciones en Moonbeam que es muy similar a Uniswap. Solarflare tiene un puente incorporado que permite a los usuarios puentear activos de la red principal de Ethereum así como de la cadena BNB a Moonbeam. Solarflare también tiene una función de "Swap for gas" como se menciona en la sección Faucets anterior.

![Enviando fondos con Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) es un puente popular que también soporta Moonbeam. Tenga en cuenta que es posible que no pueda hacer un puente desde todas las cadenas a Moonbeam (no se admite el puente de Polygon a Moonbeam, por ejemplo)..

![Enviando fondos con Celer](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* Hay otros puentes disponibles, pero pueden ser específicos de la cadena, como Nomad o Axelar para el ecosistema Cosmos.

## DeFi en Moonbeam

[StellaSwap](https://app.stellaswap.com/farm) es actualmente la principal fuente de liquidez para MAI en Moonbeam. El MAI-Base4Pool se compone de MAI, FRAX, USDT, USDC y DAI y actualmente tiene un TVL (valor total bloqueado) de 535.000 dólares, lo que supone un sólido 26% de TAE (tasa de porcentaje anual) en sus stablecoins

![MAI-Base4Pool on StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam tiene un vibrante ecosistema DeFi con docenas de DApps (aplicaciones descentralizadas) disponibles para su uso, incluyendo grapas DeFi que se encuentran en otras cadenas como [Curve](https://moonbeam.curve.fi/) y [Beefy Finance](https://app.beefy.com/). Para obtener una lista completa de las DApps disponibles, consulte la siguientes pagina de [DefiLlama](https://defillama.com/chain/Moonbeam)

## Mai Finance en Moonbeam

Mientras que Mai Finance no está disponible en Moonbeam, puedes crear bóvedas y pedir prestado MAI contra xStella y wGLMR en StellaSwap. Ten en cuenta que los préstamos de MAI en StellaSwap devengarán intereses: el 12% en los depósitos de xStella y el 8% en los de wGLMR. Puede encontrar más información sobre cómo utilizar los depósitos MAI de StellaSwap en la siguiente sección titulada, [Playing with MAI legos on StellaSwap](playing-with-mai-legos-on-stellaswap.md).

![Vaults en StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. La discusión de un proyecto en esta guía no debe considerarse como una aprobación del proyecto.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}
