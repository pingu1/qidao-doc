---
Açıklama: >-
  Bu kılavuzda varlıkları piyasa fiyatından daha düşük bir fiyata almak için tahvil kavramını ve kârı artırmak için yüksek ödül protokollerini kullanacağız.
---
 
# Fantom'daki Exodia Combo
 
## Giriş
 
Kriptoya yatırım yaparken akılda tutulması gereken en önemli şeylerden biri, başlangıçtaki konumunuzun korunduğundan emin olmaktır. Buna dikkat ederseniz yalnızca kârınızı riske atmış olursunuz. Bununla birlikte, bir miktar belirsizliği temsil eden bir tokena yatırım yapmak istiyorsanız başka bir seçenek daha var: onu indirimli olarak satın alın ve ödüllerin mümkün olan en kısa sürede ilk yatırımınızı karşılayacak kadar yüksek olduğundan emin olun.

Birkaç aydır bu, tahvillerin piyasaya sürülmesi ve bazı projeler tarafından önerilen çok yüksek ödül oranları ile mümkün oldu. Bu nedenle bugün, çok farklı 2 hedefe ulaşmak için Fantom'da bono konseptini kullanan iki projeyi inceliyoruz.
 
![](<../../.gitbook/assets/exodia-tomb-0.png>)
 
## Exodia
 
### Projenin tanıtımı
 
[Exodia](https://app.exodia.fi/dashboard) Fantom'da devasa potansiyele sahip küçük bir projedir. Çeşitli varlıklar tarafından desteklenen bir rezerv para birimi olan EXOD tokenını temel alan bir Ohm çatalıdır. Exodia hazinesine eklenen ilk teminat varlıkları DAI ve FTM idi ancak protokolden sorumlu ekip ve DAO, Olympus topluluğu ile bağları geliştirmeye ve OHM'ye dayalı varlıkları satın almak için fazla rezervin %33'ünü kullanmaya karar verdi. Bu nedenle, hazinenin küçük bir kısmı gOHM tokenlarıyla ifade edilir.
 
![Ocak 2022 itibariyle Exodia'nın hazine dökümü](<../../.gitbook/assets/exodia-tomb-1.png>)
 
### Yeni Bono LP Tokenı
 
Bağları güçlendirmek için Exodia, kısa süre önce hazinesindeki OHM ile ilgili token miktarını artırmak için oy kullandı ve yakında tahvil programlarının bir parçası olarak yeni bir token kabul edecek. Yeni token, BeethovenX'te oluşturulabilecek bir LP (Likidite Sağlayıcı) tokenıdır. BeethovenX tokenlarıyla ilgili en iyi şeylerden biri, havuzdaki seçimden yalnızca tek bir varlığa sahip olsanız bile oluşturulabilmeleri ve bu sayede kolayca erişilebilir olmalarıdır. LP tokenı şunlardan oluşur
 
* 20% wFTM
* 20% EXOD
* 20% wsEXOD
* 20% gOHM
* 20% MAI
 
![Ocak 2022 itibariyle BeethovenX'teki Monolith LP havuzu](<../../.gitbook/assets/exodia-tomb-2.png>)
 
Bu muhtemelen bonolar için bir Balancer çatal LP tokenı kullanan ilk Ohm çatalıdır. Bu da artık yalnızca EXOD tokenlarınızı kullanarak yeni tahviller satın alabilmeniz açısından özellikle ilginçtir. İlgili adımlar şöyle olacaktır:
 
* LP tokenını almak için EXOD tokenınızı BeethovenX'teki `The Monolith`  havuzuna yatırın
* Yeni EXOD'u indirimli olarak satın almak için LP tokenınızı Exodia uygulamasında satın
* hak kazanma süresini bekleyin ve EXOD tokenlarınızı toplayın
* tekrarlayın
 
Bu, yalnızca protokole fayda sağlayabilecek EXOD tokenları üzerindeki satış baskısını büyük ölçüde azaltacaktır. Daha önceden tahvil paletleri, DAI'nin ek tahvil satın alabilmesi için EXOD'larını satmak zorundaydı. Bu da token fiyatını düşürdüğü için kısmen zararlı ve hazine üzerinde kademeli bir etkiye sahiptir.
 
{% hint style="info" %}
Ohm projelerine aşina değilseniz konuyla ilgili biraz daha okuma yapmanızı şiddetle tavsiye ederim. Klima ile ilgili kılavuzumuza (Polygon bölümüne bakın) veya doğrudan [Exodia'nın resmi belgelerine](https://docs.exodia.finance/) bakabilirsiniz. Ayrıca, onların discord grubuna katılabilir ve eğitim programlarına kayıt olabilirsiniz.
{% endhint %}
 
Ayrıca LP tokenının, Mai Finance'de mintleyebileceğiniz stable coin olan MAI'yi kabul ettiğini göreceksiniz. Bu aslında LP için ana kaynağımız olacak (daha sonra bakınız). Tahvillerinizi makul bir indirimle satın aldığınızda, hak kazanma süresinin sonunda EXOD tokenlarınızı alacaksınız. Ayrıca bu tokenı, %601'lik bir APR'ye (Yıllık Yüzde Oranı) veya %1,65'lik bir günlük kazanca eşdeğer olan %38,787'lik makul bir APY (Yıllık Yüzde Getiri) ile stake edebilirsiniz.
 
İndirimli EXOD tokenları satın almak için bono sistemini kullanacağız ve yeniden temel ödüllerden kazançlar toplamak için çok yüksek APY'den kar edeceğiz.
 
## Tomb Finance
 
[Tomb Finance](https://tomb.finance/) birçok yönden özgün olan çok özel bir projedir. TOMB tokenı, bir değişim aracı olarak hizmet eden ve Fantom zincirinin Gas tokenı olan FTM'ye ek likidite sağlayan FTM tokenına sabitlenmiş algoritmik bir stablecoin’dir.
 
Tomb Finance ekosistemi iki token daha öneriyor:
 
* TSHARE: Bu token, Tomb Finance için yönetişim tokenıdır. TSHARE sahipleri oy hakkına sahiptir. TSHARE stake edenleri ayrıca ek TOMB'ler alacaktır. TSHARE sahiplerine ek TOMB tokenlarının emisyonu, her yüksek APY döneminin sonunda yeni bir token çıkartılarak Ohm çatallarıyla aynı mekanikleri takip eder.
* TBOND: Bu token, temel olarak sabiti 1 FTM'de tutmak için kullanılan özel bir tokendır. TOMB fiyatı 1 FTM'nin altına düştüğünde, kullanıcılar TOMB tokenlarının mevcut fiyatından TBOND satın alabilirler. Bunu protokole TOMB tokenları satarak yapabilirler ve bu tokenlar yakılırak TOMB'nin değerini 1 FTM'ye yükseltir. TBOND tokenına adını, TBOND'un indirimli olarak satın alınması ve TOMB tokenlarının kullanabilmesi imkanı verdi. TOMB tokenı sabitleyicinin üzerinde olduğunda insanlar TOMB için TBOND'larını kullanabilirler. Yeni TOMB, tokenın değerini azaltarak basıldı. Başka bir deyişle, bu bir arbitraj tokenıdır!
 
![Ocak 2022 itibari ile TOMB, TBOND ve TSHARE değerleri](<../../.gitbook/assets/exodia-tomb-3.png>)
 
Tomb Finance size ayrıca TSHARE tokenları kazandıracak 2 LP havuzu da sunuyor. Bu özellikle Tomb Finance için çok önemli bir likidite derinliğine sahip olması açısından önemlidir. Ancak TOMB'yi FTM'ye alternatif bir çözüm haline getirme hedefine ulaşmak için protokolün TOMB kullanan kullanıcılarının, dolayısıyla likidite sahiplerinin olması önemlidir. TOMB-FTM ve TSHARE-FTM havuzlarını grupladığınızda tek bir uygulamada hoş bir küçük kapalı döngü olan daha fazla TOMB tokenı kazanmanıza izin verecek TSHARE tokenları ile ödüllendirilirsiniz.
 
## Döngüleri kapatmak için ek parçalar
 
Stratejimiz için 2 büyük parçayı da sunduğumuza göre yapbozun diğer parçalarına hızlıca bakalım.
 
### Beefy Finance
 
[Beefy Finance](https://app.beefy.finance/#/fantom) belirli DEX'lerden (Merkezi Olmayan Borsalar) LP tokenlarını ve farm ödül tokenlarını kabul edecek, algoritmalarının ek LP karşılığında ödülü satmasına izin verecek bir verim optimize edicidir. Bu nedenle yalnızca LP'deki tokenları birleştirecek ve token toplandığında ödül tokenın değerini yakalayacak artan bir yatırım pozisyonu elde edebilirsiniz.
 
Stratejimiz için TOMB-FTM LP tokenını kullanacağız. Bunun birçok nedeni vardır:
 
* TOMB, FTM tokenına bağlı olduğundan, bu çift için IL (Geçici Kayıp) yoktur, bu nedenle tek değişiklik FTM'nin fiyat değişikliğiyle bağlantılı olacaktır
* TOMB-FTM, TSHARE ile ödüllendirilir, bu nedenle TSHARE'i satmak çiftin 2 tokenını etkilemez
* TOMB-FTM, IL içermeyen bir LP tokenı için oldukça yüksek bir APY'ye sahiptir
* LP tokenını beefy üzerinde kullanırsanız `mooTombTOMB-FTM` LP tokenını alabilirsiniz

![Ocak 2022 itibarıyla Beefy Finance'de Tomb LP çiftleri](<../../.gitbook/assets/exodia-tomb-4.png>)
 
{% hint style="info" %}
Bu kılavuzun amacı doğrultusunda, paritede kalıcı kayıp olmaması nedeniyle daha az risk sunduğundan TOMB-FTM tokenını kullanıyoruz. Ancak daha yüksek ödüller için TSHARE-FTM çiftini kullanabilirsiniz. Önce riskleri ve DYOR'u (Kendi Araştırmanı Yap) anladığınızdan emin olun.
{% endhint %}
 
### Market XYZ borç verme piyasası
 
[Market.XYZ](https://fantom.market.xyz/pool/3) bazı belirli varlıkları yatırabileceğiniz ve bunlara karşı borç alabileceğiniz bir borç verme protokolüdür. Varlığınızı borç verdiğinizde, borç verdiğiniz varlıkta ödenen bazı borç verme teşvikleri alabilirsiniz. Borç aldığınızda, geri ödeme sırasında borç aldığınız aynı varlığa faiz ödemeniz gerekir.
 
Market XYZ, MAI stablecoin'ini borç almak için ek varlık sınıflarının teminat olarak kullanılmasına izin vermek için 2021'de Mai Finance ile bir ortaklık başlattı. Bu varlıklar, şu anda doğrudan Mai Finance'te kabul edilenlerden daha riskli olarak kabul edilir veya yalnızca resmi bir ChainLink Oracle'ı bekler ve doğrudan ana uygulamada kabul edilmez. Bu da ek avantajlar sağlar: QiDAO protokolü borç alınan MAI'den ücret alır, borçlular düşük faiz oranlarında MAI alır (Mai Finance, talebe bağlı olarak hazineden düzenli olarak daha fazla MAI ekler) ve kullanımını artıran stablecoin için çok ilginç bir kullanım örneği oluşturur. Öte yandan, borç verme piyasaları, varlıklarının doğrudan Mai Finance'te kabul edilmesini beklerken farklı ortaklarla güçlü ilişkiler kurmanın harika bir yoludur.
 
![Ocak 2022'den itibaren Market XYZ'de TOMB Beefy Locker](<../../.gitbook/assets/exodia-tomb-5.png>)
 
Bu strateji için ilgilendiğimiz borç piyasası TOMB Beefy Locker’dır. TOMB-FTM tokenlarımızı Beefy'ye yatırdıktan sonra, Beefy'de ödülleri birleştiren tokenın "sahiplik kanıtı" olan mooTombTOMB-FTM makbuz tokenını alıyoruz. Bu makbuz tokenı, ek MAI borç almak için MarketXYZ'de teminat olarak kullanılabilir.

{% hint style="danger" %}
Market.XYZ, yalnızca minimum 0,05 ETH değerinde (yazım sırasında ~170,00$) kredilere izin verir. Farklı locker’lardan borç almak istiyorsanız yeterli teminat yatırdığınızdan emin olun.
{% endhint %}
 
Yukarıdaki ekran görüntüsünde bunu yapabileceğimizi görebilirsiniz.
 
* mooTombTOMB-FTM tokenını teminat olarak yatırın ve Beefy tarafından sağlanan %355.4 APY alın
* MAI'yi teminatımıza karşı %15,02 faiz oranıyla (APR) borç alın
 
LP çiftçiliğinden elde ettiğimiz kazanımların, bu stratejiyi uygulanabilir kılan borçlanma faizlerinden çok daha iyi performans gösterdiğini görürüz. Ancak likidasyonu önlemek için FTM ve TOMB fiyatını doğru bir şekilde takip ettiğinizden ve çok yüksek bir CDR'de (Teminat Borç Oranı) borç aldığınızdan emin olun; bu, büyük bir fiyat düşüşü durumunda borcunuzu geri ödemeniz için yeterli zaman sağlayacaktır. 
 
{% hint style="info" %}
Bu stratejiyle ilgilenmiyorsanız ancak Mai Finance kullanıcısıysanız, Market XYZ MAI'nizi borç vermek için harika bir uygulamadır. Pozisyonunuzda birleşecek, MAI olarak ekstra ödeme alacaksınız.
{% endhint %}
 
## Farming stratejisi
 
Yatırım döngümüzü tamamlamak için MAI kullanarak EXOD tahvilleri satın almaya başlayacağız. EXOD Rebase ödülleri, TOMB-FTM LP tokenlarını satın almak için kullanılacaktır. Tokenlar, TSHARE ödüllerini birleştirmek için Beefy'de kullanılır. Ek olarak LP tokenı makbuzu, Market XYZ’de daha fazla MAI ödünç almak için teminat olarak kullanılır ve bu da bizi ilk adımımıza geri getirir.
 
Aşağıdaki simülasyon birkaç şey varsayılarak yapılmıştır:
 
* Oranlar ve fiyatlar tüm simülasyon süresi boyunca aynı kalır, bizim durumumuzda 1 yıl
* Exodia APY %38,787
* Beefy yoluyla TOMB-FTM APY %318.51
* Market XYZ’de borçlanma faizi %15,02 APR'dir (faiz bileşik değildir, bu nedenle borçlanma ücretlerinden bahsederken APR kullanıyoruz)
 
Ayrıca, tahvillerinizi ve ekstra EXOD tokenlarınızı günlük olarak topladığınızı ve mümkün olan en kısa sürede rebase’lerden yararlanmaya başlamak için %50 oranında pay sahibi olduğunuzu varsayacağız. Tahviller kolaylık olsun diye ortalama %0 indirimle satın alınacak ancak umarız daha iyi bir indirimle alırsınız. Her 5 günde bir yeni tahvil alabileceğimizi varsayacağız.
 
![](<../../.gitbook/assets/exodia-tomb-6.png>)
 
### 1.Gün
 
Önce hangi giriş noktasının daha az risk taşıdığını bulmamız gerekiyor. TOMB-FTM LP tam olarak buna uygun gibi görünüyor (LP çifti açıklamasında ayrıntılı olarak verilen nedenlere bakın), bu nedenle döngüyü bu noktada 1.000$ değerinde TOMB-FTM tokenıyla başlatacağız. SpookySwap'ta LP tokenı oluşturulduktan sonra onu Beefy Finance'e yatırabilir ve hemen borç almaya başlayabilirsiniz.
 
Bu strateji için %300'lük bir CDR'ye bağlı kalmaya çalışacağız. Bu, locker’dan %15,02 faiz oranıyla 333$ değerinde MAI ödünç alabileceğimiz anlamına geliyor. Ödünç alınan MAI, bir wFTM-EXOD-gOHM-wsEXOD-MAI LP tokenını almak için BeethovenX'te kullanılacaktır. Son olarak, LP ile bir EXOD tahvili satın alacağız. Tüm kurulumun 1. Gün'de yapılabileceğini unutmayın. İlk günün sonunda (3 rebase varsayılarak) şunları elde ederiz:
 
| Pozisyon            | Değer ($) |
|---------------------|-----------| 
| TOMB-FTM            | 1,000.000 |
| MAI                 |   333.333 |
| EXOD                |    66.667 |
| Ek TOMB-FTM         |     3.930 |
| Ek EXOD             |     1.098 |
 
### Gün 2, 3, 4 ve 5
 
Önümüzdeki birkaç gün boyunca satın aldığımız tahvil hala geçerli olduğundan EXOD ödüllerini toplama ve birleştirme konusunda herhangi bir şey yapmaya gerek yoktur. Böylece TOMB-FTM LP tokenını daha fazla borçlanmadan fiyat olarak büyütebilir ve EXOD ödüllerine odaklanabiliriz. Ödülün %50'si daha fazla EXOD ile birleştirilecek ve diğer %50'si TOMB-FTM LP'ye eklenecektir. 5. Günün sonunda teminat tamamen kazanıldığında şunları elde ederiz:

| Pozisyon            | Değer ($) |
|---------------------|-----------|
| TOMB-FTM            | 1,021.369 |
| MAI                 |   333.333 |
| EXOD                |   338.869 |
| Ek         TOMB-FTM |     4.014 |
| Ek         EXOD     |     5.582 |
 
{% hint style="info" %}
Ek TOMB-FTM ve EXOD, yalnızca 5. Günde üretilen ve 6. Günün başında birleştirilenlerdir.
{% endhint %}
 
### 6. gün
 
5. Günde birleştirilen TOMB-FTM ve ayrıca toplanan %50 EXOD, 6. Günün başında size toplam 1.028.173$ değerinde TOMB-FTM verecektir. Exodia'da yeni bir tahvil satın almak için kullanılacak ekstra 9.391$ değerinde MAI. Bu noktada sistem kullanıma hazırdır ve yatırımınızı basit bir günlük rutin ile kolayca yönetebilir.
 
### Günlük Rutin
 
Rutin 2 bölüme ayrılmıştır: her gün yapmanız gereken gerçek günlük rutin ve her 5 günde bir yapmanız gereken rutin.
 
Günlük olarak yapmanız gerekenler:
 
* Exodia'da kazanılmış EXOD tokenlarını talep edin
* Exodia'da EXOD tokenlarının %50'sini pay edin
* SpookySwap'ta FTM için EXOD tokenlarının %25'ini satın
* SpookySwap'ta TOMB için EXOD tokenlarının %25'ini satın
* SpookySwap'ta bir TOMB-FTM LP tokenı oluşturun
* TOMB-FTM LP tokenını Beefy Finance'e yatırın
* mooTombTOMB-FTM makbuz tokenını Market.xyz'e yatırın
 
Her 5 günde bir yapmanız gerekenler:
 
* %300'lük bir CDR elde etmek için Market.xyz'den ek MAI borç alın
* Borç alınan MAI'yi The Monolith havuzunda BeethovenX'e yatırın
* Beethoven LP tokenınızı Exodia'da EXOD tahvili ile değiştirin
 
### Aydan Aya Ham Sonuçlar
 
İşte aydan aya ham sonuçlar
 
| Gün |  TOMB-FTM  |    EXOD    |   MAI Borç |
|-----|------------|------------|------------|
|  30 |  1,222.088 |    488.438 |    407.363 |
|  60 |  1,531.135 |    735.586 |    510.378 |
|  90 |  1,956.250 |  1,093.089 |    652.083 |
| 120 |  2,546.404 |  1,609.179 |    848.801 |
| 150 |  3,371.740 |  2,353.088 |  1,123.913 |
| 180 |  4,532.773 |  3,424.178 |  1,510.924 |
| 210 |  6,173.591 |  4,965.049 |  2,057.864 |
| 240 |  8,500.790 |  7,180.350 |  2,833.597 |
| 270 | 11,810.653 | 10,363.762 |  3,936.884 |
| 300 | 16,528.139 | 14,936.728 |  5,509.380 |
| 330 | 23,262.834 | 21,504.023 |  7,754.278 |
| 360 | 32,889.239 | 30,933.491 | 10,963.080 |
 
### 365. gün
 
Bu sistemde tam bir yıl farming yaptığınızı ve her şeyin 1. Gün'dekiyle aynı olduğunu varsayarsak (fiyatlar, oranlar ve diğer her şey) şunları elde edersiniz:
 
* Beefy'de 34.855.954$ değerinde TOMB-FTM LP tokenı
* 32.863.908$ değerinde EXOD tokenı
* Market.xyz üzerinde 11.618.651$ değerinde MAI borcu ve geri ödenmesi gereken bazı ek faizler (toplam 13,363.772$ borca karşılık gelir)
 
Teminat Borç Oranınızın her zaman %300'e yakın veya %300'ün üzerinde kalacağına dikkat etmeniz çok önemlidir, bu nedenle TOMB-FTM veya EXOD'nizin bir kısmını geri ödemek ve faizleri düşürmek için satmanız tamamen mümkündür. Ayrıca, TOMB-FTM satarak ilk borcunuzu geri ödemek ve yeni EXOD tahvilleri satın almak için günlük sattığınız EXOD bölümünü ayarlamak da mümkündür. Varyasyonlar sonsuzdur, bu yüzden en çok neyi istediğinize  göre ayarlamaktan çekinmeyin.
 
Sonunda, 1.000$'lık bir ilk yatırımdan, 67.719.862$ ve 13.363.772$'lık bir borç elde edersiniz, bu da toplam %5.335.56'lık bir APY'ye tekabül eder.
 
## Sorumluluk Reddi
 
Bu kılavuz, yatırım döngülerinize Ohm çatalları ekleyerek kârınızı nasıl artırabileceğinizi vurgulayan deneysel bir kılavuzdur. Simülasyon, EXOD tokenlarını stake etme konusunda çok yüksek APY'ye sahip olduğu bir zamanda gerçekleştirildi. Aynı şey TOMB-FTM için de geçerlidir. Çok yüksek oranlar genellikle çok değişkendir, bu nedenle tam bir yıl boyunca çok daha az fayda bekleyebilirsiniz. Aslında Ohm çatallarının çoğu, bu kadar yüksek verimi birkaç aydan fazla sürdürecek şekilde tasarlanmamıştır ve genellikle tokenları çıkartmaya devam etmek için emisyonlarını büyük ölçüde azaltır.
 
Kullanmakta olduğunuz projeler hakkında güncel kalın, soru sormaktan çekinmeyin ve her zaman olduğu gibi kendi araştırmalarınızı yapın.
 
{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}
 
