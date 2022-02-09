---
açıklama: >-
  Bir kredi almak, bu krediyi bir yatırım stratejisinin başlangıç noktası olarak kullandığınız takdirde tam olarak bir borç sözleşmesi olmaz. Bu gerçek bir yatırım olur
---

# A Spooky Symfony

## Giriş

Varlıklarınıza karşı borç almanın her zaman hem iyi hem de kötü yanı vardır: Bir yatırım stratejisini başlatmanıza veya varlıklarınızı kaldırmanıza yardımcı olabilir ancak bir noktada geri ödeme yapmanız gereken bir borcunuz olacaktır. Bu kılavuzda, MAI'yi düşük borçlanma oranıyla alabileceğiniz bir borç verme protokolü olan Market.XYZ’den alıp bu borcu diğer platformlarda test için Fantom’da kullanacağız. Teminat olarak yatırılan varlıkların kilidini açmak için borcu geri ödeme stratejisini kullanacağız ve bunun ne kadar hızlı yapılabileceğine bakacağız.

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor. Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.

{% endhint %}

![](<../../.gitbook/assets/spooky-symfony-1.png>)

## Fantom Protokolleri: Hepsini Kullan!

Bu stratejide, birçok farklı protokolde farklı LP (Likidite Sağlama) çiftlerini kullanacağız, bu yüzden size her protokol hakkında kısa bir özet vermenin iyi bir fikir olacağını düşündük.

### Market.XYZ

[Market.XYZ](https://fantom.market.xyz/) bazı belirli varlıkları veya LP tokenlarını teminat olarak yatırabileceğiniz ve bunlara karşı borç alabileceğiniz bir borç alma-verme protokolüdür. Bir teminata karşı borçlanma, tasfiye etmediğinizden emin olmak için önemlidir. Teminat olarak yatırdığınız varlığın değeri, sözleşmenizdeki borcun değerinin altına düştüğünde bir likidasyon oluşur. Bu yüzden iki değer arasındaki oranın nispeten yüksek kaldığından ve teminatınızın piyasaya sürüldüğünde çok fazla değer kaybetmeyeceğinden emin olmak önemlidir.

Likidasyon riskini azaltmak için FTM-USDC LP tokenını teminat olarak kullanacağız.

* Bu çift üzerindeki geçici kayıp nispeten düşüktür
* USDC dolara sabitlenmiş bir stablecoindir
* FTM, Fantom'un yerli gas tokenıdır, derin likiditeye sahiptir ve her yerde kullanılır
* FTM-USDC çifti üzerindeki ödül oranları yüksektir, böylece FTM'nin fiyatı aynı kalsa bile teminatınızın değeri yükselir.

You will be able to borrow against the FTM-USDC pair from the  on market.xyz. The steps to deposit your collateral are as follows: Market.xyz'deki [Spooky LP havuzu](https://fantom.market.xyz/pool/10) FTM-USDC çiftine karşı borç alabileceksiniz. Teminatınızı yatırmanın adımları aşağıdaki gibidir:

* Her iki varlık için 1: 1 oranında likidite sağlayarak [Spooky LP havuzundan](https://spookyswap.finance/add/FTM/0x04068DA6C83AFCFA0e13ba15A6696662335D5B75) oluşturun.
* mooBooFTM-USDC lp token almak için FTM-USDC LP tokenını Beefy Finance'e yatırın (Arama filtrelerinde Spookyswap platformunu ve USDC varlığını arayın)
* mooBooFTM-USDC lp tokenını Market.xyz'ye yatırın

![Şubat 2022 yılı itibariyle MarketXYZ'de Spooky borç verme pazarı](<../../.gitbook/assets/spooky-symfony-2.png>)

Beefy LP tokenlarınız Market.xyz'de olduğunda hala Beefy tarafından sağlanan ödül APY'sini alırsınız. Bu da varlıklarınızın onlarla borç alırken hala sizin için verim oluşturduğu anlamına gelir. Bu, özellikle mSPLP-FTM-USDC'nin (moo Spookyswap FTM-USDC = mooBooFTM-USDC) %51.4 APY kazandığını ve %2,56'lık APR'de MAI’yi borç alabileceğinizden çok güçlü bir araçtır. Başka bir deyişle, teminatınız borcunuzdan daha hızlı büyür, bu nedenle teoride borcunuzu teminatınızın getirileriyle çok rahat ödeyebilirsiniz.

{% hint style="info" %}
Bir ek not olarak, Spooky LP havuzunun ayrıca diğer LP tokenlarına karşı borçlanma imkanı sunduğunu görebilirsiniz: ETH-FMT, DAI-FTM, BTC-FTM ve fUSDT-FTM. Cüzdanınızdaki varlıklara ve risk toleransınıza bağlı olarak herhangi bir Spookyswap LP'yi teminat olarak kullanabilirsiniz.
{% endhint %}

Bu eğitim için %200'lük bir CDR (Borç Teminat Oranı) ile borçlanma riskini de sınırlayacağız. Bu da teminatımızın değerinin % 50'sini borç alacağımız anlamına gelir. Çiftçilik stratejisi bölümünde daha fazlası var. Tasfiye oranları, bir CDR'nin zıttı olarak LTV (Kredi Değeri) olarak ifade edilir. mooBooFTM-USDC tokenı için LTV'nin, yukarıda tasfiye edeceğiniz % 60 olduğunu görebilirsiniz. Bu da %166.67'lik bir CDR'ye eşdeğerdir. %200 CDR hedefi ile risk toleransınıza bağlı olarak riskli olabilecek veya olmayacak tasfiye oranının %33 üzerindeyiz.

{% hint style="danger" %}
Market.XYZ only allows loans with a minimum value of 0.05 ETH (~$170.00 at time of writing). Make sure you deposit enough collateral if you want to bororw from the different lockers.
{% endhint %}

### BeethovenX

[BeethovenX](https://beets.fi/#/) Balancer’dan klonlanan merkeziyetsiz bir borsa ve otomatik pazar yapıcısıdır. Varlıklarınızı likidite havuzlarına yatırabilir ve ayrıca uygulamaları üzerinden farklı varlıkları takas edebilirsiniz. Mai Finance’de bulabileceğiniz çiftlikler için LP tokenları sağlayan QiDAO protokolünün sağlam bir ortağı olmuşlardır. Stratejimiz için Beethovenx'te iki farklı havuz kullanacağız.

* The Monolith: [Bu eğitimde sunduğumuz](investing-in-discounted-assets-using-bonds.md) bir OHM klonu olup Exodia'ya açık olan teşvik havuzudur. Mai tokenlarınızı doğrudan bu havuza yatırabilir ve verim toplayabilirsiniz.
* Pirate Party: Bu kılavuzda kullanacağımız bir başka büyük protokol, Liquid Driver’ın yerel tokenı olan LQDR tokenlarına adanmış bir teşvik havuzudur

![Beethovenx'te The Monolith Havuzu Şubat 2022'den itibaren %20 MAI ile](<../../.gitbook/assets/spooky-symfony-3.png>)

![Beethovenx'te Pirate Party Havuzu Şubat 2022'den itibaren %80 LQDR ile](<../../.gitbook/assets/spooky-symfony-4.png>)

Her zaman olduğu gibi, Beethovenx (veya Balancer) kullanmanın en büyük avantajı, tokenları dengeli bir oranda sağlamak yerine havuzlara tek varlık yatırabilmenizdir.

### SpookySwap

[Spookyswap](https://spookyswap.finance/) Fantom'daki en büyük Uniswap V2 klonudur, varlıkları takas edebileceğiniz bir platformdur ve birçok çift için likidite sağlar. SpookySwap ayrıca MAI Finance’in sağlam bir ortağı olmuştur ve MAI-USDC havuzunu önermektedir. Bazı belirli LP çiftlerine karşı MAI borç alabileceğiniz ve aynı zamanda BOO ve stake edilmiş BOO tokenlarınızı SpookSwap'in yerel tokenı ile takas edebileceğiniz yer olan Market.XYZ (Market.XYZ hakkındaki bölüme bakın) ile bu ortaklık genişletilmiştir.

Bu kılavuz için, SpookySwap'ten iki farklı LP tokenını kullanacağız:

* FTM-USDC, strateji için başlangıç noktamız olarak kullanılacak. Bu LP tokenı, Market.XYZ’de teminat olarak kullanılmaktadır
* FTM-BOO, çünkü en yüksek APR ile SpookySwap’ten Liquid Driver’a kabul edilen havuzlardan biridir. BEETS ödüllerini bu çift için The Monolith’ten takas edeceğiz (Çiftçilik Stratejisi bölümünde daha fazla ayrıntı var)

### Liquid Driver

[Liquid Driver](https://www.liquiddriver.finance/) farklı çiftliklerden LP tokenları yatırabileceğiniz ve onlar üzerinden verim kazanabileceğiniz bir verim optimize edicidir. Verim optimize edicinin çalışma şekli, hedef platformun ödül tokenlarını toplayarak bunları sizin için birleştirmektir. Fantom’daki gas pahalı olabileceğinden dolayı faydalı bir sistemdir. Bir performans ücreti alınır ancak protokolün gelirinin bir kısmı LQDR stake edenlere yeniden dağıtılır. LQDR, Liquid Driver’ın yerel tokenıdır.

Bu strateji için FTM-BOO LP çiftini kullanacağız çünkü SpookySwap için LQDR'deki en yüksek APR'den birine sahip olan bir havuzdur

![2022 Şubat itibariyle LiquidDriver'daki FTM-BOO ve FTM-USDC LP LP Çiftleri(<../../.gitbook/assets/spooky-symfony-5.png>)

## Çiftçilik Stratejisi

Bu strateji için, mooBooFTM-USDC LP tokenlarına karşı MAI borç almak için Market.XYZ’yi kullanacağız. Borç alınan MAI, The Monolith havuzundaki Beethovenx'e yatırılacaktır çünkü bu havuz, stratejimizde en yüksek ödül oranına sahip olan havuzdur. Bu havuzu borcumuzu geri ödemek için motorumuz olarak kullanacağız: BEETS’lerin %50'si Market.XYZ’deki borçları geri ödemek için satılacak ve %50'si FTM-BOO LP tokenlarına dönüştürülecektir. FTM-BOO tokenları, daha sonra Beethovenx'te Pirate Party havuzuna stake edilecek LQDR tokenlarını toplamak için LiquidDriver’a yatırılacaktır. Borç tamamen geri ödendikten sonra BEETS ödülleri tamamen FTM-BOO tokenlarına dönüştürülecektir. Pirate Party havuzunun sağladığı BEETS ödülleri de daha fazla FTM-BOO’ya birleştirilecektir.

Bu simülasyon için aşağıdaki rakamları kullanacağız:

* 1000$ değerindeki mooBooFTM-USDC tokenıyla başlıyoruz
* mooBooFTM-USDC tokenı için Beefy üzerinden SpookySwap tarafından sağlanan APR %41,5'tir.
* MAI için borçlanma oranı %2,56'dır
* Beethovenx, The Monolith için %304,17, Pirate Party için %175.77 APR verir.
* LiquidDriver FTM-BOO LP çifti için %82 APR verir.

Simülasyonlarımız için her zamanki gibi tüm fiyatların 1 yıllık süre boyunca aynı kaldığını varsayıyoruz, fiyatlar aynı kalır ve ayrıca verilen APR'leri de kullanırız. Gerçekte, fiyatlar ve oranlar değişecektir ve APR'ler sonucunu etkileyebilecek alım satım ücretlerinden ve ödül tokenlarından oluşur. Bu simülasyon için **herhangi bir işlem ücretinin alınmadığını** not etmek de önemlidir. Son olarak, birçok protokol kullanıyoruz ve her protokol kendi akıllı sözleşme risklerini sunabilir. Bir platformu kullanmadan önce kendi araştırmalarınızı yaptığınızdan emin olun.

Spooky Symfony simülasyonumuzu [bu Google e-tablosunda](https://docs.google.com/spreadsheets/d/19s6kBnT5w0b9GKuTkDiiD1u_ZoeNUZtI9XYxEmk_WM0/edit?usp=sharing). bulabilirsiniz. Döngülerin nasıl çalıştığını ve farklı oranların nihai APY'nizi nasıl etkileyebileceğini görmek için kopyalayıp deneyebilirsiniz.

![](<../../.gitbook/assets/spooky-symfony-6.png>)

### 1.Gün

1. günde, Market.XYZ için teminatınızı oluşturmanız gerekir. FTM-USDC LP tokenları oluşturmak için FTM ve USDC'nin eşit bir bölümünü alın ve SpookySwap üzerinde likidite sağlayın. Bu tokenlar, Size mooBooFTM-USDC lp tokenı kazandıracak olan Beefy’e yatırılacaktır. Bu token, Market.XYZ'de teminat olarak kullanılacak tokendır. CDR'yi %200 tutmak istediğimizden, 500$ değerinde MAI borç alacağız. Son olarak, MAI tokenları Beethovenx'te The Monolith havuzuna stake edilecektir.

İlk günün sonunda,

|     pozisyon   |  değer ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,000.000 |
| the monolith   |    500.000 |
| pirate party   |      0.000 |
| BEETS ödülleri |      4.167 |
| FTM-BOO        |      0.000 |
| LQDR ödül      |      0.000 |
| MAI borç       |    500.000 |

### 2.Gün

2. günde yapacaklarınız,

* BEETS’inizin %50'sini borcunuzun küçük bir kısmını geri ödemek üzere MAI için satın
* FTM-BOO LP çifti için BEETS ödüllerini takas edin. Beethovenx'te takas edip SpookySwap'te LP çifti oluşturabilirsiniz veya her şeyi SpookySwap'te yapabilirsiniz.
* LQDR tokenlarını toplamaya başlamak için FTM-BOO LP tokenlarını Liquid Driver’da stake edin.

İkinci günün sonunda,

|     pozisyon    |  değer ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,001.137 |
| the monolith   |    500.000 |
| pirate party   |      0.000 |
| BEETS ödülleri |      4.167 |
| FTM-BOO        |      2.083 |
| LQDR ödülleri  |      0.005 |
| MAI borç       |    497.952 |

### 3.Gün

2. günün işlemlerini tekrarlayın, ardından ilk LQDR tokenlarınızı toplayın. Bunlar, ekstra BEETS ödülleri almak için Pirate Party havuzunda Beethovenx'e yatırılacaktır ve 3. günün sonunda,

|     pozisyon    |  değer ($) |
|----------------|------------|
| mooBooFTM-USDC |  1,002.275 |
| the monolith   |    500.000 |
| pirate party   |      0.005 |
| BEETS ödülleri |      4.167 |
| FTM-BOO        |      4.167 |
| LQDR ödülleri  |      0.000 |
| MAI borç       |    495.903 |

{% hint style="info" %}
Pirate Party havuzundan elde edilen kazançlar bu noktada çok düşük ama zamanla artacaktır.
{% endhint %}

### Günlük Rutin

Bu noktada sistem tamamen hazırlanmıştır. Günlük rutininiz,

* The Monolith’ten BEETS ödüllerini toplayın
* Pirate Party’den BEETS ödüllerini toplayın
* Hala çok fazla borcunuz varsa BEETS’inizin %50sini MAI ile takas edin
* Hala borcunuz varsa borcunuzu ödeyin
* BEETS’lerin geri kalanını FTM-BOO LP tokenlarıyla takas edin
* FTM-BOO tokenlarını LiquidDriver’a yatırın
* LQDR toplayın
* Pirate Party’e yatırın

Bu stratejide gas verimi iyi değildir, bu yüzden kazanımlarınızı haftada sadece bir kez veya daha az sıklıkla birleştirmeyi düşünebilirsiniz.

### Aydan Aya Ham Sonuçlar

Yukarıda linki verilen Google e-tablosunda görebileceğiniz gibi, işte aydan aya ham sonuçlar:
 
| gün |  FTM-USDC  | The Monolith | Pirate Party |  FTM-BOO  | MAI borç |
|-----|------------|--------------|--------------|-----------|----------|
|  30 |  1,033.503 |      500.000 |        1.901 |    60.500 |  440.541 |
|  60 |  1,069.343 |      500.000 |        8.031 |   123.652 |  378.905 |
|  90 |  1,106.425 |      500.000 |       18.452 |   187.988 |  317.139 |
| 120 |  1,144.794 |      500.000 |       33.265 |   254.136 |  255.242 |
| 150 |  1,184.493 |      500.000 |       52.612 |   322.738 |  193.216 |
| 180 |  1,225.569 |      500.000 |       76.681 |   394.462 |  131.058 |
| 210 |  1,268.069 |      500.000 |      105.704 |   470.006 |   68.770 |
| 240 |  1,312.043 |      500.000 |      139.963 |   550.105 |    6.351 |
| 270 |  1,357.542 |      500.000 |      181.427 |   691.752 |    0.000 |
| 300 |  1,404.619 |      500.000 |      233.046 |   846.443 |    0.000 |
| 330 |  1,453.328 |      500.000 |      295.350 | 1,009.331 |    0.000 |
| 360 |  1,503.726 |      500.000 |      368.942 | 1,182.000 |    0.000 |

### 365. Gün

Bu sistemle bir yıllık çiftçiliğin sonunda,

* Market.XYZ’de 1.512.294$ değerinde FTM-USDC tokenı
* The Monolith havuzunda 500.000$ değerinde MAI
* Pirate Party havuzunda 382.353$ değerinde LQDR
* Market.XYZ’de 1.211.845 değerinde FTM-BOO
* 243 günden sonra tamamen geri ödenen son bir borç

Bu da toplam % 260,65'lik bir APY'ye eşdeğerdir

### Borcun geri ödenmesinin genel sonuca etkisi

Kılavuzumuzun çoğunda, stratejinin bir parçası olarak herhangi bir borcu geri ödemiyoruz. Bu, çoğu durumda, Mai Finance'ten alınan %0 faizli kredi kullanmamızdan kaynaklanmaktadır. Burada, Market.XYZ'den %2,56'lık bir borçlanma oranı ile borç alıyoruz ve bu borcu The Monolith'ten toplanan BEETS’in %50'si ile geri ödüyoruz.

Borcun geri ödenmesine %50'den fazlasını ayırırsanız daha az faiz ödersiniz ancak Liquid Driver'da pozisyonlarınızı çok daha yavaş büyütürsünüz. Borcun geri ödenmesine %50'den az pay ayırırsanız diğer platformlardan daha fazla ödül alırsınız ama Market.XYZ'de de daha fazla faiz ödersiniz.

Tahsis edilen BEETS’in borcun geri ödenmesinin genel APY'niz üzerindeki etkisini gösteren küçük bir tablo:

| BEETS % |  Genel APY  |Borçtan sonra kalan|
|---------|-------------|-------------------|
|     100 |      242.85 |          122 days |
|      90 |      245.06 |          135 days |
|      80 |      247.75 |          152 days |
|      70 |      251.05 |          174 days |
|      60 |      255.23 |          203 days |
|      50 |      260.65 |          244 days |
|      40 |      267.92 |          305 days |
|    33.5 |      274.09 |          364 days |

Borcunuzu ödemek için BEETS ödüllerinizin %33,5'inden azını kullanırsanız tam bir yıl sonra hala geri ödemeniz gereken bir miktar MAI'niz olacaktır

Ayrıca daha hızlı geri ödediğinizi ve CDR'nizi önemli bir şekilde artırdığınızı, bunun da likidasyon oranından daha hızlı kurtulmanızı sağladığını hatırlatmakta fayda var.

## Dikkate alınması gereken varyasyonlar

Bu strateji, farklı faydalar sunan birçok varyasyon sunar.

### Mai Finance VS Market.xyz

MAI'yi [Mai Finance](https://app.mai.finance)'den %0 faizle borç alabilirsiniz. Örnek olarak, teminat olarak mooBooFTM-USDC yerine mooScreamFTM kullanırsanız, bu size aşağıdaki avantajları sunacaktır

* Teminatınızda herhangi bir kalıcı kaybınız olmaz
* Çoğu durumda Market.xyz'de ödediğiniz faizden çok daha düşük olan %0,5'lik tek bir geri ödeme ücretiyle %0'dan borç alırsınız. (bu kasa için borç alınacak MAI varsa)
Platformdan borç aldığınız için Qi ödülleri alabilirsiniz; bu da protokolün yönetişimine katılmanıza ve ayrıca Qi tokenlarınızı stake ederseniz temettü almanıza izin verir. Bu da yıllık kazancınızı artıracaktır.
* Market.xyz'de dalgalı borçlanma oranlarından korunursunuz. Mai Finance, borçlanma oranlarını mümkün olduğu kadar düşük tutmak için düzenli olarak yeni MAI borç verecek ancak bu, yükselmeyeceğine dair bir garanti değildir. Borç verme piyasasına ilişkin ölçümleri [buradan](https://metrics.market.xyz/d/HChNahwGk/fuse-pool-details?orgId=1&refresh=10s&var-poolID=10&var-chain=250) kontrol edebilirsiniz.

Ancak mooScreamFTM tokenları, mooBooFTM-USDC tokenlarına kıyasla çok daha düşük bir APY alır, bu yüzden bunu kaçırabilirsiniz.

### LQDR'nizi stake edin

LQDR'nizi Pirate Party havuzunda kullanmak yerine stake ederseniz, Liquid Driver'dan farklı varlıklarda ödenen bir miktar temettü kazanırsınız (LQDR, WFTM, LINSPIRIT, BOO, SPELL ve BEETS). Ayrıca Liquid Driver yönetişimine katılmanıza izin verecek xLQDR ve muhtemelen Spirit Swap'ta ödül dağıtımına oy vermek için LINSPIRIT alacaksınız. Daha fazla ayrıntı için lütfen xLQDR sayfasını dikkatlice kontrol edin.

### BEETS’inizi stake edin

Bu stratejide The Monolith'teki BEETS'in rolü büyükse Pirate Party'dekileri aşağıdaki gibi tamamen kullanabilirsiniz:

* BEETS’i Fidelio Duetto havuzuna yatırın (BEETS-FTM)
* fBEETS almak için LP tokenını BeethovenX'te stake edin
* protokol temettüleri almak için fBEETS'inizi stake edin

Bu aynı zamanda BeethovenX protokol iyileştirmelerine ve platformdaki farklı havuzlar için ödül dağıtımına oy vermenize de olanak tanır. Bu da özellikle The Monolith'te yüksek bir APR’yi korumak için kullanışlıdır.

### Spookyswap'te FTM-BEETS havuzunu kullanın

Stratejimizde, The Monolith'in tüm BEETS ödüllerini satıyoruz. Ancak, Spookyswap'teki FTM-BEETS havuzunu döngünüze entegre edebilirsiniz. BEETS’inizin %50'sini FTM karşılığında satmanız ve iki tokenı size BOO kazandıracak yeni bir LP çiftinde birleştirmeniz gerekir. Daha sonra FTM-BOO'yu oluşturmaya ve Liquid Driver'a para yatırmaya karar verebilir veya BOO'nuzu SpookySwap'te stake edebilirsiniz. BOO'nuzu stake ederseniz xBOO lp tokenlarını yatırma ve LQDR tokenlarını doğrudan kazanma olanağına sahip olacağınızı ve hatta xBOO tokenlarını Market.xyz'de teminat olarak kullanabileceğinizi unutmayın. Bu ek, birçok olasılığın kapısını açar.

{% hint style="info" %}
Liquid Driver'da kullanılabilir olması durumunda bu çifte göz atın. Bu çift, FMT-BOO'dan daha iyi bir seçenek olabilir.
{% endhint %}

### FTM-USDC'nizi Liquid Driver'da kullanın

Borcunuz tamamen geri ödendikten sonra mooBooFTM-USDC tokenlarınızı Market.xyz’de veya Beefy'de tutabilirsiniz, ödül kazanmaya devam edeceklerdir. Bununla birlikte, daha fazla LQDR elde etmek için LP çiftini Beefy'den çıkarabilir ve Liquid Driver'a yatırabilirsiniz.

Ek bir not olarak, borcunuzu geri öderken Teminat Borç Oranınızın değeri büyür (teminat, ödülleri birleştirir ve her kısmi geri ödemeden sonra borç küçülürken değeri artar). Bu da güvenli bir CDR’yi korumak için teminat parçalarını parça parça çekebileceğiniz ve daha fazla LQDR tokenı için Liquid Driver'a yatırabileceğiniz anlamına gelir.

### Küçük bir kâr akışı tutturun

Bu sistem kendini besleyen kapalı bir döngüdür. Ancak, Market.xyz'deki borcunuzu ödemeyi bitirdikten sonra, BEETS'inizin bir kısmını başka varlıklar için satmaya devam edebilirsiniz. Örnek olarak, BEETS ödüllerinizi USDC'ye veya başka bir stablecoine dönüştürebilir veya FTM-USDC çifti için verilenlerden daha fazla ödül kazandıran pozisyonlarınızdan birini artırabilirsiniz.

## Sorumluluk Reddi

Bu kılavuz genel olarak, çiftçilik getirilerini kullanarak bir borcu nasıl geri ödeyebileceğinizi göstermek için tasarlanmıştır. Borcunuzu geri ödeme hızınız ödül oranını büyük ölçüde etkileyecektir ancak aynı zamanda bazı olumlu yönler de sunacaktır, bunlardan başlıcası tasfiye riskini azaltmaktır.

Tabii ki bu strateji ile çok kolay bir şekilde kolaya kaçabilir, döngünün parçalarını, protokolleri vb. tercih ettiğiniz başka bir şeyle değiştirebilirsiniz. Ancak, kullanmak istediğiniz tüm farklı protokoller için mevcut tüm belgeleri okuduğunuzdan ve riskleri anladığınızdan emin olun.

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}
