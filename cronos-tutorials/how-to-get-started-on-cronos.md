---
description: >-
  Bu kılavuzda, Cronos kullanmaya başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# Cronos'u Nasıl Kullanırım?

## Cronos Nedir?

Crypto.com'dan bahsetmeden Cronos'un ne olduğunu açıklamak zor olacak. Crypto.com en büyük merkezi borsalardan biridir (CEX olarak da bilinir) ve Crypto.org Chain ve Cronos dahil olmak üzere kendi zincir setini inşa ediyor. Crypto.org Chain, tescilli bir teknolojiye sahip bir zincir iken Cronos, EVM (Ethereum Virtual Machine) uyumlu kardeşidir. CEX'e adanmış Binance Chain ve EVM uyumlu Binance Smart Chain ile hemen hemen aynı şeydir.

Cronos, diğer avantajlarının yanı sıra EVM uyumluluğu sunar; bu, diğer EVM zincirlerinde başlatılan uygulamaların çoğunun, Mai Finance ve Ölçeklenebilirlik dahil olmak üzere Cronos'a dağıtılabileceği anlamına gelir: Cronos, Ethereum Mainnet'ten daha hızlı ve daha ucuzdur.

## Cronos'a Başlarken

Cronos ağını kullanmak için bir cüzdan adresine ihtiyacınız olacak. Cronos, EVM uyumlu bir ağ olduğundan, Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM uyumlu zincirlerdekiyle aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz.

Bu eğitim için, bu sitedeki diğer tüm kılavuzlarda olduğu gibi Metamask'a bağlı kalacağız. Yüklü Metamask'ınız yoksa [Polygon'u Nasıl Kullanırım?](<../polygon-tutorials/how-to-get-started-on-polygon.md>) kılavuzunda ilgili talimatları bulabilirsiniz.

### Metamask'a Cronos Eklemek

Metamask'ın en son sürümünü yüklediyseniz zaten Cronos zincirine erişiminiz olmalıdır ve Metamask'ın açılır menüsünde Cronos'u seçmekten başka bir şey yapmanıza gerek yoktur. Bu adımları kullanarak Cronos'a erişmek için kendiniz de yeni bir RPC ayarlayabilirsiniz. Metamask açılır menüsünü açın, cüzdanınızın simgesine tıklayın, Ayarlar'a gidin, ardından Ağlar'ı seçin ve Cronos'u bulun. Almanız gereken veriler aşağıdaki gibidir

* **Network Name:** Cronos
* **New RPC URL:** https://evm-cronos.crypto.org
* **Chain ID:** 25
* **Currency Symbol:** CRO
* **Block Explorer URL:** https://cronos.crypto.org/explorer/

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Cronos ağına geçirecektir:

![Tebrikler! Artık Cronos'tasınız](<../.gitbook/assets/Cronos-onboarding-1.png>)

## Cronos'a Köprüleme

### Faucets

İlk işlemlerinizde ilk CRO tokenlarınızı almak için resmi bir musluk yoktur. Bununla birlikte bazı uygulamalar Cronos'a bazı fonları köprülerseniz veya sadece biraz gas’a ihtiyacınız varsa bu hizmeti sağlayacaktır.

* [Crystl Finance Faucet](https://cronos.crystl.finance/faucet): Cüzdanınızı bağladıktan ve captcha'yı tamamladıktan sonra cüzdanınıza gönderilecek bir miktar CRO talep edebilirsiniz.
* [Elk Finance](https://app.elk.finance/#/elknet): ELK tokenlarınızı bir zincirden diğerine köprülerken transfer edilen ELK'in küçük bir kısmını hedef zincirin yerel gas tokenıyla değiştirme seçeneğine sahip olacaksınız. Bu durum özellikle varlıkları ilk kez yeni bir zincire köprülüyorsanız kullanışlıdır.

![ElkNet köprüsünü kullanarak 1 doları gaz tokena dönüştürün](<../.gitbook/assets/Cronos-onboarding-2.png>)

* [Crypto.com](https://crypto.com/): Cronos'un Crypto.com'a derinden bağlı bir zincir olduğunu unutmayın. Orada bir hesap oluşturabilir, bir banka hesabı bağlayarak doğrudan CRO tokenlarınızı satın alabilir ve bunları Cronos'a gönderebilirsiniz.

{% hint style="info" %}
İşlem yapabilmek için bir miktar gas tokenına ihtiyacınız olacağını unutmayın. Bu, CRO tokenları olmayan bir hesaptaki varlıkları başka bir zincirden Cronos'a köprülerseniz takılıp kalacağınız ve hiçbir şey yapamayacağınız anlamına gelir. Cüzdanınızın gas tokenında en az bir takas işlemi gerçekleştirmek için yeterli paraya sahip olduğundan emin olun.
{% endhint %}

### Köprüler

* MAI'nizi Cronos'a bağlamak istiyorsanız, [Relay Chain](https://app.relaychain.com/transfer#/) Mai Finance'in resmi ortağıdır. RelayChain, MAI'nin birkaç farklı zincirden köprülenmesini destekliyor, böylece varlıklarınızı Polygon, Moonriver, Avalanche veya Shiden'den Cronos'a gönderebileceksiniz. Hedef zinciri Cronos olarak seçip gönderilecek tokenı seçmeniz yeterlidir (çoğu zaman MAI olarak adlandırılır ancak bazen miMATIC altındadır). Aktarılacak tutarı seçin ve 10 dakikadan fazla sürmemesi gereken aktarımı başlatın. Transfer ücretlerine dikkat edin. Bununla birlikte RelayChain’in bir avantajı da alıcı tarafta size bir miktar CRO vermesidir, böylece bir miktar MAI'yi CRO ile değiştirebilirsiniz.

![RelayChain kullanarak MAI'yi Çokgenden Cronos'a Köprüleme](<../.gitbook/assets/Cronos-onboarding-3.png>)

* [AnySwap](https://anyswap.exchange/#/router) bazı varlıkları Cronos'a aktarmak istiyorsanız çoğu zincir için bir imkandır. Ek bir not olarak AnySwap, MAI'nin Polygon'dan Cronos'a transferini de destekler.
* [ElkNet](https://app.elk.finance/#/elknet)'dan gelen köprü, EVM uyumlu herhangi bir zincirden ELK tokenını, transfer edilen miktarın küçük bir kısmını gas tokenına (hemen yukarıdaki Musluklara ayrılmış bölüme bakın) değiştirme imkanı ile konuşlandırıldıkları diğer herhangi bir EVM uyumlu zincire köprülemenizi sağlayacak özel bir durumdur.

### MAI Hub

Bazı MAI'leri Polygon'dan Cronos'a Relay Chain aracılığıyla köprülerseniz uygulama tarafından Cronos'ta basılan yerel MAI yerine MAI'nin RelayChain sürümünü alırsınız. İki token (RelayChain'den ve Mai Finance'ten olan) aynı değere ve aynı ada sahiptir ancak sözleşme adresleri farklıdır ve Cronos'ta farming verimi için kabul edilecek olan yalnızca Mai Finance'tekidir.

 [Mai Finance'teki merkezi kullanarak](https://app.mai.finance/hub)  1: 1 oranıyla Relay Chain'den değiştirebilirsiniz, ardından gerçek MAI'nizi diğer platformlarda kullanabileceksiniz.

![Hub'daki Cronos'ta MAI'yi (RelayChain) gerçek MAI ile değiştirme](<../.gitbook/assets/Cronos-onboarding-4.png>)

Eğer Cronos'tan başka bir zincire köprülemek istiyorsanız gerçek MAI'nizi Relay Chain versiyonuna dönüştürmeniz gerekeceğini unutmayın.

{% hint style="info" %}
AnySwap, MAI'nin Polygon'dan Cronos'a transferini destekliyor gibi görünüyor ancak MAI'nin merkez aracılığıyla değiştiremeyeceğiniz AnySwap sürümünü alacaksınız. Kullanılamaz bir tokenla karşılaşabilirsiniz, bu nedenle doğru köprüyü kullandığınızdan emin olun.
{% endhint %}

## Cronos'ta DeFi

Cronos Crypto.com'a bağlı olduğundan dolayı zincire birçok yatırım akıyor ve likiditeyi desteklemek için DeFi uygulamaları mevcut. Bu nedenle, aşağıdaki platformlarda verim elde edebilirsiniz:

* [CroDex](https://swap.crodex.app/#/swap):  Cronos'taki en iyi DEX'lerden (Merkeziyetsiz Borsalar) ve AMM'lerden (Otomatik Piyasa Yapıcıları) biridir ve QuickSwap gibi bir Uniswap v2 çatalıdır. Varlıklarınızı takas edebilecek, çiftliklerde LP (Likidite Sağlayan) çiftleri sağlayarak likidite madenciliğine katılabilecek veya daha fazla ödül kazanmak için platformun yerel tokenını stake edebileceksiniz. CroDex aynı zamanda Cronos'taki Mai Finance'in ilk resmi ortağıdır ve MAI'yi diğer varlıklarla takas edebileceğiniz ve MAI-USDC ve MAI-CRO çiftlerini yetiştirerek likidite madenciliği programlarına katılabileceğiniz tek yerdir.

![CroDex'te MAI ile Çiftçilik](<../.gitbook/assets/Cronos-onboarding-5.png>)

CroDex'te farm yaptığınızda daha fazla CRX tokenı almak için bir Kasada stake edebileceğiniz CRX tokenlarında ödüller alacaksınız ancak gelecekteki bir eğitimde sunulacak başka (daha iyi) seçenekler de var.

* [VVS](https://vvs.finance/) ve [CronaSwap](https://app.cronaswap.org/): Bunlar, CroDex'tekiyle aynı özellikleri alacağınız PancakeSwap'in (başka bir Uniswap çatalı) çatalları olan diğer DEX'ler/AMM'lerdir.

* [Beefy Finance](https://app.beefy.finance/#/cronos), [Adamant](https://adamant.finance/) ve [Autofarm](https://autofarm.network/cronos/) birçok ağda bulunan ve çoğu DEX'ten LP tokenlarınızı yatırabileceğiniz ve havuzlardan sorumlu algoritmaların farm tokenlarını ve bileşiklerini toplamasını sağlayabileceğiniz ünlü toplayıcılar / getiri optimize edicilerdir.

* [Crystl Finance](https://cronos.crystl.finance) ilk olarak Polygon'da başlatılan ve şimdi Cronos'ta da bulunan düz bir kaz çatalıdır. Kullanıcılar, stake edilebilen veya farmlanabilen (veya takas edilebilen) CRYSTL tokenlarını kazanmak için kasalara LP tokenları yatırabilecekler.

* [Fortune DAO](https://www.fortunedao.com/#/) DAI ve USDC'yi kabul eden Cronos'taki ana Ohm (Olympus) çatalıdır.

## Cronos'ta Mai Finance

Şu anda uygulama henüz tam olarak başlatılmadı ve çoğunlukla ChainLink Oracles'ın tokenları teminat olarak kabul etmesini bekliyor. Merkez zaten mevcut, bu nedenle 2022'nin ilk çeyreğinde bir lansman bekleyebilirsiniz.

## Sorumluluk Reddi

Bu kılavuz finansal tavsiye DEĞİLDİR, sadece bir eğitim aracı olarak görülmelidir. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
 Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın
{% endhint %}
