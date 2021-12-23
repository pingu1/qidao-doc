---
Açıklama: >-
 Solarbeam, güzel APR oranı ile MAI-MOVR çiftçilik havuzuna sahiptir. Bugün bundan nasıl yararlanabileceğinizi göstereceğiz.
---

# SolarBeam'de MAI Çiftçiliği

Bu kılavuzda yer alan eğitimlerin çoğu, başlangıç noktası olarak stablecoinleri kullanır. Bunun temel nedeni, stablecoin çiftlerinin geçici kayıplardan veya diğer varlıkların oynaklığından etkilenmemesidir. Bu durumda başlangıçtaki değerinizi kaybetmek neredeyse imkansızdır ve kazancınızı artırmak için stablecoinlerden elde ettiğiniz kazançlarla daha riskli stratejileri kullanabilirsiniz.

Şu anda MAI kullanan tek uygulama olan Solarbeam ile Moonriver'da farklı bir yaklaşım deniyoruz. LP (Liquidity Provider) çifti MAI-MOVR'dir. MAI, Moonriver'a köprüleme yapabileceğiniz veya bir kasadan token çıkarabileceğiniz Mai Finance'in stablecoinidir ve MOVR, Moonriver'ın yerel gas tokenıdır. Bu nedenle, MOVR'nin her zaman bir faydası olacaktır. Ayrıca fiyatının asla çok sert bir şekilde düşmemesi gerekir. Bu sabit bir çift değildir ancak tokenın tek değişken kısmı MOVR ile bağlantılıdır, bu da onu her durumda iyi bir başlangıç noktası yapar.

Moonriver'da kapalı bir geri bildirim döngüsüyle süreç boyunca çok fazla farm tokenı harcamadan nasıl çok yüksek verimler elde edebileceğimize bir bakalım.

![](<../../.gitbook/assets/solarbeam-1.png>)

## SolarBeam

### SolarBeam'de MAI Çiftçiliği

Solarbeam, Moonriver'daki ilk ve ana DEX (Merkeziyetsiz Borsa) ve AMM’dir (Otomatik Piyasa Yapıcı) ve zincirdeki TVL açısından ikinci uygulamadır. Aynı zamanda Mai Finance'in ilk Moonriver ortağıdır ve yerel tokenlarının bir kısmı olan SOLAR tokenlarıyla ödüllendirilecek bir MAI-MOVR havuzu sunar. MAI için likiditeyi de burada bulabilirsiniz.

![Aralık 2021 itibariyle Solarbeam'de MAI-MOVR havuzu](<../../.gitbook/assets/solarbeam-2.png>)

Havuzun düşük kullanımı nedeniyle %84'lük APR (Yıllık Yüzde Oranı) oldukça yüksektir ve bu da onu stratejimiz için mükemmel bir başlangıç noktası yapar. Bu APR'yi aldığınızda (referans için QuickSwap'ta MAI-WMATIC gibi bir şeyle karşılaştırmak istiyorsanız %131 APY'ye karşılık gelir) ödül SOLAR tokenları olarak ödenecektir. Aralık 2021 itibariyle 1 SOLAR = 3.78 USDC.

### Tek taraf staking SOLAR

Solarbeam de dahil olmak üzere Uniswap çatallarının çoğu artık yerel tokenları için stake yapmayı öneriyor. Daha fazla SOLAR için SOLAR'ınızı bir kasaya yatırıp kilitleme uzunluğuna bağlı olarak çok ilginç oranlar elde edebilirsiniz (30 günlük bir kilitleme için %200 APR'ye kadar), ancak harici tokenlar kazanmak için stake'i kullanacağız. Moonriver'daki farklı uygulamalardan bir dizi başka token almak için SOLAR tokenlarınızı stake edebilirsiniz, aradığımız token ROME tokenıdır

![Staking SOLAR token to earn ROME tokens on Solarbeam](<../../.gitbook/assets/solarbeam-3.png>)

ROME havuzunun en düşük APR'ye sahip olduğunu göreceksiniz ancak yine de oldukça yüksektir ve yakında ROME tokenlarımızın çılgın bir oranda çoğaldığını göreceksiniz.

## Rome DAO

Rome DAO, Moonriver'daki bir başka büyük aktördür. ROME tokenını yerel token olarak kullanan bir Ohm-çatalıdır (Olympus DAO kopyası). Çok yüksek getiriler elde etmek için uygulama üzerinde ROME tokenlarınızı stake edebileceksiniz. Her Ohm-çatalının amacı, emisyonu sürdürebilmek için likiditeyi çekmek ve yerel tokena sahip olmaktır. Ohm-klon hakkında daha fazla bilgiye ihtiyacınız varsa lütfen [Polygon için Klima DAO eğitimimize](../polygon/ohm-forks-on-polygon-the-case-of-klima.md) göz atın.

![ROME tokenlarını Aralık 2021 itibariyle %771 Nisan için Roma DAO'da stake etme oranı](<../../.gitbook/assets/solarbeam-4.png>)

Solarbeam'den ROME tokenları alacağımız için onları Rome DAO'da stake edebilmeliyiz, rebase sistemi çok daha hızlı bir şekilde almanızı sağlayacaktır. Bu strateji için Rome DAO'da ROME tokenlarını stake edeceğiz ve şu anda Rome DAO'daki depozitonun ~%1'ine tekabül eden günlük ödülün %50'sini satacağız.

## Mai Finance

Mai Finance, kripto varlıklarınızı yatırabileceğiniz ve MAI stablecoinini %0 faizle borç alabileceğiniz bir borç verme platformudur. Moonriver'da tahsil edilecek tek ücret, borcunuzun %0,5'lik geri ödeme ücretidir.

![Moonriver'da çok sayıda MAI bulunan ETH kasası](<../../.gitbook/assets/solarbeam-5.png>)

Stratejimiz için bir ETH kasası kullanacağız. Rome DAO stake havuzundan çıkarılacak ROME tokenı aşağıdaki gibi bölünecektir:

* Solarbeam'deki takas özelliği kullanılarak %33'ü MOVR'ye değiştirilecek
* Solarbeam'deki takas özelliği kullanılarak %66'sı ETH'ye takas edilecek

Ardından, güvenli bölgede kalmak ve likidasyonu önlemek için %200'lük bir CDR (Borç Teminatı Oranı) ile MAI borç almak için ETH'yi Mai Finance'e yatırabileceksiniz. Borç alınan MAI, daha sonra Solarbeam'deki başlangıç konumuna eklenecek olan ek MAI-MOVR LP tokenları oluşturmak için kullanılacaktır.

Örnek olarak, Rome DAO'dan aldığınız her 1$'lık ROME için şunları elde ederiz:

* MOVR'nin 0,33$’ı
* Mai Finance'e yatırılan ETH'nin 0,66$’ı
* ETH'mize karşı borç alınan MAI’nın 0,33$’ı
* Solarbeam'e eklenecek 0,66$ değerinde MAI-MOVR LP tokenı

## Çiftçilik Stratejisi

Aşağıdaki simülasyon farklı durumlar varsayılarak yapılmıştır:

* Tüm oranlar ve fiyatlar simülasyonun tüm süresi boyunca aynı kalır, bizim durumumuzda 1 yıl:
  * Solarbeam'deki MAI-MOVR farming’de %84 APR
  * SOLAR'ı stake ederek ROME tokenları toplamak için %108 APR
  * ROME tokenlarını stake ederken Rome DAO'da %771 APR
* Tüm ödüller ve programlar da bir yıl boyunca devam ediyor
* Rome DAO'daki günlük kazançların %50'si %33 MOVR ve %66 ETH'ye satıldı
* İlk yatırım 100$ değerinde MAI-MOVR LP tokenıdır.

![](<../../.gitbook/assets/solarbeam-6.png>)

### 1.Gün

1. günde, 100$ değerindeki MIA-MOVR'nizi Solarbeam'e yatırırsınız ve günün sonunda SOLAR tokenlarınızı toplarsınız. Bu size aşağıdaki sonucu verecektir:

| MAI-MOVR | SOLAR |  ROME |  ETH  |    İlave LP   |
|----------|-------|-------|-------|---------------|
|  100.000 | 0.230 | 0.000 | 0.000 |         0.000 |

### 2. Gün

2. günde, daha fazla SOLAR toplamak için MAI-MOVR konumunuzu korursunuz ancak aynı zamanda bazı ROME tokenlarınızı toplamaya başlamak için toplayacağınız ilk SOLAR tokenınızı da riske atarsınız. 2. günün sonunda şunları elde edersiniz:

| MAI-MOVR | SOLAR |  ROME |  ETH  |    İlave LP   |
|----------|-------|-------|-------|---------------|
|  100.000 | 0.460 | 0.001 | 0.000 |         0.000 |

### 3. Gün

3. günün başında, %50 günlük stake ödülünden ilk birkaç ROME tokenınızı toplayabilmeniz gerekir. Miktar oldukça önemsiz olduğu için 3. günde yalnızca 100$ ile başlamak muhtemelen iyi bir fikir değildir ancak yine de kasanızı Mai Finance'e yatıracağınız MOVR için %33 ve ETH için %66 satacaksınız, ardından yeni teminatınız karşılığında MAI borç alacaksınız.

| MAI-MOVR | SOLAR |  ROME |    ETH   |    İlave LP   |
|----------|-------|-------|----------|---------------|
|  100.000 | 0.690 | 0.002 | 0.000005 |      0.000005 |

Bu noktada sistem tamamen ateşlenmiş olur

## Çiftçilik Sonuçları

### Günlük rutin

Sistem tamamen hazır olduğunda günlük rutininiz,

* MAI-MOVR havuzundan SOLAR toplayın
* kazandığınız SOLAR tokenlarını stake edin
* SOLAR stake havuzundan ROME tokenlarını toplayın
* topladığınız ROME tokenlarınızı stake edin
* Rome DAO'daki günlük kazançlarınızın %50'sini riske atın (~1.5 rebase’e karşılık gelir)
* ROME tokenlarınızın %66'sını ETH karşılığında satın
* MOVR için ROME tokenlarınızın %33'ünü satın
* ETH'yi Mai Finance'teki ETH kasasına yatırın
* MAI stablecoini olarak mevduatınızın %50'sini borç alın
* borç alınan MAI'yi MOVR tokenlarıyla eşleyin
* ek MAI-MOVR tokenlarınızı yatırın

### Aydan aya ham sonuçlar

| Gün | MAI-MOVR | staked SOLAR | staked ROME |    ETH   |
|-----|----------|--------------|-------------|----------|
|  30 |  100.021 |        7.135 |       0.352 |    0.023 |
|  60 |  100.190 |       14.045 |       1.550 |    0.200 |
|  90 |  100.713 |       20.978 |       3.911 |    0.740 |
| 120 |  101.872 |       27.968 |       7.869 |    1.925 |
| 150 |  104.052 |       35.072 |      14.023 |    4.148 |
| 180 |  107.788 |       42.378 |      23.204 |    7.947 |
| 210 |  113.814 |       50.019 |      36.559 |   14.065 |
| 240 |  123.142 |       58.178 |      55.580 |   23.525 |
| 270 |  137.175 |       67.158 |      82.767 |   37.745 |
| 300 |  157.848 |       77.321 |     120.875 |   58.681 |
| 330 |  187.841 |       89.226 |     174.234 |   89.041 |
| 360 |  230.861 |      103.358 |     248.711 |  132.575 |

### 365.gün

Tam bir yıllık farming’den sonra

* Solarbeam'de 239.633$ değerinde MAI-MOVR
* Solarbeam'de 106.358$ değerinde SOLAR tokenı
* Rome DAO'ya stakelenen 263.708$ değerinde ROME tokenı
* Mai Finance'de 141.450$ değerinde ETH
* Mai Finance'de 68.817$ değerinde MAI borcu

Yeni LP tokenlarının yarısını almak için takas edilen ROME tokenlarının üçte birini kullandığımızdan dolayı ek MAI-MOVR borca tam olarak karşılık gelmiyor.

Böylece bu döngü size nispeten stabil bir başlangıç konumundan %583,15'lik bir APY verecektir.

## Sorumluluk Reddi

Bu stratejiden anlaşılması gereken en önemli şey, Moonriver'ın şu anda yeterince kullanılmadığı ve ödül oranlarının çok ilginç olduğudur. Ayrıca, kazançlarınızın bir kısmını yeniden yatırmak için stratejinize bir Ohm-çatalı eklediğiniz anda, ödül oranları o kadar çılgındır ki, DAO'da ödül kazanmak için yeterli tokenınız olduğu sürece çok büyük bir kâr elde edebilirsiniz.

Bununla birlikte, projelerin bir yıllık bir süre boyunca garanti edilmeyen değişken ödeme oranlarına sahip olduğunu unutmayın. Lütfen yatırım yaptığınız tüm projeleri anladığınızdan emin olun, kendi araştırmanızı yapın ve yalnızca kaybetmeyi göze alabileceğiniz kadar yatırım yaptığınızdan emin olun. Bu strateji nispeten stabil bir başlangıç ​​yatırımına dayandığından yalnızca diğer sistemlerin avantajları risk altındadır. Bu kılavuz, kullandığı projeler için bir öneri olarak görülemez

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}
