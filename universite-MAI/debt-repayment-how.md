---
description: >-
  Cette page présente différentes options pour rembouser votre dette sur Mai
  Finance. Gardez à l'esprit que rembourser sa dette n'est jamais obligatoire.
---

# Rembourser sa dette - Comment?

Le marché est à la hausse et votre crypto, dans un coffre, gagne de plus en plus de valeur, tellement que vous décidez de la vendre. Cependant, puisque votre crypto se trouve dans un coffre sur Mai Finance, vous ne pouvez pas la récupérer entièrement, à moins de rembourser votre dette.

Le marché est à la baisse et votre crypto perd rapidement en valeur. Vos revenus ne sont pas suffisants pour compenser les dégâts et garder un ratio Collatéral/Dette (CDR, Collateral to Debt Ratio) sain, et la liquidation est proche. Il est temps de rembourser votre dette pour limiter les pertes et éviter la liquidation.

Si vous n'êtes pas dans une de ces situations, il n'est probablement pas utile de rembourser votre dette. Pour plus de détails, vous pouvez regarder cet article [Rembourser sa dette - Pourquoi et quand?](debt-repayment-why-and-when.md)

## Remboursement, complet ou partiel, avec des fiats

La méthode de remboursement la plus directe est d'utiliser des fiats, particulièrement si vous ne voulez pas toucher vos collatéraux et autres investissements.

Mai Finance a un partenariat avec [Transak](https://transak.com) pour facilement acheter, avec des fiats, des cryptos sur le réseau Polygon. Pour ce faire, aller sur [Mai Finance](https://app.mai.finance) et cliquez sur le bouton "Buy" dans la barre de menus, en haut à droite. Une fenêtre va s'ouvrir, elle vous permet d'acheter du MATIC, ainsi que d'autres cryptos, et les envoyer directement sur votre adresse Polygon.

![Achat d'USDC avec de l'euro et envois vers Polygon.](../.gitbook/assets/screen-shot-2021-08-18-at-9.43.07-am.png)

Le problème principal de cette méthode est le temps pour traiter la transaction. Cependant, cela vous permet d'échanger votre USDC pour du MAI et rembourser votre dette, entièrement ou partiellement.

## Rembourser en utilisant les bénéfices de votre prêt

### Remboursement Partiel

La plupart des gens vont emprunter du MAI sur Mai Finance pour investir dans d'autres projets. Les cultivateurs de revenus qui utilisent MAI seront surement ceux qui ont le plus de réussite pour générer des ressources supplémentaires, et, avec espoir, ne pas perdre d'argent dans des fermes dégénérées. Si vous êtes dans ce cas, vous avez 2 options

* rembourser votre prêt avec les revenus générés
* réinvestir vos gains (dans le même projet, ou un autre)

Dans la majorité des cas, il est probablement meilleur de réinvestir vos gains. En effet, en accumulant vos récompenses, l'APR (Annual Percentage Revenu) est appliqué sur un montant plus grand, ce qui génère plus de revenus. Allez jeter un oeil à nos guides d'investissement **pour vous faire une idée** de comment maximiser vos revenus.

Cependant, certaines personnes n'aiment pas l'idée d'avoir une dette et vont vouloir rembourser aussi vite que possible. Si c'est votre cas, vous pouvez simplement échanger vos gains pour du MAI et rembourser votre dette.

* Ouvrez les info de votre Vault
* Cliquez sur `Repay` en dessous de `Manage`
* Entrez le montant que vous voulez rembourser.
* Cliquez sur `Repay Mai`

![Remboursement partiel de ma dette](../.gitbook/assets/screen-shot-2021-08-17-at-1.02.23-pm.png)

Comme exemple

* Vous avez $1,000.00 de camWMATIC dans votre coffre, avec une dette de $400.00
* Vous avez échangé $10.00 de jetons ADDY pour du MAI
* Vous remboursez $10.00 aujourd'hui
  * Votre dette est de $390.00
  * La valeur de votre camWMATIC est de $999.95 (0.5% de $10 ont été payé pour les frais de remboursement)

Au bout d'un moment, vous serez capable de rembourser entièrement avec cette technique, tant que vous générez suffisamment de revenus avec votre emprunt.

Est-ce que cette stratégie est efficace? Pas vraiment, rembourser votre dette de cette manière ne change rien à part votre CDR. En effet, votre collatéral reste partiellement bloqué tant que vous avez une dette, et si vous utilisez des jetons "cam" en collatéral, avoir une dette, ou non, ne change pas le fait que votre collatéral génère du revenu. Le seul avantage est de pouvoir, possiblement, retirer une partie de votre collatéral et vous servir ailleurs / le vendre.

### Remboursement Complet

Une autre approche, très similaire, est de rembourser tout d'un coup. Dans l'exemple au-dessus, au lieu de rembourser $10 tous les jours, je pourrais, à la place, réinvestir ces $10 pour générer des revenus plus vite. Je peux aussi les investir dans un autre projet qui génèrerait des revenus. Quand j'ai reçu l'équivalent de $400, qui correspondent à mon emprunt, je peux tout rembourser.

## Rembourser en utilisant votre collatéral

### Idée principale

Sur Mai Finance, vous pouvez emprunter du MAI en déposant un certain montant de collatéral dans un coffre. Le ratio de collatéral/dette doit toujours être au-dessus d'un certain pourcentage, 130-135 pour la plupart des coffres. Cela veut dire, pour un ratio de 150%, que pour chaque $100 de collatéral, vous pouvez emprunter au plus $66.66 de MAI.

Cependant, un coffre ayant son CDR inférieur ou égal à la limite va être en position de se faire liquider car il sera considéré comme trop risqué. Cette position signifie que n'importe qui peut rembourser 50% de votre dette, en utilisant ses fonds, et être payé pour avec une portion de votre collatéral (la valeur de la dette + 10%). [La documentation officielle](https://docs.mai.finance/liquidation) donne plus de détails. 

Garder un ratio élevé est une bonne pratique pour éviter la liquidation mais, même avec un ratio proche de 150%, il est facile de voir que la valeur du collatéral est **toujours** plus élevée que celle de la dette. Cela veut dire que vous pouvez, en théorie, rembourser votre dette en vendant une partie de votre collatéral.

### Comment utiliser un collatéral

Considérons un coffre avec $1000 de MATIC et $500 de dette. Le CDR est de 200%. Le minimum, pour ce collatéral, est 150%. Dans cet exemple, nous voulons rembourser notre dette entièrement en évitant la liquidation, donc nous nous fixons une limite de 160% CDR quand nous retirons notre collatéral. Nous utiliserons les formules suivantes:

$$
CDR=\frac{Collatéral}{Dette}
$$

$$
CollatéralDisponible = Collatéral Initial - MinCDR * Dette
$$

Nous devons procéder en plusieurs étapes:

* Retirer $200 de notre collatéral
  * Le coffre a maintenant $800 de MATIC et $500 de dette, le CDR vaut 160%
* Vendre les $200 de collatéral pour acheter du MAI
* Rembourser $200, avec 0.5% de frais.
  * Le coffre a maintenant $799 de MATIC et $300 de dette, le CDR vaut 266.33%
* Calculer le nouveau montant de collatéral que l'on peut retirer: $319
* Retirer $319 de notre collatéral
  * Le coffre a maintenant $480 of MATIC et $300 de dette, le CDR vaut 160%
* Vendre les $319 de collatéral pour acheter du MAI
* Rembourser $300, avec 0.5% de frais
  * Le coffre a maintenant $478.50 de MATIC et $0 de dette, et il vous reste $19 de MAI

Vous pouvez voir que garder un CDR sain peut grandement vous aider à rembourser votre dette en répétant peu de fois cette boucle. Évidemment, si votre CDR est plus proche de 150%, vous devrez répéter cette boucle un plus grand nombre de fois puisque vous pouvez retirer moins à chaque itération.

{% hint style="info" %}
Un CDR de 260% est assez pour pouvoir retirer entièrement la valeur de votre dette et rester au-dessus de 160%. De cette manière, vous n'avez qu'une itération de la boucle à faire pour rembourser votre dette.
{% endhint %}

Notez que rembourser entièrement votre dette en vendant votre collatéral n'est jamais nécessaire si vous n'avez pas besoin de vendre votre actif sous-jacent, ou modifier votre CDR pour éviter la liquidation.

## Rembourser en utilisant un robot

Ce paragraphe est purement théorique et présent seulement pour des développeurs avancés. L'idée est d'utiliser un emprunt flash (flashloans) pour rembourser votre dette, débloqué votre collatéral et s'en servir pour rembourser l'emprunt flash. Les emprunts flash sont un élément de certaines applications, sur différents réseaux, Polygon inclus, qui vous permettent de faire un prêt et le rembourser en l'espace d'une transaction. Si l'emprunt ne peut pas être remboursé entièrement, la transaction est inversée. Sur Polygon, [AAVE](https://docs.aave.com/developers/guides/flash-loans#step-by-step) propose cet élément. 

Si nous prenons l'exemple du dessus, $1000 de MATIC et $500 de dette. L'execution serait la suivante:

* Emprunt flash de $600.00 d'USDC sur AAVE
* Échanger l'USDC pour du MAI
* Rembourser votre dette
* Retirer votre collatéral (MATIC)
* Vendre du MATIC pour de l'USDC
* Rembourser l'emprunt flash sur AAVE

Une fois soumise, la liste de transactions sera dans le même bloc et vous aurez le MATIC restant sous forme d'USDC dans votre portefeuille (plus ou moins $500 avec de petites variations due aux frais du flash loan, échanges des jetons et remboursement).

Pour l'instant, il faut interagir directement avec des smart contracts, ce qui demande de bien comprendre comment ils fonctionnent. Si vous avez besoin d'aide, faites un tour dans `#programming` sur Discord. Dans le futur, il est possible que [FuruCombo](https://furucombo.app/combo) propose des briques Mai Finance ce qui permettrait d'utiliser leur interface graphique.

Finalement, l'idée d'un bouton "Rembourser en utilisant le collatéral" a été proposé à l'équipe de devs de Mai Finance, cela sera peut-être implémenter dans le futur.

## Remboursement de dette: court vs long terme

En fonction de votre stratégie et la manière dont vous vous sentez par rapport à votre dette, il pourrait être une bonne idée de comparer à d'autres plateformes de prêt. Cependant, garder à l'esprit que Mai Finance, avec ses intérêts à 0% et frais de remboursement à 0.5%, est l'un des meilleurs produit sur Polygon. Aave est un concurrent mais seulement si vous empruntez du MAI ou USDC pour une courte période. 

* Mai est 0% interêt + 0.5% frais de remboursement
* AAVE n'a pas de frais de remboursement mais une APR variable pour les intérêts que vous devez payer.

![APY de Dépot et Emprunt sur AAVE en Août 2021](../.gitbook/assets/screen-shot-2021-08-18-at-6.52.08-am.png)

Par exemple, avec de l'USDC, vous pouvez voir que le taux d'emprunt est de 3.79% avec une récompense de 2.08% payée en MATIC. Cela donne, à l'écriture, l'équivalent de 1.71% que vous devez rembourser pour garder votre emprunt pendant 1 an. Avec Aave, puisque vous pouvez rembourser votre dette très rapidement, l'APY variable est équivalente à 0.005% par jour. Par conséquent, il faut 100 jours, un peu plus de 3 mois, pour atteindre 0.5% de votre dette.

Si vous planifiez de garder votre emprunt plus longtemps, il est plus intéressant d'utiliser Mai Finance. Il est aussi important de comprendre que les APR d'Aave sont variables, elles vont fluctuer avec les montants qui sont déposés et empruntés (plus il y a d'emprunts sur Aave, plus les APR d'emprunt sont élevées). Garder aussi à l'esprit que le programme de récompense en MATIC a une date de fin et les 1.71% d'intérêt deviendront 3.79%.

Finalement, l'équipe de Mai Finance travaille sur l'implémentation de récompenses qui fonctionneraient comme les récompenses en MATIC d'Aave, ce qui signifie que vous aurez toujours 0% d'intérêt sur votre emprunt **et** vous serez payés (en Qi) ce qui pourrait bien réduire vos frais de remboursement à 0% de votre dette. Plus votre garder votre emprunt, plus vous collecterez des récompenses, faisant ainsi un véritable emprunt à intérêts négatifs.

{% hint style="info" %}
À la traduction de cet article (04/10/21), les récompenses sur les emprunts de Mai Finance sont actives, les APRs sont comprises entre 20% pour les collatéraux les plus utilisés/anciens et 820% (BAL) pour les moins utilisés/plus récents. Voir [MAI loans and Vault incentives](mai-loans-and-vault-incentives.md)
{% endhint %}

## Avertissements

Les vues, pensées, et avis exprimés ici appartiennent à l'auteur (et/ou traducteur), et ne reflètent pas nécessairement ni le reste de la communauté, ni l'équipe derrière Mai Finance. Cet article ne devrait pas être pris comme un conseil financier ou un guide.

{% hint style="info" %}
Gardez à l'esprit qu'une stratégie qui fonctionne bien à un moment donné peut moins bien fonctionner, voir vous faire perdre de l'argent, à un autre. Restez informé, surveillez les marchés et vos investissements, et, encore une fois, **faites vos recherches**.
{% endhint %}
