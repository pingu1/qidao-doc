---
Açıklama: >-
  Bu kılavuzda Moonriver zincirini kullanmak için bilmeniz gereken her şeyi
  açıklayacağız.
---

# Moonriver'ı Nasıl Kullanırım?

## Moonriver nedir?

MoonBeam, Kusama ve Polkadot da dahil olmak üzere birkaç zincirden bahsetmeden Moonriver'ın ne olduğunu açıklamak karmaşık olacak.

Polkadot, Ethereum, Cosmos ve Eos ile doğrudan rekabet eden bir L1 blok zinciridir ve zincirin amacı, kripto para birimleri ve uygulamalardan oluşan eksiksiz bir ekosistem oluşturmaktır. Polkadot'u diğer L1'den farklı kılan ana noktalardan biri, ana zincir (relay zinciri) ve kullanıcı tarafından oluşturulan ağlar (parachains) olarak ayrılmasıdır. Relay Zinciri, çoğu geliştirme ve test parachainler üzerinde yapıldığından, bilgi işlem kaynakları açısından düşük gereksinimlerden yararlanır. Diğer yandan parachainler, relay zinciriyle aynı güvenlikten miras alırlar. Bu aynı zamanda özerk bir şekilde çalışabilen ve kullanıcı verilerini ana zincire ifşa etmeyecek izole ortamlar yaratır.

Kusama, Polkadot'un ana Relay Zincirini taklit eden ve ana zincir için tüm geliştirmelerin ve güncellemelerin ilk önce test edildiği ayrı bir zincir olan Polkadot için bir üretim öncesi ortamıdır. Bununla birlikte, üretim öncesi bir ortam olarak Kusama, gerçek kripto para birimleri ve gerçek işlemlerle çalışır ancak Polkadot'tan daha gevşek kurallarla çalışır. Kusama'da geliştirilen uygulamaların ve yan zincirlerin amacı bir noktada Polkadot'a taşınmaktır. Daha gevşek kurallar nedeniyle, bir projenin protokolü geliştirirken bir şeyleri test etmesi ve bir topluluğu büyütmesi daha kolaydır. Nihai ürün hazır olduğunda, her şey üretim ortamına geçebilir.

Moonriver aslında Kusama'da bir parachaindir. Moonriver'a dağıtılan kod, Moonriver'ın Polkadot'taki üretim versiyonu olan Moonbeam'e dağıtılabilen kodun bir test versiyonudur. Kod Moonriver'da doğrulandıktan sonra Moonbeam'e gönderilebilir. Moonbeam ve Moonriver, EVM uyumlu 2 zincirdir yani Ethereum ağıyla uyumlu diğer zincirlerle aynı akıllı sözleşmeleri kabul ederler.

Diğer EVM uyumlu zincirler gibi Moonriver, işlemleri doğrulamak için kullanılan bir gas tokenı kullanır: MOVR tokenı.

## Moonriver'ı kullanmaya başlarken

Moonriver ağını kullanmadan önce bir cüzdan adresine ihtiyacınız olacak. Moonriver bir EVM ağı olduğu için Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM zincirlerinde olduğu gibi aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz ancak ekstra yönlendirmeleri takip etmeniz gerekebilir. Soğuk cüzdanınızı ağa bağlayabilmeniz için gerekli adımlar. [Resmi Moonbeam Vakfı belgelerinden yararlanabilirsiniz](https://moonbeam.foundation/tutorials/how-to-create-moonriver-ethereum-address/)

Bu eğitim için, vakfın sitesindeki diğer tüm kılavuzlarda olduğu gibi Metamask'a bağlı kalacağız. Metamask yüklü değilse, [Polygon'u Nasıl Kullanırım?](../../polygon-tutorials/how-to-get-started-on-polygon.md) ile ilgili talimatları bulabilirsiniz.

### Moonriver'ı Metamask'a Ekleme

Teorik olarak, Moonriver MetaMask ile önceden yüklenmiş olarak gelir, yani Metamask'ın çalışması için zincir bilgilerini eklemeniz gerekmez. Ancak cüzdanınıza kaydedilen değerleri iki kez kontrol ederek kurulumunuzun doğru olduğunu doğrulamak iyi bir fikir olabilir. Metamask açılır penceresini açın, cüzdanınızın simgesine tıklayın, 'Ayarlar'a gidin, ardından 'Ağlar'ı seçin ve 'Moonriver'ı bulun. Çekmeniz gereken veriler aşağıdaki gibidir:

* **Ağ Adı:** Moonriver
* **Yeni RPC URL'si:** https://rpc.moonriver.moonbeam.network
* **Zincir Kimliği:** 1285
* **Para Birimi Sembolü:** MOVR
* **Blok Gezgini URL'si:** https://blockscout.moonriver.moonbeam.network/

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Moonriver ağına geçirecektir:

![İşte bu! Artık Moonriver'dasınız!](../../.gitbook/assets/Moonriver-setup-MM.png)

## Moonriver'a Köprü Kurmak

### Faucet

Moonriver'daki en büyük DEX'lerden biri olan SolarBeam, gas'sız kalmanız durumunda [gassız işlem takası](https://app.solarbeam.io/bridge/gas-swap) sunar. Öneri Moonriver'da bir miktar paranız olduğunu varsayar ancak cüzdanınızda 0 MOVR olduğu için hiçbir şey yapamazsınız.

![Gas takas etmenizi sağlayacak gassız işlem](../../.gitbook/assets/Moonriver-faucet.png)

Bu gassız işlem için yalnızca belirli varlıkların kabul edildiğini ve MAI'nin desteklenen paraların bir parçası olmadığını unutmayın.

### Köprüler

* [Relay Chain](https://app.relaychain.com/transfer#/), MAI'nizi Polygon'dan Moonriver'a aktarmak istiyorsanız, Mai Finance'in resmi ortağıdır. Polygon'a bağlandığınızda, sadece hedef zinciri (Moonriver) ve göndermek istediğiniz varlığı (MAI veya miMATIC) doğru miktarda seçebilir ve 'Transfer' düğmesine tıklayabilirsiniz. Transfer ücretlerine dikkat edin.

![Relay chain kullanarak MAI'den Moonriver'a Köprü Oluşturma](../../.gitbook/assets/Moonriver-relaychain.png)

* Diğer ağlardan diğer varlıklar arasında köprü kurmanız gerekiyorsa, Relay Chain'i kullanabilirsiniz (yukarıya bakın), Eth Mainnet'ten Moonriver'a köprü yapmak istiyorsanız [AnySwap](https://anyswap.exchange/#/bridge) çalışacaktır. , ve elbette [Solarbeam](https://app.solarbeam.io/bridge) adresindeki köprü özelliğini de kullanabilirsiniz.
* [Elknet](https://app.elk.finance/#/elknet) için ELK tokenı 2 ağ arasında aktardığınızda hem köprü hem de musluk görevi görecektir. ELK'nizi köprüleyebileceksiniz ve alıcı tarafta, bizim durumumuzda ELK'nizin küçük bir bölümünü gas tokenı MOVR olarak doğrudan kullanabilirsiniz.

### Hub

MAI'leri Polygon'dan Moonriver'a Relay Chain aracılığıyla köprülerseniz, Moonriver'daki uygulama tarafından basılan yerel MAI yerine MAI'nin RelayChain sürümünü alacaksınız. 2 token (RelayChain'den ve Mai Finance'den olan) aynı değere ve aynı ada sahiptir, ancak farklı sözleşme adreslerine sahiptir ve Moonriver'da çiftlik verimi için kabul edilecek tek şey Mai Finance'den olandır.

MAI'nizi 1:1 oranında [Mai Finance'teki hub](https://app.mai.finance/hub) kullanarak Relay Chainden değiştirebilir, ardından gerçek MAI'nizi diğer platformlarda kullanabilirsiniz .

![MAI'yi(RelayChain) gerçek MAI'ye değiştirmek için hub'ı kullanma](../../.gitbook/assets/Moonriver-hub.png)

{% hint style="info" %}
Not olarak, MAI'nizi Moonriver'dan Polygon'a veya diğer zincirlere köprülemek istiyorsanız, önce onları RelayChain sürümlerine dönüştürmeniz gerekecektir.
{% endhint %}

## Moonriver'da DeFi

Moonriver çok fazla ilgi görüyor ve Polkadot'a tamamen geçme potansiyeli olan bu yeni zincire giderek daha fazla uygulama taşınıyor. Bu nedenle, aşağıdaki platformda verim elde edebileceksiniz (liste tam değil):

* [Solarbeam](https://app.solarbeam.io): Bu, Moonriver'daki ana DEX ve AMM'dir. Varlıklarınızı takas edebilecek, çiftliklerde LP (**L**iquidity**P**roviding) çiftleri sağlayarak likidite madenciliğine katılabilecek veya platformun yerel tokenini stake edebileceksiniz. Solarbeam ayrıca Mai Finance'in Moonriver'daki ilk ortaklarından biridir ve MAI-MOVR çiftini kullanabilirsiniz. Ayrıca herhangi bir ödül almayan ancak bazı işlem ücretleri alabilen bir MAI-USDC havuzu da bulacaksınız.

![Aralık 2021 itibarıyla solarbeam'de MAI içeren LP havuzları](../../.gitbook/assets/Moonriver-solarbeam.png)

Solarbeam'de farm yaptığınızda, belirli bir hak kazanma süresi boyunca bir Kasada stake yapabileceğiniz ve ek SOLAR tokenları kazanabileceğiniz veya platformda yer alan egzotik diğer tokenları kazanmak için stake edebileceğiniz SOLAR ile ödüllendirileceksiniz.

* [Huckleberry Finance](https://www.huckleberry.finance): Bu, Moonriver'da verim alabileceğiniz ve kazançlarınızı birleştirmek için Beefy'yi kullanabileceğiniz başka bir DEX/AMM.
* [Beefy Finance](https://app.beefy.finance/#/moonriver): Ünlü otomatik bileşen de Moonriver'da ve hem Solarbeam hem de Huckleberry'den elde ettiğiniz kazancı birleştirmenize yardımcı olacak. Beefy, MAI-MOVR çiftini yazılı olarak önermez, ancak yakında Beefy'yi SOLAR toplamak ve birleştiriciden daha fazla MAI-MOVR almak için kullanabilirsiniz.
* [Sushiswap](https://app.sushi.com): SushiSwap'ı sunmaya gerek yok! Diğer zincirlerde yaptığınız gibi, belirli LP tokenları için varlıklarınızı ve çiftlik getirilerinizi takas edebileceksiniz. Ödüller SUSHI ve MOVR'de verilir.
* [Rome DAO](https://romedao.finance): Bu, Moonriver'daki ilk OHM çatalı. Varlıklarınızı, çok yüksek APY kazanmak için kullanabileceğiniz indirimli ROME almak için bağlayın. Yazım sırasında, 5 Günlük ROI yaklaşık %10,6'dır. RomeDAO şu anda hazinesinde FRAX ve MIM'i kabul ediyor, ancak yakında MAI'yi de kabul edecek.

## Moonriver'da Mai Finance

MooSolarETH-USDC tokenlerinizi bir kasaya koyabileceğiniz ve karşılığında MAI ödünç alabileceğiniz, ödünç verme platformu Moonriver'da zaten mevcuttur. Bunu yapmak için:

* Solarbeam'de bir ETH-USDC çifti oluşturun
* ETH-USDC çiftini Beefy'ye yatırın ve bir mooSolarETH-USDC LP token alın
* MooToken'ınızı [uygun kasaya](https://app.mai.finance/vaults/create) Mai Finance'e yatırın

![Mai Finance Aralık 2021 itibariyle Moonriver'da kasaya giriyor](../../.gitbook/assets/Moonriver-vaults.png)

Tek ETH kasası da bir seçenektir.

Teminatınız Beefy Finance'den %44.08 APY kazanırken (yazım tarihi itibariyle), MAI ödünç alabilir ve MAI-MOVR havuzundaki ödülleri toplayabilir ve Solarbeam'de % 128 APR veya RomeDAO'da yakında %158.058 APY elde edebilirsiniz.

## Sorumluluk Reddi

Bu kılavuz finansal tavsiye DEĞİLDİR ve sadece bir eğitim aracı olarak görülmelidir. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
