---
description: >-
  Neste guia, explicaremos tudo o que você precisa saber para começar a usar os
  diferentes DApps que a BNB Chain oferece.
---

# Como começar na BNB Chain

## O que é a BNB Chain?

A BNB Chain é uma rede compatível com EVM (Ethereum Virtual Machine) que é uma versão atualizada da Binance Smart Chain original que fornece baixas taxas de transação e tempos de bloco muito mais rápidos do que a Ethereum, a rede na qual se baseia.

Por isso, a BNB Chain é uma das redes mais populares do mundo, com mais de 4,5 bilhões de transações anuais e um [ecossistema de DApps](https://dappbay.bnbchain.org/) extremamente vibrante e maduro.

A BNB Chain usa o token BNB da Binance para pagar as taxas de gas, portanto, certifique-se de ter alguns em sua carteira para realizar transações. A Binance oferece [guias fáceis de serem seguidos ](https://www.binance.com/en/support/faq/85a1c394ac1d489fb0bfac0ef2fceafd)sobre como comprar ou transferir tokens para sua rede BNB.

## Começando na BNB Chain

Antes de usar a BNB Chain, você precisará de um endereço de carteira. Como o BNB Chain é uma rede EVM, ele aceitará as mesmas carteiras que em outras cadeias EVM, incluindo carteiras web como a Metamask ou a Nifty, e você poderá usar sua carteira de hardware como Trezor ou Ledger, mas pode ser necessário seguir etapas extras para poder conectá-las a rede.

Para este tutorial, vamos nos ater à Metamask, assim como fazemos em todos os outros guias deste site. Se você não tiver a Metamask instalada, poderá encontrar instruções em[ Como começar sua jornada na Polygon.](../polygon/how-to-get-started-on-polygon.md)

Além disso, você pode usar a própria Binance Wallet para começar na rede mais facilmente.

### Adicionando a BNB Chain à Metamask

Abra o pop-up Metamask, clique no ícone da sua carteira, navegue até`Settings` então escolha `Networks` e encontre `Add Network`. Você usará as seguintes informações nos campos de texto relevantes:

* **Network Name:** BNB Chain
* **New RPC URL:** [https://docs.binance.org/smart-chain/developer/rpc.html](https://docs.binance.org/smart-chain/developer/rpc.html)
* **Chain ID:** 0x38
* **Currency Symbol:** BNB
* **Block Explorer URL:** [**https://bscscan.com/**](https://bscscan.com/)\*\*\*\*

Salve as alterações e a Metamask o mudará automaticamente para o BNB:

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.28.44 AM.png>)

Se você quiser pesquisar RPCs adicionais com menor latência, dê uma olhada em ChainList para pontos de extremidade adicionais.

## Pontes à BNB Chain

### Faucets

Existem faucets, ou torneiras, disponíveis gratuitamente na BNB Chain, mas é a opinião do autor que será mais seguro usar algo como a ElkNet para obter tokens de gas gratuitos. Se você optar por usar uma faucet que encontrou online, faça-o por sua conta e risco. Com a [ElkNet](https://app.elk.finance/#/elknet), você pode optar por trocar alguns de seus tokens Elk por gas ao fazer a ponte para qualquer uma das redes suportadas.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.29.50 AM.png>)

### Pontes

* [Multi Chain](https://app.multichain.org/#/router) é o parceiro oficial da Mai Finance se você deseja transferir seu MAI ou QI para a BNB Chain de qualquer outra rede. Da sua rede selecionada, você pode simplesmente escolher a rede de destino (BNB Chain) e o ativo que deseja enviar (MAI ou QI por exemplo) com o valor correto e clicar no botão `Transfer`. Preste atenção às taxas de transferência cobradas diretamente no ativo que você está transferindo.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.32.07 AM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) é uma ponte popular e permite transferir tokens de cerca de quinze redes diferentes para a BNB Chain.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.31.15 AM.png>)

* [Hashflow](https://app.hashflow.com/) é uma tecnologia de ponte mais recente que funciona essencialmente como uma DEX (corretora descentralizada) crosschain para qualquer token com liquidez suficiente. Além disso, os usuários do Hashflow atualmente podem ganhar HFTs (tokens Hashflow) por trocar ou fornecer liquidez. Atualmente, as redes estão limitadas a Ethereum, Avalanche, Arbitrum, Optimism, Polygon e BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.33.51 AM.png>)

* [Elknet](https://app.elk.finance/#/elknet) atuará como uma ponte e como uma faucet quando você transferir o token ELK entre 2 redes. Você poderá conectar seu ELK e, na extremidade receptora, poderá ter uma pequena parte do seu ELK diretamente disponível como token de gás, BNB no nosso caso, conforme explicado na seção acima.

## DeFi na BNB Chain

* [Ellipsis Finance](https://ellipsis.finance/pool/0x68354c6E8Bbd020F9dE81EAf57ea5424ba9ef322) é o lugar ideal para prover liquidez em MAI na BNB Chain. O pool MAI na Ellipsis (MAI+val3EPS) é composto por quatro stablecoins, incluindo BUSD (Binance USD), USDC, USDT (Tether) e MAI. Ao depositar stablecoins e, em seguida, fazer staking com o LP na Ellipsis, os usuários podem ganhar um rendimento variável entre 6 e 15% pago no token EPS da Ellipsis, token VAL da Vallas, bem como taxas de negociação.

![MAI+val3EPS pool on Ellipsis](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.07.42 AM.png>)

## Mai Finance na BNB Chain

A plataforma de empréstimo já está disponível na BNB Chain, onde você poderá depositar seus tokens WBNB (Wrapped BNB) e CAKE (PancakeSwap) em um cofre e tomar emprestado MAI contra eles. Você pode então depositar seu MAI na Ellipsis para obter rendimentos.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.11.26 AM.png>)

## Aviso legal

Este guia NÃO é um conselho financeiro e deve ser simplesmente considerado uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
