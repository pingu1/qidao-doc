---
description: >-
  Neste guia, explicaremos tudo que você precisa saber para começar a usar a
  rede Moonriver.
---

# Como começar na Moonriver

## O que é Moonriver

Será complexo explicar o que é Moonriver sem conversar sobre algumas outras redes, como a Moonbeam, Kusama e Polkadot.

Polkadot é uma blockchain L1 que compete diretamente com a Ethereum, Cosmos ou Eos, e seu objetivo é cultivar um ecosistema completo de criptomoedas e aplicaçōes. Uma das maiores distinçōes entre a Polkadot e outras L1 é a sua separação em uma rede principal (relay chain) e redes criadas pelos usuários (parachains). A Relay Chain se beneficia de requisitos baixos em termos de recursos computacionais já que a maioria dos desenvolvimentos e testes são feitos nas parachains. Por outro lado, parachains herdam a sua segurança da relay chain. Isso cria ambientes isolados que podem funcionar de forma autônoma e que não compartilharão informaçōes de seus usuários à rede principal.&#x20;

Kusama é um ambiente de pré-produção para a Polkadot, uma rede separada que imita a Relay Chain da Polkadot, e onde todo o desenvolvimento e atualizaçōes para a rede principal são testados. Entretanto, como um ambiente de pré-produção, a Kusama opera com criptomoedas e transaçōes de verdade, mas com regras mais relaxadas do que na Polkadot. Entretanto, o objetivo das aplicaçōes e sidechains desenvolvidas na Kusama é de migrar para a Polkadot no futuro. Por conta das regras mais relaxadas, é mais fácil para os projetos testarem coisas diferentes e crescerem como uma comunidade, enquanto desenvolvem o protocolo. Quando o produto final estiver pronto, tudo pode ser migrado para o ambiente de produção.

A Moonriver é uma parachain da Kusama. O código que é implantando na Moonriver é uma versão teste do código que pode ser implantado na Moonbeam, a versão de produção da Moonriver na Polkadot. A partir do momento que o código é validado na Moonriver, ele pode ser enviado à Moonbeam. Moonbeam e Moonriver são redes compativeis com EVM, o que significa que elas aceitam os mesmos contratos inteligentes que outras redes, compativeis com a Ethereum, aceitam. Por conta disso, a Moonriver rapidamente se tornou o ponto de entrada de muitos DApps (**D**ecentralized **App**lications, Aplicaçōes Decentralizadas) que queriam expandir da rede Ethereum (Ethereum Mainnet, Polygon, Avalanche, Fantom,etc) à rede Polkadot.

Como outras redes compativeis com EVM, a Moonriver possui um token que é usado para verificar as transaçōes: o token MOVR.

## Começando na Moonriver

Antes de usar a rede Moonriver, você precisará de uma carteira. Como a Moonriver é uma rede EVM, ela aceitará as mesmas carteiras que usamos em outras redes EVM, incluindo carteiras virtuais como a Metamask ou Nifty, e você poderá usar sua hardware wallet como Trezor ou Ledger, mas você pode precisar seguir etapas adicionais para poder conectar sua cold wallet à rede. Você pode encontrar um passo a passo na [documentação oficial da moonbeam foundation](https://moonbeam.foundation/tutorials/how-to-create-moonriver-ethereum-address/).

Para este tutorial, nós utilizaremos a Metamask como fazemos em todos os outros guias deste site. Se voce não tem a Metamask instalada, você pode encontrar instruçōes para isso [neste guia da Polygon.](../../polygon-tutorials/how-to-get-started-on-polygon.md)

### Adicionando a Moonriver à Metamask

Em teoria, a Moonriver vem pré-instalada com a MetaMask, o que significa que você não precisará adicionar as informaçōes da rede na interface. Entretanto, pode ser uma boa ideia conferir que as configuraçōes estão corretas checando os valores salvos em sua carteira local. Abra o popup da Metamask, clique no icone da carteira, navegue até Settings então vá ate`Networks` e `Moonriver`. A informação que você terá é deve ser a seguinte:

* **Network Name:** Moonriver
* **New RPC URL:** https://rpc.moonriver.moonbeam.network
* **Chain ID:** 1285
* **Currency Symbol:** MOVR
* **Block Explorer URL:** https://blockscout.moonriver.moonbeam.network/

Salve as mudanças, e a Metamask irá automaticamente trocar para a rede Moonriver:

![Sucesso! Agora, você está na Moonriver!](../../.gitbook/assets/Moonriver-setup-MM.png)

## Pontes à Moonriver

### Faucets

Uma das maiores DEX na Moonriver, SolarBeam, oferece [uma transação de swap sem gas](https://app.solarbeam.io/bridge/gas-swap), caso você não tenha mais gas. Aqui, assume-se que você tem fundos na Moonriver, mas não pode fazer nada com eles porque possui 0 MOVR em sua carteira.

![Transação sem gas que permitirá que você troque um ativo por gas](../../.gitbook/assets/Moonriver-faucet.png)

Observe que apenas alguns ativos são aceitos para esta transação sem pagar gas e o MAI não faz parte das moedas suportadas.

### Pontes

* [Relay Chain](https://app.relaychain.com/transfer#/) é o parceiro oficial da Mai Finance se você deseja transferir seu MAI para a Moonriver da Polygon. Quando estiver conectado à Polygon, basta escolher a rede de destino (Moonriver) e o ativo que deseja enviar (MAI ou miMATIC) com a quantidade correta e clicar no botão Transferir. Preste atenção às taxas de transferência.

![Mandando MAI da Polygon à Moonriver usando Relay Chain](../../.gitbook/assets/Moonriver-relaychain.png)

* Se você precisa conectar outros ativos de outra rede, você pode usar o Relay Chain (veja acima), [AnySwap](https://anyswap.exchange/#/bridge) funcionará se você quiser fazer a ponte de Eth Mainnet para Moonriver, e claro, você também pode usar o recurso de ponte da [Solarbeam](https://app.solarbeam.io/bridge).
* Uma observação para a [Elknet](https://app.elk.finance/#/elknet) que funcionará como uma ponte e como uma faucet quando você transferir o token ELK entre 2 redes. Você poderá conectar seu ELK e, na extremidade receptora, poderá ter uma pequena parte de seu ELK diretamente disponível como token de gás, MOVR em nosso caso.

### Hub

Caso você conecte algum MAI da Polygon ao Moonriver via Relay Chain, você obterá a versão RelayChain do MAI em vez do MAI nativo cunhado pelo aplicativo no Moonriver. Os 2 tokens (o da RelayChain e o da Mai Finance) têm o mesmo valor e o mesmo nome, mas endereços de contrato diferentes, e o único que será aceito para farming na Moonriver é o da Mai Finance.

Você pode trocar seu MAI da Relay Chain usando [o hub na Mai Finance](https://app.mai.finance/hub) com uma taxa de 1:1, então você podera usar seu MAI verdadeiro em outras plataformas.

![Usando o hub para trocar MAI(RelayChain) por MAI de verdade](../../.gitbook/assets/Moonriver-hub.png)

{% hint style="info" %}
Como uma observação, se você quiser fazer a ponte de seu MAI da Moonriver para a Polygon ou outras rede, você terá que convertê-los primeiro em sua versão RelayChain.
{% endhint %}

## DeFi na Moonriver

A Moonriver está ganhando muita força e mais e mais aplicativos estão mudando para esta nova rede, com potencial para migrar totalmente para Polkadot. Assim, você poderá fazer farming na seguinte plataforma (a lista não está completa):

* [Solarbeam](https://app.solarbeam.io): Este é a principal DEX e AMM na Moonriver. Você poderá trocar seus ativos, participar da mineração de liquidez fornecendo pares LP (Liquidity Providing) em fazendas ou fazer staking com o token nativo da plataforma. A Solarbeam também é um dos primeiros parceiros da Mai Finance na Moonriver, e você poderá fazer farming com o par MAI-MOVR. Você também encontrará um pool MAI-USDC que não está recebendo nenhuma recompensa, mas pode obter algumas taxas de operaçōes.

![Pools LP que incluem MAI na Solarbeam, Dezembro de 2021](../../.gitbook/assets/Moonriver-solarbeam.png)

Quando você faz farming na Solarbeam, você será recompensado em tokens SOLAR, que permitem a você fazer staking em um Vault por um determinado período de vesting e ganhar tokens SOLAR adicionais, ou mais staking para ganhar outros tokens exóticos para a plataforma.

* [Huckleberry Finance](https://www.huckleberry.finance): Esta é outra DEX / AMM na Moonriver onde você será capaz de obter rendimento por farming e, possivelmente, usar o Beefy para aumentar seus ganhos.
* [Beefy Finance](https://app.beefy.finance/#/moonriver): O famoso auto acumulador também está na Moonriver e o ajudará a aumentar seus ganhos com a Solarbeam e a Huckleberry. Como uma observação, a Beefy não propõe o par MAI-MOVR no momento da escrita, mas você poderá usar a Beefy para colher os tokens SOLAR e obter mais MAI-MOVR do acumulador.
* [Sushiswap](https://app.sushi.com): Não há necessidade de apresentar a SushiSwap! Você poderá trocar seus ativos e fazer farming por certos tokens LP, como faria em qualquer outra rede. As recompensas são concedidas no SUSHI e MOVR.
* [Rome DAO](https://romedao.finance): Este é o primeiro OHM-fork na Moonriver. Empreste seus ativos para obter tokens ROME com desconto, com que você pode realizar staking para ganhar um APY muito alto. No momento da escrita, o ROI de 5 dias é de cerca de 10,6%. A RomeDAO atualmente aceita FRAX e MIM em sua tesouraria, mas em breve poderá aceitar também MAI.

## Mai Finance na Moonriver

A plataforma de empréstimo já está disponível na Moonriver, onde você poderá colocar seus tokens mooSolarETH-USDC em um vault e tomar MAI emprestado. Para fazer isso:

* Crie um par ETH-USDC na Solarbeam
* Deposite o par ETH-USDC na Beefy e receba o token comprovante mooSolarETH-USDC
* Deposite seu mooToken na Mai Finance no [vault apropriado.](https://app.mai.finance/vaults/create)

![Vaults da Mai Finance na Moonriver, Dezembro de 2021](../../.gitbook/assets/Moonriver-vaults.png)

Vault de ETH apenas também é uma opção.

Enquanto sua garantia está ganhando um APY de 44,08% da Beefy Finance (no momento em que escrevo), você poderá pegar emprestado o MAI e fazer farming na pool MAI-MOVR e obter um APR de 128% no Solarbeam, ou em breve APY de 158,058% na RomeDAO.

## Aviso legal

Este guia NÃO representa conselho financeiro e deve ser considerado simplesmente uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um periodo de tempo pode performar mal (ou te fazer perder dinheiro) em outro período. Por favor, se informe, monitore os mercados, mantenha um olho em seus investimentos, e como sempre, faça a sua própria pesquisa.
{% endhint %}
