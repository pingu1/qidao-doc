---
description: >-
  Bu kılavuz, ödül çarpanı olarak bir Ohm benzeri platformda stabil yatırımlarınızı en üst düzeye çıkarmanın yeni bir yolunu önerecektir.
---
# Fil, Şempanze ve Su Samuru
 
## Introduction
 
Bu başlık bir şiir için iyi bir başlık olabilirdi ancak görünüşe göre bunlar, kılavuzda tartışacağımız protokollerin 3 totem hayvanı. Bugün, Mai Finance'deki MAI destekleyen teminat token koleksiyonuna yapılan en yeni (Ocak 2022 itibariyle) eklemelerden birine yakından bakacağız: sdam3CRV tokenı. Ne olduğunu ve nasıl elde edebileceğinizi ayrıntılı olarak açıklayacağız. Ardından, Stake DAO, Mai Finance ve OtterClam protokolünün stabil makbuz tokenını ödül çarpanı olarak kullanarak yüksek getiri elde etmek için küçük bir strateji önereceğiz.
 
![](<../../.gitbook/assets/stakedao-otter-1.png>)
 
## Stake DAO
 
### Stake DAO'nun Tanıtımı
 
[Stake DAO](https://app.stakedao.org/)kullanıcıların varlıklarını yatırmalarını ve getirilerini en üst düzeye çıkarmak için en iyi stratejileri kullanmalarını sağlayan bir getiri optimizasyon platformudur. Yatırımlar bir risk puanı ile teklif edilir ve yatırımlar, seçilen stratejilerin sonuçlarını takip etmeyi kolaylaştıran güzel bir gösterge panosunda görüntülenir. Stake DAO, öncelikle Ethereum ana ağında başlatıldı ve hızla Polygon ve Avalanche gibi diğer zincirlere doğru genişliyor. Elbette Stake DAO hakkında daha fazla bilgiyi [resmi belgelerinden](https://stakedao.gitbook.io/stakedaohq/) okuyabilirsiniz.
 
### am3CRV Stratejisi
 
Kılavuzumuz için Polygon’da `Pasif Aave USD Stratejisini` kullanacağız. Bu strateji, [Curve Finance](https://polygon.curve.fi/)'ınn am3CRV havuzunu kullanan bir stratejidir: stabil varlıklarınızı (USDC, USDT veya DAI) Curve'deki aave havuzuna yatırırsınız ve bir am3CRV makbuz tokenı alırsınız. Bu token, CRV ve WMATIC ödüllerini almak için doğrudan Curve üzerinde stake edebileceğiniz tokendır. Ayrıca bu tokenı Stake DAO'ya da yatırabilirsiniz ve böylece CRV ve WMATIC ödülleri satılarak stabil pozisyonunuza eklenecektir.

![Ocak 2022 itibariyle Curve'de aave havuzu](<../../.gitbook/assets/stakedao-otter-2.png>)
 
Yukarıda görebileceğiniz gibi am3CRV tokenlarınızı Curve'de stake etmek size toplam %8,35 APR (Yıllık Yüzde Ödül) verir. Stake DAO'ya girerseniz Polygon için Stratejiler sekmesinde am3CRV tokenlarını kullanan stratejiyi bulacaksınız, burada makbuz tokenınızı yatıracak ve %11.11 APY kazanacaksınız (Ödüllerinizi en az günlük olarak birleştirdiğinizi varsayan Yıllık Yüzde Verim)
 
![Ocak 2022 itibariyle Stake DAO'da Pasif AAVE USD Stratejisi](<../../.gitbook/assets/stakedao-otter-3.png>)
 
am3CRV tokelarınızı Stake DAO'ya yatırdığınızda, yeni bir makbuz tokenı alacaksınız: sdam3CRV (stake dao am3CRV).
 
{% hint style="info" %}
Stake DAO kullandığınız her strateji için kazançlarınızdan ücret aldığını lütfen unutmayın. Bizim durumumuzda ve Ocak 2022 itibariyle performans ücreti %15 olup ayrıca %0,5 para çekme ücreti olacaktır. Havuza girmeden önce bunu anladığınızdan emin olun.
{% endhint %}
 
Bu strateji, yalnızca stablecoin’ler kullandığından çok güvenli (DYOR) olarak kabul edilebilir. Am3CRV LP tokenı yalnızca dolara sabitlenmiş stablecoin’lerden oluştuğu için Kalıcı Kayıp riski sıfıra yakındır. Stake DAO'yu kullanmak istiyorsanız AAVE'deki varlığınız Curve aracılığıyla borç verildiğinden ve LP tokenı Stake DAO'da olduğundan akıllı sözleşme risklerini hesaba kattığınızdan emin olun, yani risklere maruz kalan 3 katman protokolünüz var.
 
Sdam3CRV tokenlarınızı yatırmak ve Stake DAO'nun yerel tokenı olan SDT tokenında ~%9 ekstra ödeme almak için Stake DAO'daki çiftçilik (farming) aracını kullanabilirsiniz. Ancak kılavuzumuz için sdam3CRV tokenını farklı şekilde kullanacağız.
 
## Mai Finance
 
[Mai Finance](https://app.mai.finance) varlıklarınızı teminat olarak yatırmanızı ve bu para karşılığında borç almanızı sağlayan bir borç verme protokolüdür. Bu, borç alanlara varlık borç veren başkalarını bulacağınız ortalama bir borç verme platformu değildir. Mai Finance'de yalnızca kendinize borç verebilirsiniz ve yalnızca sahip olduğunuz varlıklar karşılığında borç alabilirsiniz. Mai Finance hakkında daha fazla bilgi için lütfen bu web sitesini veya [resmi belgeleri](https://docs.mai.finance/) inceleyebilirsiniz.

Ocak 2022'de sdam3CRV tokenı, Mai Finance'te bir teminat seçeneği olarak onaylandı. Bu da am3CRV lp tokenı Stake DAO'ya yatırarak oluşturulan tokenın artık MAI stablecoin’ini borç almak için kullanılabileceği anlamına gelir. Bu durum özellikle bazı nedenden dolayı harikadır:
 
* sdam3CRV tokenı yalnızca stablecoin’lerden oluşur, bu nedenle Geçici Kayıptan etkilenmemeli ve sabit bir fiyat tutmalıdır
* Fiyat fazla değişmediğinden likidasyon seviyesine yakın borç alsanız bile likidasyonlardan kaçınmak oldukça kolaydır
* Verim getiren bir varlık olduğu için teminatınızın değeri artar. Bu kılavuzu yazarken değerlere göre teminatınızdan %11 APR alacaksınız.
 
![Mai Finance'de bir sdam3CRV kasası örneği](<../../.gitbook/assets/stakedao-otter-4.png>)
 
Bu kasa, yüksek bir CDR (Borç Teminat Oranı) kullanıyor çünkü bu web sitesinde sunulan kılavuzlarda her zaman güvenliği teşvik etmeye çalışıyoruz. Yüksek bir CDR çeşitli avantajlar sağlar
 
* Teminatınızın büyük olumsuz fiyat hareketlerinde sizi likidasyondan uzak tutar
* Teminatınızın önemli bir bölümünü çekmenize ve borcunuzu ödemek için satmanıza olanak tanır. Lütfen (borç geri ödeme kılavuzumuza bakın](../../mai-university/debt-repayment-how.md))
 
Risk toleransınıza uygun bir CDR almaktan çekinmeyin.
 
{% hint style="info" %}
sdam3CRV kasası, teminat olarak stablecoin’leri kullanıyor. CamDAI kasası gibi herhangi bir borçlanma teşviki ALMAYACAKTIR. Likidasyon oranı da camDAI kasasında olduğu gibi %110'a düşürülebilir.
{% endhint %}
 
MAI ile teminatınız karşılığında borç alabilir, pozisyonunuzu kaldırabilirsiniz. Ayrıntılara ihtiyacınız varsa lütfen [camDAI Başlangıç Stratejisi](camdai-beginner-strategy.md) konusundaki özel kılavuzumuzu okuyun ve bunu sdam3CRV tokenlarınızda uygulayın. Aslında Stake DAO tarafından sağlanan faiz oranlarına sadece bazı kaldıraç döngülerini uygulayarak çok daha fazla maruz kalabilirsiniz. Ancak bu, MAI tokeni üzerinde güçlü bir satış baskısı oluşturuyor, bu nedenle farklı bir yaklaşım önereceğiz.
 
## OtterClam DAO
 
[OtterClam Finance](https://app.otterclam.finance/) Polygon üzerinde, çok yenilikçi, platformlarına harika NFT'leri entegre eden benzersiz bir Ohm klonudurdur. Kasım 2021'de piyasaya sürülen OtterClam, başlangıcından bu yana önemli ölçüde büyüme gösterdi ve şimdi GameFi'ye doğru ilerliyor.

OtterClam ile ilgili en ilginç şeylerden biri Mai Finance'in arkasındaki QiDao protokolü ile ortaklığıdır. CLAM tokenlarını destekleyen stablecoin’lerin çoğu, Mai Finance'te basılan stabilcoin MAI'de bulunur. Bu, doğrudan MAI kullanarak CLAM bonoları satın alabileceğiniz anlamına gelir ve stratejimizde tam olarak bunu yapacağız. Ohm klonları çok yüksek ödül oranları sunmalarıyla bilinir ve OtterClam da bir istisna değildir. OtterClam'deki bonoların bir başka benzersiz özelliği de sCLAM (stake edilen CLAM tokenları) satın almanızdır, böylece tokenlar, kilitlenme süresi boyunca rebase ödülleri alır ve bonoları daha da çekici hale getirir.
 
![Ocak 2022'den itibaren OtterClam Finance’te sCLAM bonoları](<../../.gitbook/assets/stakedao-otter-5.png>)
 
Bu ekran görüntüsünde aslında %3.66 indirimle sCLAM alacağımızı görebilirsiniz  (satın alma fiyatı 9,20 MAI iken piyasa fiyatı 9,54$’dır) ancak 5 günlük hak etme süresi boyunca satın alınan sCLAM da %6,95 artacaktır. Çok yüksek ödül oranları nedeniyle (yazım sırasında %13,400 APY), sCLAM tokenlarını stakede tutmak önemli olacak ancak am3CRV pozisyonumuzu artırmak için stablecoin staking ödüllerini satacak ve onları Curve'e yatıracağız.
 
![Tebrikler, CLAM stake ettiniz](<../../.gitbook/assets/stakedao-otter-6.png>)
 
CLAM'lerin fiyatını kontrol ederseniz bu tokenın çok fazla oynaklığa sahip olduğunu göreceksiniz. Çoğu Ohm klonunda olduğu gibi tokenın fiyatı önemsizdir, kazançlar için çarpan olarak yalnızca OtterClam kullanıyoruz. Ohm klonları, token fiyatını 1$’a (veya tokenı destekleyen herhangi bir varlığa) düşürmek için tasarlanmıştır ve token, kullanılmak ve satın alınmak/satılmak üzere tasarlandığı anlamına gelen bir "rezerv para birimi" dir
 
{% hint style="info" %}
Stake ödülleri hak kazanma süresi boyunca erişilemeyen kazanılmış sCLAM tokenlarında birikir. Stake ödüllerini toplayıp satabilmemiz için hak kazanma tokenlarının tamamen kazanılmasını beklememiz gerekecek.
{% endhint %}
 
## Farming Stratejisi 
 
Çoğu durumda olduğu gibi stratejiler için en iyi başlangıç noktası stablecoin’lerle başlamaktır. Bu şekilde kalıcı kayıp riskini azaltırsınız ve yalnızca çiftçiliğinizden (veya bizim durumumuzda borç alınan miktardan) gelen faydalarla çalışırsınız. Böylece döngü, am3CRV tokenı almak için Curve’e stablecoin’ler yatırarak başlar. Bu makbuz tokenı, bir sdam3CRV makbuzu alabilmeniz için Stake DAO'ya yatırılır. Bu token, MAI'yi borç almak için teminat olarak Mai Finance'e yatırılacaktır. Borç, OtterClam'de MAI bonoları satın almak için kullanılır. Rebase ödülleri, stablecoin’ler için değiştirilir. Bir ek not olarak, rebase ödülleri ne kadar olursa olsun satabilirsiniz. Kılavuzumuzda bunun %100'ünü satacağız ancak CLAM konumunuzu daha hızlı artırmak ve daha büyük ödülleri daha hızlı toplamak için birazını tutabilirsiniz.
 
Simülasyonlar için her zaman olduğu gibi tüm sayıları aşağıdaki gibi düzelteceğiz:
 
* Stake DAO'daki sdam3CRV stratejisi için APY %11,11'dir
* OtterClam'de stake edilen CLAM'ler için APR %13,400'dür
 
Ayrıca borcun geri ödenmesiyle de uğraşmayacağız ve tüm fiyatların aynı kaldığını varsayacağız. Simülasyonu başlangıç noktası olarak 100$ değerinde USDC ile işleteceğiz ve ayrıca daha fazla MAI borç alındığında %235'lik bir CDR'ye bağlı kalmaya çalışacağız. Son olarak bu simülasyonda kolaylık olması için her hak kazanma döneminin sonunda %0 indirimli kullanılabilir bir MAI bonoları olduğunu varsayacağız (tabii ki %0'dan büyük indirimler kovalayacaksınız).
 
![](<../../.gitbook/assets/stakedao-otter-7.png>)
 
### 1. Gün
 
1. günde hemen hemen her şeyi hazırlayabilirsiniz:
 
* 100$ değerindeki USDC'nizi (ya da USDT veya DAI’nizi) Curve Finance’e yatırın
* am3CRV makbuz tokenınızı Stake DAO'ya yatırın
* sdam3CRV lp tokenınızı Mai Finance'e yatırın
* İlk borç için %200 CDR veya 50$ MAI değerinde borç alın
* OtterClam Finance'te bir MAI bonosu satın alın
 
Artık hazırsınız. Rebase ödüllerini toplamaya başlamak için hak etme süresinin tamamını beklemeniz gerekecek. 1. Günün sonunda,
 
| Pozisyon            | Değer ($) |
|---------------------|-----------|
| sdam3CRV            |   100.000 |
| MAI Borç            |    50.000 |
| sCLAM               |    50.000 |
| İlave sdam3CRV      |     0.030 |
| İlave sCLAM         |     0.000 |
 
### 2, 3 ve 4. Gün
 
Söyleyecek bir şey yok, sdam3CRV'niz getiri topluyor ancak bu süreçte ödülleri toplayamazsınız.
 
### 5. Gün
 
5. günün sonunda bono tamamen kazanılır. Rebase ödülleri tüm hak kazanma süresi boyunca bir araya getirildiğinden günün sonunda sahip olacağınız şey,
 
| Pozisyon            | Değer ($) |
|---------------------|-----------|
| sdam3CRV            |   100.122 |
| MAI borç            |    50.000 |
| sCLAM               |    53.382 |
| İlave sdam3CRV      |     0.030 |
| İlave sCLAM         |     0.722 |
 
### 6. Gün
 
Yeni bir bono satın almak için borç alabileceğiniz bazı ek sdam3CRV tokenlarınız var. Bu çok küçük bir bono olacak (şimdilik sadece birkaç sent) ama zamanla yeni MAI'niz ile daha fazla sCLAM satın alabileceksiniz. 6. Günün sonunda,
 
| Position            | Değer ($) |
|---------------------|-----------|
| sdam3CRV            |   100.875 |
| MAI borç            |    50.437 |
| sCLAM               |    53.820 |
| İlave sdam3CRV      |     0.031 |
| İlave sCLAM         |     0.728 |
 
Bu noktada, stake edilen CLAM'larınız her gün sdam3CRV kasanızda birleştirebileceğiniz veya bono kazanıldığında her 5 günde bir birleştirebileceğiniz ödüller üretecektir.
 
### Günlük Rutin
 
Her gün varlıkların birleştiğini varsayarsak günlük rutin
 
* stake edilen CLAM'larınızdan 3 rebase eşdeğerini unstake edin
* piyasa durumuna göre alacağınız stablecoin ne olursa olsun onları satın
* ek stablecoin’leri Curve Finance'teki aave havuzuna yatırın
* am3CRV tokenını Stake DAO'ya yatırın
* sdam3CRV tokenını Mai Finance'e yatırın
 
Ardından her 5 günde bir aşağıdaki ek adımları gerçekleştirebileceksiniz:
 
* %200'lük bir CDR'yi korumak için ek MAI borç alın
* tterClam'de ek MAI bonosu satın alın
 
### Aydan aya ham sonuçlar
 
İşte aydan aya ham sonuçlar

| gün |  sdam3CRV  |    CLAM    |   MAI borç |
|-----|------------|------------|------------|
|  30 |    121.249 |     64.007 |     60.625 |
|  60 |    150.866 |     78.815 |     75.433 |
|  90 |    187.350 |     97.057 |     93.675 |
| 120 |    232.294 |    119.529 |    116.147 |
| 150 |    287.659 |    147.212 |    143.830 |
| 180 |    355.863 |    181.314 |    177.931 |
| 210 |    439.882 |    223.323 |    219.941 |
| 240 |    543.383 |    275.074 |    271.691 |
| 270 |    670.884 |    338.825 |    335.442 |
| 300 |    827.950 |    417.358 |    413.975 |
| 330 |  1,021.437 |    514.101 |    510.719 |
| 360 |  1,259.790 |    633.277 |    629.894 |
 
### 365. Gün
 
Bu sistemde tam bir yıl çiftçilik yaptığınızı ve her şeyin 1. Gün'dekiyle aynı olduğunu varsayarsak (fiyatlar, oranlar ve diğer her şey) şunları elde edersiniz:
 
* Mai Finance'teki kasanızda 1.304.575$ değerinde sdam3CRV tokenlar
* OtterClam Finance’te 655.670$ değerinde CLAM
* 652.288$ değerinde MAI borcu
 
Yıl sonunda hala %200'lük bir CDR'niz olduğunu görebilirsiniz. Borcunuzu ödemek ve teminatınızın geri kalanının kilidini açmak için teminatınızı çekebilirsiniz. CLAM'lerinizi satarak ve teminatınızın %100'ünü açarak da borcunuzu ödeyebilirsiniz.
 
Sonunda 100$'lık bir ilk yatırımdan 1.307.958$ ve 652.288$'lık bir borç elde edersiniz, bu da toplam 1.207.958 APY'ye tekabül eder.
 
{% hint style="success" }
OtterClam Finance'ten rebase ödülünüzün yalnızca %50'sini çeker ve geri kalanını stake ederseniz yüksek APY çok daha hızlı büyüyen bir pozisyona uygulanır. Bu daha fazla risk taşır ancak her şeyin aynı kaldığını ve ödülünüzün yalnızca %50'sini sattığınızı varsayarsak, potansiyel olarak kasanız ve OtterClam arasında 3.608.447$'lık bir payla ve %2.757.619'luk eşdeğer bir APY için 750.828$'lık bir borçla sonuçlanabilirsiniz.
{% endhint %}
 
## Sorumluluk Reddi
 
Bu strateji oldukça ilgi çekicidir çünkü başlangıçta çok az risk taşır. Paranız stabillerde çalışır ve ilk para "korunur", bu nedenle onu kaybetme olasılığı çok düşüktür. Teminat ve borç alınan varlık arasında çok küçük bir fiyat farkı için kullanılan yüksek CDR nedeniyle likidasyon riski de çok küçüktür. Ek araçlar olmadan muhtemelen ~%12 APY elde edersiniz ancak ödülleri en üst düzeye çıkarmak için diğer protokolleri kullanmanın çok yüksek getirilerle sonuçlanabileceği açıktır.

Ancak bu yatırım stratejisini en ince ayrıntılarına kadar anladığınızdan emin olun. Birçok farklı protokol kullandığımız için akıllı sözleşme risklerini kabul ettiğinizden emin olun. Ayrıca Ohm klonlarının nasıl çalıştığını anlamanız ve çok değişken olabilen CLAM'lerin fiyatına dikkat etmemeniz gerekir. Son olarak, Stake DAO'da oranlar aynı kalabilirse ohm klonları bu kadar yüksek APY'leri uzun süreler boyunca sürdüremeyeceğinden OtterClam'deki ödül oranı zamanla düşecektir. Her zaman olduğu gibi kullanacağınız farklı projelerin belgelerini okuyun ve tüm riskleri anladığınızdan emin olun.
 
{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın.
{% endhint %}
 
