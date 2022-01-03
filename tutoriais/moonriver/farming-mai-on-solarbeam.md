---
description: >-
  Solarbeam tem uma farming pool de MAI-MOVR com um excelente APR. Hoje, veremos
  como podemos tomar vantagem disto.
---

# Farming de MAI na SolarBeam

A maioria dos tutoriais apresentados neste guia usa stablecoins ​​como posição inicial. Isso se deve principalmente ao fato de que pares de moedas estáveis ​​não são afetados por perdas impermanentes nem pela volatilidade de outros ativos. Então, é quase impossível perder seu investimento inicial, e você pode usar estratégias mais arriscadas com os ganhos de suas stablecoins para aumentar seus ganhos.

Hoje, tentaremos outra abordagem na Moonriver com a Solarbeam, atualmente o único aplicativo que usa MAI. O par LP (**L**iquidity **P**roviding, Provedor de Liquidez) é MAI-MOVR. MAI é a moeda estável da Mai Finance com que você também poderá fazer ponte para a Moonriver ou cunhar de um cofre, e MOVR é o token de gás nativo do Moonriver. Como tal, o MOVR sempre terá algum tipo de utilidade e nunca deve cair em preço muito drasticamente. Este não é um par estável, mas a única parte variável do token está vinculada ao MOVR, o que o torna um bom ponto de partida de qualquer maneira.

Vamos ver como podemos gerar rendimentos muito altos com um loop de feedback fechado na Moonriver sem despejar muitos tokens de farming em movimento.

![](../../.gitbook/assets/solarbeam-1.png)

## SolarBeam

### Farming de MAI na Solarbeam

Solarbeam é a primeiro e principal DEX (**D**ecentralized **EX**change) e AMM (**A**utomatic **M**arket **M**aker) na Moonriver, e o segundo aplicativo em termos de TVL na rede. É também o primeiro parceiro Moonriver da Mai Finance e oferece uma pool MAI-MOVR que é recompensada com alguns de seus tokens nativos, o token SOLAR. Este também é o lugar onde você encontrará alguma liquidez para MAI.

![Pool MAI-MOVR na Solarbeam, Dezembro de 2021](../../.gitbook/assets/solarbeam-2.png)

O APR (**A**nnual **P**ercentage **R**ate, Taxa de Percentual Anual) de 84% é bastante alto devido ao baixo uso da pool, o que faz disso um ponto de início perfeito para a nossa estratégia. Você obterá este APR (corresponente a um APY de 131% se você quiser comparar com algo como MAI-WMATIC na QuickSwap como referencia) e a recompensa será paga em tokens SOLAR. Em dezembro de 2021, 1 SOLAR = 3.78 USDC.

### Staking de SOLAR

A maioria dos forks da Uniswap estão propondo staking para o seu token nativo, e a Solarbeam também está fazendo isto. Você pode fazer staking com o seu SOLAR no Vault para receber mais SOLAR, e dependendo da extensão do seu bloqueio, você obterá taxas muito interessantes (até 200% de APR por uma trava de 30 dias), mas nós faremos staking parece receber tokens externos. De fato, você pode fazer staking com seus tokens SOLAR para receber um monte de outros tokens de diferentes apps na Moonrier, e aquele que nós estamos procurando é o token ROME.

![Staking de token SOLAR para receber tokens ROME na Solarbeam](../../.gitbook/assets/solarbeam-3.png)

Você irá notar que a pool ROME é aquela com o menor APR, mas mesmo assim ainda é bem alto, e vocé logo verá que nossos tokens ROME irão multiplicar a uma taxa insana.

## Rome DAO

Rome DAO is another big player on Moonriver. It's an Ohm-fork (Olympus DAO copy) that uses the ROME token as native token. You will be able to stake your ROME tokens on the application in order to get very high returns. The goal of each Ohm-fork is to have as much native token staked and attract liquidity to be able to sustain the emission. If you need more details on Ohm-forks, please check our [tutorials on Klima DAO](../polygon/ohm-forks-on-polygon-the-case-of-klima.md) for Polygon.

![Staking ROME tokens on Rome DAO for 771% APR as of December 2021](../../.gitbook/assets/solarbeam-4.png)

Because we'll get ROME tokens from Solarbeam, we should be able to stake them on Rome DAO and the rebase system will get you a lot more very quickly. For this strategy, we will stake ROME tokens on Rome DAO and sell 50% of the daily reward, which is currently corresponding to \~1% of the deposit on Rome DAO.

## Mai Finance

Mai Finance is a lending platform where you'll be able to deposit your crypto assets and borrow the MAI stable coin at 0% interest. The only fee that will ever be charged on Moonriver is the repayment fee of 0.5% of your loan.

![ETH vault on Moonriver with a lot of MAI available](../../.gitbook/assets/solarbeam-5.png)

For our strategy, we will be using a ETH vault. The ROME token that will be extracted from the Rome DAO staking pool will be split as follows:

* 33% will be swapped to MOVR using the swap feature on Solarbeam
* 66% will be swapped to ETH using the swap feature on Solarbeam

You will then be able to deposit the ETH on Mai Finance to borrow MAI with a CDR (**C**ollateral to **D**ebt **R**atio) of 200% to stay in the safe zone and try to prevent liquidation. The MAI borrowed will then be used to create additional MAI-MOVR LP tokens that will then be added to the initial position on Solarbeam.

As an example, for each $1 of ROME that you extract from Rome DAO we will get

* $0.33 of MOVR
* $0.66 of ETH deposited on Mai Finance
* $0.33 of MAI borrowed against our ETH
* $0.66 worth of MAI-MOVR LP token to add to Solarbeam

## Farming Strategy

The following simulation is made by assuming a few different things:

* All rates and prices remain the same for the entire period of the simulation, 1 year in our case
  * 84% APR on MAI-MOVR farming on Solarbeam
  * 108% APR on staking SOLAR to farm ROME tokens
  * 771% APR on Rome DAO when staking ROME tokens
* All rewards and programs are also running for an entire year
* 50% of the daiy gains on Rome DAO is sold for 33% MOVR and 66% ETH
* The initial investment is $100 worth of MAI-MOVR LP token

![](../../.gitbook/assets/solarbeam-6.png)

### Day 1

On day 1, you would simply deposit your $100 worth of MAI-MOVR on Solarbeam and will harvest your SOLAR tokens at the end of the day. This would give you the following result:

| MAI-MOVR | SOLAR | ROME  | ETH   | Additional LP |
| -------- | ----- | ----- | ----- | ------------- |
| 100.000  | 0.230 | 0.000 | 0.000 | 0.000         |

### Day 2

On day 2, you'd keep your MAI-MOVR position to farm more SOLAR, but you will also stake your first harvest of SOLAR token in order to start collecting some ROME tokens. At the end of day 2, you would get:

| MAI-MOVR | SOLAR | ROME  | ETH   | Additional LP |
| -------- | ----- | ----- | ----- | ------------- |
| 100.000  | 0.460 | 0.001 | 0.000 | 0.000         |

### Day 3

At the beginning of day 3, you should be able to harvest your first few ROME tokens from the 50% daily staking reward. It's probably not a good idea to do it on day 3 with only an initial of $100 because the amount is quite unsignificant, but still. You will sell 33% for MOVR and 66% for ETH that you will deposit your vault on Mai Finance, then borrow MAI against your new collateral.

| MAI-MOVR | SOLAR | ROME  | ETH      | Additional LP |
| -------- | ----- | ----- | -------- | ------------- |
| 100.000  | 0.690 | 0.002 | 0.000005 | 0.000005      |

At this point the system is fully bootstrapped.

## Farming results

### Daily routine

Once the system is fully prepared, here's your daily routine

* harvest SOLAR from the MAI-MOVR pool
* stake the SOLAR tokens you just earned
* harvest the ROME tokens from the SOLAR staking pool
* stake your freshly acquired ROME tokens
* unstake 50% of your daily gains on Rome DAO (corresponds to \~1.5 rebase)
* sell 66% of your ROME tokens for ETH
* sell 33% of your ROME tokens for MOVR
* deposit ETH in the ETH vault on Mai Finance
* borrow 50% of your deposit as MAI stable coin
* pair the borrowed MAI with the MOVR tokens
* deposit your additional MAI-MOVR tokens

### Raw results month after month

| day | MAI-MOVR | staked SOLAR | staked ROME | ETH     |
| --- | -------- | ------------ | ----------- | ------- |
| 30  | 100.021  | 7.135        | 0.352       | 0.023   |
| 60  | 100.190  | 14.045       | 1.550       | 0.200   |
| 90  | 100.713  | 20.978       | 3.911       | 0.740   |
| 120 | 101.872  | 27.968       | 7.869       | 1.925   |
| 150 | 104.052  | 35.072       | 14.023      | 4.148   |
| 180 | 107.788  | 42.378       | 23.204      | 7.947   |
| 210 | 113.814  | 50.019       | 36.559      | 14.065  |
| 240 | 123.142  | 58.178       | 55.580      | 23.525  |
| 270 | 137.175  | 67.158       | 82.767      | 37.745  |
| 300 | 157.848  | 77.321       | 120.875     | 58.681  |
| 330 | 187.841  | 89.226       | 174.234     | 89.041  |
| 360 | 230.861  | 103.358      | 248.711     | 132.575 |

### Day 365

After a complete year of farming, you would have

* $239.633 worth of MAI-MOVR on Solarbeam
* $106.358 worth of SOLAR tokens on Solarbeam
* $263.708 worth of ROME tokens staked on Rome DAO
* $141.450 worth of ETH on Mai Finance
* $68.817 worth of MAI debt on Mai Finance

The additional MAI-MOVR doesn't fully correspond to the debt since we're using a third of the swapped ROME tokens to get half of the new LP tokens.

This loop would thus give you an equivalent APY of 583.15% from a relatively stable initial position.

## Disclaimer

The main things to understand from this strategy are that Moonriver is currently under-used and reward rates are very interesting. Also, as soon as you throw a Ohm-fork in your strategy to re-invest a portion of your gains, the reward rates are so insane that you will make a very important profit as long as you keep enough tokens in the DAO to generate staking rewards.

Keep in mind though that projects will have variable reward rates that will not be guaranteed over the span of one year. Please make sure you understand all the project you're investing in, do your own research and make sure to invest only what you may be ready to loose. Because this strategy is investing on a relatively stable initial, the only thing that is at risk in here are the benefits from other systems. This guide cannot be taken as an endorsement of the projects it uses.
