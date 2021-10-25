---
description: >-
  Bu kılavuz, Mai Finance ve QuickSwap'ta yeni LP havuzlarının kullanıma açılmasından sonra Mai Finance, QuickSwap ve Adamant arasındaki şaşırtıcı etkileşimleri vurgulayan bir strateji sunacaktır.
---

# Çiftçilik (Farming) mi Staking mi? Yoksa her ikisi de mi?

![](<../.gitbook/assets/Screen Shot 2021-09-03 at 9.24.12 AM.png>)

## Giriş

DeFi (**De**centralize **Fi**nance) uygulamalarını kullanırken, özellikle de ürün yetiştirirken, çiftlik tarafından verilen bir sürü platform tokenı elde etme imkanına sahipsiniz. Çoğu insan bu tokenları sevdikleri veya tercih ettikleri tokenları satın almak için satıyorsa, gelirlerinizi artırmak için onları gerçekten tutmanın ve çalıştırmanın bazı yollarını göstermeye çalışacağız.


Stratejiyi uygulamak için, Eylül 2021'in başında QuickSwap'ta başlatılan ve Mai Finance'in Qi tokenını kullanan yeni LP havuzlarını (**L**iquidity **P**rovider havuzları) kullanacağız. QuickSwap ve Adamant uygulamalarının ne olduğu hakkında iyi bir fikre ihtiyacınız varsa, lütfen [Stack DApp'leri kılavuzunu](stack-dapps-like-lego-bricks.md) okuyun.

## Uygulama ve Havuz Tanıtımı

### Farming Bölümü

Kazanımlarımızı maksimize etmek için 3 farklı uygulama kullanacağız.

* Mai Finance
* QuickSwap
* Adamant

Aşağıdaki LP havuzlarını da kullanacağız

* Qi için Mai Finance üzerinde Qi/MATIC
* QUICK ve ADDY için QuickSwap üzerinde Qi/WETH
* ADDY ve MATIC için Adamant'ta Qi/QUICK

Her uygulamanın, diğer uygulamalarda kullanılan diğer havuzları besleyebilecek tokenlar ürettiğini zaten görebilirsiniz. Buradaki fikir, Mai Finance'de hasat edilen Qi'yi QuickSwap'ta hasat edilen QUICK ile birlikte kullanmak ve Adamant'ta 2'yi kullanmaktır. Adamant, MATIC kazanımlarınızı talep etmenize izin verecek ADDY üretecektir. MATIC, MAI ödünç almak için WMATIC kasasındaki Mai Finance'e kilitlenebilir ve ardından hem Mai Finance hem de QuickSwap'taki pozisyonlarınızı artırmak için Qi kullanabileceğimiz MATIC ve WETH satın alınabilir.

### Staking Bölümü

Ayrıca Mai Finance ve QuickSwap'ta fazla üretilen tokenlerin stake edilebileceğini de bilmeniz gerekir:

* Mai Finance'de Qi **VE** QuickSwap, QIP'de oy vermek için kullanılabilir (**Q**iDAO **I**mprovement **P**roposals).
* Mai Finance'deki Qi kilitlenebilir. Qi'nizi kilitlerseniz, Qi olarak ödenen ve her Çarşamba dağıtılan protokol temettülerine hak kazanırsınız. Qi staking hakkında daha fazla ayrıntı yakında.
* QuickSwap üzerinde QUICK, Dragon's Lair'de ek QUICK oluşturmak için de stake edilebilir.
* kilitli QUICK (dQUICK), Dragon's Syrup'ta başka tokenlar oluşturmak için QuickSwap'ta da kullanılabilir ve kullanacağımız ADDY'leri üreten çiftliktir.
* ADDY on Adamant otomatik olarak kazanılır (90 gün boyunca kilitlenir), WMATIC temettüleri oluşturur.
* ADDY on Adamant, APR'lerinizi/APY'lerinizi artırmak için de kilitlenebilir (**A**nnual **P**ercentage **R**ewards / **A**annual **P**ercentage ** Y**ield) siteye girdiğiniz havuzlarda, daha fazla ADDY üreterek ve MATIC temettülerinizi artırabilirsiniz.

## Sistemin Ateşlenmesi

![](<../.gitbook/assets/Screen Shot 2021-09-08 at 6.54.08 AM.png>)

Aşağıda, 1.000 $ değerinde Qi/MATIC ve Qi/WETH LP tokenları ve 9 Eylül 2021'de farklı platformlar tarafından verilen mevcut APR'ler / APY'ler ile yapılan bir simülasyon yer almaktadır. Tanımladığımız şeyin gerçek bir uygulaması değildir. Oranlar değişecek, token fiyatları değişecek, bazı programlar sona erecek vs... bu nedenle nihai sonuçlar, her şey sabit kalırsa elde edebileceğinizin bir tahminidir, ki bu asla böyle olmayacak.

### 1. Gün

{% hint style="info" %}
**DİKKAT:** Bu kılavuzda kullanılan havuzlar, yayınlanmadan birkaç saat önce yayına girmiştir. APR'ler ve APY'ler açıkça aynı kalmayacak ve birkaç gün içinde bazı revizyonlar yapılacak. Lütfen, DYOR ve kılavuzu dikkatli bir şekilde inceleyin.
{% endhint %}

500$ değerinde Qi/MATIC LP tokenlarımız ve 500$ değerinde Qi/WETH LP tokenımız olduğundan bunları Mai Finance ve QuickSwap'a yatıracağız. Bir yan not olarak, Qi veya QuickSwap için bir tercihiniz varsa, favori tokenınızdan daha fazlasını oluşturmak ve daha fazla stake yapmak için bir veya diğer platforma daha fazla LP token koyabilirsiniz. Örneğimiz için, kesin bir %50'lik bölünmeye bağlı kalacağız.

* 500$ Qi/MATIC, %1160.65 APR ile Mai Finance'de olacak
* 500$ Qi/WETH, %1817,44 APR ile QuickSwap'ta olacak

Simülasyonun geri kalanı için aşağıdaki APR'leri de kullanacağız.

* Dragon's Lair'den dQUICK APR %17,28
* Dragon's Syrup'tan ADDY APR %17,08'dir.
* Otomatik bileşik LP tokenları için Adamant'ta Qi/QUICK APR %133'tür
* ADDY tokenleri için Adamant'ta Qi/QUICK APR %131'dir
* Adamant'ta WMATIC APR, kilitli ADDY tokenlarının %35'idir

Mai Finance'deki APR QuickSwap'takinden daha düşük olduğundan, ek Qi/QUICK tokenları oluşturmak için Mai Finance'de üretilen Qi'nin %100'ünü kullanacağız (satmıyor, QuickSwap'ta alınan QUICK ile birleştiriyoruz), yani şu anlama geliyor: günün sonunda, elimizde 0 Qi kaldı. Tabii ki, ilk yatırımınızı farklı şekilde dengelerseniz, kalan Qi ve 0 QUICK'i elde edebilirsiniz.

Bu nedenle, 1. Günün sonunda portföyümüzde

| Ödül Tipi           | Dolar Karşılığı  |
| ------------------- | ---------------- |
| QuickSwap'ta dQUICK | 8.997            |
| QuickSwap'ta ADDY   | 0                |
| Adamant'ta Qi/QUICK | 31.799           |
| Adamant'ta ADDY     | 0                |
| Adamant'ta WMATIC   | 0                |

### 2. Gün

İkinci günde QuickSwap'ın Dragon's Syrup'una yatırılan dQUICK, ADDY tokenlarırının yanı sıra Adamant'ta Qi/QUICK LP çifti üretmeye başlar. 2. günün sonunda,

| Ödül Tipi           | Dolar Karşılığı  |
| ------------------- | ---------------- |
| QuickSwap'ta dQUIC  | 17.998           |
| QuickSwap'ta ADDY   | 0.0042           |
| Adamant'ta Qi/QUICK | 63.713           |
| Adamant'ta ADDY     | 0.114            |
| Adamant'ta WMATIC   | 0                |

WMATIC temettüleri oluşturmaya başlamak için ödüllerinizi Adamant'ta her gün talep etmeyi unutmayın!

### 3. Gün

Üçüncü günde Adamant'ta toplanan ADDY, WMATIC temettüleri üretmeye başlayacak. Bu durumda 3. günün sonunda portföyümüze gireceğimiz anlamına gelir.

|  Ödül Tipi          | Dolar Karşılığı  |
| ------------------- | ---------------- |
| QuickSwap'ta dQUICK | 27.004           |
| QuickSwap'ta ADDY   | 0.025            |
| Adamant'ta Qi/QUICK | 95.743           |
| Adamant'ta ADDY     | 0.343            |
| Adamant'ta WMATIC   | 0.0001           |

4. günden başlayarak yapılacaklar;

* WMATIC temettülerini toplayın
* WMATIC'in bir kısmını Mai Finance'e yatırın ve buna karşı MAI ödünç alın
* daha fazla WETH almak için MAI sat
* kalan MATIC'i Qi ile ve WETH'i Mai Finance'te oluşturulan biraz daha Qi ile eşleştirin
* ek Qi/WMATIC çiftini Mai Finance'e ve Qi/WETH çiftini QuickSwap'a yatırın

Bu noktada, çiftçilik sistemi tamamen hazırdır ve gelirleri tahmin etmeye başlayabiliriz.

## Farming sonuçları

### Günlük Rutin

Günlük rutin aşağıdaki işlemlerden oluşur

* Mai Finance'de Qi hasat edin
* Adamant'ta WMATIC hasat edin
* WMATIC'in %66'sını Mai Finance'e yatırın
* Mevduatın %50'si için MAI ödünç alın
* MAI'yi WETH ile değiştir
* QuickSwap'ta Qi/WMATIC çifti oluşturun
* Qi/WMATIC'i Mai Finance'e yatırın
* QuickSwap'ta Qi/WETH çifti oluşturun
* Qi/WETH'yi QuickSwap'a yatırın
* QuickSwap'ta QUICK Hasat
* QuickSwap'ta Qi/QUICK çifti oluşturun
* Dragon's Lair'de kalan QUICK'leri yatırın
* Dragon's Syrup'a dQUICK yatırın
* Dragon's Syrup'tan ADDY hasat edin
* Adamant'tan ADDY  hasat edin
* Adamant'a yeni Qi/QUICK yatırın
* ADDY'yi Adamant'ta toplayın (kilit)

### Ay sonunda oluşan ham sonuçlar

| Ay    | dQUICK    | Qi/QUICK   | ADDY       | Qi/MATIC Qi/WETH |
| ----- | --------- | ---------- | ---------- | ---------------- |
| 1     | $280.96   | $1,040.78  | $54.97     | $0.91            |
| 2     | $557.79   | $2,162.98  | $224.36    | $7.89            |
| 3     | $842.08   | $3,413.73  | $521.09    | $27.85           |
| 4     | $1,138.60 | $4,816.62  | $960.17    | $68.48           |
| 5     | $1,454.30 | $6,405.18  | $1,559.60  | $138.44          |
| 6     | $1,798.77 | $8,224.86  | $2,341.64  | $247.49          |
| 7     | $2,184.58 | $10,335.38 | $3,334.13  | $406.84          |
| 8     | $2,627.76 | $12,813.60 | $4,572.23  | $629.47          |
| 9     | $3,148.40 | $15,757.01 | $6,100.39  | $930.60          |
| 10    | $3,771.42 | $19,288.05 | $7,974.83  | $1,328.32        |
| 11    | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31        |
| 12    | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79        |

### 365 gün sonunda

Tam bir yıl sonra yatırımımızın son hali

| Ödül Tipi                     | Dolar Karşılığı  |
| ----------------------------- | ---------------- |
| QuickSwap'ta dQUICK           | 5,628.29         |
| QuickSwap'ta ADDY             | 365.25           |
| Adamant'ta Qi/QUCK            | 29,733.58        |
| Adamant'ta ADDY               | 13,587.56        |
| Ek Qi/MATIC + Qi/WETH         | 2,631.07         |

QuickSwap çiftliği aracılığıyla oluşturulan ADDY'nin günlük olarak hasat edilmediğini ve bu simülasyonda Adamant'taki ADDY ödüllerini artırmak için eklenmediğini unutmayın (zaten yeterince karmaşıktır). Ayrıca, sadece kazanılmış ADDY'yi dikkate alıyoruz. 90 günlük ilk hak kazanma döneminden sonra, ADDY talep edip kilitlerseniz, ADDY ödüllerinizi daha da artıracak ve daha fazla WMATIC üreteceksiniz.

Son olarak, bir yıl sonra elde edilen gelir 51.580,50 $ değerindedir. İlk yatırımın 1.000$ değerinde Qi/MATIC ve Qi/WETH olduğunu düşünürsek, bu, %5,087.39'luk bir nihai APY'ye yol açar.

## Sorumluluk Reddi

Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildir. Lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeye hazır olduğunuza yatırım yapın.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen farkında olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
