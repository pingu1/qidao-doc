---
description: Bu eğitim, MAI'nizi Polygon'da farklı kullanım seçeneklerini size sunacaktır.
---

# Polygon'da MAI ile ne yapabilirim?

## Eğitimin Amacı

Bu eğitimin amacı, MAI stable tokenınızla neler yapabileceğinizi ayrıntılı olarak sunmak değil, MAI'nizi Polygon'da doğrudan veya kombinasyon halinde kullanmanıza izin verecek fikirler vermek ve değerlendirebileceğiniz tüm web sitelerinin ve DeFi uygulamasının bir listesine sahip olmaktır. MAI'yi kullanmanın belirli yolları hakkında daha fazla ayrıntı için bu sitedeki diğer eğitimlere başvurabilir veya Discord veya Telegram'da yardım alabilirsiniz.

Lütfen listenin tam olmadığını ve ağda her hafta yeni dapp'ler başlatıldığı için listenin asla güncel kalmayacağını unutmayın. Hepsini inceleyemiyorum, bu yüzden sadece ana seçenekleri veya en ünlü / en "güvenli" seçenekleri sunacağım.

Belirli bir projenin listelenmesini istiyorsanız lütfen [Discord](https://discord.gg/mQq55j65xJ) üzerindeki Qi topluluğuna katılın.

{% hint style="info" %}
Mai Finans çiftliklerini sunmayacağım. Bu konu başlı başına incelenmeyi hak ediyor çünkü Qi diğer rastgele çiftlik tokenlarına benzemiyor.
{% endhint %}

## Bluechip projelerinde güvenle çiftçilik yapın

Bluechip projeleri, sağlam olduğu kanıtlanmış ve daha düşük risk arz eden DeFi uygulamalarıdır. Genellikle denetlenirler ve arkasındaki ekip uzun süredir üzerinde çalışmaktadır. Genellikle çok büyük APR'leri yoktur (**A**nnual **P**ercentage **R**ewards) ancak güvenilir olabilirler.

### Balancer

[Balancer](https://polygon.balancer.fi/#/) otomatik bir portföy yöneticisi, likidite sağlayıcısı ve fiyat sensörüdür. Platformda kripto paranızı ödünç verebileceksiniz ve arbitraj fırsatlarını takip ederek portföyünüzü yeniden dengeleyen tüccarlardan ücret alacaksınız. Balancer hakkında daha fazla ayrıntıya ihtiyacınız varsa lütfen [resmi dokümanı](https://docs.balancer.fi) okuyun.

Polygon ağında Balancer, 4 ana stabil tokendan oluşan bir havuz önerir: DAI, USDC, USDT ve MAI (miMATIC). Bu havuzun şu anda APR'ı \~%20'dir.

![Ağustos 2021 itibarıyla stabil para para havuzu durumu](<../.gitbook/assets/Screen Shot 2021-08-11 at 11.06.59 AM.png>)

Balancer'ın en iyi yanı, havuza yatırmak için kesinlikle 4 tokena sahip olmanıza gerek olmamasıdır. Dengeleyici, yaptığınız para yatırma işlemiyle otomatik olarak dengeli bir kombinasyon oluşturacaktır. Yani 100$ değerinde MAI'niz varsa, bunları Balancer havuzuna yatırabilir ve yatırma anındaki ilgili fiyatlarına bağlı olarak algoritmanın her madeni para için %25'lik bir orana sahip olacak şekilde doğru şekilde kaydırmasına izin verebilirsiniz.

Havuz ödülleri, haftalık olarak dağıtılan BAL tokenı kullanılarak ödenir. BAL'a ek olarak, girdiğiniz havuza bağlı olarak ek ödüller de verilebilir. Farklı [teşvik programını buradan](https://balancer-incentives.web.app) kontrol edebilirsiniz. Bizim durumumuzda bu havuza katılmak size MATIC ve Qi ödülleri de kazandıracak.

Tam akış böyle bir şey olurdu

![](<../.gitbook/assets/Screen Shot 2021-08-11 at 11.34.45 AM.png>)

Kriptonuzu ödünç vermek ve MAI ödünç almak için (MAI satın almak için kriptonuzu satmak yerine) Mai Finance'i nasıl kullanabileceğiniz konusunda daha fazla ayrıntıya ihtiyacınız varsa, bu sitedeki diğer kılavuzları okuyun. Hatta daha da fazla kazanmak için [döngüye AAVE'yi dahil edebilirsiniz](broken-reference).

### Curve Finance

Burada biraz tıklama işiniz var. [Curve](https://polygon.curve.fi), kripto varlıklarınızı doğrudan MAI değil (henüz değil mi?) gelir elde edecek havuzlarda ödünç verebileceğiniz başka bir platformdur. İlgilendiğimiz havuzlar

* Stabil para üçlüsünde (DAI/USDC/USDT) %5 ile %15 arasında APR (APR çok değişir) oluşturacak AAVE havuzu. Havuz, protokol tarafından AAVE'de kullanılacak tek bir varlık kullanarak havuza girebileceğiniz şekilde tam olarak Balancer gibi çalışır.
* Stabil para üçlüsünden oluşan ve kalıcı kayıpları azaltmak için wETH ve wBTC'yi de içeren atricrypto havuzu. Bu havuzun %25 ile %30 arasında değişen bir APR'si vardır. Mai Finans ekibi şu anda MAI'nin bu havuza eklenmesini sağlamaya çalışıyor.

Curve protokolünün MAI'yi havuzlarında geçerli bir stabil para olarak kabul etmesini beklerken, yine de aşağıdaki adımları izleyerek en sevdiğiniz kriptoyu Curve ile kullanabilirsiniz (örnek MATIC ile)

* MATIC'i AAVE'ye yatırın ve amWMATIC'i toplayın
* AmWMATIC'inizi Mai Finance'e yatırın ve camWMATIC toplayın (AAVE ödülleri, camWMATIC tokenları ile birleştirilecektir)
* CamWMATIC'i Mai Finance'te teminat olarak kullanın ve buna karşı MAI ödünç alın
* Tüm MAI'nizi USDC ile değiştirmek için Mai Finance'deki [değişim sayfasını](https://app.mai.finance/anchor) kullanın
* Bu durumda;
  * USDC'nizle Curve'deki atricrypto havuzuna girin ve %25 ila %30 ödül kazanın
  * USDC'nizle Curve'deki AAVE havuzuna girin ve %5 ila %15 arasında ödül kazanın

Curve'deki ödüller şu şekilde verilir:

* Havuzdaki konumunuzu artıran otomatik bileşik USDC (atricrypto havuzu için USDC/USDT/DAI ve muhtemelen wBTC/wETH karışımı olacaktır)
* Daha sonra yukarıdaki döngüyü tekrarlamak ve kredinizi ve yatırım sermayenizi artırmak için kullanabileceğiniz WMATIC
* Daha fazla MAI ödünç almak ve yatırım sermayenizi artırmak için Mai Finance'te teminat olarak da kullanılabilen CRV tokenı

![](<../.gitbook/assets/Screen Shot 2021-08-11 at 12.14.27 PM.png>)

### AAVE

[Aave Market'ten Yararlanın](broken-reference) için Mai Finance'i nasıl kullanabileceğinize dair eksiksiz bir kılavuz var. Aave, MAI'nin doğrudan kullanımını yapmıyor, ancak gelecekte AAVE'nin kriptonuzu ödünç verebileceğiniz bir MAI havuzuna sahip olacağını hayal edebiliyoruz.

### QuickSwap

[QuickSwap](https://quickswap.exchange/#/) muhtemelen SushiSwap ve 1Inch ile Polygon'daki en ünlü DEX'lerden (Merkezi Olmayan Değişim) biridir. Aynı zamanda, kullanıcıların likidite havuzlarını kullanarak Polygon ağında verimli bir şekilde işlem yapmalarını sağlayan bir AMM'dir (Otomatik Piyasa Yapıcı). Borsadaki herhangi bir işlem, likiditelerini platforma yatıran kullanıcılara kısmen yeniden dağıtılan bir ücrete tabidir.

QuickSwap'ta MAI'yi kullanma şekliniz \[düzenli verim çiftliğine]\(secure-your-get- farm-profits.md) çok benzer, bu nedenle QuickSwap'ta MAI/USDC havuzuna girmek için kesin adımlar atmanız gerekiyorsa bu makaleyi okumanız sizin için daha iyi olacaktır.

Şu anda QuickSwap'ta MAI/USDC LP (**L**iquidity**P**rovider) havuzuna girerseniz, neler kazanacaksınız;

* ticaret ücretleri
* QUICK

![Ağustos 2021 itibarıyla QuickSwap'taki MAI/USDC havuzunun ayrıntıları](<../.gitbook/assets/Screen Shot 2021-08-11 at 12.37.56 PM.png>)

## Degen Çiftlikleri ve Toplayıcılar

### Adamant

[Adamant](https://adamant.finance/home), Polygon'daki tüm "en iyi APR" çiftlikleri listeleyen ve doğrudan web sitelerinden girmenize izin veren bir toplayıcıdır. Varlıklarınızı (LP tokenları) Adamant'taki belirli bir havuza yatırarak, algoritmalar havuz tarafından verilen ödülleri toplar ve ödülün bir kısmını otomatik olarak LP pozisyonunuza ekler. Ödülün geri kalanı genellikle WMATIC'e dönüştürülür ve daha sonra ADDY'nin (Adamant'ın kendi tokenı) sahiplerine yeniden dağıtılır. Son olarak, WMATIC temettülerinin bir kısmını kazanarak 90 gün boyunca hasat edip yelek yapabileceğiniz ADDY ödülü alırsınız.

Genel olarak, çiftlik tokenını gerçekten umursamıyorsanız ve ödüllerinizi günde birkaç kez manuel olarak birleştirmek istemiyorsanız, Adamant gitmek için iyi bir yerdir. Ayrıca, havuz tarafından verilen ödüle ek olarak bazı ADDY ödülleri aldığınız için daha fazla gelir sağlar.

Adamant şu anda MAI/USDC LP çiftini kabul eden birkaç havuzu desteklemektedir. Bu havuzlarda neler kazanırız;

* QuickSwap: QUICK ödül, daha fazla MAI/USDC LP ve WMATIC ödülüyle değiştirildi
* DinoSwap: Dino ödülü, daha fazla MAI/USDC LP ve WMATIC ödülüyle değiştirildi
* Mai Finance: Qi ödülü, daha fazla MAI/USDC LP ve WMATIC ödülüyle değiştirildi

![Adamant'ta QuickSwap MAI/USDC havuzu](<../.gitbook/assets/Screen Shot 2021-08-11 at 12.51.12 PM.png>)

{% hint style="info" %}
QuickSwap web sitesindeki QuickSwap havuzunun ekran görüntüleri (yukarıdaki paragrafa bakın) ve Adamant aynı gün çekilmiştir, ancak farklı APY'leri göstermektedir (**A**nnual **P**ercentage **Y**ields).
{% endhint %}

Adamant'taki APY'nin doğrudan QuickSwap'tan biraz daha yüksek olduğunu görebilirsiniz. Ödül dağılımı aşağıdaki gibidir

* %12.88 Otomatik birleştirilmiş QUICK (QUICK'lerin daha fazla LP tokena dönüştürüldüğü anlamına gelir)
* %9.16 ADDY ödülü (bileşik değil)
* %3.40 ücret payı temettü (günlük ADDY talep edilerek)

Bu dağıtım QuickSwap tarafından verilen %20.92'den yalnızca %12.88'inin LP pozisiyonunuzu artırmak için kullanıldığı, geri kalanının WMATIC temettülerine dönüştürüldüğü anlamına gelir. ADDY ödülünüzü günlük olarak (veya istediğiniz zaman) talep edebilecek ve bunları stake edebileceksiniz. Bu da karşılığında talep edilebilir WMATIC temettüleri oluşturacaktır. Başka bir deyişle, Adamant otomatik olarak daha iyi APY'lere ve bileşik ödüllere sahip olduğu için daha iyi bir seçenek gibi görünmesine rağmen birçok manuel eylemi de içeriyor.

{% hint style="info" %}
Adamant'ı kullanmanın token fiyatları üzerinde de güçlü bir etkisi vardır. Gerçekten de Adamant, ADDY sahiplerine temettü olarak daha fazla LP çifti ve WMATIC üretmek için çiftlik tokenlerini sürekli olarak sattığından, çiftlik tokenleri üzerindeki satış baskısı çok yüksektir ve fiyatlarının neden sürekli olarak düştüğünü açıklayabilir.
{% endhint %}

### MAI/USDC LP çiftini kabul eden diğer çiftlikler

MAI, Polygon'da giderek daha fazla popülerlik kazanıyor ve QuickSwap, MAI/USDC çiftini desteklediğinden, artık birçok çiftlik de onu destekliyor. Aşağıdaki liste, MAI/USDC kullanarak getiri elde edebileceğiniz birkaç proje sunacaktır.

* DinoSwap
* Augury
* Polypup
* ...

Diğer çiftlikler de MAI/USDC havuzunu kabul edebilir. Yeni çiftlikler ve bunların piyasaya sürülme tarihleri ​​hakkında bilgi sahibi olmak istiyorsanız, Polygon çiftlikleri ve muhtemelen diğer çiftlikler için [RugDoc.io takvimine](https://rugdoc.io/calendar/) bir göz atmanızı şiddetle tavsiye ederim. Her bir çiftliğin yanı sıra potansiyel riskleri hakkında çok akıllı bir genel bakış sunacak olan web siteleri.

## Impermax

### Ek Açıklama

[Impermax](https://polygon.impermax.finance), kullanıcıların daha yüksek getiri için LP tokenlardan yararlanmalarına olanak tanıyan bir platformdur. Amaç çok basit: LP token sağlayarak ve bunları teminat olarak kullanarak, daha fazla LP tokenı oluşturmak ve döngüyü tekrarlamak için 2 temel varlıktan daha fazlasını ödünç alabilir.

![Impermax döngüsü açıklaması](<../.gitbook/assets/Screen Shot 2021-08-11 at 1.15.21 PM.png>)

Bunu yaparken, kullanıcı kalıcı kayba maruz kalır ve kayıp, döngünün tekrarlanma sayısı kadar büyütülür. Çok fazla döngü uygulandığında likidasyon riski de katlanmaktadır. Gerçekten de, APR çarpılırsa, çifti oluşturan iki tokenın fiyat değişimi kaldıraç etkisi ile güçlendirilir ve bu da daha hızlı likidasyona yol açar.

Stabil tokenlarla fiyat değişimi ihmal edilebilir olduğu için likidasyon riski daha düşüktür. Bu aynı zamanda Teminat Borç Oranının (CDR) %100'e çok yakın olabileceği ve çok sayıda döngüye, dolayısıyla yüksek bir APR'ye yol açabileceği anlamına gelir.

Pozisyonunuzu ödünç aldığınızda ve kaldıraç kullandığınızda Impermax'ın ücret talep ettiğini unutmayın. Ücret, nihai pozisyonunuzun %0,1'ine karşılık gelir. Örnek olarak, 100$ değerinde MAI/USDC'ye sahipsem ve 50x kaldıraç kullanırsam, son pozisyonum 5.000$ değerinde olacak ve ödünç aldığım 4.900$'a karşılık gelen 4,90$ ücret ödeyeceğim.

Borç verme/borç alma kombinasyonunu döngüye almanın etkisi, nihai APY'nin çoğaltılmasına izin verir. %110 CDR'ye sahip MAI/USDC çifti için %20'lik bir başlangıç ​​APY'si ile, döngüyü 50 kez çalıştırarak ve formülü kullanarak;

$$
Equivalent APR = Initial APR * \sum_{i=0}^{n}{\frac{100}{CDR}}^i
$$

%228'lik bir son APR'yi kolayca alabiliriz. Nihai APR'yi etkileyecek diğer bazı unsurlar vardır. Ödünç alma APR'si (daha fazla LP tokenu ödünç almak için kredi faizi) ve LP çiftini oluşturan her iki varlığın arz/talebi (doğrudan ödünç alma APR'sini yönlendirir).

Ayrıca, tüm oranlar, döngünün uygulanma sayısı ile büyütüldüğünden APR büyük ölçüde değişecektir ve bazen kısa süreler için negatif olabilir (LP tokenınız negatif APR'yi geri ödemek için kullanılacaktır).

### MAI/USDC çiftinin kaldıraçlı pozisyonu

Günün sonunda temel APR'yi çok daha büyük bir değerde kullanıyorsunuz, bu da çok daha büyük faizler kazandırıyor ve ilk konumunuzun APR'sini artırıyor.

![Başlangıçta 70,52$ MAI/USDC çifti olan bir Impermax panosu örneği](<../.gitbook/assets/Screen Shot 2021-08-11 at 1.38.33 PM.png>)

Ne kadar teminat kullandığımı, başlangıçta ne kadar yatırım yaptığımı, kaldıraç oranının ne olduğunu ve kaldıraç oranından dolayı likidasyon değerlerinin ne olduğunu çok rahat görebiliyorum. Bu pozisyon bana aşağıdaki oranları verecek

![Belirli bir zamanda kazanç ve harcama tahmini](<../.gitbook/assets/Screen Shot 2021-08-11 at 1.41.55 PM.png>)

APR, daha fazla MAI/USDC ile takas edilebilen (Mai Finance'in gücünü %0 faizle borç almak için kullanın, RFTM) veya Impermax'ta IMX'i kabul eden belirli havuzlarda likidite sağlamak için kullanılabilen IMX tokenı olarak verilir.

### Ödünç alanlara MAI sağlama

Aslında uygulamada pozisyonlarına kaldıraç döngüleri uygulamak isteyenlere de likidite sağlayabilirsiniz (daha fazla LP tokenı oluşturmak için temel varlıklara ihtiyaç duyacaklar). Varlıkları ödünç vermek, getiri elde etmenin ve borç alanların tüm riskleri almasına izin vermenin harika bir yoludur. Ayrıca ne kadar çok kullanıcı ödünç alırsa, arz APR'si o kadar yüksek olacaktır.

![Belirli bir zamanda Impermax'ta MAI sağlama ve ödünç alma oranları](<../.gitbook/assets/Screen Shot 2021-08-11 at 1.47.56 PM.png>)

Bu yöntem Mai Finance'deki %0 kredinizi optimize etmenin başka bir harika yoludur. MAI ödünç almak için hiçbir şey ödemenize gerek yok. Aynı zamanda Impermax'a yatırarak çok fazla faiz kazanabilirsiniz.

## Sorumluluk Reddi

Bu içerik tamamen eğitim niteliği taşır. Amaç Polygon'da kripto dünyasında gelişen insanlara layık olduğunu düşündüğüm projelere ışık tutmak. Açıkçası Mai Finance'ten bir çiftlik olarak bahsetmedim çünkü çok yakında özel bir eğitim yazılacak. Son olarak bu kılavuzu KESİNLİKLE olduğu gibi uygulanmaya yönelik DEĞİLDİR. Herhangi bir finansal tavsiye değildir ve yazdıklarımı körü körüne takip etmemelisiniz. Lütfen platformlarına yatırım yapmayı düşünmeden önce bahsettiğim farklı projelerin belgelerini okuyun.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen olan bitenden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
