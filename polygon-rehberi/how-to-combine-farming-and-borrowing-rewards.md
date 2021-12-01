---
description: >-
  Bu sayfa, yatırımlarınızı büyütmek için verim çiftçiliğini, Mai Finance
  tarafından sağlanan borçlanma ödülleriyle nasıl birleştireceğinizi sunar.
---

# Çiftçilik ve Borçlanma (Borrowing) Ödülleri Nasıl Birleştirilir?

## Giriş

Eylül 2021'de Mai Finance, borçlanma işini geliştirmek ve insanların MAI'yi ödünç almak için tokenlarını kullanmasını sağlamak için kasa ödüllerini tanıttı. Sadece küçük bir geri ödeme ücreti ile %0 faizli kredi almakla kalmıyor, artık insanlar borç para almak için de ödeme alabiliyor. Bu kılavuz, Mai Finance'deki kasaları besleyecek, yüksek borçlanma teşviklerine yol açacak bir token kaynağı olarak Augury Finance'i kullanarak istikrarlı token çiftçiliğine dayalı bir strateji ve daha sonra çiftliğe yeniden enjekte edilecek ek MAI önerecektir.

![](<../.gitbook/assets/image (29).png>)

## Uygulama ve Havuz Tanıtımı

### Augury Finance

Augury Finance, LP (**L**iquidity**P**ool) tokenlarınızı otomatik olarak birleştirmeye odaklanmayan bir getiri toplayıcıdır. Bunun yerine Augury Finance, _Infusions_'larında yatırımlarının olduğu çiftliklerin çiftlik tokenlarını otomatik olarak satıyor.

Örnek olarak, DFYN-WETH çiftini Augury'de değerlendirebilirsiniz.

![Augury Finance'deki DFYN-WETH madencilik havuzu örneği](<../.gitbook/assets/image (30).png>)

Bu infüzyon, temel çiftlik olarak DinoSwap'ı ve birinin DFYN'de alabileceği bir LP tokenını kullanıyor. %123,43'lük bir APR ile bu havuza likidite yatıran kullanıcılar ile ödüllendirilecektir.

* 30% WETH ile
* 20% LINK ile
* 20% WBTC ile
* 15% USDT ile
* 15% WMATIC ile

DinoSwap üzerinde farm yaparsanız, fiyatı çok değişken olan DINO tokenları ile ödeme alırsınız. Adamant veya Beefy gibi diğer toplayıcılarda LP konumunuzu yükseltirsiniz, ancak Augury ile çok yüksek oynaklığa sahip olma olasılığı daha düşük olan tokenlar alarak konumunuzu "güvence altına alırsınız". Dezavantajı ise, hasat DINO'nun %100'ü Augury'de ödülü oluşturan token setine dönüştürüldüğü için ilk konumunuzun zaman içinde büyümemesidir.

{% hint style="info" %}
Augury Finance, farklı yatırım ücretleri ve performans ücretleri olan 3 farklı İnfüzyon katmanı kullanıyor. Lütfen kullanmak istediğiniz katman türleri hakkında bilgi edinin ve bunların çiftçilik stratejiniz üzerindeki etkisini anladığınızdan emin olun.
{% endhint %}

Stratejimizde, kullanıcıları bir WETH/WBTC/LINK/WMATIC/USDC karışımı ile ödüllendiren USDT-UST tier2 çiftliğini kullanacağız. Mai Finance, ödül olarak alacağımız 5 tokendan 4'ü için 4 kasa önermektedir. Kârımızı en üst düzeye çıkarmak için, Augury'nin çıktısı ile Mai Finance'deki kasalar arasına AAVE ekleyeceğiz, çünkü hasat edeceğimiz 5 tokendan 3'ü AAVE'ye ödünç verilebilir.

![Stratejimiz için istikrarlı madeni para çiftçiliği USDT-UST](<../.gitbook/assets/image (31).png>)

### Curve

Curve, _blue chip_ tokenları ödünç veren kullanıcıları ödüllendiren bir projedir. Ödül, Mai Finance'te teminat olarak kabul edilen 2 token olan otomatik olarak birleştirilmiş tokenlarıdan (yatırıma geri eklenir), WMATIC tokenlarından ve CRV tokenlarından oluşur.

Curve ve havuzları hakkında dikkat edilmesi gereken çok ilginç şeylerden biri, belirli bir havuz için her tokenın kesin bir miktarını yatırmak zorunda olmamasıdır. Bunun yerine, tek bir token sağlanabilir ve havuzu yöneten algoritma, yatırdığınız miktarın bir kısmını satarak diğer tokenları otomatik olarak ayarlayacak ve havuzda doğru bir oranı korumak için diğer tokenları satın alacaktır.

Herhangi bir WBTC/WETH/USDC/USDT/DAI kombinasyonunu kabul eden atricrypto3 havuzunu kullanacağız ve bu havuza Augur tarafından oluşturulacak havuza USDC'yi ekleyeceğiz.

![Eylül 2021 itibarıyla Curve'deki atricrypto3 havuzunun ayrıntıları](<../.gitbook/assets/image (32).png>)

### AAVE

Augury ile ilgili paragrafta bahsedildiği gibi, AAVE, Augury'de yetiştirilen tokenlara Mai Finance'de kullanmadan önce küçük bir ödül eklemek için kullanılır. WBTC, WETH ve WMATIC'imizi doğrudan Mai Finance'e koymak yerine, bu tokenları AAVE'ye yatıracağız ve AAVE'den gelen ödülleri amToken havuzlarında otomatik olarak birleştirmek için Mai Finance'in getiri aracını kullanacağız ve camToken'ı kasalarda teminat olarak kullanacağız. [AAVE](broken-reference) bölümünü okuyarak fazla bilgi alabilirsiniz.

![Eylül 2021 itibarıyla AAVE kredi ödülleri](<../.gitbook/assets/image (33).png>)

### Balancer

Balancer, Curve gibi başka bir _blue chip_ projesidir. 2'den fazla tokendan oluşan havuzlara belirli tokenları yatırabileceksiniz ve aynı zamanda tek bir token yatırabileceksiniz. Havuz, içeriği oluşturan her tokenın eşit bir oranını elde etmek için otomatik olarak dengelenecektir.

Stratejimiz için WETH/BAL/Qi/MAI/USDC havuzunu kullanacağız. Bu havuz, Mai Finance'deki kasalardan toplanacak Qi tokenını kabul edecek ve bizi ek Qi ile ödüllendirecek ve BAL kasasında Mai Finance'e yatırabileceğimiz BAL tokenları ile daha fazla MAI elde ederek Augury'de pozisyonumuzu artıracağız.

![Eylül 2021 itibarıyla Balancer 5 havuzu](<../.gitbook/assets/image (34).png>)

## Sistemin Ateşlenmesi

![](<../.gitbook/assets/image (35).png>)

Aşağıda, 500$ değerinde MAI ödünç almak için camWETH kasasına yatırılan ve 500$ değerinde USDT-UST'ye dönüştürülen 1.000$ değerinde ETH'lik bir başlangıç yatırımı ile yapılan bir simülasyon yer almaktadır. Bu simülasyon, farklı sistemler için aşağıdaki ödülleri alır.

* USDT-UST farming APR'ı %22,53
* %0,39 amWBTC APR
* %1,71 amWETH APR
* %3,80 amWMATIC APR
* %3,86 otomatik bileşik LP tokenlı atricrypto3 APR, %13,09 WMATIC ve %17,63 CRV
* 1:6 BAL:Qi oranıyla %43,46 APR ile 5 tokenlı Balancer havuzu
* Apps Kasası, APR'leri ödüllendirir
  * camWBTC için %23,28
  * camWETH için %21,52
  * camWMATIC için %32,93
  * BAĞLANTI için %24,51
  * CRV için %116,71
  * BAL için %62,38

Bu APR'lerin tümü farklı platformlarda değişebilir ve bir yıl boyunca devam edeceklerinin garantisi yoktur. Sistemin olası genel APR'si hakkında bir fikir edinmek için onları bu simülasyon için olduğu gibi alacağız. Simülasyonu daha da "basitleştirmek" için fiyat değişikliklerini veya işlem ücretlerini dikkate almayacağız. Ayrıca bu simülasyonun, Mai Finance'deki Kasa Ödüllerinin ve Balancer ödüllerinin haftalık yerine günlük olarak birleştirildiğini, ancak bu ödüllerin şu anda kullanıcıların cüzdanına haftalık olarak gönderildiğini dikkate aldığını unutmayın. Son olarak, bu simülasyonun CDR'nin (**C**ollateral **D**ebt **R**atio) her zaman %200 olduğunu varsayacağız. Yani aldığımızın sadece yarısını ödünç alıyoruz. Ödülleri almaya devam etmek için para yatırın ve kolay likidasyonları önleyin.

### Birinci Gün

1000$ değerinde WETH'niz varsa amWETH almak için AAVE'ye yatırın, ardından camWETH almak için amWETH'inizi [Mai Finance](https://app.mai.finance/yield)'e yatırın ve son olarak camWETH'inizi 500 MAI ödünç alabilmek ilgili kasaya yatırın.

MAI'nizi USDT'ye dönüştürmek için [Anchor](https://app.mai.finance/anchor) kullanın (veya varsa [QuickSwap](https://quickswap.exchange/#/) gibi başka bir DEX kullanabilirsiniz. Bağlantıda likidite yoksa o zaman USDT'nizin %50'sini UST'ye takas etmek için [DFYN](https://exchange.dfyn.network/#/) kullanabilir ve daha sonra para yatırabileceğiniz bir USDT-UST çifti oluşturabilirsiniz. [Ağustos](https://augury.finance/infusions/). QuickSwap üzerinden satın alabileceğiniz bazı OMEN'lere de ihtiyacınız olacağını unutmayın.

Birinci günün sonunda aşağıdaki ödülleri toplarız

| Ödül Tipi             | Dolar karşılığı |
| --------------------- | --------------- |
| WBTC çiftçiliğinden   | 0.123           |
| WETH çiftçiliğinden   | 0.031           |
| WMATIC çiftçiliğinden | 0.031           |
| LINK çiftçiliğinden   | 0.031           |
| USDC çiftçiliğinden   | 0.092           |
| Qi kasa ödülü         | 0.295           |

Bunlar sadece ilk günün sonunda çiftçilikten ve borçlanarak elde ettiğimiz ödüller.

### İkinci Gün

Ödüller toplanır, WBTC, WETH ve WMATIC, AAVE ve Mai'deki getiri aracından geçtikten sonra Mai Finance'taki ilgili kasalara gönderilir. LINK, doğrudan LINK kasasına yatırılır ve USDC, atricrypto3 havuzunda Curve'e gönderilir. Qi ödülü Balancer'a gönderilir. Bu noktada, 3 camToken kasasından ve LINK kasasından (tam olarak 0.13$ değerinde MAI) daha fazla MAI ödünç alabiliriz ve ödünç aldığımız MAI'den daha fazla USDT-UST çifti oluşturabiliriz.

İkinci günün sonunda aşağıdaki ödülleri toplarız

| Ödül Tipi                 | Dolar karşılığı |
| ------------------------- | --------------- |
| WBTC çiftçiliğinden       | 0.123           |
| WETH çiftçiliğinden       | 0.031           |
| WMATIC çiftçiliği + Curve | 0.031           |
| LINK çiftçiliğinden       | 0.031           |
| USDC çiftçiliğinden       | 0.093           |
| CRV Curve'den ödül        | 0.00004         |
| BAL ödülü                 | 0.00005         |
| Qi kasa ödülü             | 0.296           |

Sistem tıkır tıkır çalışıyor, ödülleri topluyoruz ve her adım bir sonrakini besleyecek akışa sahip. Güzel ve küçük bir döngü oluşturduk.

## Farming Sonuçları

### Günlük Rutin

Günlük rutin aşağıdaki işlemlerden oluşur

* Augury'de hasat ödülleri
* AAVE'de WBTC, WETH ve WMATIC yatırın
* Getiri aracında Mai Finance'e amWBTC, amWETH ve amWMATIC yatırın
* Mai Finance'deki ilgili kasalara camWBTC, camWETH ve camWMATIC yatırın
* LINK'i Mai Finance'deki LINK kasasına yatırın
* Curve'deki atricrypto3 havuzuna USDC yatırın
* WMATIC'i Curve'den toplayın ve bunları camWMATIC kasasında kullanın
* CRV'yi Curve'den toplayın ve bunları CRV kasasında kullanın
* Farklı kasalardan MAI ödünç alın
* Anchor aracılığıyla Mai Finance'de MAI'yi USDT'ye dönüştürün
* DFYN'de USDT'nin %50'sini UST'ye dönüştürün
* DFYN'de yeni USDT-UST LP çifti oluşturun
* Yeni LP tokenlarını Augury'de yatırın

### Haftalık Rutin

Ek olarak, BAL (Balancerdaki Qi yatırımınızdan) ve Qi tokenlarından (kasa ödüllerinden) haftalık ödüller alacaksınız. Yapmanız gerekenler;

* Qi tokenını Balancer'a yatırın
* BAL tokenini Mai Finance'e BAL kasasına yatırın
* Ek BAL depozitonuzdan MAI ödünç alın ve bunları Augury'de USDT-UST çiftine dönüştürün

### Aylık Ham Sonuçlar

| Ay | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| -- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1  | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2  | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3  | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4  | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5  | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6  | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7  | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8  | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9  | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10 | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11 | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12 | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

Birkaç not:

* USDT-UST havuzunun büyümesi, kasalardan ödünç alınan ek MAI'nin tek sonucudur
* CRV havuzu, Curve'de çok düşük miktarda USDC yatırıldığı için neredeyse yok denecek kadar azdır.
* Balancer ödülünün %14,28'inin BAL tokenlarından ödenmesi, geri kalanının Qi tokenlarından ödenmesi nedeniyle BAL kasası önemli değildir.
* Balancer havuzundaki miktar en büyük kazançtır ve yalnızca Kasa ödüllerinin ve BAL ödüllerinin sonucudur

### 365 Gün Sonunda

Tam bir yıl sonra yatırımımızın son hali;

| Pozisyon    | Dolar Karşılığı |
| ----------- | --------------- |
| USDT-UST    | 553.24          |
| atricrypto3 | 36.20           |
| Balancer    | 137.62          |
| camWBTC     | 47.45           |
| camWETH     | 1,029.19        |
| camWMATIC   | 14.39           |
| LINK        | 11.84           |
| CRV         | 0.017           |
| BAL         | 3.93            |

Toplam borç aslında USDT-UST pozisyonunun tamamıdır, yani 553.24$ ve üretilen toplam ödül 280.63$'dır, bu da %28.06'lık bir nihai APY'ye karşılık gelir.

### Diğer Stratejilerle Karşılaştırma

Stabil coin çiftçiliğinde %28 APY almak çok da kötü değil. Peki 1.000 $ değerinde ETH ile uygulayabileceğimiz diğer daha kolay stratejilerle nasıl karşılaştırabiliriz? Aşağıdaki stratejiler için son APY'yi kontrol edelim

* AAVE aracılığıyla 8 kez amWETH'den yararlanın: bunun için [AAVE token kılavuzunda](broken-reference) açıklanan tam akışı kullanacağız.
* Augury'de stable coin çiftçilik: Bu strateji için, WETH'i satıyoruz ve Augury'de aynı infüzyonda 1.000 $ değerinde USDT-UST ile çiftliği satıyoruz
* QuickSwap'ta stabil coin çiftçilik: Bu strateji için, kasa ödülünden yararlanmak için camWETH kasasını kullanacağız ve Mai Finance'deki dQUICK kasasını kullanarak QuickSwap'ta 500$ değerinde MAI ile çiftlik yapacağız (MAI-DAI %19.78 APY'de) ek MAI ödünç almak ve çiftçilik havuzuna yeniden yatırım yapmak (%55,72 APR ile dQUICK kasaları)

| Strateji                          | Son APY |
| --------------------------------- | ------- |
| Bu kılavuzda sunulan strateji     | 28.06%  |
| AAVE'den 8x yararlanma            | 46.46%  |
| Sadece Augury'de stabil çiftçilik | 22.53%  |
| Quickswap çiftçiliği + dQUICK     | 35.96%  |

## Sorumluluk Reddi

Bu strateji gerçekten ilginç ve Mai Finance'in çoğu kasasını kullanıyor. Kılavuz çoğunlukla Eylül 2021'den itibaren stabil paralar üretirken daha fazla ödül kazanılabilecek stratejiler olduğunu göstermek için yazılmıştır. Ancak bu strateji en ilginç olanı olmayabilir ve çeşitli platformlarda çok sayıda manipülasyon içerir. Son olarak Augury çeşitli stratejilere dahil edilebilecek ancak muhtemelen yalnızca stabil çiftçilik yapmayan tokenlar üreten harika bir araçtır. Ve bir dip not olarak, nihai APY hesaplanırken hiçbir depozito ücreti veya performans ücreti dikkate alınmamıştır.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
