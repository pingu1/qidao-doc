---
description: >-
  Este artigo é uma explicação detalhada de como você pode usar a Mai Finance
  para tomar emprestado MAI com juros a 0% e ser pago por isso, transformando
  estes juros em negativos.
---

# Empréstimos em MAI e incentivos de Vaults

## Introdução

O business central da Mai Finance é ser uma plataforma de empréstimos. Em vez de vender suas criptomoedas para comprar outros ativos, as pessoas podem bloquear seus fundos na Mai Finance e tomar ativos emprestados. Isso apresenta a oportunidade de manter ativos de alto valor (WBTC, WETH, etc) enquanto ainda é possível obter outros ativos e obter rendimentos de farming. Nesse caso, o empréstimo é usado para gerar receita, enquanto a garantia ganha valor.

Uma das outras grandes vantagens de usar a Mai Finance é que não há um cronograma de reembolso. Em outras palavras, você empresta suas criptomoedas, toma emprestado a stablecoin MAI graça, não paga juros e pode pagar sua dívida quando quiser. Veja os diferentes artigos sobre [gestão de dívida](../debt-management-tutorials/debt-repayment-why-and-when.md) para mais detalhes. A unica taxa que você pagaria seria uma taxa de reembolso correspondente a 0.5% do dinheiro que você tomou emprestado, que você paga ao quitar seu empréstimo, e que é tomado da sua garantia.&#x20;

Por exemplo, se você depositou $200 em WETH para emprestar $100 em MAI, quando você pagar seu empréstimo, você terá que pagar uma taxa de $0,50 retirada diretamente de seu depósito de WETH. \
\
Se isso já não fosse uma oportunidade incrível, a equipe da Mai Finance introduziu em setembro de 2021 os incentivos de Vaults pagos em Qi, o token nativo da Mai Finance. Em outras palavras, ao depositar seus ativos na Mai Finance em um vault para tomar emprestado MAI, você será pago. Este artigo apresenta em detalhes como funciona essa funcionalidade.

## Vaults: O que são e como funcionam

### Criando um Vault

Na Mai Finance, os vaults são lugares especiais onde se pode depositar seus ativos. Atualmente, existem 10 tipos de vaults:

![Os diferentes tipos de vaults que você pode criar no Mai Finance](<../.gitbook/assets/image (1).png>)

Existem 2 tipos diferentes de vaults:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

e

* camWETH
* camWBTC
* camWMATIC
* camAAVE

Os primeiros 6 vaults da lista são para ativos simples, enquanto os 4 últimos são para camTokens. CamTokens são tokens de mercado AAVE compostos, uma representação de um depósito que você poderia ter feito no AAVE e depois depositado nos pools de rendimento da Mai Finance. Enquanto seus ativos estão gerando rendimentos no AAVE (e enquanto as recompensas são automaticamente acumuladas pelo pool de rendimentos), você ainda pode emprestar stablecoins MAI com estes tokens como garantia.

Como observação, você pode ver na captura de tela acima que a página de criação mostra algumas informações muito importantes:

* _MAI Available_: corresponde ao teto máximo da dívida, o número máximo de MAI que podem ser cunhados a partir de depósitos em vaults.
* _Min Coll. ratio_: este é o taxa mínima de garantia para dívida (CDR) para esse vault
* _Vault incentives APR_

### Entendendo o Teto de Dívida

O número máximo de MAI que se pode cunhar em um cofre específico depende da quantidade de ativos depositados nesse cofre. O teto da dívida é implementado para garantir que o mercado não seja inundado com MAI em um tempo muito curto, o que pode afetar o preço da stablecoin.

Por exemplo, se uma grande instituição depositasse 5.000 WBTC de uma só vez e conseguisse tomar emprestado $100.000.000 em MAI, trocando a totalidade por mais WBTC, isso poderia reduzir tanto o preço do MAI que o preço se desviaria muito de seu valor de pareamento, colocando toda a plataforma em risco. O teto da dívida é o mecanismo que impede que isso aconteça: há uma quantidade máxima de MAI que pode ser cunhada para um determinado tipo de vault.

Quando o teto da dívida é atingido, é registrado o momento em que não há mais MAI disponíveis para cunhar, e o sistema aumenta automaticamente o teto da dívida após 48 horas. Isso é considerado tempo suficiente para que o preço do MAI se estabilize (no caso de alta pressão de venda após uma grande venda do MAI).

Isso significa que por 48h, ninguém poderá emprestar mais MAI de um vault que atingiu seu teto de dívida, a menos que uma dívida seja paga.

Como observação, quanto mais MAI no mercado, mais estável é o preço. De fato, uma venda maciça de MAI é menos invasiva se houver mais MAI em circulação.

* Se alguém vender 1.000 MAI enquanto houver apenas 10.000 MAI em circulação, a venda corresponde a 10%
* Se alguém vender 1.000 MAI enquanto houver 10.000.000 MAI em circulação, a venda corresponde a 0,01%

Portanto, o teto da dívida não é aumentado de forma incremental, mas exponencial: quanto mais MAI em circulação, menos impacto teria uma grande venda, de modo que o teto da dívida pode ser aumentado muito mais.

{% hint style="info" %}
Quando você toma emprestado MAI, pode acontecer que o valor máximo de MAI que você pode tomar emprestado seja limitado pelo teto da dívida, independentemente do valor atual de sua garantia e do valor atual de MAI que você já emprestou. Quando for esse o caso, você pode esperar até 48h antes de poder emprestar mais MAI.
{% endhint %}

### Entendendo a Taxa de Garantia para Dívida

CDR, ou _Colateral to Debt Ratio_, é a relação entre o valor dos ativos depositados em seu cofre em relação ao valor do MAI que você tomou emprestado.&#x20;

Por exemplo, se você depositou $200 em WETH para tomar emprestado $100 em MAI, seu CDR seria:

$$
CDR=\frac{ValorGarantia}{ValorDívida}=\frac{200}{100}=200\%
$$

Manter uma CDR acima de 100% significa que, a qualquer momento, há mais garantia do que dívidas. Isso é obrigatório para garantir que a stablecoin MAI seja supercolateralizada e é uma das bases da tokenomics do Mai Finance. Você pode obter mais detalhes na [documentação oficial da Mai Finance.](https://docs.mai.finance/stablecoin-economics)

Cada vault possuí uma CDR minima aceita, um limite abaixo do qual o vault é considerado em risco porque o valor emprestado pode não ser suportado por garantia suficiente. Neste ponto, qualquer pessoa pode liquidar o cofre, o que significa que uma parte da dívida é reembolsada pelo liquidante que pode obter uma parte da garantia depositada em pagamento. Mais uma vez, você pode encontrar mais detalhes sobre o processo de liquidação na documentação oficial.

Quando você tomar emprestado MAI com uma determinada garantia, você receberá algumas dicas sobre qual é o valor máximo de MAI que você pode tomar e qual seria o impacto no seu **nível de saúde** dependendo do valor emprestado, como você pode ver na captura de tela abaixo:

![ Nível de saúde dependente do valor de empréstimo](<../.gitbook/assets/image (4).png>)

É muito importante ficar de olho na sua CDR e manter uma proporção saudável para:

* prevenir liquidação
* aumentar a saúde de toda a plataforma Mai Finance, garantindo que o volume MAI em circulação seja devidamente suportado

O CDR “saudável”, conforme definido pela equipe da Mai Finance, está entre 25% e 270% acima do valor mínimo do CDR. Como observação, você também pode verificar nossos guias de estratégia para ver como você pode usar CDRs conservadores/agressivos para [investir ](../tutoriais/polygon/leverage-aave-tokens.md#examples-with-numbers)em outros projetos, ou [pagar sua dívida](../debt-management-tutorials/debt-repayment-how.md#repayment-using-your-collateral) usando sua dívida.

## Incentivos de Vaults

### Entendendo os APRs dos Incentivos de Vaults

Em setembro de 2021, a Mai Finance introduziu incentivos de vault. Esta é uma recompensa atribuída pela plataforma Mai Finance a qualquer pessoa que tome emprestado MAI e participe do crescimento da plataforma.&#x20;

Cada tipo de Vault (entre os 10 tipos diferentes) recebe 0,05 Qi por bloco, que é então distribuído entre todos os usuários que possuem uma Taxa de Garantia para Dívida saudável. O APR do cofre é definido pela quantidade de MAI emprestado.

Como exemplo, Ben e Kila são 2 amigos que depositaram seus ETH nos cofres do WETH na Mai Finance.

* Ben depositou o equivalente a $2.000 em ETH e tomou emprestado 1.000 MAI
* Kila depositou o equivalente a $10.000 em ETH e tomou emprestado 6.000 MAI

O valor atual de MAI emprestado a usuários que depositaram WETH no cofre é de 1.000.000 MAI.

Tanto Ben quanto Kila se qualificam para os incentivos do vault porque Ben tem um CDR de 200% e Kila um CDR de 166,67%. Ben, com seu empréstimo, possui 0,1% do valor total emprestado, enquanto Kila possui 0,6%.

A quantidade total de Qi alocada para o cofre WETH (ou qualquer cofre) é

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86.400 é o número de segundos em um dia e, na Polygon, o tempo de blocos é de 2 segundos, o que significa que o número esperado de blocos todos os dias é 86.400 / 2 = 43.200. Assim, a emissão para cada Vault é de 2.160 Qi/dia.

**Observação:** O tempo de blocos aumentou e está, atualmente, em torno de 2,6 segundos. No entanto, todos os APRs e APYs exibidos em todos os aplicativos assumem um tempo de blocos de 2 segundos. Por favor, faça sua própria pesquisa e verifique o [tempo de blocos na PolygonScan.](https://polygonscan.com/chart/blocktime)
{% endhint %}

Portanto, se o estado do Vault permanecer o mesmo, Ben receberá 0,1% dos 2.160 Qi distribuídos, enquanto Kila receberá 0,6% da recompensa concedida.

* Ben receberá 2,16 Qi todos os dias, que é uma recompensa diária de 0,216%, ou um APR de 78,84%
* Kila receberá 12,96 Qi todos os dias, que é uma recompensa diária de 0,216%, ou um APR de 78,84%

Como observação, 2.160 Qi por 1.000.000 MAI é uma recompensa diária de 0,216%, ou 78,84%, que é o APR do Vault.

{% hint style="info" %}
É fácil perceber que o APR do Vault está diretamente ligado ao valor do MAI emprestado. Quanto mais MAI tomarmos emprestado, menor será o APR. Além disso, o montante de MAI que pode ser emprestado também é limitado pelo teto da dívida, que é aumentado com a demanda por MAI.
{% endhint %}

Como verificação, podemos calcular o APR teórico para o vault MATIC com base em números publicados na [pagina de análise](https://app.mai.finance/analytics) da Mai Finance. A quantidade de MAI emprestada do cofre MATIC é de 799.328. A recompensa é de 216 Qi por dia para esse vault. Que corresponde a um APR de

$$
APR=\frac{RecompensaQi*Qi_{Preço}}{MAI_{emprestado}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

Isso corresponde mais ou menos ao APR do Vault MATIC, conforme exibido na captura de tela a seguir:

![APR do Vault MATIC na Mai Finance após o lançamento das Recompensas de Vault](<../.gitbook/assets/image (23) (2) (3) (4).png>)

###

### Calculating starting vaults' APRs

With the same data as the example above, it's possible to calculate the starting APRs for all vaults

| Vault type | Starting APR |
| ---------- | ------------ |
| MATIC      | 44.29%       |
| WETH       | 24.03%       |
| LINK       | 27.41%       |
| AAVE       | 164.14%      |
| CRV        | 159.96%      |
| WBTC       | 36.92%       |
| camWETH    | 25.46%       |
| camWMATIC  | 44.33%       |
| camAAVE    | 167.23%      |
| camWBTC    | 47.38%       |

{% hint style="info" %}
As you can see, some vaults will generate more rewards than others. Also, you can see that it's super important to deposit your assets as soon as possible to benefit from high APRs before the debt ceiling is increased and more loan is taken (lowering the APR).

You can also see that if you keep your loan for one year of more, the 0.5% repayment fee will easily be compensated by the reward program.
{% endhint %}

### Incentives distribution

Rewards allocated by the vault incentives will be distributed the same way as for staked Qi. Every Wednesday, the Qi allocated by the Vaults incentives program will be airdropped / claimed for the week prior to the pay day.

## Vaults incentives FAQs

If you want to know more about the way Vault incentives are working, here's an official FAQ from the Discord server.

* **What vaults are receiving rewards?**

Right now all the vault types have been allocated Qi rewards

* **How much rewards are given out for the borrowing incentives?**

0.05 Qi/block for each vault type

*   **How much MAI do I need to borrow to earn rewards?**

    For Vault Borrow Incentives, stay between 25% and 270% above the liquidation ratio to receive QI token airdrop. This means:
* _Matic_ - Liquidation ratio 150% - Eligible for Incentives between 175% and 420%
* _Tokens_: - Liquidation ratio 130% - Eligible for Incentives between 155% and 400%
* _CamTokens_: - Liquidation ratio 135% - Eligible for Incentives between 160% and 405%
*   **How can I see if my vault is earning rewards?**

    If you see the fire emoji on your vault overview page that means that vault is earning rewards
* **How much will I earn?**

Your percent of the reward pool is based on the percentage of MAI you borrowed compared to the total amount of MAI borrowed from that vault type.

* **How long will the incentives program last?**

The scheduled length of the borrowing incentives program is to last 3 months. The DAO can vote to stop incentives before the 3 months is over or vote to extend the program.

* **How will we receive rewards?**

Qi will be airdropped to eligible vault holders.

* **How is eligibility for rewards gathered?**

Eligibility for rewards is calculated per block. You will earn rewards for the blocks you were eligible during the week.

* **When do tracking rewards for the week start?**

We will follow the same schedule as eQi. You can find the block numbers on the boost page.

## Disclaimer

This guide has been written **prior** to the launch of Vault incentives, meaning that the APRs promoted in this document (as well as this document) are subject to modifications, and/or may not be accurate. The amount of MAI borrowed, the debt ceiling and the value of the Qi token will highly impact the final APR of each vault type. Please, make sure that you invest responsibly.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
