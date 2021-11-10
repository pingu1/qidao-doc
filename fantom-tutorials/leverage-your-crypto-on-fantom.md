---
Açıklama: >-
  Bu kılavuz, Yearn kasaları ve Beefy kasaları kullanılarak Fantom'da Mai Finance tarafından önerilen farklı kaldıraç seçeneklerinin eksiksiz bir analizini sunmaktadır.
---

# Fantom'dan Kaldıraçlı Yararlanın

## Giriş

Mai Finance, Fantom'da birçok farklı kasa tipiyle kredi verme platformunu başlattı ve bir kasaya yatıracağınız varlıklara dayalı olarak MAI basma olanağını sağladı. Buradaki fikir, yüksek APR'lerle diğer paraları ve çiftlik getirilerini satın almaya devam ederken, kripto para birimlerinizi koruyabilecek ve fiyat değerlerinden yararlanabilecek olmanızdır. Kredinizi, daha önce yatırmış olduğunuz aynı varlığın daha fazlasını satın almak için kullanırsanız, buna tokenlarınızı kaldırmak denir. DAI tokenlarımızdan yararlanmak için Fantom'da 2 farklı borç verme platformunu kullanarak bu stratejinin faydalarını size göstereceğiz.

## Yearn Vault tokenlarınızdan yararlanın

### Varlıklarınızı Yearn Finance'e yatırın

[Fantom ağındaki Yearn Finance kasaları](https://beta.yearn.finance/#/home), Ethereum Mainnet ve diğer blok zincirlerinde çalışan ve kullanıcıların kredi verme ve ticaret hizmetleri yoluyla kripto varlıklarındaki kazançlarını optimize etmelerine olanak tanıyan bir protokol grubudur. Fantom'da kullanacağımız ürün, özlem finansmanındaki kasalar. Bu, tek tokenlı para yatırma işlemlerini kabul edecek ve bu para yatırma işleminde getiri elde etmenizi sağlayacak bir araçtır. Para yatırma kanıtı olarak bir yvToken alacaksınız. Bizim durumumuzda, DAI yatıracağız ve karşılığında yvDAI alacağız.

![Fantom ağındaki Yearn Finance kasaları](../.gitbook/assets/ftm-leverage-yv1.png)

{% hint style="info" %}
Yearn Finance web sitesi Fantom'da hala beta modunda. Ekip hala platform üzerinde çalışıyor ve APR'ler/APY'ler görünmüyor. Yearn platformunda ödünç verme/ödünç alma protokolü olan Iron Bank sekmesine giderseniz, ödünç verme DAI'sinin %8 APR aldığını göreceksiniz. Lütfen riski size ait olmak üzere yatırım yapın.
{% endhint %}

### yvToken'ınızı Mai Finance'e yatırın

DAI'nizi Yearn Finance'a yatırdıktan sonra, cüzdanınızda yvDAI olmalıdır. Getiri getiren token dediğimiz şey budur: Kendi başına herhangi bir değeri olmayan, ancak varlıklarınızın getiri elde ettiği ve ödüllerin otomatik olarak birleştirildiği bir havuzdaki payınızı temsil eden bir tokendır. Başka bir deyişle, DAI ABD dolarına sabitlendiği için DAI'nizin değeri değişmezse, yvDAI simgenizin temel değeri yine de artar.

Mai Finance, yvDAI dahil olmak üzere birçok farklı getiri sağlayan tokenı teminat olarak kabul eder. Artık bu tokenı yatırabilir ve karşılığında MAI ödünç alabilirsiniz.

![yvToken'ınızı Mai Finance'e yatırın](../.gitbook/assets/ftm-leverage-yv2.png)

yvDAI kasasının likidasyon eşiği %110'dur, yani teminat değeriniz ile borç değeri arasındaki oran %110 olacak şekilde MAI ödünç alabilirsiniz. %110'un aslında kasanızın likidasyon edileceği oran olduğuna dikkat edin. Oranı bu minimum eşiğin üzerinde tutmanız gerekir. DAI'nin fiyatı çok fazla değişmediği için (birkaç sentten daha az yukarı veya aşağı), "güvenli" bir CDR (**C**ollateral to **D**ebt**R**atio) tutmak mümkündür. %115, ancak daha yüksek bir şey tutmaktan çekinmeyin.

Her zaman olduğu gibi, teminatımızın değerine ve almak istediğimiz hedef CDR'ye göre alabileceğimiz kredi değerini hesaplamak için aşağıdaki formülü kullanacağız:

$$
MAI_{available} = \frac{Collateral_{value} - Debt_{value} * Target_{CDR}}{Target_{CDR}}
$$

​100$'lık bir teminat değeriyle ve borcumuz olmadan, %115'lik sağlıklı bir CDR'yi korumak istiyorsak,

$$
MAI_{available}=\frac{100-0*1.15}{1.15}=86.95
$$

​Artık bir Yearn kasasında DAI kazanç getirilerine sahip olduğunuz bir konumdasınız ve ayrıca kullanıma hazır bir miktar MAI'niz var. DAI konumumuzu güçlendirmek istediğimizden, şimdi MAI'mizi daha fazla DAI ile değiştireceğiz.

### MAI'nizi BeethovenX'te değiştirme

Fantom'da MAI için ana likidite kaynağı [BeethovenX](https://app.beets.fi/#/trade). Stratejimiz için MAI tokenlerinizi daha fazla DAI ile değiştirebileceğiniz ana yer burasıdır.

![MAI'yi daha fazla DAI için değiştirme](../.gitbook/assets/ftm-leverage-yv3.png)

Bu işlem döngümüzün son adımıdır. Artık daha fazla DAI'ye sahip olduğunuza göre, bunları bir Yearn kasasına yatırabilir ve döngüyü tekrarlayabilirsiniz. Böylece Yearn kasasında sahip olduğunuz varlık miktarını artırır, yani DAI'nizi bu platformda ödünç vererek daha fazla ödül toplayacağınız anlamına gelir. APR/APY aynı kalır, ancak daha fazla varlığa sahip olduğunuz için daha fazla getiri elde edersiniz ve ilk yatırımınızla karşılaştırırsanız, artan APR'nizdir. yvDAI döngülerini kullanarak hangi APR'yi elde edebileceğinize dair daha fazla örnek almak istiyorsanız, lütfen Polygon için [camDAI token kılavuzumuzu](../polygon-tutorials/camdai-beginner-strategy.md#main-strategy) okuyun. Tamamen aynı stratejiyi ancak farklı araçları kullanır.

{% hint style="success" %}
BeethovenX aslında ödünç aldığınız MAI'niz ile verim elde etmek için harika bir fırsattır. MAI'nizi MAI-DAI-USDC havuzuna (Kasım 2021 itibarıyla \~%30 APR) yatırmanız yeterlidir.
{% endhint %}

$$
MAI_
$$

## Mai Finance'de mooScreamTokens'ınızı kullanın

### Varlıklarınızı Beefy Finance'e yatırın

[Beefy Finance](https://app.beefy.finance/#/fantom), kullanıcılarının kripto varlıkları üzerinde bileşik faiz kazanmalarını sağlayan bir Merkeziyetsiz Çok Zincirli Getiri Optimize Edici platformudur. Başka bir deyişle, Beefy Finance'deki diğer platformlardan bazı varlıkları veya LP tokenlarını yatırabilir ve otomatik birleştiricinin çiftlik jetonlarını toplamasına ve bunları yatırdığınız varlık / LP tokenınızdan daha fazlasını birleştirmesine izin verebilirsiniz. Örneğimiz için, Beefy'de tekli DAI mevduatlarını kullanacağız ve temel platform olarak [Scream](https://scream.sh/lend) kullanacağız. Scream, Fantom ağındaki varlıklarınızı ödünç verebileceğiniz ve SCREAM tokenlarını toplayabileceğiniz bir Compound klonudur. Beefy daha sonra daha fazla DAI karşılığında SCREAM tokenlerini satacak.

DAI'mizi yatırmak için Beefy Finance uygulamasını ziyaret edeceğiz ve verimleri artıracağımız platform olarak Scream'i seçeceğiz. Doğrudan DAI depozitosu almak için DAI filtresini de ekleyebilirsiniz.

![DAI'nizi Scream kullanarak Beefy'ye yatırın](../.gitbook/assets/ftm-leverage-beefy1.png)

Gördüğünüz gibi, Beefy, DAI tekli mevduatlarda zaten inanılmaz bir APY veriyor. DAI'nizi Beefy'ye yatırdıktan sonra, cüzdanınızda mooScreamDAI şeklinde bir para yatırma kanıtınız olmalıdır. yvDAI tokenına gelince, mooScreamDAI getiri taşıyan bir depozitodur, yani varlığınızın hala Scream'de kullanıldığı ve Beefy'de birleştirilerek getiri elde edildiği anlamına gelir. Ancak MAI'yi onlara karşı ödünç almak için bu tokenı Mai Finance'de kullanabileceksiniz.

### mooScreamToken'ınızı Mai Finance'e yatırın

DAI'nizi Yearn Finance'a yatırdıktan sonra, cüzdanınızda mooScreamDAI olmalıdır. Yukarıdaki Yearn Vault stratejisiyle aynı adımları kullanabilirsiniz, tek fark mooScreamDAI likidasyon oranının %135 olmasıdır. DAI stablecoin olduğundan, MAI ödünç almak ve bir CDR'yi likidasyon oranına çok yakın tutmak hala mümkündür. Örneğimiz için %140'lık bir CDR hedefleyeceğiz ve yukarıdakiyle aynı formülle, 100$ değerinde DAI ile basabileceğimiz MAI miktarını hesaplayabiliriz.


$$
MAI_{available}=\frac{100-0*1.4}{1.4}=71.43
$$

Daha az ödünç aldığımız için daha az döngü gerçekleştirebileceğiz ve nihai eşdeğer APY de daha düşük olacaktır, ancak bu yine de oldukça iyi bir başlangıç ​​stratejisidir.

Döngünün geri kalanı yvDAI ile aynıdır, yani MAI'nizi BeethovenX'te DAI ile değiştirmeniz ve memnun kalana kadar tekrarlamanız gerekecek.

## Stratejilerden yararlanmayla ilgili bazı notlar

Kaldıraç DAI, çok az risk sunduğu (sabit paralarla çalışıyorsunuz) ve en fazla 3 protokol kullanarak bazı güzel getiriler elde edebileceğiniz anlamında başlangıç ​​stratejisi olarak kabul edilir. Ancak yine de _bazı_ risk var.

### Likidasyon riski

Ne kadar çok döngü gerçekleştirirseniz, likidasyon riski o kadar yüksek olur. Aslında, DAI fiyatındaki küçük bir değişiklik bile uyguladığınız kaldıraçla büyüyecektir ve likidasyon oranının 5 puan üzerinde bir CDR tutsanız bile kasanız risk altında olabilir. Varlıklarınızı MAI finansmanına yatırdığınız ve daha iyi bir CDR elde etmek için ek MAI ödünç almadığınız adımda kaldıraç döngülerini durdurmak her zaman iyi bir fikirdir.

Ayrıca, bir likidasyon durumunda, MAI Finance'taki kasanız çok daha fazla varlık içerdiğinden, bir likidasyonun pozisyonunuzu kaldırmamış olmanıza göre daha büyük bir etkisi olacaktır. Çünkü ödemeniz gereken borç da çok daha büyüktür.

### Teknoloji riski

Yatırım legolarınız için çok sayıda protokol kullanıyorsanız, bu protokollerin güvenli olduğundan emin olmanız gerekir. Gerçekten de, bizim kaldıraç stratejimizde tek bir protokol saldırıya uğrarsa tüm strateji çökebilir. DeFi projelerine yatırım yapmadan önce gerekli özeni gösterdiğinizden emin olun.

### Borç tavanlarına ulaşmak

Bu stratejilerin belirlenmesi kolay olduğundan ve düşük riskler sunduğundan, onlara çok yüksek talep vardır. Ancak, kaldıraç sürecinde ödünç alınan MAI'nin DAI (veya diğer tokenlar) ile değiştirildiğini kesinlikle fark etmişsinizdir. Beethoven'da çok fazla MAI satılırsa, fiyatı yavaş yavaş düşecek ve MAI'nin oldukça kötü olan sabitini kaybetme riski var. Fiyatın istikrar kazanması için zaman tanımak için Mai Finance'in güvenlik mekanizmaları vardır ve en önemlisi her kasa için bir borç tavanıdır.

Borç tavanı, belirli bir kasa için basılabilecek maksimum MAI sayısını temsil eder. Tavana ulaşıldığında, artık MAI ödünç alınamaz. Ardından, MAI Finance'taki sorumlu çekirdek ekip, tavanı artırmaya veya MAI için daha iyi bir fiyat için biraz daha beklemeye karar verebilir.

Basılabilecek MAI miktarını [kasa oluşturma sayfasında](https://app.mai.finance/vaults/create) her zaman doğrulayabilirsiniz, ancak genellikle başka MAI olmadığını fark edeceksiniz. aşağıdaki hata mesajını alırsanız:

![Borç tavanına ulaşıldığında alınan hata mesajı](../.gitbook/assets/ftm-leverage-error.png)

Sağlık faktörünüz doğru olsa bile bu hata mesajı görünecektir. Çoğu durumda tavanın yükseltilmesini beklemek tek çözümdür. Bunun ne zaman olduğunu öğrenmek için gözünü Twitter'da veya Discord'da tut.

## Sorumluluk Reddi

Bu kılavuz, varlıklarınızı Fantom'da kullanmanın bazı yollarını sunar ve kazançlarınızı artırmak için Mai Finans'ı stratejinize dahil eder. Ancak, her zamanki gibi, bu eğitim finansal bir tavsiye değildir ve bir yatırım stratejisi uygulamadan önce her zaman kendi araştırmanızı yapmalı ve tecrübeli kullanıcılara başvurmalı ve sorumlu bir şekilde yatırım yapmalısınız.

Ayrıca, ne zaman kullanmayı planladığınıza bağlı olarak bu çözümün en iyi strateji olmayabileceğini de unutmayın. BeethovenX'in MAI'niz için de oldukça ilginç APR'leri olduğunu vurguladık ve BEETS ödüllerini stablecoine dönüştürmek için Beefy Finance'i de kullanabilirsiniz.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
