---
description: >-
  Bu eğitimde, USD dışı Fiat'lara sabitlenmiş sentetik varlıklarla yatırım yapmak isteyen kişiler için Jarvis tarafından etkinleştirilen bazı DeFi çözümlerini ele almaya çalışacağız.
---

# Jarvis ile Geleneksel Finanstan DeFi'a

Tüm stablecoin’ler eşit değildir. Çoğu DeFi (Merkeziyetsiz Finans) kullanıcısı için stablecoin’ler, ABD dolarına sabitlenmiş bir kripto para birimini temsil eder. Örneğin:

* Merkezi kuruluşlar tarafından çıkartılan ve ABD doları ile desteklenen USDC veya USDT
* ABD dolarına yumuşak bir şekilde sabitlenmiş ancak farklı kripto para birimlerinden oluşan bir sepet tarafından desteklenen DAI veya MAI gibi aşırı teminatlandırılmış varlıklar
* UST veya MIM gibi kısmen desteklenen ve belirli bir algoritma kullanılarak 1$’lık sabitin korunduğu algoritmik stablecoin’ler

Peki başka stablecoin’ler bulabileceğinizi biliyor muydunuz? Örnek olarak, TOMB, algoritmalar kullanılarak FTM (Fantom Network’ün yerel gas tokenı) fiyatına sabitlenmiş bir tokendır.

Bu yazıda, FIAT'lara (devlet tarafından çıkartılan para birimleri) sabitlenmiş stablecoin’lere odaklanacağız ve yatırım stratejileriniz için neden önemli olduklarını açıklamaya çalışacağız.


![](<../../.gitbook/assets/Jarvis-0.png>)

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}

## Neden sentetik FIAT'lara ihtiyacımız var?

Bir Avrupa ülkesinde yaşadığınızı ve günlük olarak Euro kullandığınızı düşünelim. Kripto varlıkları satın alacak olsaydınız büyük olasılıkla onları Euro'nuzla satın alırdınız. Para kazanıp kazanmadığınızı değerlendirmek için Bitcoin'in Euro cinsinden fiyatına odaklanırsınız. Ve umarım biraz kazanırsınız.

Peki ya bunun yerine DeFi'ya yatırım yapmak ve çiftçilik yapmak istiyorsanız? Ya riskleri azaltmak için yalnızca stablecoin’leri kullanarak likidite sağlamak istiyorsanız? Birçok zincirdeki stabil likiditenin çoğu USD'ye sabitlenmiş varlıklar olarak sağlanır; bunun anlamı, Euro'nuzu kullanarak USDC/USDT/DAI/MAI satın almanız gerekeceğidir. Bu noktada sağladığınız likiditenin faiz getirip getirmediğini, aynı zamanda ABD Doları ile Euro arasındaki fiyat farkının aleyhinize olup olmadığını kontrol etmelisiniz.

![Geçen yıl boyunca EUR/USD](<../../.gitbook/assets/Jarvis-1.png>)

I20 Eylül 2021'de 100€ değerinde USDC satın aldıysanız, o sırada EUR:USD oranı 1:1.1729 olduğundan 117.29$ değerinde USDC'ye sahip olacaktınız. Bugün (24 Mart 2022) 117.29$ değerinde USDC'yi 1:1.0994 oranında Euro'ya çevirirseniz 106.69€ veya %6.69'luk bir kazanç elde edersiniz.

Ancak aynı gün (20 Eylül 2021) 1:0.7796 oranıyla 100 CAD (100 Kanada Doları) değerinde USDC satın almış olsaydınız 77.96 USD değerinde USDC'ye sahip olurdunuz. Bunları bugün 1:0,7972 oranıyla CAD'e dönüştürmek, 97,79 CAD veya %2,21 kayıp olacaktır.

Ancak 1 CAD her zaman 1 CAD'a eşittir, örneğin 1 USD = 1 USD ve 1 EUR = 1 EUR gibi.

Her ülkenin para birimi jeopolitik duruma, iç ve dış politikaya, mikro ve makro ekonomik kararlara göre değişir. Bu nedenle kripto varlıklarınız "stabil" olsalar bile fiyat değişimlerine dikkat etmeniz gerekiyor.

## Jarvis Network ve Mt. Pelerin

### Jarvis Network Nedir?

[Jarvis Network](https://jarvis.network/) kullanıcıların kripto varlıklarını sentetik FIAT'ler ile değiştirmelerini sağlayan özel bir uygulamadır. Sentetik bir FIAT, mevcut bir FIAT'ın fiyatına sabitlenmiş bir kripto para birimidir. Bu nedenle, Jarvis USDC'lerinizi aşağıdakilerle değiştirmenize imkan sağlar:

* jCAD: Kanada Dolarının kripto versiyonu
* jEUR: Euro'nun kripto gösterimi
* jJPY: Japon Yeni'nin kripto versiyonu
* jSGD, jCHF, jGBP ve daha fazlası

Bu nedenle, Jarvis gerçekten Ethereum Mainnet'te ve aynı zamanda Polygon, BNB Chain, Gnosis Chain ve Avalanche'da aktif olan bir On-Chain Forex'tir (Foreign Exchange).

Bu kadarla bitmiyor. Jarvis, jFIAT'ları içeren teşvikli likidite havuzları önermektedir. Bu, kullanıcıları jFIAT'lerini yatırmaya ve stablecoin'lerinden getiri elde etmeye çekmek için (Curve havuzları aracılığıyla tek bir varlık yatırma imkanı ile), çok fazla likiditeye sahip olmayan stablecoin’ler sunan diğer protokollere yardımcı olmak ve DeFi kullanıcılarının kazançlarını artırmalarını kolaylaştırmak için yapılır.

![Mart 2022 itibariyle Jarvis'te likidite havuzları](<../../.gitbook/assets/Jarvis-2.png>)

{% hint style="info" %}
Yukarıdaki ekran görüntüsünde 2CAD çiftinin jCAD ve CADC'den oluştuğunu görebilirsiniz. CADC tokenı, aslında başka bir merkeziyetsiz Forex çözümü olan DFX tarafından sağlanan Kanada Doları'nın başka bir versiyonudur.
{% endhint %}

### Mt. Pelerin

[Mt. Pelerin](https://www.mtpelerin.com/bridge-wallet) gözetimsiz bir fiat-kripto OTC panelidir. Kullanıcıların doğrudan banka hesapları ile kripto satın almalarına ve doğrudan kripto cüzdanlarına yatırmalarına olanak tanır. Aynı zamanda Jarvis'in doğrudan ortağıdır ve jFIAT satın almanızı sağlar.

{% hint style="info" %}
Mt. Pelerin’i kullanmanın en kolay yolu Bridge Wallet mobil uygulamasıdır. Merkezi bir hizmet olduğundan, hizmeti kullanabilmek istiyorsanız kimliğinizi kanıtlamak için kişisel bilgilerinizi vermeniz gerekeceğini unutmayın. Ayrıca İsviçre'ye banka havalesi yapmanıza izin veren bir bankanızın olması gerekir. Ancak, banka havalesinden veya Kredi Kartı kullanarak kripto para satın almanıza izin veren bir widget bulacağınız web sitelerini kullanmak her zaman mümkündür. Bu herhangi bir KYC'ye tabi değildir, ancak bazı sınırlamaları vardır. Web sitesini kullandığınızda satın aldığınız ürünün doğrudan web cüzdanınıza gönderileceğini unutmayın. Bu kılavuzun geri kalanında Birdge Wallet çözümünü sunacağız.
{% endhint %}

![EUR banka havalesi ile bir miktar jEUR satın almak](<../../.gitbook/assets/Jarvis-3.png>)

Banka havaleleri ücrete tabi olabilir ve büyük olasılıkla tamamlanması biraz zaman alacaktır, ancak genel olarak Mt. Pelerin, sentetik FIAT'larınızı FIAT muadilleri için kolayca alıp satmanıza olanak tanır. Ayrıca daha detaylı okuyabileceğiniz dahili bir ücret yapısına sahiptirler ve satın aldığınız varlığa bağlı olarak yılda 100.000$'a kadar ücretsiz olarak alıp satabilirsiniz.

![Banka hesabıma biraz jCAD satıyorum](<../../.gitbook/assets/Jarvis-6.png>)

{% hint style="info" %}
jFIAT satın aldıysanız banka hesabınız otomatik olarak Bridge Wallet hesabınıza bağlanır ve onu alıcı listesinden seçebilirsiniz. Aksi takdirde, bir IBAN'dan yeni bir hesap oluşturmanız gerekecektir.
{% endhint %}

### Polygon cüzdanınızı Mt. Pelerin hesabınıza bağlayın (Bridge wallet adresi)

Cüzdanınızı Mt. Pelerin / Bridge Wallet hesabınıza bağlamak bu kadar kolay.

* Bridge Wallet uygulamasını açın
* En alttaki Adresler sekmesini açın
* Adresi bağla'ya tıklayın
* Polygon cüzdanınızın QR kodunun fotoğrafını çekin veya tam adresi kopyalayıp alana yapıştırın
* Doğrulamak için Bridge Wallet adresine birkaç MATIC gönderin

![](<../../.gitbook/assets/Jarvis-5.png>)

![Polygon cüzdanlarımı Mt. Pelerin’e bağlama](<../../.gitbook/assets/Jarvis-4.png>)

{% hint style="info" %}
Bir kez daha, Bridge Wallet'ı kullanmadan doğrudan web cüzdanınızı (veya donanım cüzdanınızı) kullanarak kripto paranızı alıp satmak için Mt. Pelerin web sitesindeki widget'ı kullanabilirsiniz. Lütfen Mt. Pelerin’in web sitesine göz atın.
{% endhint %}

### Polygon cüzdanınıza jFIAT gönderme

JFIAT'lerinizi Polygon (veya desteklenen herhangi bir zincir) üzerindeki cüzdanınıza göndermek çok kolaydır. Cüzdan sekmesinden, hedef olarak kullanmak istediğiniz ağda olduğunuzdan emin olun ve jWallet Para Birimlerinizi yükleyin.

![Polygon’a jCAD gönderme](<../../.gitbook/assets/Jarvis-8.png>)

Göndermek istediğiniz jFIAT'ı seçtikten sonra gönder'e tıklayın, diğer alanları doldurun, ardından işlemi başlatın ve düşük gas ve hızlı işlemin tadını çıkarın!

{% hint style="info" %}
Her jFIAT'ın aktivite bölümünden ve ana ekrandaki Aktivite sekmesinden tüm işlemlerinizin tam bir özetini alabilirsiniz.
{% endhint %}

![DeBank.com'da jCAD'imi aldığımı kontrol ediyorum](<../../.gitbook/assets/Jarvis-7.png>)

{% hint style="success" %}
Mt. Pelerin, kripto para birimleri ve sentetik FIAT'ler alıp satmak için çok iyi bir çözümdür. Aynı zamanda bu hizmeti, uygulamayı kullanıyorlarsa arkadaşlarınıza ve ailenize para göndermek ve karmaşık banka transferlerini veya sınırlamaları atlamak için de kullanabilirsiniz.
{% endhint %}

## Stabil jFIAT'larınızdan en iyi şekilde yararlanma

Polygon'da sentetik FIAT'larınız var, bu yüzden şimdi bunları kullanmak için akıllı bir yola ihtiyacımız var. Girişte, USD ile sabitlenmiş stablecoin’lerle değiştirmek (satmak) yerine onları olduğu gibi kullanmanın daha iyi bir fikir olabileceğini gördük.

Şu senaryoyu da düşünün: Kanada dolarınız var ve Ethereum'dan yararlanmak istiyorsunuz. Gerçekten de risk almadan Ethereum satın alabilseydiniz güzel olmaz mıydı? Eh, kredi piyasaları bunun için var!!!

### Market.xyz

[Market.xyz](https://www.market.xyz/) kripto varlıklarınızın bir kısmını diğer varlıkları borç almak için teminat olarak kullanabileceğiniz bir borç verme protokolüdür. Kısa bir süre önce %100 Jarvis sentetik FIAT'lara özel yeni bir havuz başlattılar: https://polygon.market.xyz/pool/7

![Jarvis Forex, Mart 2022 itibarıyla Market.xyz'e kilitlendi](<../../.gitbook/assets/Jarvis-9.png>)

Gördüğünüz gibi jFIAT'larınızı borç verebilir ve borç alanlardan faiz kazanabilirsiniz. Locker ayrıca bazı LP (Likidite Sağlayıcı) tokenlarını teminat olarak kabul eder. Bu, m2CAD veya m2JPY'nizi borç verebileceğiniz ve yine de bunlar üzerinden ~%27 APY (Yıllık Yüzde Getiri) kazanabileceğiniz ve pozisyonunuzdan yararlanmak için jCAD veya jJPY gibi diğer jFIAT'ları borç alabileceğiniz anlamına gelir. Ayrıca, Mai Finance'in arkasındaki QiDAO protokolü tarafından oluşturulan USD sabitli stablecoin olan MAI'yi de borç alabilirsiniz. QiDAO topluluğu, Market.xyz'deki Jarvis locker’dan MAI kredilerinde düşük faiz oranını korumak için düzenli olarak yeni MAI sağlamayı kabul etti.

{% hint style="danger" %}
Market.xyz locker’larında minimum 0,05 ETH tutarında bir borçlanma tutarı vardır ve bu tutar Mart 2022 itibarıyla 150$'a eşittir. Sağlıklı bir Teminat Borç Oranına sahip olmanız gerektiğinden, platformdan kredi almak istiyorsanız yeterli teminat yatırdığınızdan emin olun.
{% endhint %}

Polygon'daki herhangi bir borç verme platformunda olduğu gibi Market.xyz de Borç Oranına karşı sağlıklı bir Teminat uygulayacaktır. Bu, her bir teminatın LTV'sinin temsil ettiği şeydir (Krediden Değere, CDR'nin tersi). Örnek olarak, m2CAD'in LTV'si %60'tır, yani borcunuz ile teminat değeriniz arasındaki oranın %60'ın üzerinde kalması gerekir.

m2CAD durumunda, teminat, borç alacağınız MAI'ye (ABD dolarına sabitlenmiş) göre değişebilen Kanada Dolarına sabitlenir. Bununla birlikte, varyasyon çok küçüktür, bu nedenle teorik olarak %60 eşiğine çok yakın borç alabilirsiniz. Kılavuzumuzda, 0,4'lük bir LTV'ye (1 / 2,5 = 0,5) karşılık gelen %200'lük bir CDR'ye bağlı kalmaya çalışacağız. 0,05 ETH değerinde MAI'yi borç alabilmek için gerekli teminat değeri:

$$
AvailableCollateral = \frac{Debt Value}{LTV} = \frac{0.05 ETH}{0.4} = 300\$
$$

Bugün USD:CAD oranı 1:0.7972 olduğundan, bir başlangıç yatırımına ihtiyacım olacak

$$
InvestmentCAD = \frac{300}{0.7972} = 376.32 CAD
$$

{% hint style="info" %}
300$ değerinde CAD yatırımı yaptığımı ve 150$ değerinde MAI borç aldığımı varsayarsak, şu anda teminatımdan %27 APY (%23,91 APR) kazanacağım ve kredime %11,28 faiz ödemem gerekecek. 1 yıllık süre içinde bu, teminatımın 81$'lık ve ödenmesi gereken 16.92$'lık faizin büyümesini temsil ediyor.
{% endhint %}

Şimdi USD sabitli kredinizi ne yapacağınıza bakalım.

### Uniswap V3

[Uniswap V3](https://app.uniswap.org/) kullanıcıların varlıklarını diğer kripto para birimleriyle değiştirebilecekleri ve bu değişimleri desteklemek için likidite sağlayabilecekleri birçok DEX'in (Merkeziyetsiz Borsalar) ana projesi olan Uniswap'in en son sürümüdür.

UUniswap V3, Polygon için teşvik edilmedi (henüz), ancak likidite sağlamanın yeni bir yolunu sunuyor: konsantre likidite! Likidite sağlamak istediğiniz aralığı seçersiniz ve aralık çok dar ise daha geniş bir aralıkta likidite sağlayan kullanıcılardan daha fazla ücret kazanırsınız. Uniswap V3'te likidite çiftlerini resmi kılavuzlarıyla nasıl sağlayacağınızı öğrenebilir ve ayrıca Finematics'in UniswapV3'teki [şaşırtıcı videosunu izleyebilirsiniz.](https://youtu.be/Ehm-OYBmlPM)

Bu eğitimde, bir miktar MAI borç aldığımız için MAI-USDC çiftine odaklanmak ve stablecoin farming’i yaparak riske maruz kalmayı sınırlamak istiyoruz.

Yapılacak ilk şey bir hedef aralığı tanımlamaktır. Artık sürekli artan likidite, daha fazla havuz ve fiyatı sabit tutmaya yardımcı olan Curve havuzu gibi bazı mekanizmalar nedeniyle MAI'nin fiyatı çok daha stabil olduğuna göre, MAI:USDC için 1:1 oranını hedefleyeceğiz. Gerçekte, 1 MAI 0.998 USDC'ye daha yakındır.

Piyasa koşullarına bağlı olarak 1 MAI için beklenen fiyat aralığı 0,99 ile 1,01 USDC arasındadır. Değişken varlıklar arttığında, insanlar daha fazla borçlanma gücüne sahip olur ve çok fazla MAI değiştirme eğiliminde olup fiyatını düşürür. Piyasa daraldığında ve insanların tasfiyeyi önlemek için borçlarını geri ödemeleri gerektiğinde bunun tam tersi bir etki meydana gelir: MAI, borçları geri ödemek için piyasadan satın alınır ve fiyatı artar. Aslında, gerçek fiyat aralığı, MAI başına 0,994 ile 1,004 USDC arasında olma eğilimindedir.

![LP'nizi geniş veya dar bir pozisyona yaymak topladığınız ücretler üzerinde büyük bir etkiye sahip olacaktır.](<../../.gitbook/assets/Jarvis-10.png>)

Aslında anlamanız gereken şey,

* Geniş bir aralık seçerseniz likiditeniz daha geniş bir aralığa yayıldığından, dar bir aralık seçtiğinizden daha az ücret alırsınız.
* Dar bir aralık seçerseniz ve fiyat bu aralığın dışına çıkarsa ücret almazsınız.
* Likiditeniz fiyata göre ayarlanmaz. MAI:USDC için [0.99;1.01] aralığı seçerseniz ve MAI fiyatı 0.99 USDC ise %100 MAI ve %0 USDC'ye sahip olursunuz. Öte yandan, fiyat MAI başına 1,01 USDC ise, %100 USDC ve %0 MAI'ye sahip olursunuz.
* İlk kurulumunuzun yeterli ücret toplamadığını görürseniz istediğiniz zaman likidite havuzunuzdan çıkabilir ve daha geniş / daha dar bir aralıkta yeni bir tane oluşturabilirsiniz.
* Stablecoin’ler için, kullanıcılar stablecoin’lerini değiştirirken zapper veya 1inch gibi toplayıcıların havuzunuzu seçmesi için %0.05'lik bir ücret aralığı belirlemek daha iyidir.

Kolaylık olsun diye bu kılavuzda, MAI başına 0.995 ile 1.005 USDC arasında %1'lik bir dağılımla 1.000 merkezli bir aralık belirleyeceğiz

![MAI-USDC çifti için konsantre bir likidite havuzu oluşturma](<../../.gitbook/assets/Jarvis-11.png>)

{% hint style="info" %}
Çiftiniz için token sırasına dikkat edin. Yani, önce MAI (mimatik) ve ikinci olarak USDC'yi seçmeniz ile önce USDC'yi ve ikinci olarak MAI'yi seçmenizde fiyat aralığı aynı olmayacaktır !!!
{% endhint %}

Kurulumunuza bağlı olarak, MAI ve USDC olarak ödenen LP'nizi %8 APR (geniş aralık) ile %20 APR (dar aralık) arasında bekleyebilirsiniz. Bu, büyük ölçüde UniswapV3'te yürütülen işlemlerin fiyat hareketine ve hacmine bağlı olacaktır. Bu aracı, işlemlerinizi çok düşük bir fiyat etkisi ile yürütmek ve kendi işlemlerinizden ücret toplamak için de kullanabileceğinizi unutmayın!

## Farming Stratejisi

Bu strateji için başlangıç noktamız olarak Jarvis'i kullanacağız. Bunun için Mt. Pelerin üzerinden satın alınan jCAD'i kullanacağız. jCAD, 2CAD LP tokenı almak için Curve Finance'te uygun havuza yatırılacaktır. Bu LP tokenı, Jarvis tarafından sağlanan takas ücretleri ve ödül tokenlarının ek 2CAD'e dönüşebilmesi için Beefy'ye yatırılacaktır. Depozito kanıtı olarak, %200 CDR (%50 LTV) ile MAI borç almak için daha sonra Market.xyz'de kullanabileceğimiz mooJarvis2CAD tokenlarını alacağız. MAI kredisi, UniswapV3'te likidite sağlayan bir token oluşturmak için kullanılacak, böylece takas ücretlerini %12 APR'de tahsil edebilecek.

Bu ilk kurulum, CAD ile ilgili olarak USD'nin fiyat değişikliklerinden etkilenmemenizi sağlar. Ayrıca borç alınan miktar UniswapV3 havuzunda güvence altına alınır ve herhangi bir zamanda geri ödenebilir.

Hem 2CAD hem de UniswapV3 havuzlarından elde edilen kazançlar, bir "ödül artırıcıya", yani ilk yatırım veya kredi üzerinde 0 etkisi olacak ancak aslında yüksek bir ödül oranından elde edilen kazançları artıracak bir havuza eklenecektir. 2CAD havuzundan daha yüksek bir ödül oranına sahip hemen hemen her havuzu kullanabilirsiniz. QuickSwap'ta cxDOGE/cxETH (Mart 2022 itibarıyla %44,24 APY) gibi bir likidite havuzu veya Klima (Mart 2022 itibariyle %944 APY) gibi bir ohm-klonu olabilir. Simülasyonumuz için JRT-MAY22-USDC havuzunu doğrudan Jarvis Network üzerinde kullanacağız.[Likidite Kyber Network](https://kyberswap.com/#/add/0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174/0xF5f480Edc68589B51F4217E6aA82Ef7Df5cf789e/0xdaa2c66b06b62bad2e192be0a93f895c855484ee) üzerinden satın alınabilir/eklenebilir ve USDC ile Jarvis Network'ten yerel bir token kullanır. Bu LP tokenı şu anda %143 APR alıyor.

Bu strateji, stablecoin’lere odaklanıyor, ancak aynı zamanda birçok olası varyasyon sunuyor:

* Bu FIAT'ları jCAD yerine tercih ederseniz 2JPY veya 2SGD kullanabilirsiniz.
* Market.xyz'de jCAD'inizi (veya herhangi bir jFIAT'ı) borç verebilir ve borç alan kişilerden borç alma ücreti alabilirsiniz.
* Market.xyz'den aldığınız krediyi UniswapV3'te likidite sağlayacağınız herhangi bir token ile değiştirebilirsiniz. Tercih ettiğiniz havuzu seçin, ancak potansiyel kalıcı kayıplara dikkat edin.
* UniV3'te topladığınız ücretleri Mai Finance'de kabul edilen herhangi bir şeyle (BTC, CRV, LINK, GHST ...) değiştirebilir ve Mai Finance'ten aldığınız krediyi kullanarak Market.xyz'deki kredinizi geri ödeyebilir, %11'lik kredinizi %0'lık bir krediye transfer edebilirsiniz.
* Market.xyz'deki kredinizi daha hızlı geri ödemek için toplanan ücretleri de kullanabilirsiniz.
Olasılıklar sonsuzdur


Her zaman olduğu gibi, simülasyon için birkaç şeyi varsayacağız:

* 2CAD için APY %27 APY'dir (%23.91 APR)
* Market.xyz'deki kredinin faiz oranı %11,28'dir.
* UniswapV3'teki konumunuzun APR'si %12'dir (daha güvenli ama daha az verimli)
* Jarvis Network'te JRT-MAY22-USDC ödül artırıcıda %143 APR alacaksını

![](<../../.gitbook/assets/Jarvis-12.png>)

{% hint style="info" %}
Bu sistemde simülasyonlar çalıştırmak istiyorsanız bu stratejiye bağlı [Google E-Tablosunu ](https://docs.google.com/spreadsheets/d/10-n5IyZLl0GZyjM16SNuVOONNsfJ15pm2GL0e2MagzE/edit?usp=sharing) kullanabilirsiniz. Bu döngüden alabileceğiniz nihai APY'yi tahmin etmek için farklı ödül oranlarını veya istenen CDR'yi değiştirmeniz yeterlidir.

{% endhint %}

### 1. gün

Sisteminizi şunları yaparak başlatmanız gerekir:

* Jarvis Network'te 300$ değerinde USDC'yi jCAD ile değiştirin (veya jCAD'i doğrudan Mt. Pelerin aracılığıyla satın alın)

* jCAD'i [pool #23](https://polygon.curve.fi/factory/23/deposit)’te Curve Finance'e yatırın 
* 2CAD LP tokenını [Beefy Finance’e](https://app.beefy.finance/#/polygon/vault/jarvis-2cad)yatırın 
* Beefy makbuz tokenını Market.xyz'e yatırın
* MAI'yi bir CDR veya %200 (%50 LTV) ile borç alın
* MAI'nizin bir kısmını Uniswap V3'te USDC ile değiştirin ve MAI ve USDC'yi seçtiğiniz parametrelerle yeni bir likidite havuzuna yatırın

Farming’in 1. gününden sonra,

|     pozisyon     |  değer ($) |
|------------------|------------|
| mooJarvis2CAD    |    300.000 |
| 2CAD rewards     |      0.197 |
| MAI-USDC UniV3   |    150.000 |
| UniV3 fees       |      0.049 |
| JRT-MAY22-USDC   |      0.000 |
| Jarvis rewards   |      0.000 |
| MAI debt         |    150.000 |

Tamamen hazırsınız, gerisi basit bakım ve ödülleri Jarvis havuzuna taşımak.

### Günlük Rutin

Kazanımlarınızı ödül artırıcıya koyma zamanı:

* Uniswap V3'te MAI ve USDC toplayın
* mooJarvis2CAD'inizin birleşik olana karşılık gelen küçük bir kısmını çıkarın
* Jarvis Network'te ödülü toplayın
* Kyber Network'te her şeyi JRT-MAY22 ve USDC ile değiştirin ve LP tokenları oluşturun
* LP tokenını Jarvis Network'e yatırın

2. günün sonunda,

|     pozisyon     |  değer ($) |
|------------------|------------|
| mooJarvis2CAD    |    300.000 |
| 2CAD rewards     |      0.197 |
| MAI-USDC UniV3   |    150.000 |
| UniV3 fees       |      0.049 |
| JRT-MAY22-USDC   |      0.246 |
| Jarvis rewards   |      0.001 |
| MAI debt         |    150.000 |

### Aydan aya ham sonuçlar

Yukarıda bağlantısı verilen Google E-Tabloda bulabileceğiniz gibi, aydan aya ham sonuçlar aşağıdadır.
 
| gün | mooJarvis2CAD | MAI-USDC  | JRT-MAY22-USDC |  MAI borç|
|-----|---------------|-----------|----------------|-----------|
|  30 |       300.000 |   150.000 |          7.534 |   151.350 |
|  60 |       300.000 |   150.000 |         16.282 |   152.760 |
|  90 |       300.000 |   150.000 |         26.118 |   154.182 |
| 120 |       300.000 |   150.000 |         37.179 |   155.618 |
| 150 |       300.000 |   150.000 |         49.616 |   157.067 |
| 180 |       300.000 |   150.000 |         63.601 |   158.530 |
| 210 |       300.000 |   150.000 |         79.326 |   160.007 |
| 240 |       300.000 |   150.000 |         97.009 |   161.497 |
| 270 |       300.000 |   150.000 |        116.893 |   163.001 |
| 300 |       300.000 |   150.000 |        139.252 |   164.519 |
| 330 |       300.000 |   150.000 |        164.393 |   166.051 |
| 360 |       300.000 |   150.000 |          7.343 |     0.000 |

### Day 365

%200'lük bir CDR ile 11. ay boyunca tüm borcunuzu geri ödersiniz, isterseniz ilk CAD'yi serbest bırakır, isterseniz banka hesabınıza geri aktarabilirsiniz, ve hala şunlara sahip olursunuz:

* 150$ değerinde MAI-USDC
* Jarvis'te 7.343$ değerinde LP

Genel toplam için %52,91 APY.

{% hint style="info" %}
2CAD likidite havuzunuzdan elde ettiğiniz kârı Jarvis'teki JRT-MAY22-USDC havuzuna yatırırsanız ortasına Market.xyz eklemeden toplamda %52,68 APY elde edersiniz. Ayrıntılar için Google E-Tablosundaki 2. sayfaya bakabilir veya CDR'yi 1.000.000 olarak ayarlayabilirsiniz.
{% endhint %}

## Sorumluluk Reddi

Bu kılavuz çoğunlukla, Mt. Pelerin ve Jarvis Network'ü kullanarak FIAT'lerinizi kripto varlıklara (ya da tam tersi) nasıl dönüştürebileceğinizi göstermek için yazılmıştır. ABD vatandaşı olmayanlar için bu, neredeyse hiç ücret ödemeden bir "dünyadan" diğerine para aktarmak için çok güzel bir fırsattır. Sentetik FIAT'larınızı Polygon'dan da alabilmeniz, gas maliyetleri ve işlem süresi DeFi için en iyiler arasında olduğundan ekstra verimli hale getirir.

Ayrıca, giderek daha fazla birinci sınıf uygulamanın jFIAT'ları, özellikle de jEUR ve EURS borç verme piyasalarını önermeye başlayan AAVE v3'ü kullandığını ve TradFi'dan (Geleneksel Finans) DeFi'ya geçişi kolaylaştırdığını belirtmek gerekir.

Bu kılavuzda önerilen strateji, tüm fiyatların ve oranların aynı kaldığını varsaymaktır ki bu açıkça gerçek hayatta olan bir şey değildir. Borcunuzu geri ödeyebilmek için herhangi bir yatırım yapmadan önce ödül borçlanma oranlarına dikkat ettiğinizden emin olun

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}
