---
description: >-
  En esté artículo explicaremos todo lo que necesitas para empezar a utilizar la
  blockchain de Fantom
---

# Cómo comenzar en Fantom

## ¿Qué es Fantom?

Fantom es una alternativa a Ethereum para los programadores de blockchain. Fantom es una blockchain de código abierto con contratos inteligentes, que permite a los diseñadores desarrollar **DApps** (aplicaciones descentralizadas) seguras, completas y modulares.&#x20;

La red ha sido diseñada para superar todas las limitaciones de la anterior generación de plataformas blockchain, a veces referidas como el _trilema blockchain_: **descentralización**, **seguridad** y **escalabilidad**. Para poder mejorar uno de estos aspectos, siempre había que hacerlo a costa de uno de los otros dos. Fantom trató de resolver esto gracias a su mecanismo de consenso Lachesis aBFT (Asynchronous Byzantine Fault Tolerant) basado en DAG (Directed Acyclic Graphs), lo que le permite tener un alto rendimiento, ser escalable y seguro. Los test iniciales mostraron que Fantom puede manejar fácilmente más de 20.000 transacciones por segundo.

Por último, Fantom es 100% compatible con **EVM** (Ethereum Virtual Machine), lo que significa que las DApps que han sido desarrolladas en redes compatibles con EVM podrán ser desplegadas también en Fantom. Esto también trae otras ventajas para los usuarios, ya que MetaMask y otras aplicaciones web3 también son compatibles con Fantom. Podrás cambiar sin problemas de Polygon o Avalanche a Fantom dentro del mismo monedero sin ninguna complicación.

## Comenzando en Fantom

Fantom al ser compatible con **EVM**, si ya tienes un monedero con otras cadenas EVM (Ethereum Mainnet, Polygon o Avalanche), serás capaz de utilizar esta red sin ningún problema. Si no lo has hecho anteriormente, es el momento de crear una nueva dirección de monedero. Hay diferentes tipos de monederos que se pueden utilizar: **monederos de software** como Metamask o [fWallet](https://pwawallet.fantom.network/#/), o **monederos de hardware** como [Trezor ](https://trezor.io/coins/)o [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/?\_\_cf\_chl\_jschl\_tk\_\_=pmd\_yGSaskxM9Y.hIl5QLRLLktRbV9OAJvYIVHg5DDa6Pw0-1634317961-0-gqNtZGzNAlCjcnBszQiR).&#x20;

Para esta guía, y debido a que hemos usamos Metamask en todas nuestras guías anteriores, volveremos a usar Metamask, pero siéntete libre de usar cualquier otra cartera de software/hardware que te guste. Si necesitas saber cómo instalar Metamask, puedes encontrar más información en el artículo [Cómo comenzar en Polygon](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/tutoriales-de-polygon/how-to-get-started-on-polygon).

### Añadiendo Fantom a Metamask

Para utilizar la red Fantom, tendrás que configurarla manualmente en Metamask. Para ello, haz clic en el menú desplegable que se encuentra en la parte superior de la ventana de Metamask (donde indica la red que estás utilizando actualmente, Ethereum Mainnet por defecto), y luego selecciona `Custom RPC`. Esto será lo que tendrás que añadir si quieres comenzar a usar Fantom:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Tras guardar los cambios, Metamask se cambiará automáticamente a la red de Fantom.

![¡Buen trabajo! ¡Ya puedes utilizar Fantom!](<../../.gitbook/assets/image (41).png>)

Si necesitas más detalles para poder realizar esto, puedes consultar la [guía oficial de Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask).

### ¿Cómo obtener FTM gratis?

Ahora que estás en FTM, necesitarás algunos **FTM** (token nativo utilizado para cubrir el gas). Puedes hacer un puente con algunos tokens FTM desde otras cadenas, o utilizar un faucet que deposite algunos tokens FTM de forma gratuita en tu cartera para realizar algunas transacciones. El [faucet principal en Fantom](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas) se puede encontrar en SpookySwap, uno de los principales DEXs de allí (Decentralized Exchange). Ten en cuenta que es un servicio ofrecido por SpookySwap en Discord, por lo que tendrás que tener una cuenta de Discord válida y que lleve activa durante más de 30 días (aunque no es necesario estar en el servidor de Discord de SpookySwap durante 30 días).

* Una vez te hayas unido al [Discord de SpookySwap](http://discord.gg/AqbsWsWDgn), y hayas verificado tu cuenta, vaya a #faucet section.

![](<../../.gitbook/assets/image (42).png>)

* Una vez en #faucet, solo tienes que escribir el comando `!faucet` y el bot te enviará unos $FTM gratis. Cabe destacar que solo podrás realizar esto 1 vez cada 30 días.
* Si quieres comprobar si has recibido el token FTM, debes hacer clic en **Fantom Tip Bot** para interactuar directamente con él y escribir `!balance`

![Gracias Fantom Tip Bot y SpookySwap](<../../.gitbook/assets/image (45).png>)

* Lo único que te falta por hacer es retirar los fondos hacia tu cartera de Metamask, para realizar esto, tienes que escribir `!withdraw <dirección de tu cartera>`. Para saber cual es la dirección de tu cartera, tendrás que hacer clic en el logo de Metamask y tu dirección se encontrará arriba.

![Retirando desde una cuenta de Discord ](../../.gitbook/assets/ftm-faucet.png)

![Recibiendo el FTM gratis](../../.gitbook/assets/ftm-mm.png)

## Traspasando fondos a Fantom

### Transfiriendo stablecoins / ETH / BTC

Si quieres transferirte algunas monedas desde otras cadenas a Fantom, puedes usar la siguiente lista de **bridges**:

* [AnySwap](https://anyswap.exchange/#/bridge): Este es el puente oficial recomendado para enviar el MAI que has generado en Polygon a Fantom (ver la guía del [universo MAI ](https://qidao-qimps.gitbook.io/mai-finance-tutorials/v/espanol/universidade-de-mai/mai-metaverse)para más detalles). Esta aplicación soporta muchos activos y muchas cadenas, por lo que te será fácil enviar tus criptomonedas a Fantom. Por favor, compruebe las notas que se encuentran en la parte inferior de la interfaz de usuario de la aplicación para ver cúales son las tasas de transacción y el tiempo de ejecución previsto de la transacción.

![Transfiriendo MAI desde Polygon a Fantom](<../../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): ofrece servicio para transferir stablecoins a muchas blockchains distintas, con las comisiones rondando desde el 0.04% al 0.19% para enviar a Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): bajas comisiones, y asegura que siempre hay suficiente liquidez en la cadena de destino para el token que se quiere transferir. Cuanto menor sea la liquidez (o mayor sea la cantidad a transferir), tendrás que esperar más tiempo para que se realice la transferencia.

### Transfiriendo otros activos

* Binance CEX: Podrás comprar el token FTM directamente en Binance y enviarlo directamente a su red, el único problema es que el único token que podrás enviar a la red es FTM.
* [SpookySwap](https://spookyswap.finance/bridge): Tiene soporte de varios tokens de distintas redes que podrás enviar directamente a la red FTM.
* AnySwap: Puedes encontrar más información sobre esta aplicacion en el apartado anterior  .

## DeFi en Fantom

Fantom ha tenido un crecimiento bastante impresionante a partir de finales del verano de 2021, especialmente con los programas de recompensa que ayudaron a atraer inversores y desarrolladores en la cadena. El crecimiento también se ha visto apoyado por proyectos de primera línea que desplegaron sus DApps en Fantom en Septiembre de 2021, incluyendo Curve y SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Esta aplicación es muy similar a Balancer. Podrás intercambiar unos tokens por otros, y también entrar en pools equilibrados compuestos por múltiples tokens. Este es también el **primer socio oficial** de Mai Finance en Fantom, y el único lugar donde podrás intercambiar tus MAI, o utilizarlos en un pool MAI-USDC.

![Swapping MAI for a little more FTM](<../../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): Se trata del mayor DEX (Exchange Descentralizada) de Fantom, donde podrás intercambiar tus tokens por otros, depositar liquidez y cultivar rendimientos, prácticamente de la misma manera que lo harías en QuickSwap en Polygon. SpookySwap te recompensará utilizando el token BOO, el token nativo de la plataforma. Además, cuando deposites tus tokens BOO, obtendrás a cambio xBOO, un token de rendimiento, y podrás utilizarlo para obtener recompensas extra (el mismo principio que usa QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): Plataforma tradicional de AMM y cultivo de rendimientos donde podrás intercambiar tokens, crear tokens LP y cultivar rendimientos en pools de liquidez. SpiritSwap te pagará con tokens SPIRIT que podrás apostar en la plataforma y obtener tokens inSPIRIT (SPIRIT estará bloqueado durante un periodo de tiempo determinado), el colgante de los tokens veCRV. También puedes utilizar SpiritSwap para prestar y pedir prestado mientras esperas a Mai Finance en Fantom.
* [Tarot](https://www.tarot.to): Tarot es la versión en Fantom de Impermax, donde podrás usar tus tokens LP de SpookySwap (u otros DEXs/AMM) y usarlos para hacer farming en la plataforma. También puedes depositar tokens individuales y prestarlos en los pools específicos donde la gente podrá pedirlos prestados para generar nuevos tokens LP y apalancar su cantidad de farming. Ten en cuenta las liquidaciones si apalancas tus LPs en un pool donde la utilización es alta.
* [Scream](https://scream.sh): Se trata de un clon de Compound en el que podrás prestar tus tokens y pedir préstamos con ellos. Prestando tus tokens ganarás recompensas en el token que prestes, así como tokens SCREAM que podrás utilizar en otras plataformas.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Se trata de un clon de Compound en el que podrás prestar tus tokens y pedir préstamos con ellos. Prestando tus tokens ganarás recompensas en el token que prestes, así como tokens SCREAM que podrás utilizar en otras plataformas.

![Par DAI+USDC en Curve de Fantom](../../.gitbook/assets/ftm-crv.png)

Hay muchas más oportunidades en Fantom que serán explicadas en artículos posteriores, asi que estate atento ;).

## Otros link útiles

* [Explorador de Fantom](https://explorer.fantom.network)
* [Comprobar el precio del gas en Fantom](https://ftmscan.com/gastracker)
* [Discord de Fantom](how-to-get-started-on-fantom.md#ftm-faucet)&#x20;
* [DeBank](https://debank.com)&#x20;

## Descargo de Responsabilidad

Esta guía NO es un consejo financiero, y debe considerarse simplemente como una herramienta educativa. Haga siempre su propia investigación. Los proyectos presentados en esta guía sólo muestran las distintas posibilidades que hay en la red, y no debe tomarse como una promoción al proyecto.

{% hint style="info" %}
Tenga en cuenta que una estrategia que funciona bien en un momento dado puede dar malos resultados (o hacerle perder dinero) en otro momento. Manténgase informado, controle los mercados, vigile sus inversiones y, como siempre, investigue por su cuenta.
{% endhint %}

