---
description: >-
  Bu kılavuzda, Avalanche kullanmaya başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# Avalanche nasıl kullanılır?

## Avalanche nedir?

Avalanche, merkezi olmayan uygulamalar ve özel blok zinciri ağları için bir platform olarak işlev gören birinci katman blok zinciridir. Avalanche ağı üç ayrı blok zincirinden oluşur: X-Chain, C-Chain ve P-Chain. Her zincirin diğerinin yaklaşımından kökten farklı olan, yani tüm düğümlerin tüm işlemleri doğrulamasını sağlayan farklı bir amacı vardır. Avalanche blok zincirleri kullanım durumlarına göre farklı fikir birliği mekanizmaları bile kullanır.

Avalanche, mevcut Ethereum toolkit ile %100 EVM uyumludur ve C-Chain'i, Ethereum ile aynı işlevselliği sunar. Ancak daha yüksek verim, yüksek işlem kapasitesi ve çok daha düşük işlem ücretleri sunar. AVAX, Avalanche ağının gas simgesidir

## Avalanche'a Başlarken

Avalanche ağını kullanmadan önce bir cüzdan adresi oluşturmanız gerekecektir. Metamask veya yerel [Avalanche Wallet](https://wallet.avax.network) gibi \*\*yazılım cüzdanları \*\* ve ayrıca \*\*donanım dahil olmak üzere kullanılabilecek farklı cüzdan türleri vardır. [Trezor](https://trezor.io/coins/) veya [Ledger](https://support.ledger.com/hc/en-us/articles/360020765779-Avalanche-AVAX) gibi \*\* cüzdanlar -?docs=true)

Bu eğitimin amacı için Metamask kullanacağız. Yüklü Metamask'ınız yoksa, [Polygon'a nasıl başlanır](../polygon-tutorials/how-to-get-started-on-polygon.md#downloading-metamask) ile ilgili talimatları bulabilirsiniz.

### Metamask'a Avalanche Ekleme

valanche ağını kullanmak için Metamask'a eklemeniz gerekir. Bunu yapmak için Ağ menüsüne tıklayın (eğer bunu ilk kez kuruyorsanız Ethereum Mainnet'i okuyacaktır), ardından özel RPC'yi seçin. Daha sonra açılan forma aşağıdaki değerleri ekleyebilirsiniz:

* **Network Name**: Avalanche Network
* **New RPC URL**: [https://api.avax.network/ext/bc/C/rpc](https://api.avax.network/ext/bc/C/rpc)
* **ChainID**: 43114
* **Symbol**: AVAX
* **Explorer**: [https://cchain.explorer.avax.network/](https://cchain.explorer.avax.network)

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Avalanche ağına geçirecektir.

![Aferin! Artık Avalanche'dasınız!](<../.gitbook/assets/Screen Shot 2021-10-12 at 8.59.08 PM.png>)

## Avalanche'dan Köprü Kurmak

### Faucet

Şu anda Avalanche ana ağında faucet bulunmamaktadır. Gas maliyetlerini karşılamak için biraz AVAX'a ihtiyacınız varsa, AVAX'i merkezi bir borsadan doğrudan cüzdanınıza veya Elknet köprüsü aracılığıyla tokenları köprüleyerek göndermeniz gerekir. Aşağıdaki [Köprüler](nasıl-başlangıç-on-avalanche.md#bridges) bölümünde bu ikinci seçenek hakkında daha fazla bilgi bulabilirsiniz.

### Köprüler

* [Resmi Avalanche köprüsü](https://bridge.avax.network) - Avalanche, Ethereum ana ağından Avalanche'a varlıkları köprülemek için kullanılabilecek kendi köprüsüne sahiptir. Gaz ücretleri köprülü token ile ödenir ve Ethereum'dan köprü kurduğunuz için yüksek olabilir.
* [Anyswap](https://anyswap.exchange/#/bridge) ayrıca varlıkların birçok farklı zincire bağlanmasına izin verir. Köprüleme için tokena bağlı olarak değişen minimum token miktarları vardır, ancak köprüleme maliyeti sabit bir ücrettir.
* [Celer Bridge](https://cbridge.celer.network/#/transfer), harika bir kullanıcı arayüzü ile birçok zincir için köprüleme hizmetleri sunar. Avalanche'a köprüleme ücreti yaklaşık %3'tür.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer), düşük ücretlerle kullanımı kolay ve sezgisel bir arayüz sunar. Ek not olarak, Relay Chain, [MAI to Avalanche köprüsü](../mai-university/mai-metaverse.md#avalanche) için resmi olarak desteklenen çözümdür.
* [Elknet](https://app.elk.finance/#/elknet), Avalanche, Binance, Fantom, Polygon ve xDai dahil olmak üzere birden fazla ağda bulunan merkezi olmayan bir borsa olan Elk Finance tarafından sunulan bir köprüleme hizmetidir. Elknet'i bu listedeki diğer köprülerden ayıran şey, köprüleme için AVAX'a gerek olmamasıdır. Köprüleme maliyeti sadece işlem için gas ücretidir.
  * Tokenlarınızı Elknet üzerinden Avalanche'a taşımak için, önce onları Elk Finance'in tokenı olan Elk'e dönüştürmeniz gerekir.
  * Ardından, ELK'nizi desteklenen ağlardan Avalanche'a taşımak için köprüyü kullanabilirsiniz ve "$ELK 1'i gazla takas et" seçeneğini işaretlerseniz, transferinizin bir kısmı AVAX'a dönüştürülür.
  * Köprüleme tamamlandıktan sonra (genellikle 10 dakikadan az), cüzdanınızı Avalanche ağına geçirebilirsiniz ve ELK'nizi ve bir miktar AVAX'ın dağıtılmaya hazır olduğunu göreceksiniz. Artık ELK'nızı doğrudan sitede Avalanche'ta desteklenen herhangi bir token ile değiştirebilirsiniz.
  * Aynısı, Polygon'a veya başka bir desteklenen zincire geri dönmek için tersine yapılabilir.

![Elknet arayüzü](<../.gitbook/assets/Screen Shot 2021-10-12 at 9.49.30 PM.png>)

## Avalanche'da DeFi Uygulamaları

Avalanche, son aylarda yalnızca büyük  projelerin geliştirilmesine değil, aynı zamanda henüz piyasaya sürülmemiş olan Curve dahil olmak üzere büyük deFi bluechip'lerinin ağa geçiş yapmaya başlamasına yol açan büyük bir büyüme gördü.

* [Aave](https://app.aave.com/dashboard) kısa süre önce Avalanche'da piyasaya sürüldü ve şimdiden toplam 4 milyar dolarlık kilitli değer gördü. Avalanche'da desteklenen teminat tokenları arasında Aave, Avalanche, Dai, Tether, USDC, WBTC ve WETH bulunur. camAVAX tokenları, Mai Finance kasaları için teminat olarak kabul edilecektir.
* [Beefy Finance](https://app.beefy.finance/#/avax) Binance, Fantom, Harmony, Polygon ve daha fazlası dahil olmak üzere diğer zincirlerde mevcut olduğundan muhtemelen çoğu DeFi kullanıcısı tarafından iyi bilinmektedir. Beefy, otomatik birleştirici olarak bilinen araçtır ve şu anda hem tek tek hem de çift tokenlı çiftlikler için harika APY sağlar. Beefy, [MAI/AVAX](https://app.beefy.finance/#/avax/vault/joe-mai-wavax) ve [MAI/USDC.e ](https://app.beefy.finance/#/avax/vault/joe-mai-usdc.e)Trader Joe'da bulunan LP'ler.
* [Benqi](https://app.benqi.fi/markets) Aave'ye benzer bir piyasa protokolüdür ve ağda türünün ilk örneğidir. Desteklenen teminat tokenları Avalanche, Dai, Link, Tether, USDC, WBTC ve WETH'dir.

![BenQI arayüzü](<../.gitbook/assets/Screen Shot 2021-10-12 at 10.11.19 PM.png>)

* [TraderJoe](https://www.traderjoexyz.com/#/home) merkezi olmayan bir borsadır ve sezgisel bir kullanıcı arayüzü ve kullanıcıların bir tokenı doğrudan bir likidite havuzu tokenına dönüştürebilirsiniz. TraderJoe ayrıca [Avalanche üzerinde MAI-USDC LP havuzunun](../mai-university/mai-metaverse.md#using-mai-on-avax) resmi ortağıdır.

![](<../.gitbook/assets/Screen Shot 2021-10-12 at 10.31.18 PM.png>)

* [YieldYak](https://yieldyak.com/farms), aynı zamanda yüksek çiftçilik APY'leri sağlayan başka bir otomatik bileşendir. Tek token çiftlikleri, daha yüksek getirilerden yararlanmak için BenQI ile birlikte çalışır ve bu nedenle riskli olarak kabul edilir.

![](<../.gitbook/assets/Screen Shot 2021-10-12 at 10.20.18 PM.png>)

## Diğer faydalı bağlantılar

* [Avalanche Ağı](https://www.avax.network/)
* [Avalanche topluluğu bağlantıları](https://www.avax.network/community) (Discord, Medium, Reddit, Twitter, vb.)
* [Debank](https://debank.com), portföy yöneticisi

## Sorumluluk Reddi

Bu kılavuz finansal tavsiye DEĞİLDİR ve sadece bir eğitim aracı olarak görülmelidir. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.
