---
description: >-
  SpiritSwap kısa bir süre önce MAI-WFTM için bir getiri çiftliği başlattı. Bu kılavuz, SpiritSwap'ta neler yapabileceğinizi göstermek için oluşturuldu.
---

# SpiritSwap ile çiftçilik döngüsü

Çiftçilikte verim söz konusu olduğunda, LP çifti (Likidite Sağlayan çift) çok önemlidir. İlk yatırımınızı kaybetmemek için mümkün olduğunca az kalıcı kayıp istersiniz. Bu ilk çift verim üretecektir. Başlangıç ​​için herhangi bir ekstra risk olmadan eşleştirdiğiniz tokenı yeniden yatırım yaparak kazançlarınızı artırabilirsiniz. Kılavuzlarımızın, yalnızca stablecoin ve Bitcoin, Ethereum veya stratejiyi uyguladığımız zincirdeki yerel gas tokenı gibi bir Blue Chip tokenından oluşan çiftlere dayalı stratejiler önermesinin nedenlerinden biri budur.

Bugün, SpiritSwap tarafından lansmanını ve mevcut yükselişini kutlamak için sunulan MAI-WFTM-LP çiftine dayanan nispeten karmaşık bir döngü keşfedeceğiz.

![](<../../.gitbook/assets/spiritswap-1.png>)

## SpiritSwap'te MAI Çiftçiliği

[SpiritSwap](https://app.spiritswap.finance/#/) Fantom'daki ana DEX'lerden (Merkeziyetsiz Borsa) ve AMM'den (Otomatik Piyasa Yapıcı) biridir. Uniswap platformuna dayanmaktadır, bu nedenle SpiritSwap'in temel özelliklerini, yani varlıkları takas etmeyi, getiri elde etmek için likidite sağlamayı kesinlikle anlayacaksınız. Ödülleri, platformun yerel tokenında, stake edebileceğiniz ve inSPIRIT alabileceğiniz SPIRIT tokenıyla alacaksınız. inSPIRIT tokenı özellikle yararlıdır, ek boost uygulanacak likidite havuzları için oy vermenize ve protokol gelirinden ekstra getiri elde etmenize olanak tanır.

Stratejimiz için MAI-WFTM havuzunu kullanacağız. Aralık 2021'den itibaren bu havuz `Booster Farms` sekmesinde bulunabilir.

![MAI-WFTM pool on SpiritSwap as of December 2021](<../../.gitbook/assets/spiritswap-2.png>)

{% hint style="info" %}
Bu kılavuz oluşturulduğunda, havuz hala çok erken aşamalarındaydı (son 24 saat içinde piyasaya sürüldü), bu da çok yüksek APR'yi (Yıllık Yüzde Oranı) açıklar. Her zaman olduğu gibi, stratejilerimizden herhangi birini uygulamadan önce kendi araştırmalarınızı yapmalı ve yatırım yapmadan önce APR'yi gözden geçirmelisiniz. Karşılaştırma için: Polygon'da USDC-WMATIC yaklaşık %75 ve Moonbeam'de MAI-MOVR %158'dir. USDC-WFTM gibi diğer havuzlar, Fantom'da %50 civarında sabitlendi.

Bu kılavuzun amacı doğrultusunda, en düşük APR'yi %152,98 aralığında tutacağız; bu oran olması gerekenden çok daha fazladır.
{% endhint %}

MAI-WFTM'yi SpiritSwap üzerinde gruplandırırsanız DApp'in (merkeziyetsiz uygulama) yerel tokenı olan SPIRIT ile ödüller alırsınız. Aralık 2021 itibariyle: 1 SPIRIT = 0.130 USDC

## Liquid Driver'da SPIRIT tokenlarını kullanarak çiftçilik yapmak

[Liquid Driver](https://www.liquiddriver.finance/) Fantom'da likidite sağlamaya odaklanan başka bir Uniswap klonudur. Liquid Driver'ın en çok ilgi çeken özelliklerinden biri, SPIRIT tokenlarından linSPIRIT tokenları oluşturabilmeleridir. linSPIRIT, inSPIRIT tokenının likit versiyonudur. linSPIRIT ve inSPIRIT arasındaki oran 1:1'dir, bu inSPIRIT tokenının wrapped versiyonudur ve ayrıca her iki tokenı doğrudan Liquid Driver'da birbiriyle takas edebilirsiniz.

![LiquidSwapper on Liquid Driver](<../../.gitbook/assets/spiritswap-3.png>)

Ancak bu özelliği kullanmayacağız. Liquid Driver'da SPIRIT-linSPIRIT havuzunu oluşturacağız, ancak küçük bir aldatmaca var:

![Farming SPIRIT-linSPIRIT LP token on Liquid Driver](<../../.gitbook/assets/spiritswap-4.png>)

Gördüğünüz gibi, LQDR tokenıyla ödenen %61 APR'yi almak için BeethovenX'te LP tokenını oluşturmanız gerekiyor. Aralık 2021 itibariyle, 1 LQDR = 4.560 USDC. Bu LP tokenını nasıl alabileceğinizi görelim.

## BeethovenX üzerinde SPIRIT-linSPIRIT oluşturma

[BeethovenX](https://app.beets.fi/#/) Fantom'da resmi Balancer havuzu olarak kabul edildi. Balancer'a gelince, bir LP tokenı oluşturmak için her iki tokenın aynı miktarını yatırmanız gerekmez. Bu durum SPIRIT tokenlarınızın %100'ünü doğrudan yatırabileceğiniz ve havuzu dengede tutmak için havuzdan sorumlu algoritmaya izin verebileceğiniz anlamına gelir.

![Water Music By LiquidDriver on BeethovenX](<../../.gitbook/assets/spiritswap-5.png>)

Karşılığında Liquid Driver'a yatırabileceğiniz LP tokenı alacaksınız

{% hint style="info" %}
Gördüğünüz gibi, bu havuz BeethovenX'te teşvikli değil, bundan BEETS kazanmayacaksınız. Teşvikler, LP tokenını platformlarına yatırdığınızda yalnızca Liquid Driver tarafından sağlanır ve alacağınız tek ödül LQDR olarak ödenir.
{% endhint %}

## Liquid Driver'da LQDR Staking

SPIRIT-linSPIRIT LP tokenınızı BeenthovenX'te oluşturduktan ve Liquid Driver'da doğru havuza yatırdıktan sonra LQDR tokenları kazanmaya başlayacaksınız. Ardından, protokol gelirinin bir kısmını kazanmak için LQDR tokenlarını stake edebilirsiniz. İşin güzel yanı, LQDR'nizin stake edileceği süreyi seçebilmenizdir ve bu, APR'nizi doğrudan etkileyecektir (protokol geliri elde etmek için Qi'yi stake etmeniz gibidir). Ortalama kilitleme süresi 2 yıldan biraz daha azdır (maksimum kilitleme süresi) ve ödüller şu şekillerde ödenir:

* LQDR: bu ödülü yeniden kazanabileceksiniz
* WFTM: Bunu daha sonra kullanacağız
* BOO: Bunu daha sonra kullanacağız
* linSPIRIT: Liquid Driver'da SPIRIT-linSPIRIT konumunuzu artırmak için kullanılabilir
* SPELL: ek WFTM için takasta değerlendirebiliriz !!!

![Staking rewards when you stake LQDR as of December 2021](<../../.gitbook/assets/spiritswap-6.png>)

## SpookySwap'te BOO Staking

[SpookySwap](https://spookyswap.finance)  yapbozumuzun neredeyse son parçasıdır. Liquid Driver'da LQDR'yi stake etmek, SpookySwap'in yerel tokenı olan BOO tokenlarını kazanmamızı sağlayacaktır. SpookySwap, Fantom'daki en büyük DEX/AMM'dir, bu nedenle SpiritSwap’te yapabileceğinizin hemen hemen aynısını yapabilirsiniz, yerel tokenlarının BOO tokenı olması dışında bir fark yoktur. Bu özellikle xBOO tokenlarını almak için BOO tokenlarınızı SpookySwap'te stake edebileceğiniz için kullanışlıdır ve BOO'nun bu stake edilmiş versiyonu diğer tokenları toplamak için kullanılabilir (Uniswap çatalları için ortak bir özelliktir). Böylece, xBOO'ya sahip olduğunuzda, ek WFTM kazanmak için bu tokenları SpookySwap'e yatırabileceksiniz.

![Staking xBOO on SpookySwap to farm additional WFTM as of December 2021](<../../.gitbook/assets/spiritswap-7.png>)

## Daha fazla MAI-WTFM LP tokenı alma

Liquid Driver ve SpookySwap, WFTM tokenları üretecek, bu nedenle SpiritSwap'teki ilk konumumuza daha fazla LP tokenı eklemek için MAI'yi gerçekten çok istiyoruz. Bunu birkaç farklı yolla yapabilirsiniz

* WFTM'nizin %50'sini MAI ile takas edin
* MooScreamFTM veya yvWFTM almak için WFTM'nizin %66'sını Beefy veya Yearn Finance'e borç verin, ardından teminat tokenlarını Mai Finance'e yatırın ve onlara karşı MAI borç alın
* WFTM'nizin %66'sını başka bir varlıkla değiştirin ve MAI'yi borç almak için yukarıdakiyle aynı stratejiyi kullanın

{% hint style="info" %}
Son 2 maddeyle ilgili daha fazla ayrıntıya ihtiyacınız varsa, varlıklarınızı [Fantom'da kullanmaya yönelik](<leverage-your-crypto-on-fantom.md>) özel bir makalemiz var..
{% endhint %}

Rehberimiz için kazançlarımızı maksimize etmeye ve mooScreamDAI kullanmaya çalışacağız. Bu, WFTM'mizin %66'sını Spirit Swap'te DAI ile takas edeceğimiz ve ardından mooScreamDAI almak için temel platform olarak SCREAM'i kullanarak DAI'yi doğrudan Beefy'ye yatıracağımız anlamına gelir. Bu token daha sonra Mai Finance'de bir kasaya yatırılacak ve MAI'yi borç alabileceğiz. Likidasyon riskini azaltmak için %200'lük bir CDR (Borç Teminatı Oranı) tutacağız, bu da mevduatımızın değerinin yarısını borç alacağımız anlamına geliyor. Bu, tuttuğumuz WFTM'nin aynı değerine karşılık geldiği için mükemmeldir, böylece ek MAI-WFTM LP tokenları oluşturmak mümkün olacaktır.

![Getting mooScreamDAI on Beefy Finance](<../../.gitbook/assets/spiritswap-8.png>)

Döngünün sonunda daha fazla MAI-WFTM ve Mai Finance'te teminat olarak kullanılan gelir getiren bir token elde ederiz.

## Çiftçilik Stratejisi

Aşağıdaki simülasyon birkaç şey varsayılarak yapılmıştır:

* Oranlar ve fiyatlar tüm simülasyon süresi boyunca aynı kalır, bizim durumumuzda 1 yıl sürecek
  * SpiritSwap'te MAI-WFTM farming’de %153 APR
  * linSPIRIT'te ödül yok
  * Liquid Driver’da SPIRIT-linSPIRIT üzerinde %61 APR
  * LQDR stake için %139 APR
    * LQDR'de %26 APR
    * WFTM'de %6
    * BOO'da %30
    * linSPIRIT'te %74
    * SPEEL’de %3
  * xBOO stake için %36 APR
  * mooScreamDAI için %21 APR
* Tüm ödüller ve programlar da bir yıl boyunca devam eder
* İlk yatırım 1.000$ değerinde MAI-WFTM LP tokenıdır

![](<../../.gitbook/assets/spiritswap-9.png>)

### 1.Gün

İlk gün, MAI-WFTM çiftinizi SpiritSwap'e yatırmanız yeterlidir. Günün sonunda, SPIRIT tokenlarınızı toplayıp ve bunları BeethovenX'te bir SPIRIT-linSPIRIT çiftinde birleştirin, ardından bu LP tokenını Liquid Driver'a yatırın. Günün sonunda

| MAI-WFTM | linPIRIT-SPIRIT | LQDR | xBOO | mooScreamDAI |
|----------|-----------------|------|------|--------------|
| 1,000.00 |            4.19 | 0.00 | 0.00 |         0.00 |

### 2. Gün

2. günde, MAI-WFTM'niz hala Liquid Driver'daki linSPIRIT-SPIRIT havuzuna yatıracağınız SPIRIT tokenları üretiyor ancak aynı zamanda ilk birkaç LQDR tokenınızı toplayabilecek ve bunları çoklu ödüller için stake edebileceksiniz. 2. Günün sonunda,

| MAI-WFTM | linPIRIT-SPIRIT |  LQDR | xBOO | mooScreamDAI |
|----------|-----------------|-------|------|--------------|
| 1,000.00 |            8.38 | 0.007 | 0.00 |         0.00 |

### 3. Gün

3. günde, LQDR'niz dışında aynı şey protokol gelirlerinden ilk birkaç egzotik tokenınızı üretmiş olacaktır. BOO'nuzu stake edeceğinizi, havuza linSPIRIT'inizi ekleyeceğinizi, LQDR'nizin yeniden tahsis edilip geri kalanının WFTM ile takas edileceğini unutmayın. Ortaya çıkan WFTM daha sonra kısmen DAI ile takas edilir ve ardından mooScreamDAI, MAI borç almak için bir Kasaya yatırılır, ek MAI-WFTM oluşturur ve daha sonra SpiritSwap'e yatırılır. 3. Günün sonunda,

| MAI-WFTM | linPIRIT-SPIRIT |  LQDR | xBOO | mooScreamDAI |
|----------|-----------------|-------|------|--------------|
| 1,000.00 |           12.58 | 0.021 | 0.00 |         0.00 |

{% hint style="info" %}
xBOO ve mooScreamDAI pozisyonu görüntülenemeyecek kadar küçüktür, bu nedenle ilk birkaç gün için bu adımları atlayabilirsiniz. Ayrıca, kolaylık olması açısından, kazançlarınız üzerinde etkisi olabilecek herhangi bir işlem ücretini dahil etmiyorum.
{% endhint %}

Bu noktada sistem hazır durumda, artık getirileri toplama zamanı.

## Çiftçilik Sonuçları

### Günlük Rutin

Sistem tamamen hazır olduğunda izlemeniz gereken günlük rutin şu şekildedir:

* SpiritSwap'teki MAI-WFTM havuzundan SPIRIT tokenlarını toplayın
* Liquid Driver stake havuzundan ödülleri toplayın
* SpookySwap stake havuzundan ödülleri toplayın
* SpiritSwap'ten SPIRIT'i ve Liquid Driver'dan linSPIRIT'i BeethovenX'teki havuza yatırın
* SPIRIT-linSPIRIT LP tokenını Liquid Driver'a yatırın
* xBOO almak için BOO'nuzu SpookySwap'a yatırın
* WFTM farmı için xBOO'nuzu riske atın
* SPELL'inizi WFTM ile takas edin
* WFTM'nizin %66'sını DAI ile takas edin
* mooScreamDAI almak için oluşturulan DAI'yi Beefy'de yatırın
* mooScreamDAI tokenlarını Mai Finance'e yatırın
* MAI ödünç alın ve %200'lük bir CDR'ye sahip olun (yatırdığınızın %50'si)
* SpiritSwap'te MAI-WFTM havuzu için likidite sağlayın


### Aydan aya ham sonuçlar

| gün |  MAI-WFTM | linPIRIT-SPIRIT |   LQDR  |  xBOO  | mooScreamDAI | MAI borç |
|-----|-----------|-----------------|---------|--------|--------------|----------|
|  30 | 1,000.004 |         130.010 |   3.281 |  0.026 |        0.005 |    0.002 |
|  60 | 1,000.039 |         256.218 |  13.014 |  0.210 |        0.041 |    0.021 |
|  90 | 1,000.140 |         383.220 |  29.369 |  0.712 |        0.147 |    0.074 |
| 120 | 1,000.349 |         511.436 |  52.538 |  1.698 |        0.364 |    0.182 |
| 150 | 1,000.708 |         641.302 |  82.741 |  3.338 |        0.738 |    0.369 |
| 180 | 1,001.268 |         773.275 | 120.224 |  5.810 |        1.323 |    0.661 |
| 210 | 1,002.081 |         907.835 | 165.263 |  9.295 |        2.175 |    1.088 |
| 240 | 1,003.207 |       1,045.486 | 218.165 | 13.984 |        3.360 |    1.680 |
| 270 | 1,004.710 |       1,186.759 | 279.268 | 20.075 |        4.947 |    2.473 |
| 300 | 1,006.659 |       1,332.316 | 348.947 | 27.773 |        7.014 |    3.507 |
| 330 | 1,009.130 |       1,482.451 | 427.613 | 37.296 |        9.645 |    4.823 |
| 360 | 1,012.205 |       1,638.095 | 515.717 | 48.870 |       12.935 |    6.467 |

### 365. gün

ASistemin tam bir yılını doldurduktan sonra

* SpiritSwap’te 1.012.782$ değerinde MAI-WFTM
* Liquid Driver'da $1,664.608 değerinde linSPIRIT-SPIRIT
* Liquid Driver'a 531.353$ değerinde LQDR 
* SpookySwap'te 51.015$ değerinde xBOO
* Mai Finance’de 13.554$ değerinde mooScreamDAI
* 6.777$ değerinde MAI borcu 

1.000 $'lık bir başlangıç ​​yatırımı ile bu, %227.096'lık bir APY'ye dönüşecektir.

### Stratejide küçük değişiklikler

Daha az risk almak istiyorsanız, ilk yatırımınızın bir kasada 1.000$ değerinde mooScreamDAI olmasıyla başlayabilir, 500$ değerinde MAI borç alabilir ve SpiritSwap'te başlangıç bloğunu almak için %50'sini WFTM ile takas ederek başlayabilirsiniz. Bunu yapmanız FTM fiyatının çok fazla düşmesi durumunda başlangıç yatırımınızın bir kısmını kaybetme riskinizi önemli ölçüde azaltacaktır.

Şu anda en yüksek oran SpiritSwap havuzu tarafından verilmektedir, bu nedenle döngünün olası bir basitleştirilmesi, daha fazla MAI-WFTM için Liquid Driver'da aldığınız tüm LQDR tokenlarını basitçe takas etmek olacaktır.

## Sorumluluk Reddi

Bu kılavuz, Fantom'da uygulayabileceğinizin teorik bir versiyonudur. Eğitimlerimizde döngüleri ortaya çıkarırken tokenları elden çıkarmamaya ve topladığımız her şeyi kullanmanın mümkün olan en iyi yolunu bulmaya çalışıyoruz. Bunu yapmak, fiyatın yükselmesini sağlamak için harika bir yoldur çünkü bir tokenı çiftçilikte kullanıp kazanım elde edince satmak, genellikle çiftçilik yapılan tokenın fiyatının düşmesine neden olur ve verimleri daha az çekici hale getirir. Herkes çiftçilik yaptığı tokenları satmadan tutsaydı, fiyatlar zamanla artacaktı.

Kılavuz birçok varsayıma (fiyat değişmez, ödül oranları değişmez) dayanmaktadır ve işlem ücretlerini hesaba katmaz. Dolayısıyla, bu tür bir kapalı döngü uygulamak istiyorsanız günün sonunda kârlı olduğunuzdan emin olun veya kazançlarınızı haftada sadece bir kez birleştirin. Ve her zaman olduğu gibi DYOR!

{% hint style="info" %}
Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor... Amaç körü körüne takip edilebilecek tarifler önermek değildi. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın..
{% endhint %}
