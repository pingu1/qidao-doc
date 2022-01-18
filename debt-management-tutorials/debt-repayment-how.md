---
description: >-
  Esta página mostrará opções para pagar sua dívida na Mai Finance. Lembre-se de
  que o pagamento da dívida não é obrigatório, desde que você queira manter seu
  empréstimo e não precise de sua garantia.
---

# Reembolso de Dívida - Como?

O mercado está em alta e sua criptomoeda, trancada no Vault, está ganhando cada vez mais valor, tanto que você decidiu vendê-la. No entanto, como está no Vault na Mai Finance, você não pode desbloqueá-lo totalmente, a menos que pague seu empréstimo.

O mercado está em baixa e sua criptomoeda está perdendo valor muito rapidamente. Você não gera rendimento rápido o suficiente para cobrir os danos e manter um índice de garantia para dívida (CDR) saudável, e a liquidação está próxima. É hora de pagar sua dívida para garantir que você não esteja perdendo muito e evitar a liquidação.

Se você não estiver em nenhuma das situações acima, provavelmente não vale a pena pagar sua dívida. Por favor, veja o capítulo sobre [Reembolso de Dívida](debt-repayment-why-and-when.md) para mais detalhes.

## Reembolso parcial ou total usando dinheiro

A maneira mais fácil de pagar sua dívida é usar alguma moeda fiduciária, especialmente se você quiser manter suas garantias e outros investimentos intocados.

A Mai Finance está em parceria com a [Transak](https://transak.com)  para conectar facilmente o dinheiro comprado por Cartões de Crédito/Débito, ou transferências bancárias, diretamente para a rede Polygon. Simplesmente vá para Mai Finance e clique no ícone transak na barra de menu para abrir um modal que permitirá comprar alguns MATIC e enviá-los diretamente para sua carteira Polygon.

![Comprando um pouco de USDC usando dinheiro e enviando diretamente para a Polygon.](../.gitbook/assets/screen-shot-2021-08-18-at-9.43.07-am.png)

O principal problema é o tempo necessário para processar a transação. No entanto, isso permitirá que você troque USDC por MAI e, em seguida, pague parcial ou totalmente sua dívida.

## Reembolso usando os benefícios do seu empréstimo

### Reembolso Parcial

A maioria das pessoas vai querer emprestar MAI na Mai Finance para investir em projetos específicos. Investidores em farming que estão usando MAI provavelmente terão sucesso gerando recursos adicionais e não perderão dinheiro em degen farms, ou assim esperamos. Se você se encontra nesta situação, você tem 2 opções:

* reembolsar seu empréstimo com a receita gerada&#x20;
* reinvestir seus ganhos no mesmo (ou outro) projeto

Na maioria dos casos, provavelmente é melhor reinvestir seus ganhos. De fato, ao reacumular suas recompensas, o APR (**A**nnual **P**ercentage **R**evenue, ou Receita Percentual Anual) é aplicado em um valor maior, o que, por sua vez, gera mais receita. Consulte os nossos guias de investimento para obter ideias sobre como pode maximizar os seus investimentos.

No entanto, algumas pessoas simplesmente não gostam da ideia de ter uma dívida e vão querer pagá-la o mais rápido possível. Se for esse o seu caso, você pode simplesmente trocar seus ganhos em MAI e pagar sua dívida.

* Abra as informações do seu cofre.
* Selecione a opção `Manage.`
* Selecione a guia `Repay` na parte inferior do seu Vault.
* Insira o valor que você deseja reembolsar.
* Clique em `Repay MAI` e está tudo pronto.

![Reembolsando parcialmente uma parte da minha dívida.](../.gitbook/assets/screen-shot-2021-08-17-at-1.02.23-pm.png)

Como exemplo:

* Você tem $1.000,00 em camWMATIC em seu vault, com uma dívida de $400,00&#x20;
* Você trocou $10,00 em tokens ADDY por MAI&#x20;
* Você paga $10,00 hoje
  * Sua dívida agora é de $390,00
  * O valor do seu camWMATIC é de $999,95 (você adiciona para pagar 0,5% de $10,00 em taxas de reembolso)

Em algum momento, você poderá pagar totalmente sua dívida usando essa técnica, desde que possa gerar receita suficiente por meio de seu empréstimo.

Essa estratégia é eficiente? Na verdade, não. Reembolsar sua dívida dessa maneira não muda nada, exceto sua CDR. De fato, sua garantia permanece parcialmente bloqueada até que você pague totalmente sua dívida, e se você estiver usando amTokens como garantia, ter uma dívida ou não não mudará o fato de que sua garantia está gerando rendimento. A única vantagem é que você pode retirar uma parte de sua garantia e reutilizá-la em outro lugar / vendê-la.

### Reembolso Total

Outra abordagem, muito semelhante à estratégia acima, é pagar tudo de uma vez. No exemplo acima, em vez de pagar $10,00 a cada poucos dias, eu poderia compor os $10,00 ganhos em meu investimento para gerar rendimento mais rapidamente. Também posso investir esses ganhos em outro projeto que também geraria receita. Assim que receber o equivalente a $400,00 que corresponde ao meu empréstimo, posso pagar tudo de uma vez.

## Reembolso usando sua garantia

### Idéia principal

Na Mai Finance, você pode emprestar moedas estáveis MAI depositando uma certa quantia de garantia em um vault. A relação garantia/dívida precisa estar sempre acima de um certo limite, 150% para a maioria dos vaults. Isso significa que, para uma CDR de 150%, para qualquer garantia de $100, você só pode emprestar $66,6667 de MAI.

No entanto, isso o colocaria diretamente em uma posição de liquidação. Isso significa que a saúde do seu cofre é considerada muito arriscada e qualquer pessoa pode pagar uma parte de sua dívida usando seus fundos e ser pago de volta obtendo uma parte de sua garantia. Para mais detalhes sobre liquidação, leia a[ documentação oficial.](https://docs.mai.finance/liquidation)

Geralmente é considerada uma boa prática manter um alto índice de garantia/dívida para evitar liquidação, mas mesmo com uma CDR próximo a 150%, é fácil perceber que o valor da garantia é SEMPRE maior que o valor da dívida. Isso significa que você pode, em teoria, pagar sua dívida vendendo alguns de seus ativos colaterais.

### Como usar garantia

Vamos considerar um vault com $1.000,00 em MATIC e uma dívida de $500,00. O CDR é de 200%. O CDR mínimo é de 150%. Neste exemplo, queremos pagar a dívida por completo, mas queremos evitar a liquidação, e evitaremos possuir uma CDR abaixo de 160% ao sacar nossa garantia. Usaremos as seguintes fórmulas:

$$
CDR=\frac{Garantia}{Dívida}
$$

$$
GarantiaDisponível = GarantiaInicial - CDRAlvo*Dívida
$$

Nesta situação, se quisermos manter uma CDR de 160%, o valor da garantia que podemos retirar "com segurança" é de:

$$
GarantiaDisponível=$1000-1.60*$500=$200
$$

Portanto, teremos que proceder em várias etapas:

* Retirar $200 da garantia
  * o vault agora tem $800 em MATIC e $500 em dívidas, e a CDR é de 160%
* Vender os $200 em garantia para comprar MAI
* Reembolsar $200 da dívida com uma taxa de reembolso de 0,5%
  * o vault agora tem $799 em MATIC e $300 em dívidas, e a CDR é de 266,33%
* Calcule o novo valor de garantia que podemos retirar: $319
* Retirar $319 da garantia
  * o vault agora tem $480 de MATIC e $300 em dívidas, e a CDR é de 160%
* Vender os $319 em garantia para comprar MAI
* Reembolsar $300 da dívida com uma taxa de reembolso de 0,5%
  * o vault tem $478,50 de MATIC e $0 de dívida, e você ainda tem $19 de MAI

Você pode ver que manter uma CDR saudável pode te ajudar a pagar sua dívida com um número muito pequeno de loops. Obviamente, se o seu CDR estiver mais próximo do limite de 150%, você pode ter que operar mais loops, pois não pode sacar tanto de uma só vez.

{% hint style="info" %}
Uma CDR de 260% é suficiente para poder sacar o valor total de sua dívida e permanecer acima de 160%. Dessa forma, você só precisa de um loop para pagar totalmente sua dívida.
{% endhint %}

Observe que o pagamento total de sua dívida com a venda de sua garantia nunca é necessário se você não precisar vender seus ativos subjacentes ou modificar sua CDR para impedir que seu cofre seja liquidado.

## Reembolso usando um robô

Este parágrafo é pura teoria e está disponível apenas para programadores avançados. A ideia é usar empréstimos relâmpago que o ajudarão a pagar sua dívida e desbloquear a garantia para que ela possa ser paga. Empréstimos relâmpago são uma opção proposta por alguns aplicativos em diferentes redes, incluindo a Polygon, que permitem tomar emprestado fundos e pagar o empréstimo no mesmo bloco de transação. Se o empréstimo não puder ser totalmente reembolsado no mesmo bloco, a transação é simplesmente revertida. No Polygon, a AAVE está propondo empréstimos relâmpago.

Se tomarmos o exemplo acima com $1.000,00 em MATIC e uma dívida de$ 500,00, o fluxo seria o seguinte:

* Emprestar $ 600,00 de USDC no AAVE em um empréstimo relâmpago&#x20;
* Troque o USDC por MAI&#x20;
* Pague sua dívida completamente&#x20;
* Retire sua garantia MATIC&#x20;
* Venda seu MATIC por USDC&#x20;
* Reembolsar o empréstimo relâmpago da AAVE

Quando submetida, esta lista de transações acontecerá todas no mesmo bloco, e você terminará com o que sobrar do seu MATIC como USDC em sua carteira (mais ou menos $500,00, com algumas pequenas variações devido à taxa de juros do empréstimo relampâgo, taxas de troca e taxas de reembolso).

No momento, você teria que interagir diretamente com os contratos inteligentes, o que requer uma boa compreensão de como eles funcionam. Se precisar de ajuda, você pode acessar nosso servidor Discord, que possuí um canal dedicaco a programação. Talvez em um futuro próximo, FuruCombo proporá tijolos Mai Finance que permitiriam operar isso diretamente usando sua ferramenta gráfica, mas por enquanto não é possível. Por fim, a ideia de um botão para “pagar dívidas usando garantias” foi proposta à equipe de desenvolvedores da Mai Finance, e a opção poderá ser implementada no futuro.

## Short term VS Long term Debt Repayments

Depending on your strategy and the way you feel regarding your debt, it may be a good idea to compare different lending platforms. However, keep in mind that Mai Finance with its 0% interest and 0.5% repayment fee is one of the top product on the Polygon market. The real competitor is AAVE, but only if you want to borrow MAI or USDC for a short period of time.

* Mais is 0% interest + 0.5% repayment fee
* AAVE has no repayment fees, but a variable APR for interests you need to pay back

![Supplying and Borrowing APY on AAVE as of August 2021](../.gitbook/assets/screen-shot-2021-08-18-at-6.52.08-am.png)

As an example for USDC, you can see that the borrowing rate is 3.79% with a current reward of 2.08% paid back in MATIC. This gives, at the moment of writing, the equivalent of 1.71% you need to pay back if you keep your loan for a complete year. With AAVE, since you can repay your debt very quickly, the variable APY is equivalent to 0.005% daily. Hence, it would take 100 days (a bit more than 3 months) to reach 0.5% of your debt.

If you plan to keep your loan longer than that, it's definitely better to use Mai Finance. Also, it's important to understand that AAVE borrowing APRs are variable, they will fluctuate with the amounts that are deposited and required (the more people want to borrow from AAVE, the higher the borrowing APR). Keep also in mind that the MATIC reward program will end at some point, and the 1.71% interest will soon become a 3.79% interest rate. At least with Mai Finance, you don't have to keep a close eye on your loan to see when it becomes dangerous to keep it.

Finally, the team of Mai Finance is working on Vaults incentives that would work the same way as the MATIC reward, meaning that you would still get a 0% interest loan and a bonus paid in Qi that may very well reduce the repayment fee to 0% of your debt. And the longer you keep your loan, the more reward you will collect, making it a true negative interest loan.

## Disclaimer

The views, thoughts, and opinions expressed in the text belong solely to the author, and not necessarily to the rest of the community, nor the development team behind Mai Finance. It should not be taken as a financial advice or guidance of any kind.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
