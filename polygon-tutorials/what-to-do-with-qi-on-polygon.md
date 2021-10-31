---
Açıklama: >-
  Bu kılavuz, Mai Finance'in tokenı olan Qi'yi Polygon'da nasıl kullanabileceğinizi ayrıntılı olarak açıklayacaktır. Ayrıca Qi'nin iyi bir yatırım fırsatı olup olmadığını ve fiyatını neyin yönlendirdiğini de analiz edeceğiz.
---

# Polygon üzerinde Qi ile Neler Yapabiliriz?

## Giriş

Qi (\[tʃ Í] veya _chee_), Mai Finance'in tokenıdır. Bazıları onu oy vermek ve QIP (**Q**iDAO **I**geliştirme **P**roposallar) için kullanır, bazıları daha fazlasını elde etmek için riske atar ve bazıları basitçe onunla farmlar. [Pasif gelire ayrılmış kılavuzda](../mai-university/earning-passive-income-with-qidao.md) Mai Finance ile Qi'yi nasıl kullanabileceğiniz hakkında çok iyi bilgiler bulabilirsiniz.

Bu kılavuz, Qi kullanarak öncelikle çiftçilik ve hasat verimine (*yield farming*) odaklanacaktır. Nasıl çok sayıda Qi üretebileceğinizi ve bunları Polygon'daki farklı platformlarda nasıl kullanabileceğinizi göreceğiz.

Mütevazı çiftçiler bazen size alçakgönüllü kalmanız, hasat ettiğinizi satmanız ve kar etmeniz gerektiğini söyleyecektir. Ama kişisel olarak şunu söyleyeceğim:

> Bir adama balık verirsen onu bir gün beslersin. Bir adama balık tutmayı öğretirsen onu ömür boyu beslersin.

Bu yüzden oltalarınızı alın ve kılavuzu takip edin.

## Polygon üzerinde Qi ile ne yapmalısınız?

### Staking

Bu kısma çok fazla zaman ayırmayacağım. Zaten konuyla ilgili tam bir rehber var. Mai Finance'in gelir topladığını ve çok büyük bir kısmı Qi stakerlarına yeniden dağıttığını unutmayın. Qi'nizi Mai finansında stake etmek, token için en iyi kullanımlardan biridir ve Eylül 2021 itibariyle, dolaşımdaki tüm Qi'nin %23'ü ortalama 2 yıl boyunca kilitlenmiştir.

### LP token çiftçiliği

Verim elde etmek ve farming tokenlarını asla satmayarak, Qi çiftçilik stratejinize nasıl dahil edebileceğinizi gösteren birkaç sayfa daha var. Örnek ayrıntılar için [DApps like Lego bricks](stack-dapps-like-lego-bricks.md) veya [Farming or Staking?](tarım-or-stake-or-both.md) kılavuzlarına bakın.

Hızlı bir hatırlatma olarak, Qi, [QuickSwap](https://quickswap.exchange/#/quick) üzerinde LP (**L**iquidity **P**rovider) çiftleri oluşturmak için farklı tokenlarla eşleştirilir.

* Mai Finance'de Qi-WMATIC ve Qi tokenları ile ödüllendirin
* QuickSwap'ta Qi-WETH ve QUICK tokenları ödüllendirin
* QuickSwap'ta Qi-QUICK ve QUICK tokenları ödüllendirilin

![Qi-WETH çifti için QuickSwap'ta LP havuzu](<../.gitbook/assets/image (19) (2).png>)

### Tek yönlü Qi çiftçiliği

Qi, yalnızca [Impermax](https://polygon.impermax.finance) üzerinde de kullanılabilir. Impermax, QuickSwap'tan kazancınızı artırmak için belirli bir LP çiftinden birkaç kez yararlanabileceğiniz bir platformdur.

Çalışma şekli, farm yapmak istediğiniz çifti oluşturan 2 tokenı ödünç almanız, bunları daha fazla LP tokenında birleştirmeniz ve çok daha yüksek bir pozisyonda farm yapmanızdır. Çoğu durumda, borçlanma oranları büyük ölçüde farming APR'si ile telafi edilir ve size bazı net pozitif ödüller verir.

![Impermax'ta kaldıraçlı Qi-WETH pozisyonu](<../.gitbook/assets/image (10).png>)

Burada, QuickSwap'ta %239.68'lik bir APY'ye dayalı olarak, 5 kez kaldıraç kullandıktan sonra Impermax'ta nihai ödül olan APR'nin %393.88 olduğunu görebiliriz.

{% hint style="info" %}
Ayrıca Impermax'ın tahmini APR'leri (**A**nnual **P**ercentage **R**eward) verirken QuickSwap'in tahmini APY'leri (**A**annual **P**ercentage **Y**ields) verdiğini unutmayın. ields), yani QuickSwap, ödüllerinizi günlük olarak birleştirdiğinizi varsayar. QuickSwap'taki %239.68 APY, %122.49 APR'ye karşılık gelir.
{% endhint %}

Impermax'ta, pozisyonunuzu güçlendirmek için Qi ve WETH'i ödünç almak için, onları bir yerden almanız gerekir. Bu durum yalnızca bazı diğer kullanıcılar (veya sizin) her iki tokenı da ayrı olarak sağladığı için mümkündür. Ne kadar çok token ödünç alınırsa, borçlanma oranı o kadar yüksek olur ve nihai APR o kadar düşük olur, bazen negatif olur.

![Impermax'ta Qi-WETH için Qi ve WETH istatistikleri](<../.gitbook/assets/image (11).png>)

Örneğimiz için Qi'ye odaklanacağız. Toplam Qi arzının 427,21$ ve kaldıraçlı pozisyonda kullanılan toplam miktarın 321,44$ olduğunu ve %75,24 kullanım oranı sağladığını görebilirsiniz. Impermax, arz APR'sini (Qi'ye borç veren kişilerin alacağı APR) ve ödünç alma APR'sini (krediyi ödemek için kesilecek çiftlik ödülünün yüzdesi) otomatik olarak hesaplayan bazı dahili mekanizmalara sahiptir.

Bu durumda Qi'yi yalnızca Impermax'ta sağlayabileceğiniz ve örneğimizde içeriği yazım anında %43,73 APR alabileceğiniz anlamına gelir. Arz ve talep değiştikçe, arz APR'si de artacak/azalacaktır. Impermax'ta tek token tedarik ettiğinizde, sağladığınız token ile ödüllendirileceksiniz. Böylece stratejiniz zamanla daha fazla Qi biriktirmenizi sağlayacaktır.

Impermax'tayken, IMX ödülleri almak için kaldıraç seçeneğini de kullanabilirsiniz. Çiftçilik stratejinize Impermax'ı nasıl dahil edebileceğiniz hakkında daha fazla bilgi almak için lütfen [bu kılavuzu](stack-dapps-like-lego-bricks.md) okuyun.

### Balancer

Balancer, özellikle Qi ve/veya MAI olmak üzere, herhangi bir strateji için gerçekten güzel bir araçtır. Balancer, LP çifti madenciliğine eşdeğer bir teklif sunar ancak 1:1 oranında 2'den fazla token sağlanır. Havuz, farklı ağırlıkta 3, 4 veya 5 tokena (bazen daha da fazla) sahip olabilir ve havuzdan sorumlu algoritma, her tokenın oranına her zaman saygı gösterilmesini sağlar. Bazılarını satar ve diğerlerini dengede tutmak için satın alır.

Burada kullanmak istediğimiz havuz Qi, WMATIC, BAL, USDC ve MAI içeren bir havuzdur. Bu havuz sizi hem Qi hem de BAL tokenları ile ödüllendirecek ve her ikisini de havuza dahil edebileceğinizi şimdiden görebilirsiniz. Balancer'daki havuzların bir başka şaşırtıcı avantajı da havuzu oluşturan tüm tokenları uygun oranda sağlamanız gerekmemesi olduğundan, algoritma bunu sizin için yapacaktır. Havuza yalnızca Qi yatırabileceğiniz ve her şeyi yeniden dengelemek için gerisini algoritmaya bırakabileceğiniz anlamına gelir.

![Eylül 2021 itibariyle havuzun detayları](<../.gitbook/assets/image (12).png>)

Ek bir not olarak, BAL tokenları Mai Finance'de teminat olarak kullanılabilir (veya yakında olacak), bu da BAL tokenlarınızı Mai Finance'teki BAL kasasında saklama ve zamana karşı MAI ödünç alma seçeneğiniz olacağı anlamına gelir. Buna ek olarak, MAI'yi BAL tokenlarınıza karşı ödünç almak, sizi Balancer'daki havuzu besleyecek Qi ödülleri için uygun hale getirecektir.

![Mai Finance ve Balancer kullanarak döngü yaratmak](<../.gitbook/assets/image (13).png>)

BAL kasalarının APR'si, kasanın döngüde olmasının ne kadar ilginç olduğunu veya Qi'nizi Balancer havuzunda birleştirmenin daha iyi olup olmayacağını büyük ölçüde belirleyecektir.

## Qi'nin Fiyatı Üzerine

Çok fazla Qi'ye sahip olmak iyi bir şeydir, ancak token zamanla değer kaybederse onu tutmak gerçekten iyi bir strateji midir? Bu bölümde, Qi'nizin fiyatını doğrudan etkileyen farklı faktörleri anlamaya çalışacağız. Böylece Qi'nize yatırım yapmaya başladığınızda, fiyatının nasıl değişebileceği ve bunun üzerinde ne gibi bir etki yaratacağınız hakkında daha iyi bir fikir edineceksiniz. 

### Qi Emisyonu

Qi'nin fiyatını etkileyecek ana faktörlerden biri, oluşturuldukları orandır. Gerçekten de fiyat her zaman talep ve arz tarafından yönlendirilir. Arz çok ve talep çok düşükse, fiyat doğal olarak çökecektir. Bu nedenle, Qi'nin nasıl üretildiğini anlamak, zaman içindeki değerini tahmin etmek için çok önemlidir.

Şu anda 2 Qi emisyon kaynağı var: çiftçilik ödülleri ve kasa ödülleri.

![Eylül 2021'de Mai Finance'te LP çiftlikleri](<../.gitbook/assets/image (16).png>)

MAI finansmanı üzerinden çiftçilik yapıyorsanız, MAI/USDC çifti ile Qi/WMATIC çifti (Eylül 2021 itibariyle) arasında seçim yapabilirsiniz.

* MAI/USDC çifti 0,5 Qi/blok ile ödüllendirilir
* Qi/WMATIC çifti 1 Qi / blok ile ödüllendirilir

Polygon'da, beklenen blok süresi 2 saniyedir ve bir günde 86.400 saniye olduğundan MAI/USDC havuzunun her gün 21.600 Qi ile ve Qi/WMATIC'in 43.200 Qi ile ödüllendirildiği anlamına gelir.

Yalnızca Mai Finance havuzları günlük 64.800 yeni Qi'den sorumludur.

Kasalara gelince, her kasa 0,05 Qi / blok emisyon veya günlük 2,160 Qi emisyon alır ve şu anda kasa ödülleri olarak tahsis edilen toplam 21,600 Qi için 10 Kasa vardır.

Bu durum her gün 86.400 yeni Qi'nin basıldığı ve kullanıcılara dağıtıldığı anlamına gelir.

### Getiri Optimizasyon Araçları

Getiri optimizasyon araçları, ödülleri önceden tanımlanmış bazı stratejilerle otomatik olarak birleştirecek ve stratejinizi seçmeniz için ek ödüller tahsis edecek platformlardır. Ancak, hasat edilen ödülün büyük bir kısmı doğrudan satılmakta ve bu platformlarda başka bir şekilde yeniden kullanılmaktadır.

Örnek olarak, Adamant size Qi/WMATIC LP çiftini aşağıdaki ödül dağıtımıyla kendi platformlarında toplamanızı önerir.

![Adamant'taki Qi-WMATIC havuzu ](<../.gitbook/assets/image (15).png>)

![Adamant tarafından verilen %179.23 APR'nin ayrıntıları](<../.gitbook/assets/image (14).png>)

Genel APR'nin Mai Finance'dekinden daha yüksek olması durumunda, bunun yalnızca Adamant'ın çiftçilere ek ADDY ödülleri tahsis etmesinden kaynaklandığını fark edeceksiniz. Çiftçiye gerçekte yeniden dağıtılan Qi miktarı, Mai Finance'de alabileceğiniz %134,42'ye kıyasla %98,45'tir.

Bu %98,45 Qi ödülünün yarısı doğrudan WMATIC satın almak ve daha sonra çiftçiye verilecek ek LP tokenları oluşturmak için satılmaktadır.

100$ değerinde LP tokenı ile APR-token fiyatlarının tam bir yıl boyunca aynı kaldığını ve bileşik olmadığını varsayarsak, bir yıllık çiftçiliğin ardından şunları elde edersiniz;

* Mai Finance'de 134,42 $ değerinde yeni Qi
* 98,45 $ değerinde yeni Qi/WMATIC tokenı veya Adamant'ta 49,23 $ değerinde yeni Qi

Bu süreçte 85.20 $ değerinde Qi'nin doğrudan piyasada satıldığı anlamına gelir. Adamant'ta havuza tahsis edilen toplam emisyonun %60'ından fazlasıdır.

Adamant bu hizmet türünü öneren tek platform değildir. Diğer bazı örnekler Beefy Finance ve Kogecoin'dir. Mai Finance'deki Qi/WMATIC çiftliğinde bulunan 4,9 milyon dolarlık TVL'den 2,3 milyon dolar doğrudan Adamant'tan, 41 bin dolar Beefy'den ve 12 bin dolar Kogecoin'den geliyor ve bu 3 platform için Mai Finance'e kilitlenen değerin %50'sinden fazlasını temsil ediyor. Ham bir tahmin, toplam günlük Qi emisyonunun %30'undan fazlasının bu platformlar tarafından boşaltılması, token üzerinde çok olumsuz bir satış baskısı oluşturması ve fiyatını düşürmesi, bu da kısmen Qi'nin neden yüksek bir fiyat tutmakta zorluk çektiğini açıklıyor.

### LP Çiftleri Üzerine

LP çiftleri sağlayarak verimleri topladığınızda, LP tokenı aslında bir tokenı başka bir tokenla değiştiren kullanıcılara likidite sağlamak için kullanılır. Qi/WETH örneğimizde, birisi WETH satın aldığında, tokenın bir kısmı LP havuzundan alınabilir ve ihtiyacı olan kullanıcıya satılabilir.

Bu noktada, havuzdan bir miktar WETH alındığından, bir denge uyuşmazlığı vardır. Aynı miktarda Qi için daha az WETH. Havuz oranını 1:1 olarak tutmaktan sorumlu algoritma daha sonra biraz daha WETH geri almak ve mükemmel 1:1 oranını yeniden oluşturmak için bu havuzdan bir miktar Qi satacaktır. Birisi Qi satın aldığında, yani bazı Qi'leri geri almak için WETH satıldığında da bunun tersi olur.

Aynı fenomen, çifti oluşturan 2 tokendan biri değer kazandığında veya kaybettiğinde ortaya çıkar. Örnek olarak, Qi fiyatının 1$ ve ETH fiyatının 1.000$ olduğunu ve 100$ değerinde Qi ve 100$ değerinde WETH içeren bir havuzumuz olduğunu varsayacağız. Bu durum havuzların 100 Qi ve 0.1 WETH içerdiği anlamına gelir.

Şimdi ETH fiyatı 2.000 dolara çıkarsa, havuz aynı miktarda token tutarsa, 100 dolar değerinde Qi, ancak 200 dolar değerinde WETH olur ve bakiyeyi kaybederdik. Bu nedenle, havuzdan sorumlu algoritma, bir miktar Qi satın almak için biraz ETH satacaktır. Kolay örneğimizde, 50$ değerinde Qi satın almak için 50$ değerinde ETH satılacak ve son durum şu şekilde olacaktır.

* 150$ değerinde 150 Qi
* 150$ değerinde 0,075 ETH

Bu aynı zamanda, 2 tokendan birinin fiyatı yükseldiğinde, havuzun diğeri için bir miktar talep yaratması ve aynı zamanda fiyatını yükseltmesi anlamına gelir. Bunun tersi de doğrudur. Mesela bir token değer kaybederse, diğeri 1:1 oranını korumak için satılarak fiyatı düşürür. Bu, WEHT ve WMATIC'in (Qi'nin eşleştirildiği 2 ana token) fiyat dalgalanmasıyla karşılaştırıldığında Qi'nin fiyat dalgalanmasını da kısmen açıklar.

![Qi fiyatı (soldaki) ve WMATIC fiyatı (sağdaki)](<../.gitbook/assets/image (17).png>)

### Kullanım Eksikliği

Son olarak, Qi'nin kullanılmaması veya bilinen kullanım durumlarının olmaması, tokenin fiyatının neden düştüğünü açıklayabilir. Kasa ödüllerinden Qi toplayan ve/veya Mai Finance'de çiftçilik yapan insanlar, uzun vadeli bir vizyon olmadan, aslında oldukça makul bir strateji olan bir kar elde etmek için hala "bir miktar" değeri varken onu satacaklar. Bu kılavuz aslında Qi tokenlarınızı satmadan kullanmanın farklı yollarını tanıtmaya çalışır. Fiyat artmazsa veya diğer tokenlarda fayda sağlayamazsanız (yani karlı değilse), onları biriktirmenin çok az avantajı vardır.

### Fiyatın yükselmesine nasıl yardımcı olabiliriz?

Qi'nin fiyatının artmasını istiyorsak (ki kim istemez ki), birkaç seçenek var.

* Emisyonu azaltın: Günlük basılan 86.400 yeni Qi ile arz çok yüksek. Bu emisyonu azaltırsak, arz daha düşük olabilir ve daha az arz ile fiyat teorik olarak yükselmelidir. Ancak, QuickSwap ile mevcut bir ortaklığın parçası oldukları için çiftlikler için mevcut emisyonun aynı kalması gerekiyor. Kasa teşvikleri başlatıldı ve kredi verme platformunu tanıtmanın harika bir yolu, insanları kredi almaya itiyor, bu nedenle bu emisyonları azaltmak muhtemelen kötü fikir.
* Sorumlu bir şekilde çiftlik yapın: Adamant'ın asıl suçlu veya kötü bir ürün olduğunu söylemiyorum. Gerçekten de bu platformu stratejilerimin çoğuna dahil ediyorum ve günlük olarak kullanıyorum. Ancak, tokenın çöpe atılacağına dair daha az endişe duyduğum havuzlarda çiftçilik yapmaya çalışıyorum. Adamant'ta Mai Finance çiftliğini kullanan bir havuzda hasılat elde etmek istiyorsanız, Qi amortismanına katıldığınızı unutmayın. Eğer bu durumla barışıksan, bu tamamen iyi fikir.
* İşlerin nasıl yürüdüğünü anlayın: TÜM kripto para birimlerinin fiyatları oldukça değişkendir ve çoğu zaman BTC ve ETH'nin fiyatı diğer tüm tokenların fiyatını belirler. Bu sihirli bir şekilde yapılmaz. Ayrıca, bazı insanlar para kazandığında, bazılarının biraz kaybetmesinden kaynaklandığını lütfen anlayın. Bedava para yok ve sihirli internet parası aslında o kadar da sihirli değil.
* Qi kullanmanın yeni yollarını bulun. Bu kılavuz her zaman portföyünüzün hacmini artırmanıza ve mümkün olduğunca az tken satmanıza yardımcı olacak fikirler sağlayacaktır. Kapalı döngüler en iyisidir çünkü bir ürünün çıktısı bir sonrakinin girdisini besler ve zamanla büyüyecek güzel bir balon oluşturur.

Şunu da unutmayın

$$
Değer = Miktar * Fiyat
$$

Fiyat düştüğünde ancak miktarınız arttığında, değeriniz artabilir veya en azından o kadar hızlı düşmeyecektir.

## Sorumluluk Reddi

Bu rehber aslında Discord kanalında Qi fiyatıyla ilgili birçok tartışmanın bir sonucudur. Fiyat düşüşünden şikayet eden bazı kişilerin, Qi fiyatının neden sürekli bir düşüş eğiliminde olduğunun nedenlerini tam olarak anlamadığını fark ettim. Qi, Mai Finance ürünü ve genel olarak tüm DeFi ekosistemi için çok olumsuz olan hayal kırıklığı ve yanılsamaya yol açar. Fiyatın artacağının kesinlikle garantisi yoktur. Q'larınızı korumak ve yatırım yapmak istiyorsanız, lütfen kendi araştırmanızı yapın ve riski size ait olmak üzere yapın. Stratejinizi doğru bir şekilde planlayın ve ona bağlı kalın.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen olan bitenden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
