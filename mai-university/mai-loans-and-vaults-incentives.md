---
description: >-
  Bu makale, MAI'yi %0 faizle ödünç almak için Mai Finance'i nasıl
  kullanabileceğinizin, bunun için nasıl ödeme alacağınızın, %0 faizli kredinizi
  negatif faizli krediye nasıl dönüştürebileceğinizin ayrı
---

# MAI kredileri ve Kasa teşvikleri

## Giriş

Mai Finance'in ana işi bir borç verme platformudur. İnsanlar diğer varlıkları satın almak için kriptolarını satmak yerine, fonlarını Mai Finance'e kilitleyebilir ve onlara karşı borç alabilir. Bu sayede yüksek değerli varlıkları (WBTC, WETH ...) korurken diğer varlıkları ve çiftlik verimini elde etme fırsatı sunar. Kullanıcılar krediler ile gelir elde ederken, teminatları değer kazanır.

Mai Finance kullanmanın diğer büyük avantajlarından biri de geri ödeme planının olmamasıdır. Yani kripto paranız karşılığında MAI stabilcoin ödünç alıyorsunuz, faiz ödemiyorsunuz ve borcunuzu istediğiniz zaman geri ödeyebiliyorsunuz. Daha fazla ayrıntı için [borç yönetimi](debt-repayment-why-and-while.md) hakkındaki farklı makalelere bakın. Ödeyeceğiniz tek ücret, kredinizi geri ödediğinizde ödediğiniz borç paranın %0,5'i kadar olan ve teminatınızdan kesilen bir geri ödeme ücretidir.

Örnek olarak, 100$ değerinde MAI ödünç almak için 200$ değerinde WETH yatırdıysanız, kredinizi geri ödediğinizde WETH depozitonuzdan doğrudan 0,50$'lık bir ücret ödemeniz gerekir.

Bu zaten harika bir fırsat değilse, Mai Finance ekibi Eylül 2021'de Mai Finance'in platform tokenı olan Qi'de ödenen Vault teşviklerini tanıttı. Başka bir deyişle, MAI'yi ödünç almak için varlıklarınızı Mai Finance'e bir kasaya yatırarak, bunu yapmak için de ödeme alacaksınız. Bu makaleler, fonksiyonların işlevin çalıştığını ayrıntılı olarak sunar.

## Kasalar - Nedir, nasıl çalışır

### Kasa oluşturma

Mai Finance'de kasalar, varlıklarını yatırabilecekleri özel depolardır. Şu anda 10 tip kasa vardır:

![Mai Finance'te oluşturabileceğiniz farklı kasa türleri](<../.gitbook/assets/image (1).png>)

2 farklı kasa tipi vardır:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

and

* camWETH
* camWBTC
* camWMATIC
* camAAVE

Listedeki ilk 6 kasa basit varlıklar içindir, son 4 kasa ise camTokens içindir. camTokens, AAVE'de yapabileceğiniz ve ardından Mai Finance'in getiri havuzlarına yatırabileceğiniz bir mevduatın temsili olan AAVE piyasa tokenlarını birleştiriyor. Varlıklarınız AAVE'de getiri üretirken (ve ödüller getiri havuzu tarafından otomatik olarak birleştirilirken), yine de bu tokenlara karşı MAI ödünç alabilirsiniz.

Bir yan not olarak, yukarıdaki ekran görüntüsünde, oluşturma sayfasının bazı çok önemli bilgileri gösterdiğini görebilirsiniz:

* MAI mevcut: bu maksimum borç tavanına, kasa mevduatlarından basılabilecek maksimum MAI sayısına karşılık gelir.
* Min Kol. oran: bu, o kasa için minimum Teminat-Borç oranıdır (CDR)
* Kasa teşvikleri APR

### Borç Tavanını Anlama

Belirli bir kasada basılabilecek maksimum MAI sayısı, o kasaya ne kadar varlık yatırıldığına bağlıdır. Piyasanın çok kısa sürede MAI ile dolup taşmamasını sağlamak için borç tavanı uygulanmaktadır. Borç tavanı stabil coinin fiyatını etkileyebilir.

Örnek olarak, büyük bir kurum bir kerede 5.000 WBTC yatırırsa ve toplamını daha fazla WBTC ile takas ederek 100.000.000$ değerinde MAI ödünç alabilseydi MAI'nin fiyatını o kadar aşağı çekebilir ki fiyat kendi değerinden çok fazla sapabilirdi. Bu durum yani 'peg' tüm platformu riske atıyor. Borç tavanı bunun olmasını engelleyen mekanizmadır: belirli bir kasa tipi için basılabilecek maksimum MAI miktarı vardır.

Borç tavanına ulaşıldığında, basılacak MAI'nin kalmadığı zaman kaydedilir ve sistem 48 saat sonra borç tavanını otomatik olarak artırır. 48 saat MAI fiyatının dengelenmesi için yeterli bir süre olarak kabul edilir (MAI'nin büyük bir satışını takiben yüksek satış baskısı olması durumunda).

48 saat ayrıca borç geri ödenmedikçe, borç tavanına ulaşan bir kasadan 48 saat boyunca hiç kimsenin daha fazla MAI ödünç alamayacağı anlamına gelir.

Bir yan not düşelim, piyasada ne kadar çok MAI varsa fiyat o kadar istikrarlı olur. Gerçekten de, dolaşımda daha fazla MAI varsa büyük bir MAI satışı daha az istilacı olur.

* Dolaşımda sadece 10.000 MAI varken biri 1.000 MAI satarsa, satış %10'a tekabül eder.
* Dolaşımda 10.000.000 MAI varken biri 1.000 MAI satarsa, satış %0.01'e tekabül eder.

Bu nedenle, borç tavanı kademeli olarak değil, katlanarak artırılır: dolaşımda daha fazla MAI, büyük bir satışın daha az etkisi olur. Böylece borç tavanı çok daha fazla artırılabilir.

{% hint style="info" %}
MAI ödünç aldığınızda, teminatınızın cari değeri ve halihazırda ödünç almış olduğunuz MAI miktarı ne olursa olsun, ödünç alabileceğiniz maksimum MAI miktarı borç tavanıyla sınırlanabilir. Bu durumda, gerçekten daha fazla MAI ödünç almadan önce 48 saat bekleyebilirsiniz.
{% endhint %}

### Teminatın Borç Oranını Anlama

CDR veya **D**ebt **R**atio **C**ollateral, kasanıza yatırılan varlıkların değeri ile ödünç aldığınız MAI miktarı arasındaki orandır.

Örnek olarak, 100$ değerinde MAI ödünç almak için 200$ değerinde WETH yatırdıysanız, CDR'niz

$$
CDR=\frac{CollateralValue}{DebtValue}=\frac{200}{100}=200\%
$$

CDR'yi %100'ün üzerinde tutmak, herhangi bir noktada borçtan daha fazla teminat olduğu anlamına gelir. Bu, MAI istikrarlı parasının aşırı teminatlandırılmasını sağlamak için zorunludur ve Mai Finance tokenomiklerinin temellerinden biridir. Resmi [Mai Finance belgelerinden](https://docs.mai.finance/stablecoin-economics) daha fazla ayrıntı alabilirsiniz.

Her kasa tipinin kabul edilen bir minimum CDR oranı vardır.Ödünç alınan miktar yeterli teminatla desteklenmeyebileceğinden kasanın risk altında olduğu kabul edilen bir eşik değerine sahiptir. Bu noktada, herkes kasayı likidasyona maruz bırakabilir. Yani borcun bir kısmı likidasyon memuru tarafından geri ödenir ve daha sonra yatırılan teminatın bir kısmını geri ödeme olarak alabilir. Likidasyon süreciyle ilgili daha fazla ayrıntıyı yine resmi belgelerde bulabilirsiniz.

MAI'yi belirli bir teminat karşılığında ödünç aldığınızda, ödünç alabileceğiniz maksimum MAI miktarı ve ödünç alınan miktara bağlı olarak sağlık oranınız üzerindeki etkisinin ne olacağı konusunda bazı ipuçları alacaksınız. Aşağıdaki ekran görüntüsünde de görebilirsiniz:

![Ödünç alınan miktara bağlı olarak sağlığın azaltılması](<../.gitbook/assets/image (2).png>)

CDR'nize dikkat etmek ve sağlıklı bir oran tutmak çok önemlidir.

* Likidasyonu önlemek
* dolaşımdaki MAI hacminin uygun şekilde desteklenmesini sağlayarak tüm Mai Finance platformunun sağlığını artırmak

Mai Finance ekibi tarafından tanımlanan "sağlıklı" CDR, minimum CDR değerinin %25 ila %270 üzerindedir. Ek bir not olarak, diğerlerine [yatırım yapmak](../polygon-tutorials/leverage-aave-tokens.md#examples-with-numbers) için pasif/agresif CDR'leri nasıl kullanabileceğinizi görmek için strateji kılavuzlarımıza da göz atabilirsiniz. Borcunuzu kullanarak [borcunuzu geri ödeyin](debt-repayment-how.md#repayment-using-your-collateral).

## Kasa teşvikleri

### Apps Kasası teşviklerini anlama ve APR

Eylül 2021'de Mai Finance, kasa teşviklerini uygulamaya koydu. Bu teşvikler Mai Finance platformu tarafından MAI ödünç alan ve platformun büyümesine katılan herkese tahsis edilen bir ödüldür.

Her Kasa türü (10 farklı tür arasında) blok başına 0,05 Qi alır, bu daha sonra sağlıklı bir Teminat Borç Oranına sahip tüm kullanıcılar arasında dağıtılır. Kasanın APR'si, ödünç alınan MAI'nin mevcut miktarı ile tanımlanır.

Örnek olarak, Ben ve Kila, ETH'lerini Mai Finance'deki WETH kasalarına yatıran 2 arkadaştır.

* Ben, 2.000 $ değerinde ETH yatırdı ve 1.000 MAI ödünç aldı
* Kila, 10.000 dolar değerinde ETH yatırdı ve 6.000 MAI ödünç aldı

Kasaya WETH yatıran kullanıcılar tarafından ödünç alınan mevcut MAI miktarı 1.000.000 MAI'dir.

Hem Ben hem de Kila kasa teşviklerine hak kazanır çünkü Ben'in CDR'si %200 ve Kila'nın CDR'si %166,67'dir. Ben, aldığı krediyle, ödünç alınan toplam tutarın %0,1'ine, Kila ise %0,6'sına sahiptir.

WETH kasasına (veya herhangi bir kasaya) tahsis edilen toplam Qi miktarı

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86.400, bir gündeki saniye sayısıdır ve Polygon'da blok süresi 2 saniyedir. Yani her gün beklenen blok sayısı 86.400 / 2 = 43.200'dür. Bu nedenle, her bir Kasa için emisyon 2.160 Qi / gün'dür.

**Not:** Blok süresi son zamanlarda arttı. Şu sıralar 2,6 saniye civarında. Ancak, tüm uygulamalarda görüntülenen tüm APR'ler ve APY'ler, 2 saniyelik bir blok süresi varsaymaktadır. Lütfen DYOR yapın ve mevcut [PolygonScan'deki engelleme süresini](https://polygonscan.com/chart/blocktime) kontrol edin.
{% endhint %}

Dolayısıyla kasanın durumu aynı kalırsa Ben, dağıtılan 2.160 Qi'nin %0.1'ini alırken, Kila verilen ödülün %0.6'sını alacak.

* Ben, her gün %0.216'lık bir günlük ödül veya %78.84'lük bir APR olan 2.16 Qi alacak
* Kila her gün 12.96 Qi alacak, bu da günlük %0.216 ödül veya %78.84 APR

Bir yan not ekleyelim, 1.000.000 MAI için 2.160 Qi, kasanın APR'si olan %0.216 veya %78.84'lük bir günlük ödüldür.

{% hint style="info" %}
Kasanın APR'sinin doğrudan ödünç alınan MAI miktarıyla bağlantılı olduğunu görmek kolaydır. MAI ne kadar çok ödünç alınırsa, APR o kadar düşük olur. Bir dip not olarak, ödünç alınabilecek MAI miktarı da MAI talebiyle artan borç tavanı ile sınırlandırılmıştır.
{% endhint %}

Doğrulama olarak, Mai Finance'de [analitik sayfasında](https://app.mai.finance/analytics) yayınlanan sayılara dayalı olarak MATIC kasası için teorik APR'yi hesaplayabiliriz. MATIC kasasından ödünç alınan MAI miktarı 799.328'dir. Bu kasa için ödül günde 216 Qi'dir. Bu, bir APR'ye karşılık gelir

$$
APR=\frac{QiReward*Qi_{Price}}{MAI_{borrowed}}*365=\frac{2160*0.441}{785008}*365=44.29\%
$$

Aşağıdaki ekran görüntüsünde gösterildiği gibi, aşağı yukarı MATIC Kasasının APR'sine karşılık gelir:

![Kasa ödüllerinin başlatılmasından sonra Mai Finance'te bir MATIC kasasının Nisan ayı görünümü](<../.gitbook/assets/image (23) (2) (3) (4).png>)

### Başlangıç ​​kasalarının APR'larını hesaplama

Yukarıdaki örnekle aynı verilerle, tüm kasalar için başlangıç ​​APR'larını hesaplamak mümkündür.

| Kasa Tipi | Başlangıç APR |
| --------- | ------------- |
| MATIC     | 44.29%        |
| WETH      | 24.03%        |
| LINK      | 27.41%        |
| AAVE      | 164.14%       |
| CRV       | 159.96%       |
| WBTC      | 36.92%        |
| camWETH   | 25.46%        |
| camWMATIC | 44.33%        |
| camAAVE   | 167.23%       |
| camWBTC   | 47.38%        |

{% hint style="info" %}
Gördüğünüz gibi bazı kasalar diğerlerinden daha fazla ödül üretecek. Ayrıca, yüksek APR'lerden yararlanmak için varlıklarınızı borç tavanı yükseltilmeden ve daha fazla kredi alınmadan (APR'yi düşürmeden) önce mümkün olan en kısa sürede yatırmanın çok önemli olduğunu görebilirsiniz.

Ayrıca kredinizi bir yıl daha saklarsanız, %0,5 geri ödeme ücretinin ödül programı tarafından kolayca telafi edileceğini görebilirsiniz.
{% endhint %}

### Teşvik dağıtımı

Kasa teşvikleri tarafından tahsis edilen ödüller, stake edilen Qi ile aynı şekilde dağıtılacaktır. Her Çarşamba, kasa teşvik programı tarafından tahsis edilen Qi, ödeme gününden önceki hafta için havadan düşürülecek / talep edilecektir.

## Apps Kasası teşvikleriyle ilgili SSS

Apps Kasası teşviklerinin çalışma şekli hakkında daha fazla bilgi edinmek istiyorsanız, Discord sunucusundan resmi bir SSS hazırladık.

* **Ödülleri hangi kasalar alıyor?**

Şu anda tüm kasa türlerine Qi ödülleri verildi

* **Borçlanma teşvikleri için ne kadar ödül veriliyor?**

Her kasa tipi için 0,05 Qi/blok

*   **Ödül kazanmak için ne kadar MAI ödünç almam gerekiyor?**

    Kasa Ödünç Alma Teşvikleri için, QI airdrop almak için tasfiye oranının %25 ila %270 üzerinde kalın. Bu şu anlama gelir:
* _Matic_ - Likidasyon oranı %150 - %175 ile %420 arası Teşviklere Uygun
* _Tokens_: - Tasfiye oranı %130 - %155 ile %400 arası Teşvikler için uygun
* _CamTokens_: - Tasfiye oranı %135 - %160 ile %405 arası Teşvikler için Uygun
*   **Kasamın ödül kazanıp kazanmadığını nasıl görebilirim?**

    Kasaya genel bakış sayfanızda yangın emojisini görüyorsanız bu kasanın ödül kazandığı anlamına gelir.
* **Ne kadar kazanacağım?**

Ödül havuzunun yüzdesi, o kasa türünden ödünç alınan MAI'nin toplam miktarına kıyasla ödünç aldığınız MAI yüzdesine dayanır.

* **Teşvik programı ne kadar sürecek?**

Borçlanma teşvik programının planlanan süresi 3 ay sürecektir. DAO, 3 ay dolmadan teşvikleri durdurmak için oy kullanabilir veya programı uzatmak için oy kullanabilir.

* **Ödülleri nasıl alacağız?**

Qi, uygun kasa sahiplerine havadan indirilecek.

* **Ödüller için uygunluk nasıl toplanır?**

Ödüller için uygunluk, blok başına hesaplanır. Hafta boyunca hak ettiğiniz bloklar için ödüller kazanacaksınız.

* **Haftanın takip ödülleri ne zaman başlıyor?**

eQi ile aynı programı takip edeceğiz. Blok numaralarını destek sayfasında bulabilirsiniz.

## Sorumluluk Reddi

Bu kılavuz, Apps Kasası teşviklerinin başlatılmasından **önce** yazılmıştır; bu, bu belgede (ve bu belgede) tanıtılan APR'lerin değişikliğe tabi olduğu ve/veya doğru olmayabileceği anlamına gelir. Ödünç alınan MAI miktarı, borç tavanı ve Qi değeri, her kasa tipinin nihai APR'sini büyük ölçüde etkileyecektir. Lütfen sorumlu bir şekilde yatırım yaptığınızdan emin olun.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
