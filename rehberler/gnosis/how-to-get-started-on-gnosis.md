---
description: >-
  Bu kılavuzda, Gnosis'in blok zincirinde bulunan farklı DApp'lerini kullanmaya başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# Gnosis Chain Başlangıç Rehberi

## Gnosis Chain Nedir?

Gnosis Chain, EVM uyumlu bir blok zinciridir, yani Ethereum ağında kullanılan kodla uyumludur (EVM = Ethereum Sanal Makinesi). Çoğu zincir Güvenlik/Ölçeklenebilirlik/Merkeziyetsizlik Üçgeni'ne ulaşmaya çalışırken, Gnosis Chain hıza (5s işlem kesinliği) ve düşük işlem maliyetlerine odaklanır. Düzenli işlemler için ana gas tokenı olarak xDAI'yi (gnosis chain wrapped DAI) kullanır, ancak aynı zamanda yönetişim ve stake için GNO tokenını kullanır. Gnosis Chain başlangıçta Ethereum'un üzerine inşa edilmiş tahmin piyasaları için geliştirilmiştir. Tahmin piyasaları, olayların sonuçlarının alınıp satıldığı borsalar gibidir. Olaylar ortaya çıktıkça tahmin edilene bağlı olarak Gnosis tokenlarının değeri artar veya azalır.

Gnosis Chain hedefini desteklemek için özel merkeziyetsiz uygulamalar bulacağınız bir uygulama katmanı eklenmiştir. Örneğin:

RealT: Tokenize Emlak uygulaması
Kleros: Blok zinciri teknolojisini kullanarak çatışmaları çözmeyi amaçlayan bir Hizmet Olarak Adalet platformu

[DeFi Llama](https://defillama.com/chain/Gnosis)'dan TVL ve diğer uygulamalar gibi Gnosis Chain ile ilgili ek detayları inceleyebilirsiniz. 

## Gnosis Chain’e Başlarken

Gnosis Chain’i kullanmadan önce bir cüzdan adresine ihtiyacınız olacak. Gnosis bir EVM ağı olduğu için Metamask veya Nifty gibi web cüzdanları da dahil olmak üzere diğer EVM zincirlerinde olduğu gibi aynı cüzdanları kabul edecek ve Trezor veya Ledger gibi donanım cüzdanınızı kullanabileceksiniz ancak soğuk cüzdanınızı ağa bağlayabilmeniz için ekstra adımlar izlemeniz gerekebilir.

Bu eğitim için, bu sitedeki diğer tüm kılavuzlarda olduğu gibi Metamask'a bağlı kalacağız. Yüklü Metamask'ınız yoksa, [Polygon'a nasıl başlayacağınızla](../polygon/how-to-get-started-on-polygon.md) ilgili talimatlara bakabilirsiniz. 

### Metamask'a Gnosis Chain Ekleme

Teorik olarak, Gnosis MetaMask ile önceden yüklenmiş olarak gelir, yani Metamask'ın çalışması için zincir bilgilerini eklemeniz gerekmemelidir. Ancak, yerel cüzdanınıza kaydedilen değerleri iki kez kontrol ederek kurulumunuzun doğru olduğunu doğrulamak iyi bir fikir olabilir. Metamask açılır penceresini açın, cüzdanınızın simgesine tıklayın, `Ayarlar`'a gidin, ardından `Ağlar`'ı seçin ve `Gnosis Chain`’i bulun. Almanız gereken veriler aşağıdaki gibidir:

* **Network Name:** Gnosis Chain
* **New RPC URL:** https://rpc.gnosischain.com/
* **Chain ID:** 100
* **Currency Symbol:** xDAI
* **Block Explorer URL:** https://blockscout.com/xdai/mainnet

Değişiklikleri kaydedin, Metamask sizi otomatik olarak Gnosis Chain’e geçirecektir:

![Başardınız!! Artık Gnosis'tesiniz!](../../.gitbook/assets/gnosis-0.png)

## Gnosis Chain’e Köprüleme

### Musluklar

İşleme başlamak için ilk birkaç xDAI'nizi talep edebileceğiniz Gnosis Chain'de birkaç musluk bulmak için Google'ı kullanabilirsiniz. Özellikle bir şey önermiyorum, ancak her istekte 0.002 xDAI sağlayan [topluluk destekli musluğu](https://www.gimlu.com/faucet) buldum. Çalıştırabileceğiniz istek sayısının bir sınırı olduğunu ve bunun kesinlikle ücretsiz para kazanmanın bir yolu olmadığını unutmayın.
 
![Musluktan birkaç xDAI aldım, şimdi biraz işlem yapalım.](../../.gitbook/assets/gnosis-1.png)

### Köprüler

* MAI'nizi Polygon veya diğer ağlardan Gnosis Chain'e aktarmak istiyorsanız, [Multi Chain](https://app.multichain.org/#/router) Mai Finance'in resmi ortağıdır. Polygon'a bağlandığınızda, sadece hedef zinciri (Gnosis Chain) ve göndermek istediğiniz varlığı (MAI veya miMATIC) doğru miktarda seçip Aktar düğmesine tıklayabilirsiniz. Doğrudan aktardığınız varlık üzerinden alınan aktarım ücretlerine dikkat edin.

![Multi Chain kullanarak MAI'yi Polygon’dan Gnosis'e Köprüleme](../../.gitbook/assets/gnosis-2.png)

* [Elknet](https://app.elk.finance/#/elknet) ELK tokenını 2 ağ arasında aktardığınızda hem köprü hem de musluk görevi görecektir. ELK'inizi köprüleyebileceksiniz ve alıcı tarafta, bizim durumumuzda xDAI gas tokenı olarak ELK'inizin küçük bir kısmına doğrudan sahip olabilirsiniz.

## Gnosis'te DeFi

Gnosis, zincirinde aşağıdakiler de dahil olmak üzere birkaç DeFi seçeneği sunacaktır:

* [SushiSwap](https://app.sushi.com/farm?chainId=100): Gnosis/xDAI'deki ana DEX ve AMM'lerden biridir. Çiftliklerde LP (Likidite Sağlayıcı) çiftleri sağlayarak varlıklarınızı takas edebilecek veya likidite madenciliğine katılabileceksiniz.
* [Curve](https://xdai.curve.fi/): Likiditenin çoğunluğunun Gnosis Chain’den sağlandığı yer burasıdır. Burası aynı zamanda [MAI Stablecoin](https://xdai.curve.fi/factory/4) havuzunda MAI stablecoini sağlayabileceğiniz ve GNO tokenlarında ödüller alabileceğiniz yerdir.

![Haziran 2022 itibariyle Curve’de MAI içeren LP havuzları](../../.gitbook/assets/gnosis-3.png)

* [Honeyswap](https://app.honeyswap.org/#/pool), [Honeycomb](https://1hive.io/#/wallet) ve [Agave](https://app.agave.finance/#/dashboard): Sırasıyla, tokenları takas etmenize ve Likidite Sağlayan tokenlar oluşturmanıza olanak tanıyan bir DEX (Uniswap klonu), Honeyswap üzerinde oluşturulan LP tokenlarınızı stake etmenize ve likidite sağlamak için getiri elde etmenize olanak tanıyan bir AMM (Goose klonu) ve belirli varlıkları ödünç vermenize ve ödünç almanızı sağlayan bir ödünç verme protokolü (AAVE klonu). Bu 3 dApp, aynı ekip tarafından yönetilen eksiksiz bir ekosistem oluşturuyor. 
* [Elk Finance](https://app.elk.finance/#/farms): Elk, takas işlemleri yapmanızı, likidite yatırmanızı ve $ELK tokenlarını $MAI dahil olmak üzere Gnosis Chain’in farklı varlıklarını kullanarak toplamanızı sağlayacak bir Uniswap V2 klonudur. Ayrıca daha fazla ödül için ELK tokenlarınızı stake edebilir veya ElkNet köprüsünü kullanarak bir zincirden diğerine aktarabilirsiniz.

![Haziran 2022'den itibaren Elk Finance'te MAI kullanarak ELK çiftçiliği](../../.gitbook/assets/gnosis-5.png)

## Gnosis Chain’de Mai Finance

GNO tokenlarınızı bir kasaya yatırabileceğiniz ve buna karşı MAI ödünç alabileceğiniz ödünç verme platformu Gnosis Chain'de zaten mevcuttur. Bu şekilde, GNO tokenlarınızı teminat olarak kullanabilir ve MAI’nizi Curve'de daha fazla GNO tokenı toplamak için kullanabilirsiniz. Döngü şunlardan oluşacaktır:

* [Mai Finance](https://app.mai.finance) kasa oluştur
* $GNO tokenları bu kasaya yükle
* 0% faiz ile $MAI borç al
* Curve'deki $MAI havuzuna yükle ve GNO kazan

![Gnosis Chain’de Verim Çiftçiliği](../../.gitbook/assets/gnosis-4.png)

## Sorumluluk Reddi

Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Fiyat değişimlerine, arz ve talebe, ödül programlarının bitiş tarihlerine, kalıcı kayıplara vs. dikkat etmeniz gerekiyor.

{% hint style="info" %}
Amaç körü körüne takip edilebilecek tarifler önermek değildir. Lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeye hazır olduğunuza yatırım yapın.
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
