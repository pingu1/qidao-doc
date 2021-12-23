---
description: >-
  Este guia apresenta uma analise completa das diferentes opçōes de alavancagem
  propostas pela Mai Finance na Fantom, utilizando vaults de rendimento e da
  Beefy.
---

# Alavanque as suas criptomoedas na Fantom

## Introdução

A Mai Finance lançou a sua plataforma de empréstimos na Fantom com muitos tipos diferentes de vaults, permitindo a possibilidade de cunhar a stablecoin MAI dependendo dos ativos que você depositar no vault. A idéia é que você poderá manter suas criptomoedas e se beneficiar da sua apreciação de preço, enquanto pode comprar outras moedas e render em farming com altos APRs. Se você utilizar o seu empréstimo para comprar mais do mesmo ativo que você já depositou, isto chama-se alavancagem. Nós mostraremos os beneficios desta estratégia utilizando 2 plataformas de empréstimos diferentes na Fantom para alavancar nosso tokens DAI.

## Alavanque seus tokens em vaults

### Deposite seus ativos na Yearn Finance

[Yearn Finance](https://beta.yearn.finance/#/home) é um de protocolos rodando na Ethereum Mainnet e em outras blockchains, que permite aos seus usuários otimizar seus rendimentos através de empéstimos e trading. Na Fantom, o produto que nós utilizaremos serão os vaults na Yearn Finance. Esta é uma ferramenta que aceitará depósitos de únicos tokens e fará você colher rendimentos deste depósito. Como prova de depósito, você receberá yvToken. No nosso caso, nós depositaremos DAI e receberemos yvDAI em troca.

![Vaults de rendimento na rede Fantom](../../.gitbook/assets/ftm-leverage-yv1.png)

{% hint style="info" %}
O website da Yearn Finance ainda está em sua versão beta na rede Fantom. O time ainda está trabalhando na plataforma e APRs/APYs ainda não são exibidos. Se você ir a aba Iron Bank, que é o protocolo de empréstimos da plataforma, você notará que emprestar DAI rende um APR de aproximadamente 8%. Por favor, invista a seu próprio risco.
{% endhint %}

### Deposite seu yvToken na Mai Finance

Após depositar seu DAI na Yearn Finance, você deverá obter yvDAI em sua carteira. Isto é o que nós chamamos de token comprovante de rendimento: é um token que não possui nenhum valor em si mesmo, mas representa a faria da pool em que seus ativos estão rendendo e em que recompensas são acumuladas automaticamente. Em outras palavras, se o seu DAI não alterar em valor pois ele é pareado ao dólar americano, o valor subjacente de seu token yvDAI só deve aumentar.

A Mai Finance aceita diversos tokens comprovantes de rendimentos como garantia, incluindo yvDAI. Agora, você pode depositar esse token como garantia e tomar emprestado MAI.

![Deposite seu yvToken na Mai Finance](../../.gitbook/assets/ftm-leverage-yv2.png)

O vault yvDAI possui um limite de liquidação em 110%, isso significa que você pode tomar MAI emprestado até o ponto que a razão entre o valor de sua garantia e o valor da dívida é de 110%. Tenha cuidado, pois 110% é o valor pelo qual você já é liquidado. Você precisa, portanto, manter uma proporção acima deste limite minimo. Como DAI não varia muito em preço (menos de centavos) é possivel mantermos uma CDR (**C**ollateral to **D**ebt **R**atio) "segura" de 115%, mas sinta-se livre para manter a taxa mais alta.

Como sempre, para calcular o valor do empréstimo que nós podemos obter baseado no valor de nossa garantia e a CDR alvo que queremos, nós usaremos a seguinte fórmula:

$$
MAI_{disponível} = \frac{Garantia_{valor} - Dívida_{valor} * CDR_{alvo}}{CDR_{alvo}}
$$

​Como uma garantia de $100 e nenhuma dívida, se nós queremos manter uma CDR saudável de 115%, nos podemos tomar emprestado até:

$$
MAI_{disponível}=\frac{100-0*1.15}{1.15}=86.95
$$

​Você está agora em uma posição onde você possui seu rendimentos em DAI de um vault, e você também tem um pouco da stablecoin MAI disponível para uso. Como nós queremos alavancar nossa posição em DAI, nós trocaremos nosso MAI por mais DAI.

### Trocando seu MAI na BeethovenX

Na Fantom, o principal provedor de liquidez para MAI é a [BeethovenX](https://app.beets.fi/#/trade). Este é o principal lugar para você trocar seus tokens MAI para mais DAI, para a nossa estratégia.

![Trocando MAI por mais DAI](../../.gitbook/assets/ftm-leverage-yv3.png)

Esta é a última etapa de nosso loop. Agora que temos mais DAI, podemos depositá-lo no vault, e repetir o loop. Fazer isto aumenta a quantidade de ativos que temos no vault, o que significa que colheremos mais recompensas ao emprestar DAI naquela plataforma. O APR/APY continua o mesmo, mas como temos mais ativos, recebemos mais juros, e se compararmos ao nosso investimento inicial, é o o nosso APR que aumenta. Se você quer mais exemplos de que APR pode obter utilizando loops com yvDAI, por favor, leia nosso [guia de token camDAI](../../polygon-tutorials/camdai-beginner-strategy.md#main-strategy) para a Polygon, que utiliza a mesma estratégia, mas com ferramentas diferentes.

{% hint style="success" %}
BeethovenX is actually a fantastic opportunity to farm yields with your borrowed MAI. Simply deposit your MAI in the MAI-DAI-USDC pool (APR of \~30% as of November 2021) if you cannot achieve a better APR using leveraged loops.
{% endhint %}

$$
MAI_
$$

## Leverage your mooScreamTokens on Mai Finance

### Deposit your assets on Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) is a Decentralized, Multi-Chain Yield Optimizer platform that allows its users to earn compound interest on their crypto holdings. In other words, you can deposit some assets or LP tokens from other platforms on Beefy Finance and let the auto-compounder harvest farm tokens and compound them into more of your deposited asset / LP token. For our exemple, we will use single DAI deposits on Beefy and use [Scream](https://scream.sh/lend) as the underlying platform. Scream is a Compound fork on the Fantom network on which you will be able to lend your assets and collect SCREAM tokens. Beefy will then sell the SCREAM tokens for more DAI.

To deposit our DAI, we will visit the Beefy Finance app and select Scream as the platform on which we will farm yields. You can also add the DAI filter in order to get the direct DAI deposit.

![Deposit your DAI on Beefy using Scream](../../.gitbook/assets/ftm-leverage-beefy1.png)

As you can see, Beefy is already giving an unbelievable APY on DAI single deposits. Once you have your DAI deposited on Beefy, you should have a proof of deposit in your wallet under the form of mooScreamDAI tokens. As for the yvDAI token, the mooScreamDAI token is a yield bearing deposit, meaning that you asset is still used on Scream and compounded on Beefy, earning yields. But you will be able to use this token on Mai Finance to borrow MAI against them.

### Deposit your mooScreamToken on Mai Finance

Once you deposited your DAI on yearn finance, you should have mooScreamDAI in your wallet. You can use the exact same steps as for the Yearn Vault strategy above, the only difference is that the mooScreamDAI liquidation ratio is 135%. Since DAI is a stable coin, it's still possible to borrow MAI and keep a CDR very close to the liquidation ration. For our exemple, we will aim at a 140% CDR, and with the same formula as above, we can calculate the amount of MAI we can mint with 100$ worth of DAI.

$$
MAI_{available}=\frac{100-0*1.4}{1.4}=71.43
$$

​Since we are borrowing less, we will be able to perform less loops and the final equivalent APY will also be lower, however this is still a pretty good beginner strategy.

The rest of the loop is the same as for yvDAI, meaning you will have to swap your MAI for DAI on BeethovenX and repeat until you're satisfied.

## Some notes on leveraging strategies

Leverage DAI is considered a beginner strategy in the sense that it presents very little risk (you are working with stable coins) and you can get some nice yields using at most 3 protocols. However, there's still _some_ risk.

### Liquidation risk

The more loops you will perform, the higher the liquidation risk. Indeed, even a small variation of the DAI price will be magnified by the leverage you applied, and even if you keep a CDR 5 points above the liquidation ratio, your vault can be at risk. It's always a good idea to stop the leverage loops at the step where you deposit your assets on MAI finance and don't borrow additional MAI in order to keep a better CDR.

Also, in case of a liquidation, because your vault on MAI finance contains a lot more assets, a liquidation will also have a bigger impact than if you didn't levered your position, simply because the debt you have to repay is also much bigger.

### Technology risk

If you use a lot of protocols for your investment legos, you need to make sure that these protocols are safe. Indeed, in our leveraging strategy, if a single protocol gets hacked, the entire strategy may collapse. Make sure you do your due diligence before investing in DeFi projects.

### Hitting debt ceilings

Because these strategies are easy to set and present low risks, there's a very high demand for them. However, you certainly noticed that in the leverage process, borrowed MAI is swapped for DAI (or other tokens). If too much MAI is sold on Beethoven, its price will decrease slowly and there is a risk for MAI to lose its peg, which is pretty bad for a stable coin. In order to let time for the price to stabilize, Mai Finance has security mechanisms in place, and the most important one is a debt ceiling for each vault.

A debt ceiling represents the maximum number of MAI that can be minted for a given vault. Once the ceiling is reached, no more MAI can be borrowed. Then the core team in charge of MAI finance can decide to increase the ceiling or wait a little more for a better price for MAI.

You can at all time verify the amount of MAI that can be minted on the [vault creation page](https://app.mai.finance/vaults/create), but you will usually notice that there aren't any more MAI if you get the following error message:

![Error message received when debt ceiling is reached](../../.gitbook/assets/ftm-leverage-error.png)

This error message will appear even if your health factor is correct. In most cases, waiting for the ceiling to be increased is the only solution. Keep an eye on twitter or on Discord to know when this happen.

## Disclaimer

This guide presented some of the ways you can use your assets on Fantom and include Mai Finance to your strategy in order to increase your gains. However, as usual, this tutorial isn't a financial advice and you should always DYOR before applying an investment strategy, and invest in a responsible manner.

Keep also in mind that this solution may not be the best strategy depending on when you plan to use it. We just highlighted that BeethovenX has pretty interesting APRs too for your MAI, and you can also use Beefy Finance to compound the BEETS rewards into more stable coins.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
