---
description: >-
  Bu kılavuzda, Optimism'in sunduğu farklı DApp'leri kullanmaya başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# Optimism Nasıl Kullanırım?



## Optimism Nedir?

Optimism veya bazen adlandırıldığı gibi Optimistik Ethereum, kullanıcıların Ethereum ağı üzerinde işlem göndermelerine ve bunları çok daha düşük bir gas maliyetiyle daha hızlı yürütmelerine olanak tanıyan bir toplama ölçeklendirme çözümüdür. Bu nedenle Optimism, Ethereum Layer 2 (kısaca L2) olarak bilinir. Optimism adı, ağın ana Ethereum zinciriyle (Layer 1 veya L1) birlikte çalışmak için kullandığı kanıt türlerini ifade eden optimistik toplama teknolojisinin kullanımından gelir. Optimism toplamalar ve ZK (Zero Knowledge) gibi diğer rollup çözümleri hakkında daha fazla bilgi için [bu linke](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/) göz atın.

Optimism bir toplama teknolojisi olduğu için kendi bloklarını üretmez ve bu nedenle bir blok zinciri değildir. Ek olarak, Optimism ağ API'si büyük ölçüde Ethereum ile aynı JSON-RPC spesifikasyonunu kullanır ve bu nedenle esasen EVM (Ethereum Virtual Machine) eşdeğeridir ve Ethereum ana ağı için oluşturulan uygulamaların kod tabanlarında esasen hiçbir değişiklik olmaksızın Optimism üzerinde çalışmasına izin verir.\
\
Bu nedenle, Optimism'in kendi gas tokenını kullanmadığını, bunun yerine işlemler için ödeme yaparken gas olarak Ether'i kullandığını unutmayın.

## Optimism'e Başlarken

Optimism'i kullanmadan önce bir cüzdan adresine ihtiyacınız olacak. Optimism bir EVM ağı olduğu için Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM zincirlerinde olduğu gibi aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz ancak Soğuk cüzdanınızı ağa bağlayabilmek için ekstra adımları izlemeniz gerekebilir.

Bu eğitim için, tıpkı bu sitedeki diğer tüm kılavuzlar için yaptığımız gibi Metamask'a bağlı kalacağız. Yüklü Metamask'ınız yoksa, [Polygon Başlangıç Rehberine](../polygon/how-to-get-started-on-polygon.md) göz atın.

### Cüzdan Kurulumu

Metamask açılır penceresini açın, cüzdanınızın simgesine tıklayın, Ayarlar'a gidin, ardından Ağlar'ı seçin ve Ağ Ekle'yi bulun. İlgili metin alanlarında aşağıdaki bilgileri kullanacaksınız:


* **Network Name:** Optimism
* **New RPC URL:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Optimism’e geçirecektir:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## Optimism’e Köprüleme

### Musluklar

Optimism'de gas için musluk yoktur, ancak ElkNet gibi bir DApp kullanıyorsanız desteklenen ağlardan herhangi birinden köprülerken Elk tokenlarınızın bir kısmını gas olarak değiştirebilirsiniz.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Köprüler

* MAI veya QI'nizi başka herhangi bir ağdan Optimism'e aktarmak istiyorsanız, [Multi Chain](https://app.multichain.org/#/router) Mai Finance'in resmi ortağıdır. Seçtiğiniz ağdan sadece hedef zinciri (Optimism) ve göndermek istediğiniz varlığı (MAI veya ETH) doğru miktarda seçip Aktar tuşuna tıklayabilirsiniz. Doğrudan aktardığınız varlık üzerinden alınan aktarım ücretlerine dikkat edin.


![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) popüler bir köprüdür ve Optimism ağının resmi köprü ortaklarından biridir.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) iaynı zamanda Optimism ağının resmi ortağı olan bir başka popüler köprüdür. ETH ve USDC, DAI ve USDT gibi çeşitli stablecoinler dahil olmak üzere yalnızca az sayıda desteklenen token vardır, ancak diğer çoğu çözümden daha düşük köprü ücretleri sunar.
* [Hashflow](https://app.hashflow.com/) yeterli likiditeye sahip herhangi bir token için temelde çapraz zincir DEX (merkeziyetsiz borsa) olarak çalışan daha yeni bir köprüleme teknolojisidir. Ek olarak, Hashflow kullanıcıları şu anda token likiditesini değiştirmek veya sağlamak için HFT (Hashflow tokenları) kazanabilirler. Zincirler şu anda Ethereum, Avalanche, Arbitrum, Optimism, Polygon ve BNB ile sınırlıdır.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) wELK tokenını 2 ağ arasında aktardığınızda hem köprü hem de musluk görevi görecektir. ELK'inizi köprüleyebilir ve ELK'inizin küçük bir kısmına, yukarıdaki bölümde açıklandığı gibi, bizim durumumuzda ETH olan bir gas tokenı olarak doğrudan alıcı tarafta sahip olabilirsiniz.

## Optimism’de DeFi

Optimism’e başlamak için, MAI ve QI'nizi kullanırken yararlı bulabileceğiniz bazı DApp'ler şunlardır:

* [Curve](https://optimism.curve.fi/factory/4/deposit): Curve, stablecoin takasları gerçekleştirmede son derece verimli olduğundan, Optimism üzerindeki MAI likiditesinin çoğu şu anda burada bulunuyor.\
  \
  MAI'yi Curve LP'ye yatırarak, QI tokenlarında getiri elde etmek için Mai Finance'in Farm sayfasındaki Curve çiftliğine yatırılabilen LP tokenları alacaksınız.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) kısa süre önce Optimism'i başlattı ve QI/WETH likidite havuzunu bulacağınız yer burasıdır. Şu anda protokol tarafından oluşturulmamıştır, ancak ağda QI staking başlayana kadar QI için ek bir kullanım durumu sağlamalıdır. Lütfen Arrakis'in Uniswap havuzları kullandığını unutmayın, bu nedenle LP'ye girmek için hem QI hem de WETH'yi belirtilen oranlarda yatırmanız gerekir.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* Resmi olarak onaylanmış bir Balancer klonu olan [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019), Haziran 2022'de Optimism'de piyasaya sürüldü ve FRAX, USDC ve MAI'den oluşan "Come Together" adlı yepyeni bir yüksek likiditeye sahip stablecoin havuzu sunuyor. QI, BEETS ve BAL tokenları dahil olmak üzere büyük ödülleri nedeniyle, Optimism’de MAI için fiili stablecoin havuzu olacağı kesindir.


![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Optimisim’de Mai Finance

WETH (wrapped Ether) veya WBTC (wrapped Bitcoin) tokenlarınızı bir kasaya yatırabileceğiniz ve bunlara karşı MAI ödünç alabileceğiniz ödünç verme platformu Optimism'de zaten mevcuttur. MAI, QI kazanmak için Curve çiftliğine veya QI, BEETS ve BAL tokenlarında ödüller kazanan yeni başlatılan BeethovenX'teki yeni FRAX/USDC/MAI stabil havuzuna yatırılabilir.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## Sorumluluk Reddi

Bu kılavuz kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
