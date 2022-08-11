---
description: Usando MAI na Moonbeam para gerar rendimentos com a StellaSwap.
---

# Brincando de LEGO na StellaSwap

Embora a Mai Finance não ofereça vaults (cofres) na Moonbeam, é possível usar alguns de seus tokens favoritos na rede para cunhar MAI usando os novos vaults MAI da StellaSwap. Ao alavancar seus tokens de garantia e tomar emprestado MAI, você pode obter um ótimo rendimento por meio de uma estratégia de loop envolvendo xSTELLA e MAI.

_NOTA: Este guia não pretende ser um conselho financeiro. Foi criado com um objetivo educacional em mente. O objetivo deste guia não é propor uma estratégia a ser seguida às cegas, portanto, faça sua lição de casa e sua própria simulação, e invista apenas o que estiver disposto a perder._

[StellaSwap](https://stellaswap.com/) é a principal DEX (Corretora Descentralizada) na Moonbeam. Como uma DEX completa, a StellaSwap oferece aos usuários a capacidade de trocar tokens, obter rendimento em farms e participar da governança de protocolos. O que diferencia a StellaSwap é que é o primeiro protocolo desse tipo que permite aos usuários cunhar MAI nativamente diretamente de sua interface por meio de uma parceria com a Mai Finance.

![Cunhando MAI diretamente da StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### Cunhando MAI na StellaSwap

Ao contrário dos cofres MAI na Mai Finance, os cofres MAI da StellaSwap cobram juros pelo empréstimo contra seus ativos. Atualmente, os usuários podem tomar emprestado MAI contra xStella, o token de compartilhamento de receita da StellaSwap, com juros de 12%, ou contra wGLMR, uma versão embrulhada do token de gas nativo da Moonbeam, com juros de 8%. Embora os usuários familiarizados com os cofres de juros de 0% da Mai Finance possam ficar surpresos com as taxas de juros mais altas, passaremos por uma estratégia de loop neste guia para permitir que você obtenha altos rendimentos em suas stablecoins emprestadas sem nunca sair da StellaSwap.

![Cofres na StellSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. Primeiro, dirija-se às instalações[ de cunhagem de MAI na StellaSwap](https://app.stellaswap.com/mai).
2. A partir daqui, você poderá criar um cofre xStella ou wGLMR para usar o MAI emprestado. Para criar nossa estratégia de looping, criaremos um cofre xStella.
3. Agora entre no seu cofre recém-criado e deposite xStella. Observe que os cofres xStella têm um LTV de 40% (relação empréstimo/valor), o que significa que para cada $100 em xStella, você poderá tomar emprestado $40 em MAI.
4. Em seguida, você deve ir para a seção de empréstimo e pedir emprestado o MAI. Por favor, tenha em mente o seu LTV para evitar ser liquidado.

![Cofre xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### Montando as peças do LEGO

Agora que você tomou emprestado o MAI com sucesso, é hora de colocá-lo em uso! Aproveitaremos nosso MAI depositando-o no farm de stablecoins MAI-Base4Pool da StellaSwap e usando os rendimentos para ganhar mais tokens Stella fazendo staking com eles. Lembre-se sempre de que, se você entrar nessa estratégia, o fará por sua conta e risco e seu cofre poderá ser liquidado se você não fizer a devida diligência!\
\
Vamos primeiro encontrar a MAI-Base4Pool na página de [Farms](https://app.stellaswap.com/farm) da StellaSwap.

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Atualmente, esta farm oferece um rendimento muito atraente de 26% em stablecoins com um pool composto por MAI, FRAX, USDT, USDC e DAI com um rendimento pago em tokens Stella. Observe que esse rendimento compensa principalmente os juros que estamos pagando atualmente em nosso MAI emprestado (12%). Podemos dar uma olhada no nosso desempenho até agora:

$$juros efetivos = (garantia * jurosempréstimo)-(mai*rendimentofarming)$$

Isso nos dá um rendimento efetivo de 1,6% para tomar emprestado MAI - não é ruim, mas podemos fazer melhor. Agora podemos pegar os tokens Stella que estamos ganhando por estar no MAI-Base4Pool e realizar [staking para receber xStella](https://app.stellaswap.com/xstella).

![Staking de xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

Fazer staking de xStella traz dois benefícios adicionais. Primeiro, ele fornece um APR de staking de 70%, aumentando assim nossos rendimentos, mas, mais importante, o xStella aumenta de valor ao longo do tempo, à medida que a receita de swap do protocolo é compartilhada entre os usuários. Isso significa que quaisquer rendimentos que estamos ganhando com nossa posição relativamente segura em uma fazenda de stablecoins estão aumentando continuamente. Podemos então usar esses rendimentos adicionais e depositar xStella adicionais em nosso cofre para aumentar nosso LTV ou para tomar emprestado mais MAI contra ele.

## Aviso legal

Este guia NÃO é um conselho financeiro e deve ser simplesmente considerado uma ferramenta educacional. Sempre faça sua própria pesquisa. A discussão de um projeto neste guia não deve ser considerada como um endosso do projeto.

{% hint style="info" %}
Tenha em mente que uma estratégia que funciona bem em um determinado momento pode ter um desempenho ruim (ou fazer você perder dinheiro) em outro momento. Por favor, mantenha-se informado, monitore os mercados, fique de olho em seus investimentos e, como sempre, faça sua própria pesquisa.
{% endhint %}
