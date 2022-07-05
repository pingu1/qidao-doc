---
description: >-
  Bu kılavuzda, Arbitrum’un sunduğu farklı DApp'leri kullanmaya başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# HArbitrum’u Nasıl Kullanırım?

## Arbitrum Nedir?

Arbitrum, kullanıcıların Ethereum ağı üzerinde işlem göndermelerine ve bunları çok daha düşük bir gas maliyetiyle daha hızlı yürütmelerine olanak tanıyan bir toplama ölçeklendirme çözümüdür. Bu nedenle Arbitrum, Ethereum Layer 2 (kısaca L2) olarak bilinir. Kardeş ağı Optimism gibi, Arbitrum da ağın ana Ethereum zinciriyle (Layer 1 veya L1) birlikte çalışmak için kullandığı kanıt türlerini ifade eden optimistik toplama teknolojisini kullanır. Optimism toplamalar ve ZK (Zero Knowledge) gibi diğer rollup çözümleri hakkında daha fazla bilgi için [bu linke](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/) göz atın.

Bir toplama teknolojisi olduğu için Arbitrum kendi bloklarını üretmez ve bu nedenle gerçek bir blok zinciri değildir. Arbitrum'un arkasındaki geliştiriciler olan Offchain Labs, ağ EVM'sini (Ethereum Virtual Machine) gelecekteki yükseltmelerle eşdeğer hale getirmeyi amaçlıyor.

Bu nedenle, Arbitrum’un kendi gas tokenını kullanmadığını, bunun yerine işlemler için ödeme yaparken gas olarak Ether'i kullandığını unutmayın.

## Arbitrium’a Başlarken

Arbitrum’u kullanmadan önce bir cüzdan adresine ihtiyacınız olacak. Arbitrum bir EVM ağı olduğu için Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM zincirlerinde olduğu gibi aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz ancak Soğuk cüzdanınızı ağa bağlayabilmek için ekstra adımları izlemeniz gerekebilir.

Bu eğitim için, tıpkı bu sitedeki diğer tüm kılavuzlar için yaptığımız gibi Metamask'a bağlı kalacağız. Yüklü Metamask'ınız yoksa, 
[Polygon başlangıç rehberine](../polygon/how-to-get-started-on-polygon.md) göz atın.

### Cüzdan Kurulumu

Metamask açılır penceresini açın, cüzdanınızın simgesine tıklayın, Ayarlar'a gidin, ardından Ağlar'ı seçin ve Ağ Ekle'yi bulun. İlgili metin alanlarında aşağıdaki bilgileri kullanacaksınız:

* **Network Name:** Arbitrum
* **New RPC URL:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **Chain ID:** 4216
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://arbiscan.io/](https://arbiscan.io/)

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Arbitrium’a geçirecektir:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## Arbitrium’a Köprüleme

### Musluklar

Arbitrium’da gas için musluk yoktur, ancak ElkNet gibi bir DApp kullanıyorsanız desteklenen ağlardan herhangi birinden köprülerken Elk tokenlarınızın bir kısmını gas olarak değiştirebilirsiniz.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### Köprüler

* MAI veya QI'nizi başka herhangi bir ağdan Arbitrium’a aktarmak istiyorsanız, [Multi Chain](https://app.multichain.org/#/router) Mai Finance'in resmi ortağıdır. Seçtiğiniz ağdan sadece hedef zinciri (Arbitrium) ve göndermek istediğiniz varlığı (MAI veya ETH) doğru miktarda seçip Aktar tuşuna tıklayabilirsiniz. Doğrudan aktardığınız varlık üzerinden alınan aktarım ücretlerine dikkat edin.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) popüler bir köprüdür ve yaklaşık on beş farklı ağdan tokenları Arbitrum'a aktarmanıza olanak tanır.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) bir başka popüler köprüdür. ETH ve USDC, DAI ve USDT gibi çeşitli stablecoinler dahil olmak üzere yalnızca az sayıda desteklenen token vardır, ancak diğer çoğu çözümden daha düşük köprü ücretleri sunar.
* [Hashflow](https://app.hashflow.com/) yeterli likiditeye sahip herhangi bir token için temelde çapraz zincir DEX (merkeziyetsiz borsa) olarak çalışan daha yeni bir köprüleme teknolojisidir. Ek olarak, Hashflow kullanıcıları şu anda token likiditesini değiştirmek veya sağlamak için HFT (Hashflow tokenları) kazanabilirler. Zincirler şu anda Ethereum, Avalanche, Arbitrum, Optimism, Polygon ve BNB ile sınırlıdır.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) wELK tokenını 2 ağ arasında aktardığınızda hem köprü hem de musluk görevi görecektir. ELK'inizi köprüleyebilir ve ELK'inizin küçük bir kısmına, yukarıdaki bölümde açıklandığı gibi, bizim durumumuzda ETH olan bir gas tokenı olarak doğrudan alıcı tarafta sahip olabilirsiniz.

## Arbitrum'da DeFi

* [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) şu anda Arbitrum'da MAI likiditesi olan tek havuza sahiptir. MAI'nizi MAI/USDC/USDT havuzuna yatırarak stablecoinlerden yaklaşık %13 getiri elde edebilirsiniz. Lütfen bu havuzun kısa süre içinde taşınacağını ve mevcut bir likidite hatasını düzelteceğini unutmayın.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## Arbitrum’da Mai Finance

WETH (wrapped Ether) veya WBTC (wrapped Bitcoin) tokenlarınızı bir kasaya yatırabileceğiniz ve bunlara karşı MAI ödünç alabileceğiniz ödünç verme platformu Arbitrium’da zaten mevcuttur. Daha sonra getiri elde etmek için ödünç aldığınız MAI'nizi Balancer'a yatırabilirsiniz.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## Sorumluluk Reddi

Bu kılavuz kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
