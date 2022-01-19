---
description: >-
  Neste guia, explicaremos tudo o que você precisa saber para começar a usar a
  rede Fantom.
---

# Como começar na Fantom

## O que é Fantom

Fantom é uma alternativa a Ethereum para desenvolvedores de blockchain. Como uma blockchain open-source com suporte para contratos inteligentes, ela permite que os desenvolvedores construam Dapps (**D**ecentralized **App**lications) seguros, compreensivos e modulares.

A rede foi projetada para vencer todas as limitaçōes da geração anterior das plataformas blockchains, as vezes referenciado como o trilema das blockchains: decentralização, segurança e escalabilidade. Para melhorar um destes aspectos, precisamos sacrificar um dos outros dois. A Fantom tenta resolver isso graças ao seu mecanismo de consenso Lachesis aBFT (Asynchronous Byzantine Fault Tolerant) baseado em DAG (Directed Acyclic Graphs), permitindo alta performance,  escalabilidade e segurança. Testes iniciais mostraram que a Fantom pode facilmente aguentar mais de 20,000 transaçōes por segundo..

Por último, a Fantom é 100% compativel com EVM (**E**thereum **V**irtual **M**achine), o que significa que DApps que foram desenvolvidos em redes compativeis a EVM podem rodar na Fantom também. Isso traz outra vantagem aos usuários, já que a MetaMask e outras aplicaçōes web3 também são compativeis com a Fantom. Você será capaz de alternar entrar a Polygon ou a Avalanche à Fantom pela mesma carteira.

## Começando na Fantom

Como a Fantom é compativel a EVM, se você já possuir uma carteira para outras redes EVM (Ethereum Mainnet, Polygon ou Avalanche), você será capaz de usá-la. Se não, é hora de criar uma nova carteira. Há muitos tipos diferentes de carteiras que podem ser usadas: **carteiras de software** como a Metamask ou a [fWallet](https://pwawallet.fantom.network/#/), e **carteiras de hardware** como a [Trezor](https://trezor.io/coins/) ou a [Ledger](https://fantom.foundation/blog/how-to-set-up-your-ledger-nano-s-x-with-fantom/).

Aqui, como ela é a nossa escolha nos outros guias, usaremos a Metamask, mas sinta-se livre para utilizar a carteira que preferir, seja de software ou hardware. Se precisar de ajuda para instalar a Metamask, você pode visitar este [guia da rede polygon](../../polygon-tutorials/how-to-get-started-on-polygon.md#downloading-metamask).

### Adicionando a rede Fantom à Metamask

Para usar a rede Fantom, você precisará configurá-la manualmente na Metamask. Para fazer isto, clique no menu "Network" na parte superior da janela (onde é exibida a rede que está sendo utilizada, Ethereum Mainnet originalmente), então selecione `Custom RPC`. As informaçōes seguintes são as que te permitirão conectar-se a rede Fantom:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Após salvar as mudanças, a Metamask irá automaticamente trocar para a rede Fantom.

![Bom trabalho! Você está na Fantom!](../../.gitbook/assets/ftm-mm0.png)

Se precisar de mais detalhes para configurar a Metamask, você pode encontrar mais informaçōes no [guia oficial da Fantom](https://docs.fantom.foundation/tutorials/set-up-metamask).

### Faucet de FTM

Agora que você está na FTM, você precisará de um pouco de FTM (token nativo usado para cobrir taxas de transaçōes). Voce pode fazer a ponte de FTM de outras redes, ou utilizar uma faucet (torneira) que depositará tokens FTM em sua carteira para realizar algumas transaçōes. A [principal faucet na Fantom](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas) pode ser ecnontrada na SpookySwap, uma das principais DEXes (**D**ecentralized **Ex**change) da rede. Perceba que é um serviço oferecido pela SpookySwap que depende do Discord, e que exigirá uma conta no Discord ativa por mais de 30 dias (porém não é necessário estar no servidor da SpookySwap por 30 dais).&#x20;

* Após você entrar no servidor da [SpookySwap](http://discord.gg/AqbsWsWDgn), e verificar sua conta, vá até o canal #faucet.

![](<../../.gitbook/assets/image (42).png>)

* No canal da #faucet, simplesmente digite o comando `!faucet` e o bot irá te enviar um pouco de $FTM. Perceba que você estará limitado a 1 interação a cada 30 dias.
* Se você quer verificar se recebeu seu token FTM, você pode clicar no nome do Fantom Tip Bot para interagir com ele diretamente, e escrever`!balance`

![Obrigado Fantom Tip Bot e SpookySwap](<../../.gitbook/assets/image (45).png>)

* Tudo o que você precisa fazer agora é enviar seus tokens FTM a sua carteira utilizando o comando `!withdraw <endereço_sua_carteira>`. Você pode encontrar o endereço de sua carteira no topo da janela da Metamask.

![Retirando fundos pela conta do Discord](../../.gitbook/assets/ftm-faucet.png)

![Depósito recente em minha carteira Metamask](../../.gitbook/assets/ftm-mm.png)

## Ponte à rede Fantom

### Fazendo a ponte com stablecoins / ETH / BTC

Se você que enviar seus ativos à Fantom, você pode utilizar as seguintes pontes:

* [AnySwap](https://anyswap.exchange/#/bridge): Esta é ponte oficial para enviar seu MAI da Polygon à Fantom (leia o [guia de MAI no metaverso](../../mai-university/mai-metaverse.md#fantom) para mais detalhes). Esta solução suporta vários ativos e muitas redes, o que torna fácil o envio de moedas à Fantom. Por favor confira os lembretes na parte de baixo da interface da ponte para obter as taxas de transaçōes e tempo de execução esperado.

![Mandando um pouco de MAI da Polygon à Fantom](<../../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): oferece serviço de ponte para muitas redes e para a maioria das stablecoins, com taxas variando entre 0.04% e 0.19% para a ponte da Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): taxas baixas, e garante que há liquidez suficiente there's na rede alvo para o token que você quer mandar. Quanto mais baixo a liquidez (ou maior a quantidade para mandar), mais demorada a transferência.

### Fazendo a ponte com outros ativos

* Binance CEX: você será capaz de comprar o token FTM na Binance e mandá-lo diretamente à Fantom, mas este é o unico token que você será capaz de transferir.
* [SpookySwap](https://spookyswap.finance/bridge): suporta varias redes e muitos tokens que você poderá enviar à Fantom.
* AnySwap: veja a descrição feita na seção de stablecoins.

## DeFi na Fantom

A Fantom teve uma expansão impressionante após a metade de 2021, especialmente com programas de recompensa que ajudaram a atrair investidores e desenvolvedores à rede. O crescimento também tem sido suportado projetos blue chip que lançaram seus DApps na Fantom em setembro de 2021, incluindo a Curve e SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Esta aplicação é muito semelhante a Balancer. Você poderá trocar alguns tokens por outros, e também participar de de pools equilibradas compostas de vários tokens. Este é também o primeiro parceiro oficial da Mai Finance na Fantom, e o único lugar onde você será capaz de trocar seu MAI, ou usá-los na pool MAI-USDC.

![Trocando MAI por um pouco de FTM](<../../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): Esta é a maior DEX (**D**ecentralized **Ex**change) na Fantom onde você poderá trocar seus tokens por outros, depositar liquidez e gerar renda por farms, praticamente da mesma maneira que você faria na QuickSwap da Polygon. A SpookySwap te recompensará usando o token BOO, o token nativo da plataforma. Além disso, quando você fizer staking com  tokens BOO, você receberá xBOO, um token que comprova teu rendimento, em troca, e você pode usá-los para ganhar recompensas adicionais (mesmo princípio da Dragon Syrup na QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): Plataforma de AMM tradicional e farm de rendimento, onde você será capaz de trocar tokens, criar LP tokens e gerar rendimento de farm em pools de liquidez. A SpiritSwap irá te pagar com tokens SPIRIT que você pode colocar em staking na plataforma e receber tokens inSPIRIT (SPIRIT será bloqueado por um certo período), o pendente de tokens veCRV. Você pode também usar a SpiritSwap para empréstimo e tomar emprestado enquanto espera pela Mai Finance na Fantom.
* [Tarot](https://www.tarot.to): Tarot é a versão da Impermax na Fantom, onde você pode usar seus LP tokens da SpookySwap (ou outras DEXs/AMM) e usá-los para farming em outras plataformas. Você também pode depositar tokens únicos e emprestá-los em pools específicas onde pessoas poderão tomar emprestado para gerar mais LP tokens e alavancar suas posiçōes em farming. Esteja atento às liquidaçōes se você alavancar seus LPs em uma pool onde a utilização é alta.
* [Scream](https://scream.sh): Este é um clone da Compound onde você poderá emprestar seus tokens e tomar emprestado, com eles como garantia. Emprestar seus tokens te fará receber recompensas no token que você emprestou, assim como tokens SCREAM que você poderá usar em outras plataformas.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve é o projeto blue chip que todos conhecem bem, onde você poderá depositar seus tokens em pools específicas (não é necessário depositar uma quantidade equilibrada) e você será recompensado nos tokens que você emprestou, assim como em CRV e wFTM.

![Pool dupla de PoDAI+USDC da Curve na rede Fantom](../../.gitbook/assets/ftm-crv.png)

Há diversas oportunidades disponiveis na Fantom que serão descritas em nossos guias.

## Outros links úteis

* [Fantom explorer](https://explorer.fantom.network)
* Rastreador de [Gas da Fantom](https://ftmscan.com/gastracker)
* Servidor oficial da [Fantom no Discord](how-to-get-started-on-fantom.md#ftm-faucet)
* Gerenciador de portfólios [DeBank](https://debank.com)

## Aviso legal

Este guia não é conselho financeiro, e tem cunho meramente educacional. Sempre faça a sua própria pesquisa. Os projetos apresentados aqui são para mostrar possibilidades na rede, este guia não deve ser tomado como recomendação.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um periodo de tempo pode performar mal (ou te fazer perder dinheiro) em outro período. Por favor, se informe, monitore os mercados, mantenha um olho em seus investimentos, e como sempre, faça a sua própria pesquisa.
{% endhint %}
