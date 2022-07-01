---
description: Bu kılavuzda, Moonbeam'i kullanmaya nasıl başlayacağınızı açıklayacağız.
---

# Moonbeam’i Nasıl Kullanırım?

## Moonbeam Nedir?

Ocak 2020'de piyasaya sürülen Moonbeam, Polkadot ağında çalışan ve Polkadot parachain olarak adlandırılan bir EVM (Ethereum Virtual Machine) uyumlu akıllı kontrat platformudur. Parachainler, Polkadot'un ana aktarıcı zincirinden yararlanan ve birlikte çalışabilir olan, böylece ana zincirin avantajlarından ve güvenliğinden yararlanan birbirine paralel zincirler kümesidir.

Polkadot, parachainlerin faydalarını şu şekilde açıklıyor: “Parachainler, daha önce sadece kendi kabile topluluklarına sahip izole ağların olduğu yerde, merkeziyetsiz, bağlantılı bir blok zincirler interneti oluşturarak izole blok zincirleri çağını sona erdiriyor.”

![Moonbeam bir Polkadot parachainidir](<../../.gitbook/assets/moonbeam (1).jpg>)

Moonbeam, EVM uyumluluk katmanı nedeniyle, Solidity geliştiricilerinin mevcut uygulamalarını diğer EVM uyumlu ağlardan birkaç kod değişikliği ile Moonbeam'e taşımasını kolaylaştırır. Moonbeam şu anda 130m$’lık bir TVL'ye ve [hızlı büyüyen](https://defillama.com/chain/Moonbeam) bir uygulama ekosistemine sahip.

Moonbeat ayrıca Substrat uyumluluğu sunar. Substrate, geliştiriciler tarafından palet adı verilen yeniden kullanılabilir bileşenleri kullanarak ihtiyaçlarına göre uyarlanmış blok zincirleri oluşturmak için kullanılan modüler bir blok zinciri çerçevesidir. Rust programlama dilini kullanır ve çoğu geliştiricinin Polkadot ağı için parachain oluştururken kullandığı çerçevedir.

Moonbeam, Substrat tabanlı bir blok zinciri olduğundan, ağıyla entegre olan uygulamalar, Polkadot ve Ethereum zincirlerinin yanı sıra Bitcoin gibi diğerleri arasındaki birlikte çalışabilirlikten yararlanır.

Geliştiriciler ayrıca, blok kaşifler, front-end geliştirme kitaplıkları ve cüzdanlar dahil olmak üzere Ethereum'da yaygın olarak kullanılan Substrate uyumlu ekosistem araçlarını ve ayrıca Truffle ve Remix gibi geliştirme araçlarını kullanabilir.

Moonbeam’in yerel gas tokenı GLMR'dir.

## Moonbeam’e Başlarken

Moonbeam’i kullanmadan önce bir cüzdan adresine ihtiyacınız olacak. Moonbeam bir EVM ağı olduğu için Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM zincirlerinde olduğu gibi aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz ancak Soğuk cüzdanınızı ağa bağlayabilmek için ekstra adımları izlemeniz gerekebilir.

Bu eğitim için, tıpkı bu sitedeki diğer tüm kılavuzlar için yaptığımız gibi Metamask'a bağlı kalacağız. Yüklü Metamask'ınız yoksa, Polygon Başlangıç Rehberine göz atın.

### Metamask'ta Cüzdan Kurulumu

Metamask açılır penceresini açın, cüzdanınızın simgesine tıklayın, Ayarlar'a gidin, ardından Ağlar'ı seçin ve Ağ Ekle'yi bulun. İlgili metin alanlarında aşağıdaki bilgileri kullanacaksınız:

* **Network Name:** Moonbeam
* **New RPC URL:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **Chain ID:** 128
* **Currency Symbol:** GLMR
* **Block Explorer URL:** [https://moonscan.io/](https://moonscan.io/)

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Moonbeam’e geçirecektir:

![Moonbeam hesabınız artık Metamaskta](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## Moonbeam'e Köprüleme

### Musluklar

GLMR, Moonbeam'in yerel gas tokenıdır, bu nedenle zincir üzerinde işlem yapmak için cüzdanınızda biraz token olması gerekir. Neyse ki, resmi Moonbeam musluğu, küçük bir miktar GLMR ile başlamanıza yardımcı olacaktır, ancak lütfen ağ sıkışıksa dağıtılan token miktarının bazen bir işlemi tamamlamak için yeterli olmayabileceğini unutmayın.

Ücretsiz GLMR almak için, captcha botu aracılığıyla robot olmadığınızı doğrulamanız ve Metamask cüzdanınızı siteye bağlamanız gerekir. Ardından hemen cüzdanınıza küçük bir miktar (0,007 GLMR) gönderilecektir.

![GLMR.sağlayan musluk](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

Ek olarak, kullanıcılar Solarflare'in "[Gas ile değiştir](https://app.solarflare.io/bridge/gas-swap)"  özelliğini kullanmak isteyebilir. Bu özellik, kullanıcıların WETH, WBTC, USDC, DAI, USDT, BUSD, FLARE ve BNB dahil olmak üzere diğer tokenları Moonbeam'in yerel gas tokenı olan GLMR ile değiştirmesine olanak tanır.

![Solarflare'in "Gas ile değiştir" özelliği](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### Köprüler

* [Multichain](https://app.multichain.org/#/router) MAI Finance ile olan ortaklığından dolayı MAI için resmi köprüdür. Bu köprüyü kullanarak MAI'nizi kolayca Moonbeam'e gönderebilirsiniz.

![Multichain Moonbeam Köprüsü](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) Moonbeam'de Uniswap'e çok benzeyen tam özellikli bir AMM'dir (Automated Market Maker). Solarflare, kullanıcıların Ethereum ana ağından ve BNB zincirinden Moonbeam'e varlıkları köprülemelerine olanak tanıyan yerleşik bir köprüye sahiptir. Solarflare ayrıca yukarıdaki Musluklar bölümünde belirtildiği gibi "Gas ile Değiştir" özelliğine sahiptir.

![Solarflare'de köprüleme](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) Moonbeam'i de destekleyen popüler bir köprüdür. Lütfen her zincirden Moonbeam'e köprü yapamayabileceğinizi unutmayın (Örneğin, Polygon’dan Moonbeam'e köprüleme yapılamaz).

![Celer ile köprüleme](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* Başka köprüler de mevcuttur ancak Cosmos ekosistemi için Nomad veya Axelar gibi zincire özel olabilir.

## Moonbeam’de DeFi

[StellaSwap](https://app.stellaswap.com/farm) şu anda Moonbeam'deki MAI için ana likidite kaynağıdır. MAI-Base4Pool, MAI, FRAX, USDT, USDC ve DAI'den oluşur, şu anda 535k$’lık bir TVL'ye sahiptir ve stablecoinlerinizde %26'lık sağlam bir APR sağlar.

![MAI-Base4Pool on StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam, [Curve](https://moonbeam.curve.fi/) ve [Beefy Finance](https://app.beefy.com/) gibi diğer zincirlerde bulunan düzinelerce DApp (merkeziyetsiz uygulama) ile canlı bir DeFi ekosistemine sahiptir. Mevcut DApp'lerin tam listesi için [DefiLlama Moonbeam sayfasına](https://defillama.com/chain/Moonbeam)ayfasına göz atın.

## Moonbeam'de Mai Finance

Mai Finance, Moonbeam'de mevcut olmasa da kasalar oluşturabilir ve StellaSwap'te xStella ve wGLMR'ye karşı MAI ödünç alabilirsiniz. Lütfen MAI'yi StellaSwap üzerinden ödünç almanın faiz getireceğini unutmayın - xStella kasalarında %12 ve wGLMR kasalarında %8. StellaSwap'in MAI kasalarının nasıl kullanılacağı hakkında daha fazla bilgiyi StellaSwap'te MAI legolarıyla oynamak başlıklı bir sonraki bölümde bulabilirsiniz.

![StellaSwap'taki kasalar](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## Sorumluluk Reddi

Bu kılavuz kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
