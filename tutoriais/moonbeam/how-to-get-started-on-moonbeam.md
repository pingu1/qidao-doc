---
description: Neste guia, explicaremos como começar a usar o Moonbeam.
---

# Como começar na Moonbeam

## O que é Moonbeam?

Lançada em janeiro de 2020, a Moonbeam é uma plataforma de contratos inteligentes compatível com EVM (Ethereum Virtual Machine) em execução na rede Polkadot, tornando-se o que é chamado de parachain Polkadot. Parachains são conjuntos interconectados de redes que se beneficiam da relay chain da Polkadot enquanto permanecem interoperáveis, participando dos benefícios e da segurança da rede principal enquanto são executadas em paralelo a ela.

A Polkadot descreve os benefícios das parachains da seguinte forma: “Parachains encerram a era das blockchains em silos, criando uma internet descentralizada e conectada de blockchains onde antes existiam apenas redes isoladas com suas próprias comunidades tribalistas”.

![Moonbeam, uma parachain da Polkadot](<../../.gitbook/assets/moonbeam (1).jpg>)

Devido à sua camada de compatibilidade com EVM, a Moonbeam torna mais fácil para os desenvolvedores do Solidity portar seus aplicativos existentes de outras redes compatíveis com EVM para a Moonbeam com poucas alterações de código. Atualmente, a Moonbeam tem um TVL de US$ 130 milhões e um ecossistema de aplicativos [vibrante e crescente](https://defillama.com/chain/Moonbeam).

A Moonbeam também oferece compatibilidade com Substrate. Substrate é uma estrutura modular de blockchain usada por desenvolvedores para construir blockchains adaptados às suas necessidades usando componentes reutilizáveis chamados pallets. Ele usa a linguagem de programação Rust e é a estrutura que a maioria dos desenvolvedores usa ao construir parachains para a rede Polkadot.

Como a Moonbeam é um blockchain baseado em Substrate, os aplicativos integrados à sua rede se beneficiam da interoperabilidade entre as redes Polkadot e Ethereum, além de outras como Bitcoin.

Os desenvolvedores também podem usar ferramentas de ecossistema compatíveis com Substrate comumente usadas no Ethereum, incluindo exploradores de blocos, bibliotecas de desenvolvimento front-end e carteiras, bem como ferramentas de desenvolvimento como Truffle e Remix.

O token de gas nativo da Moonbeam é GLMR.

## Começando na Moonbeam

Antes de usar o Moonbeam, você precisará de um endereço de carteira. Como a Moonbeam é uma rede EVM, ela aceitará as mesmas carteiras que em outras redes EVM, incluindo carteira da web como Metamask ou Nifty, e você poderá usar sua carteira de hardware, como Trezor ou Ledger, mas talvez seja necessário seguir mais passos para poder conectá-la à rede.

Para este tutorial, vamos nos ater à Metamask, assim como fizemos para todos os outros guias deste site. Se você não tiver a Metamask instalada, poderá encontrar instruções em [Como começar sua jornada na Polygon](../polygon/how-to-get-started-on-polygon.md).

### Adicionando a Moonbeam à Metamask

Abra o pop-up Metamask, clique no ícone da sua carteira, navegue até `Settings` então selecione `Networks` e por último `Add Network`. Você usará as seguintes informações nos campos de texto relevantes:

* **Network Name:** Moonbeam
* **New RPC URL:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **Chain ID:** 128
* **Currency Symbol:** GLMR
* **Block Explorer URL:** [https://moonscan.io/](https://moonscan.io/)

Salve as alterações e a Metamask o mudará automaticamente para a Moonbeam:

![Moonbeam na Metamask](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## Pontes na Moonbeam

### Faucets

GLMR é o token de gas nativo da Moonbeam, então você precisará ter alguns em sua carteira para fazer transações na rede. Felizmente, a torneira oficial, Moonbeam Faucet, ajudará você a começar com uma pequena quantidade de GLMR, embora a quantidade dispersa pelo token às vezes pode não ser suficiente para concluir uma transação se a rede estiver congestionada.

Para receber GLMR gratuito, você precisará verificar se é humano por meio do captcha e conectar sua carteira Metamask ao site. Uma pequena quantia (0,007 GLMR) será enviada imediatamente para sua carteira.

![Moonbeam Faucet para GLMR](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

Além disso, os usuários podem querer usar o recurso "[Swap for Gas](https://app.solarflare.io/bridge/gas-swap)" da Solarflare. Isso permite que os usuários troquem outros tokens, incluindo WETH, WBTC, USDC, DAI, USDT, BUSD, FLARE e BNB por GLMR, o token de gas nativo da Moonbeam.

![Recurso "Swap for Gas" da Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### Pontes

* [Multichain](https://app.multichain.org/#/router) é a ponte oficial para MAI através de sua parceria com MAI Finance, e você pode facilmente enviar seu MAI para a Moonbeam usando-a.

![Multichain na Moonbeam](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) é uma AMM completa (Automated Market Maker) na Moonbeam que é muito semelhante à Uniswap. A Solarflare possui uma ponte integrada que permite aos usuários enviar ativos da rede principal Ethereum, bem como da BNB Chain para a Moonbeam. A Solarflare também possui um recurso "Trocar por gas", conforme mencionado na seção Faucets acima.

![Ponte pela Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) é uma ponte popular que também suporta Moonbeam. Observe que você pode não conseguir fazer a ponte de todas as rede para a Moonbeam (Polygon para Moonbeam não é suportado, por exemplo).

![Ponte pela Celer](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* Outras pontes estão disponíveis, mas podem ser específicas da rede, como Nomad ou Axelar para o ecossistema Cosmos.

## DeFi na Moonbeam

[StellaSwap](https://app.stellaswap.com/farm) é atualmente a principal fonte de liquidez para MAI na Moonbeam. A MAI-Base4Pool é composto por MAI, FRAX, USDT, USDC e DAI e atualmente possui um TVL (valor total bloqueado) de $535k, gerando um sólido APR (taxa percentual anual) de 26% em suas stablecoins.

![MAI-Base4Pool na StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam tem um ecossistema DeFi vibrante com dezenas de DApps (aplicativos descentralizados) disponíveis para uso, incluindo grampos DeFi encontrados em outras redes, como [Curve](https://moonbeam.curve.fi/) e [Beefy Finance](https://app.beefy.com/). Para obter uma lista completa dos DApps disponíveis, confira [a página da Moonbeam na DefiLlama.](https://defillama.com/chain/Moonbeam)

## Mai Finance na Moonbeam

Embora a Mai Finance não esteja disponível na Moonbeam, você pode criar vaults e tomar emprestado MAI tendo como garantia xStella e wGLMR na StellaSwap. Observe que o empréstimo de MAI na StellaSwap incorrerá em juros - 12% nos vaults xStella e 8% nos vaults wGLMR. Você pode descobrir mais sobre como usar os vaults de MAI da StellaSwap na próxima seção intitulada [Brincando de LEGO na StellaSwap](playing-with-mai-legos-on-stellaswap.md).

![Vaults na StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## Aviso legal

Este guia NÃO é um conselho financeiro e deve ser simplesmente considerado uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
