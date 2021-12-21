---
description: >-
  Stablecoin ile farming ödülleri genellikle düşük oranlara sahiptir. Yeni bir yatırım döngüsü ile kazançlarınızı nasıl artırabileceğinizi innceleyelim.
---

# CroDex ile Legos Farming

Yield farming belli açılardan kolay olabilir. 2 tokenınız var, bunları bir LP (Likidite Sağlayıcı) çiftinde birleştiriyorsunuz, LP tokenını bir havuza yatırıyorsunuz ve takas ücretleri ile çoğu zaman kullandığınız farmın yerel tokenıyla ödenen ödülleri almaya başlıyorsunuz. Çoğu insan, çoğu zaman tamamen geçerli ancak optimize edilmiş bir çözümden çok uzak olan aradıkları varlık için ödülü satar. Bugün, Cronos'ta birkaç DApp'te önerilen çok yüksek APR'den (Yıllık Yüzde Oranı) nasıl kâr edebileceğinizi göreceğiz. Bu yöntem ile stablecoin’de %30'luk bir APR'yi çok daha yüksek bir orana dönüştürecektir. 

![](../../.gitbook/assets/crodex-lego-1.png)

## CroDex

### MAI ile Farming

Mai Finance'in kredi uygulaması henüz Cronos'ta yayında olmasa olsa bile MAI'yi diğer zincirlerden köprülemek zaten mümkün. Bunu yapmanın nedenlerinden biri Cronos'ta çok fazla MAI olmamasıdır. MAI ile farming öneren herhangi bir uygulamanın aynı zamanda yüksek APR'ler sağlayacağı anlamına gelir diyebiliriz. Şu anda Cronos'ta MAI likiditesine sahip tek yer olan CroDex'in durumu budur. Bu kılavuzda ilk yatırımınızda Geçici Kayıp riskini azaltmak için CroDex'teki MAI-USDC havuzunu kullanacağız ancak MAI-CRO ile farming yaparak kazançlarınızı artırabilirsiniz.

![Aralık 2021 itibarıyla CroDex'te MAI-USDC LP havuzu](../../.gitbook/assets/crodex-lego-2.png)

{% hint style="info" %}
Verimi toplamak için bir uygulama seçtiğinizde ödülün APR (Yıllık Yüzde Oranı) veya APY (Yıllık Yüzde Verim) olarak görüntülenip görüntülenmediğini not etmeniz önemlidir. İkincisi, aldığınız tüm ödüllerin bir tam yıl boyunca günlük olarak birleştirildiğini varsayar. Örneğimizde, MAI-USDC çiftindeki %30 APR, %34,97'lik bir APY'ye karşılık gelir.

Bunu Mai Finance'deki MAI-USDC havuzuyla karşılaştırırsanız verilen APR Polygon'da %20.18, Fantom'da %22.10'dur ve Avalanche'daki MAI-av3CRV havuzu %23.24 APR önerir. CroDex, tüm zincirlerde MAI en iyi oranı önerir!
{% endhint %}

CroDex size yerel tokenları olan CRX ile ödeme yapacaktır. Aralık 2021 itibariyle 1 CRX = 127,56 USDC

### Tek yönlü CRX Staking

İşte işler bu noktada ilginçleşiyor. CroDex, ek ödüller için CRX tokenlarınızı stake edebileceğiniz iki farklı havuza sahiptir. Daha fazla CRX elde etmek için stake yapabilirsiniz ancak CRX stake etmenin sizi wCRO tokenlarıyla ödüllendireceği havuzu kullanacağız. wCRO, Cronos ağının gas tokenı olan CRO'nun sarılı (wrapped) versiyonudur.

![Aralık 2021 itibarıyla CroDex'te tek staking CRX](../../.gitbook/assets/crodex-lego-3.png)

Daha fazla MAI-USDC LP tokenı karşılığında CRX'inizi çok iyi bir şekilde satabileceğinizi ve istikrarlı çiftte neredeyse %35 APY alabileceğinizi zaten biliyorsunuz ancak CRO almak için CRX'inizi stake etmek net olarak daha iyidir. Yalnızca işlem ücretlerini ödemek için kullanılmaz aynı zamanda MAI-CRO'yu CroDex’te de toplayabilirsiniz. Ve zamanla ne kadar çok CRX alıp CRX'inizi stake ederseniz o kadar çok CRO elde edersiniz. Bu rehberde Cronos'u biraz daha keşfedeceğiz!

## CRYSTL Finance

CRYSTL Finance, Polygon’da Polycrystal olarak bilinirdi. LP çift kasaları ve tek staking havuzları öneren bir Goose klonudur ve tam olarak Beefy Finance gibi çalışır. Her ikisini de stratejimiz için kullanacağız.

### CRX-WCRO ile CRYSTL Farming

Ödülün %50'sini daha fazla CRX ile takas etmek ve bu iki tokenı CroDex'te bir CRX-WCRO çiftinde birleştirmek için CRX staking tarafından üretilen CRO tokenlarını kullanacağız, ardından LP tokenını Crystl Finance'te bir kasaya yatıracağız. Bu size bileşik olacak yüksek bir APY kazandıracak.

![Aralık 2021'den itibaren Crystl Finance'te CRX-WCRO Farming](../../.gitbook/assets/crodex-lego-4.png)

Görüntülenen oranlar bir APY'dir. %1,21k APY, %258,17 APR'ye karşılık gelir ancak tahmini günlük kazançları doğrudan kasa bilgisinden de alabilirsiniz. CRX-WCRO farming şu anda size %0,71 günlük kazanç sağlayacaktır. Günlük ödülü takip etmeniz çok önemlidir çünkü LP pozisyonumuzun bu kısmını çıkaracağız ve ayrı tokenlara ayıracağız. CRX, daha fazla CRO tokenı almak için CroDex'te yeniden stake edilecek ve CRO, CRYSTL ile değiştirilecektir. Ayrıca her gün elde edeceğimiz kazançlar için bir para çekme ücreti olduğunu da unutmayın.

### Tek Taraflı CRYSTL Staking

Önceki adımda elde edilen CRYSTL tokenı ile CRYSTL Finance'in tek staking havuzundan USDC alabileceksiniz. Sadece CRYSTL tokenınızı stake edip oldukça yüksek bir APR ile USDC olarak ödeme alacaksınız.

![Aralık 2021 itibariyle USDC veya SALEM için CRYSTL staking](../../.gitbook/assets/crodex-lego-5.png)

Ardından USDC'nin %50'sini MAI ile takas edebilir ve CroDex'teki orijinal konumunuza geri ekleyebilirsiniz.

Alternatif olarak, yukarıdaki ile aynı yaklaşımı kullanarak Salem Finance'in yerel tokenı olan SALEM tokenlarını kazanmak için CRYSTL tokenlarını stake edebiliriz.

## Salem Finance

Salem Finance, SALEM tokenını toplayabileceğiniz başka bir Goose klonudur. Çoğu LP havuzunun bir depozito ücreti vardır ancak CRYSTL Finance bize zaten ihtiyacımız olan SALEM tokenlarını verdiği için LP farmlarını kullanmayacağız. Bunun yerine bir kez daha çok yüksek bir APR ile ek WCRO kazanmak için SALEM'leri havuzlara stake edeceğiz.

![Aralık 2021 itibariyle WCRO için SALEM staking](../../.gitbook/assets/crodex-lego-6.png)

w)CRO tokenı, Cronos'un gas tokenı olduğundan çok fazla faydası vardır. İsterseniz bunu ana Crypto.org zincirine de bağlayabilirsiniz. Bizim durumumuzda, yatırım döngümüzü kapatmak istediğimizden, Salem Finance'ten elde ettiğimiz kazançları satabilir ve daha fazla USDC ve MAI satın alabiliriz

## Farming Stratejisi

Zaten sadece 3 protokolle birkaç seçeneğiniz olduğunu göreceksiniz:

* CRX almak için MAI-USDC ile farming, WCRO almak için CRX'i staking, daha fazla MAI-USDC için WCRO satmak
* CRX almak için MAI-USDC ile farming, WCRO almak için CRX'i staking, CRYSTL almak için CRX-WCRO ile farming, USDC almak için CRYSTL'yi staking, USDC'yi daha fazla MAI-USDC ile değiştirmek
* CRX almak için MAI-USDC ile farming, WCRO almak için CRX staking, CRYSTL almak için CRX-WCRO ile farming, SALEM almak için CRYSTL staking, WCRO almak için SALEM staking, daha fazla MAI-USDC için WCRO satmak

Bu kılavuzun geri kalanında en karmaşık olan ve birçok manipülasyon gerektiren ancak aynı zamanda genel olarak en iyi sonucu veren son stratejiye odaklanacağız. Risk kabulünüze bağlı olarak tercih ettiğinizi uygulamakta özgürsünüz.

![](../../.gitbook/assets/crodex-lego-7.png)

### Sistemin Ateşlenmesi

Aşağıda 1.000$ değerinde MAI-USDC LP tokenları ve bu belgede Aralık 2021 itibariyle sunulan mevcut APR'ler/APY'ler ile yapılan bir simülasyon yer almaktadır. Elbette oranlar ve fiyatlar zamanla değişecektir, bu nedenle bu simülasyon yalnızca yazıldığı sırada geçerlidir ve simülasyon yalnızca bu sistemi kurarsanız potansiyel olarak ne elde edebileceğinize dair bir tahmin sağlar.

### 1.gün

MAI-USDC'nizi uygun havuzda CroDex'e yatırırsınız ve %30 APR alırsınız. İlk günün sonunda CRX ödüllerinizi topladığınızda,

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM | WCRO  |
| -------- | ---------- | -------- | ------ | ----- | ----- |
| 1,000.00 | 0.822      | 0.000    | 0.000  | 0.000 | 0.000 |

### 2.gün

Stake edilen CRX'iniz WCRO üretiyor. Ödülü toplayabilir ve daha sonra CRYSTL Finance'e yatırabileceğiniz bir CRX-WCRO L çifti oluşturmak için %50'sini daha fazla CRX'e çevirebilirsiniz. İkinci günün sonunda,

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM | WCRO  |
| -------- | ---------- | -------- | ------ | ----- | ----- |
| 1,000.00 | 1.644      | 0.002    | 0.000  | 0.000 | 0.000 |

### 3.gün

CRYSTL Finance kasasında kilitlenen CRX-WCRO çifti, ek LP tokenı üretti. Günlük kazancı çıkarmanız ve %0,1 ücret ödemeniz ve çıkarılan LP bölümünü CRX ve WCRO tokenlarına ayırmanız gerekecek. CRX'i CroDex'te yeniden alabilir ve WCRO'yu CRYSTL ile değiştirebilirsiniz. Bu, [takas özelliği kullanılarak CroDex](https://swap.crodex.app/#/swap?outputCurrency=0xCbDE0E17d14F49e10a10302a32d17AE88a7Ecb8B) te yapılabilir. Günün sonunda;

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL  | SALEM | WCRO  |
| -------- | ---------- | -------- | ------- | ----- | ----- |
| 1,000.00 | 2.466      | 0.005    | 0.00003 | 0.000 | 0.000 |

{% hint style="info" %}
CRYSTL'deki ödüllerin çok küçük olduğunu ve ödülü 1. günden toplamanın iyi bir fikir olmayabileceğini unutmayın. Bu simülasyon hala almanız gereken ödülleri gösteriyor. Yine de günlük olarak birleştirdiğinizi varsayacaktır. Ancak bu, sonuçları basitleştirmek için yapılmıştır. Tüm ödülünüzü işlem ücretlerine harcamadığınızdan emin olun. İlk birkaç haftanın yalnızca haftalık olarak birleştirilmesi daha iyi olabilir.
{% endhint %}

### 4.gün

SALEM tokenları kazanmak için Crystl Finance'ten CRYSTL ödülünüz yatırılabilir. Dördüncü günün sonunda,

| MAI-USDC | staked CRX | CRX-WCRO | CRYSTL  | SALEM     | WCRO  |
| -------- | ---------- | -------- | ------- | --------- | ----- |
| 1,000.00 | 3.288      | 0.010    | 0.00011 | 0.0000002 | 0.000 |

### 5.gün

Salem Finance'ten ödülleri toplayacağınız son önyükleme günü. WCRO ödülü daha fazla MAI-USDC ile değiştirilebilir. Ancak fark edebileceğiniz gibi ödülün değeri o kadar küçüktür ki Salem Finance'ten WCRO'yu 50. Günden önce toplayamazsınız.

## Farming Sonuçları

### Günlük Rutin

Sistem tamamen hazır olduğunda günlük rutininiz

* MAI-USDC havuzundan CRX toplayın
* CroDex'teki tek staking havuzundan WCRO ödülünü toplayın
* CroDex'te daha fazla CRX için WCRO ödülünün %50'sini değiştirin ve bir miktar CRX-WCRO LP tokenı oluşturun
* İlave CRX-WCRO tokenınızı CRYSTAL Finance'e yatırın
* Günlük ödülünüze karşılık gelen CRX-WCRO'nun bir kısmını geri çekin
* LP tokenını CroDex'te CRX ve WCRO'ya ayırın
* CRX'i, WCRO ödülleri alan CroDex'teki tek staking havuzuna stake edin
* CroDex'te WCRO'yu CRYSTL ile değiştirin
* SALEM tokenlarını almak için CRYSTL tokenını Crytl Finance'e yatırın
* SALEM tokenını toplayın
* Salem Finance'te SALEM tokenını tek stake edin
* Salem Finance'ten WCRO tokenını toplayın
* WCRO'yu MAI ve USDC ile değiştirin ve daha fazla LP çifti oluşturun
* Yeni MAI-USDC çiftini CroDex'teki uygun havuza yatırın

### Aylık Ham Sonuçlar

| day | MAI-USDC | staked CRX | CRX-WCRO | CRYSTL | SALEM  |
| --- | -------- | ---------- | -------- | ------ | ------ |
| 30  | 1,000.00 | 25.583     | 0.600    | 0.104  | 0.004  |
| 60  | 1,000.00 | 50.819     | 1.830    | 0.682  | 0.059  |
| 90  | 1,000.04 | 76.736     | 3.315    | 1.941  | 0.260  |
| 120 | 1,000.14 | 103.424    | 4.922    | 3.970  | 0.729  |
| 150 | 1,000.41 | 130.935    | 6.606    | 6.816  | 1.594  |
| 180 | 1,001.93 | 159.307    | 8.352    | 10.515 | 2.994  |
| 210 | 1,001.87 | 188.578    | 10.156   | 15.094 | 5.070  |
| 240 | 1,003.39 | 218.789    | 12.019   | 20.584 | 7.969  |
| 270 | 1,005.71 | 249.988    | 13.942   | 27.014 | 11.843 |
| 300 | 1,009.10 | 282.227    | 15.929   | 34.414 | 16.848 |
| 330 | 1,013.82 | 315.569    | 17.982   | 42.817 | 23.147 |
| 360 | 1,020.23 | 350.084    | 20.105   | 52.256 | 30.906 |

### 365.gün

Bu sistemle tam bir yıl farming yaptıktan sonra,

* CroDex'te 1.021.49$ değerinde MAI-USDC
* CroDex'te tek stake edilen 355,96$ değerinde CRX
* CRYSTL Finance'e yatırılan 20,47$ değerinde CRX-WCRO
* CRYSTL Finance'te tek stake edilen 53,93$ değerinde CRYSTL 
* Salem Finance'te tek stake edilen 32.353$ değerinde SALEM

Salem Finance'ten WCRO, bu çifti artırmak için tamamen satıldığından dolayı ek MAI-USDC pozisyonu olarak dahil edilmiştir.

1.000$'lık bir ilk yatırımla yıl sonunda tüm uygulamalarda 1.484,45$'a ve toplam %48,45 APY'ye sahip olacağınız anlamına gelir. Bunun, stratejinin kökü olarak yalnızca stabil bir çift farm edilerek yapıldığını unutmayın. Zaman içinde değiştirilen tek tokenın CRO tokenı olduğunu da belirtmekte fayda var.

### Mai Finance'in Alternatif Kullanımı

Mai Finance uygulaması, Cronos'taki kasaları desteklemez çünkü Cronos'taki tokenlarda henüz Chainlink Oracles yoktur. 2022'nin ilk çeyreğinde Chainlink'in Cronos'a oracle eklemesi ve MAI stablecoin’ini borç almak için WCRO tokenlarınızı bir Kasaya yatırabilmeniz bekleniyor. Bu, yukarıdaki stratejinin WCRO yatırmak ve WCRO tokenlarını satmak yerine MAI kullanmak için değiştirilebileceği anlamına gelir ve bu da nihai ödül oranınızı biraz artıracaktır.

![Mai Finance üzerinde WCRO kasası (emulation)](../../.gitbook/assets/crodex-lego-8.png)

## Sorumluluk reddi

Bu kılavuz, topladığınız tokenların değerini düşürmeden ödül oranınızı artırabileceğinizi göstermek için yazılmıştır. Döngüleri oluştururken doğru uyumu bulmak kolay değil ancak kesinlikle uygulanabilir ve çoğu zaman doğru kombinasyonu bulabilirseniz ödüllendirilirsiniz. Ancak bu kılavuz sadece bunu nasıl yapabileceğinizi göstermek için yazılmıştır, benzer bir sistem kurmak için değil. Tüm işlem ücretleri bilerek atıldı ve bazı ödüller tam bir yıl sürmez, bu da kişisel yatırımlarınız için daha basit döngüler düşünmek isteyebileceğiniz anlamına gelir. Ancak CroDex bu tür bir sistem için çok iyi bir başlangıç noktasıdır.

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınıza yatırım yapın.
{% endhint %}
