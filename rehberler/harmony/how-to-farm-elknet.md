---
description: >-
  Bu kılavuz, stake etme ve birleştirme arasındaki farkları göstermek için tek bir LP çifti oluşturmanın farklı yollarını sunar.
---

# Bir LP ile Çiftçilik Yapmanın Farklı Yolları

## Giriş

Bir DEX'te (Merkeziyetsiz Borsa) likidite ve çiftçilik ödülü sağlamak DeFi'de (Merkeziyetsiz Finans) verim toplamanın en yaygın yollarından biridir. Bununla birlikte birçok kullanıcı, oranın bir APR (Yıllık Yüzde Ödül) veya bir APY (Yıllık Yüzde Getiri) olup olmadığını gerçekten kontrol etmeden yalnızca girdikleri LP (Likidite Sağlayıcı) havuzunun oranlarına dikkat etmektedir. Bir havuz oluşturmanın ve ödül tokenlarını yönetmenin birçok yolu vardır. Bu kılavuzda Harmony'deki en yeni havuzlardan biri olan MAI-ELK’in çiftçiliğini yapmanın farklı yollarından bazılarını ve ödül olarak alacağınız ELK tokenlarıyla neler yapabileceğinizi göreceğiz.

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}

![](<../../.gitbook/assets/elk-farming-1.png>)

## Elk Finance

[Elk Finance](https://app.elk.finance/#/) Uniswap v2'den klonlanmış bir DEX'in yanı sıra bir AMM'dir (Otomatik Piyasa Yapıcı). Uniswap klonlarının tüm olağan özellikleri mevcuttur: varlıklarınızı takas etme, farklı kripto para birimlerinizi LP tokenlarında birleştirme, bazı LP çiftlerini toplama ve yerel tokenları ELK'i stake etme.

Ancak Elk Finance'i tamamen farklı bir proje yapan şey, sadece EVM uyumlu zincirlerde değil, birçok blok zincirinde bulunmasıdır. Elk Finance şu anda 16 zincirde mevcut ve diğerlerine de genişlemeyi planlıyor. Kullanıcıların ELK tokenını transfer etmesine izin vermek için tüm bu zincirler arasında bir köprü kurmayı başardılar: ELKNET.

![ElkNet'i kullanarak bazı ELK'leri Harmony'den Moonriver'a köprüleme](<../../.gitbook/assets/elk-farming-2.png>)

Ayrıca, ElkNet'in önerdiği bir başka harika özellik de transfer edilen varlığın bir kısmını varış noktasında bir miktar gas tokenı ile takas etme imkanıdır. Bu özellik, özellikle musluğun bulunmadığı bir blok zincirine ilk kez gidiyorsanız kullanışlıdır.

{% hint style="success" %}
Gas ücretinin yüksek olduğu zincirler dışında (yazı yazılırken yalnızca Avalanche ve Cronos), ELK tokenlarınızı bir zincirden diğerine köprülemek için ElkNet'i kullanmak hiçbir masraf gerektirmeden yapılır. Doğru okudunuz, herhangi bir köprü ücreti ödemiyorsunuz!
{% endhint %}

Son olarak Elk Finance, Kalıcı Kayıp koruması sağlar. Geçici Kayıp programıyla ilgili tüm ayrıntıları [resmi belgelerinden](https://docs.elk.finance/features/impermanent-loss-protection) okuyabilirsiniz. Temel olarak bilmeniz gereken tek şey ELK'in fiyatı para yatırdığınız an ile para çektiğiniz an arasında değişirse kalıcı kaybı karşılamak için fazladan ELK ödeyeceğinizdir. MAI 1 USD'ye sabitlendiğinden kalıcı kayıp yalnızca ELK'in fiyat hareketiyle bağlantılıdır, bu nedenle Elk Finance DEX'te LP havuzlarına girerken her zaman kazanan siz olursunuz. 

## MAI-ELK LP Çiftçiliği

Elk Finance, Ocak 2022'de DEX'lerinde MAI-ELK LP çiftini kullanarak token çiftçiliği önermek için Mai Finance ile ortaklık kurdu. MAI-ELK çifti şimdilik 3 farklı ağda kullanılabilir: Harmony, Moonriver ve Gnosis. Bazı ek havuzlar daha sonra Polygon, Cronos ve Fantom'da başlatılabilir. Bu yeni havuz için uygulayabileceğiniz farklı stratejilere bakalım.

{% hint style="info" %}
Harmony için bu kılavuzu öneriyoruz çünkü gas ücretleri çok düşüktür ve bu da ödülünüzü günlük olarak manuel birleştirmenize olanak tanır. Bu da onu deneme parası olarak yalnızca birkaç dolar yatırabilen yeni başlayanlar için çok iyi bir blok zinciri yapar. Ancak, bu kılavuzda sunulan her şey başka herhangi bir zincire de uygulanabilir.
{% endhint %}

### Çiftçilik ve Stake Etme

İlk strateji oldukça basittir:

* LP çifti yaratın
* LP'yi MAI-ELK havuzuna yatırın ve %200 APR kazanın
* ödüllerinizi günlük olarak toplayın
* %32.53 APR'de stake edin

100$ ile başladığınızı ve yukarıda verilen oranların tüm çiftçilik dönemi boyunca aynı kaldığını varsayarsak, tam bir çiftçilik yılı boyunca aydan aya alabileceğiniz sonuçlar aşağıdaki gibi olacaktır.

| gün | MAI-ELK ($) | staked ELK ($) |
|-----|-------------|----------------|
|  30 |     100.000 |         16.653 |
|  60 |     100.000 |         33.756 |
|  90 |     100.000 |         51.323 |
| 120 |     100.000 |         69.366 |
| 150 |     100.000 |         87.897 |
| 180 |     100.000 |        106.930 |
| 210 |     100.000 |        126.479 |
| 240 |     100.000 |        146.557 |
| 270 |     100.000 |        167.180 |
| 300 |     100.000 |        188.360 |
| 330 |     100.000 |        210.115 |
| 360 |     100.000 |        232.458 |

Yıl sonunda,

* Havuzda 100,00$ değerinde MAI-ELK LP tokenı
* 236,24$ değerinde stake edilmiş ELK tokenı

Bu da %236,24'lük genel bir APY'ye karşılık gelir. Tam olarak APR değil çünkü ödülün bir kısmı birleştirildi (stake edilmiş ELK).

{% hint style="info" %}
Bu tabloyu oluşturmak için kullanılan tüm sonuçları ve formülü aşağıdaki [Google Sheet'in](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) ilk sekmede bulabilirsiniz. Bu dosyayı kendi sürücünüze kopyalayabilir ve girdiğiniz sayı ile genel APY değişimini görmek için oranları ve ilk yatırımı ayarlayabilirsiniz.
{% endhint %}

### Çiftçilik ve Doğrudan Birleştirme

Birleştirme, ödüllerinizi topladığınız ve bunu ek LP tokenları oluşturmak için kullandığınız anlamına gelir. Bizim durumumuzda, şunları yaparsınız:

* ELK ödüllerinizi toplamak
* 50%'sini MAI almak için satmak
* ek MAI-ELK LP tokenlarında birleştirmekn
* havuza yüklemek

100$'lık aynı ilk yatırımla başladığınızı ve verilen oranların tüm çiftçilik dönemi boyunca aynı kaldığını varsayarsak, tam bir çiftçilik yılı boyunca bekleyebileceğiniz sonuçlar aşağıdaki gibidir:

| gün | MAI-ELK ($) |
|-----|-------------|
|  30 |     117.172 |
|  60 |     138.044 |
|  90 |     162.635 |
| 120 |     191.607 |
| 150 |     225.739 |
| 180 |     265.952 |
| 210 |     313.328 |
| 240 |     369.143 |
| 270 |     434.901 |
| 300 |     512.374 |
| 330 |     603.647 |
| 360 |     711.179 |

Ve yılın sonunda,

* Havuzda 730.878$ değerinde MAI-ELK LP tokenı

Bu da 100$'lık bir ilk yatırım için %630,88'lik bir toplam APY'ye karşılık gelir. Ödülü birleştirdiğimiz için %200'lük bir APR'den alacağınız tam APY budur.

Bir ek not olarak günlük bileşik ile bir APR'den APY'yi (veya bir APY'den bir APR'yi) hesaplamak için formüller aşağıdaki gibidir:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

$$
APR = N * (( 1 + APY)^\frac{1}{N} - 1)
$$

`N`, ödüllerinizi birleştirme sayınızdır. Bizim durumumuzda, 2 formülü bize

$$
APY = ( 1 + \frac{2}{365})^{365}-1 = 634.88\%
$$

$$
APR = 365 * (( 1 + 6.3488)^\frac{1}{365} - 1) = 199.99\%
$$

Ödülünüze %200'lük bir APR (LP havuzunun APR'si) uygularsanız %32,53'lük bir APR (stake APR) uygulamanızdan daha iyi getiri elde edeceğinizi görmek ve anlamak kolaydır. Bu anlamda, çiftçilik APR'si, stake APR'sinin üzerinde kalırken birleştirmek stake etmekten çok daha iyidir. Bu, havuzdaki likidite miktarı ile açıkça değişebilir

{% hint style="info" %}
Bir önceki bölümde olduğu gibi simülasyonu aynı [Google SpreadSheet](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) ikinci sekmede bulabilirsiniz.
{% endhint %}

### Mai Finance Kullanarak Çiftçilik ve Birleştime

Stake etme ve birleştirme iyi getiri sağlıyorsa her iki yöntem de doğrudan ELK tokenının fiyatıyla bağlantılıdır, bu nedenle yatırımınızın değeri ELK fiyatına göre değişecektir. Birleştirmenin stake etmeye kıyasla daha iyi seçenekler sunduğunu zaten gördük. Şimdi, çiftçilik ödüllerinizden nasıl bir miktar değer elde edebileceğinizi ve Mai Finance'i kullanarak aynı havuza nasıl yatırım yapmaya devam edebileceğinizi göreceğiz. Günlük rutin aşağıdaki gibi olacaktır:

* ELK ödüllerini toplayın
* Mai Finance'de teminat olarak kabul edilen bir miktar mavi çip tokenı satın almak için ödülün %66'sını satın. Örneğimiz için burada ONE tokenını kullanacağız
* ONE tokenlarını Mai Finance'te kasanıza yatırın
* Kalan ELK tokenlarınıza karşılık gelen değer olan %200 CDR'de (Borç Teminatı Oranı) ek MAI borç alın
* Ek MAI-ELK LP tokenlarında birleştirin
* havuza ekleyin

{% hint style="info" %}
Ödül tokenlarınızı ONE'a dönüştürmek, varlıklarınızı korumanın en güvenli yolu olmayabilir, bunu yapmanın en iyi yollarından biri stablecoin’lere dönüştürmektir. Ancak bu makaleyi yazarken Harmony’deki Mai Finance ile ilgili seçenekler oldukça sınırlıdır. Gelecekte (Ocak 2021'den sonra) Stake DAO LP tokenlarını teminat olarak stake etmek gibi daha iyi seçenekler elde edebilirsiniz (Stake DAO tokenlarını Mai Finance'te nasıl kullanabileceğinizi görmek için [makalemize göz atın](<../polygon/the-elephant-and-the-otter.md>)
{% endhint %}

100$'lık aynı ilk yatırımla başladığınızı, verilen oranların tüm çiftçilik dönemi boyunca aynı kaldığını ve kasanızın tasfiye edilmediğini varsayarsak, tam bir yıllık çiftçilik boyunca bekleyebileceğiniz sonuçlar aşağıdaki gibidir:

| gün | MAI-ELK ($) | ONE ($) | Mai borcu ($)|
|-----|-------------|---------|--------------|
|  30 |     111.154 |  11.560 |        5.780 |
|  60 |     124.003 |  24.456 |       12.228 |
|  90 |     138.337 |  38.842 |       19.421 |
| 120 |     154.328 |  54.892 |       27.446 |
| 150 |     172.168 |  72.797 |       36.398 |
| 180 |     192.070 |  92.772 |       46.386 |
| 210 |     214.273 | 115.055 |       57.528 |
| 240 |     239.042 | 139.915 |       69.958 |
| 270 |     266.674 | 167.648 |       83.824 |
| 300 |     297.501 | 198.588 |       99.294 |
| 330 |     331.891 | 233.106 |      116.552 |
| 360 |     370.257 | 271.609 |      135.805 |

Ve yılın sonunda,

* Havuzda 377.069$ değerinde MAI-ELK LP tokenı
* ONE kasanızda 278.446$ değerinde ONE tokenı
* Kasanızdan 139.223$ değerinde borç
* Beklendiği gibi %200'lük bir CDR

MAI-ELK'in 100$ değerindeki başlangıç ​​pozisyonundan başlayarak, bu toplam %416,29'luk bir genel APY'yi temsil eder. Burada saf bileşiğe kıyasla biraz daha az kar elde ediyoruz ancak aynı zamanda karımızın iyi bir kısmını ELK'den daha az değişken olabilecek ve bu nedenle daha düşük riske sahip olabilecek ONE'a çektik.

{% hint style="info" %}
Simülasyon yine aynı [Google SpreadSheet](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit?usp=sharing) üçüncü sekmede bulunabilir.
{% endhint %}

Alternatif olarak, MAI-ELK havuzundaki konumunuzu artırmak için Mai Finance'de kabul edilen tokenlar için tüm ELK ödüllerinizi satabilir, MAI borç alabilir ve bir kısmını satarak ek ELK satın alabilirsiniz. Bunu yaparak ONE'a olan bağlılığınızı artırırsınız ancak aynı zamanda borcunuzu da artırırsınız. Toplamda %342.17'lik bir APY için 270.715$ değerinde MAI-ELK, 352.913$ değerinde ONE ve 171.457$ değerinde borç elde edersiniz.

## Birleştirme Sıklığının Etkisi

İster ödüllerinizi stake etmeye ister birleştirmeye karar verin, ödülünüzün, toplama + yatırım rutininizi gerçekleştirme sıklığınıza bağlı olarak değişeceğini anlamanız önemlidir. Bir hatırlatma olarak APY ve APR'yi birbirine bağlayan formül aşağıdaki gibidir:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Bu denklemde`N`, ödüllerinizi bir yılda kaç kez birleştirdiğinizi temsil eder. Dolayısıyla, yukarıdaki gibi %200'lük APR, birleştirdiğiniz sıklığa bağlı olarak size aşağıdaki APY'yi verir

| Birleştirme sıklığı   |  APY karşılığı |
|-----------------------|----------------|
|                 daily |       634.88 % |
|       twice in a week |       625.01 % |
|                weekly |       611.71 % |
|      twice in a month |       609.55 % |
|               monthly |       535.86 % |
|             quarterly |       406.25 % |
|       twice in a year |       300.00 % |

Günde bir defadan fazla manuel olarak birleştirme, içinde bulunduğunuz zincire bağlı olarak pahalı olabilir. Ama temel olarak ne kadar sık birleştirirseniz ödül o kadar iyi olur. Bu aynı zamanda verim optimize edicilerin / otomatik birleştiricilerin neden popüler olduğunu da açıklıyor. Birleştirerek, çiftçilik yaptığınız tokenın üzerindeki satış baskısını artırdığınızı ve bunun o tokenın fiyatı üzerinde olumsuz bir etkisi olacağını unutmayın. Bu aynı zamanda çiftçilik yapmak için kullandığınız token ise (örneğimizde ELK), sizi kalıcı kayıplardan koruyan Elk Finance DEX kullanmadığınız sürece kalıcı kayıplardan etkilenebilirsiniz.

## Doğru Havuzu Seçmek

MAI-ELK çifti birkaç zincire dağıtıldı, bu da sermayenizi en iyi oranları sunan zincire dağıtmanıza olanak tanır.

![Ocak 2021 itibariyle Gnosis (üstte), Moonriver (ortada) ve Harmony'de (altta) MAI-ELK havuzları](<../../.gitbook/assets/elk-farming-3.png>)

{% hint style="info" %}
MAI-ELK havuzu yakın bir gelecekte, muhtemelen Polygon, Cronos ve Fantom'da diğer zincirlere de dağıtılabilir. Bu garanti edilmez ve bunun için belirli bir tarih yoktur, bu nedenle her iki projenin Discord sunucularını ve Twitter'larını takip ederek güncel kalın.
{% endhint %}

Her zincirdeki ödül oranının yanı sıra, her zincirdeki ELK tokenının fiyatını da göz önünde bulundurmanız gerekebilir. Fiyat tüm zincirlerde hemen hemen aynıysa aradaki küçük fark, ELK tokenını toplamak istediğiniz zinciri seçmeniz için bir faktör olabilir.

![ELK tokenının bulunduğu tüm zincirlerdeki fiyatı](<../../.gitbook/assets/elk-farming-4.png>)

Gördüğünüz gibi, Moonriver'daki MAI-ELK havuzu daha iyi bir ödül oranı sunuyor ve ELK tokenının da bu zincirde daha yüksek bir fiyatı var. Bu, özellikle çiftlik tokenlarının bir kısmını satmayı planlıyorsanız Harmony veya Gnosis'ten ziyade MAI-ELK havuzunu Moonriver'da toplamanın daha iyi olabileceği anlamına gelir. Bunun her zaman böyle olmayabileceğini unutmayın. Bu nedenle bir LP havuzuna katılmadan önce zincirinizi doğru seçtiğinizden ve kendi araştırmalarınızı yaptığınızdan emin olun. Son olarak, sigorta, LP tokenlarınızın havuza yatırıldığı günlerin sayısına büyük ölçüde bağlı olduğundan, [geçici kayıp korumasıyla ilgili belgeleri](https://docs.elk.finance/features/impermanent-loss-protection) okumanız şiddetle tavsiye edilir.

Bir ek not olarak, ELK arasında köprü kurmak ücretsiz olduğundan, her zaman en iyi oranlardan yararlanmak için bir zincirden diğerine geçiş yapabilirsiniz. Bunu yaparak, çıktığınız ve katıldığınız havuzun ödül oranlarını da etkileyeceğinizi anladığınızdan emin olun (daha az likidite APR'yi artırır, daha fazla likidite düşürür).

## Sorumluluk Reddi 

Bu kılavuz, likidite sağlayan tokenları kullanarak verim toplamanın farklı yollarını göstermek için yazılmıştır. Seçtiğiniz strateji ve riske maruz kalmanız ile kazançlarınızı oldukça etkileyeceksiniz. Tabii ki, bu belgede belirtilen tüm kavramlar herhangi bir LP çifti için de geçerlidir ve bir strateji, LP çifti, havuz ve hatta bir DEX seçmeden önce kendi simülasyonlarınızı çalıştırmanız şiddetle tavsiye edilir

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel kalın, piyasalar ile yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
