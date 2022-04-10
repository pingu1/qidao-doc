---
description: >-
  Bu kılavuzda, Polygon'un blok zincirinde bulunan farklı DApp'leri kullanmaya
  başlamak için bilmeniz gereken her şeyi açıklayacağız.
---

# Polygon'u Nasıl Kullanırım?

## Polygon nedir?

Polygon ağı, Ethereum Blockchain'in üzerine inşa edilmiş bir ağdır ve Ethereum Mainnet'in sahip olduğu ölçeklenebilirlik sorunlarını çözmek için tasarlanmıştır. Ortalama olarak, Polygon ağındaki bir işlem 3 ila 5 saniye sürer ve çok düşük işlem ücretlerine sahiptir. Bu da çok küçük bakiyeli bir cüzdanla her gün birkaç düzine işlem yapılmasına izin verir.

Polygon aynı zamanda piyasaya sürülen ilk “yan zincirlerden” diğer bir adıyla sidechainlerden biridir ve mevcut diğer zincirlere göre çok fazla ilerleme kaydederek Polygon şunları toplamayı başardı:

* Sürekli artan kullanıcı sayısı
* Her geçen gün artan uygulama sayısı
* Şu anda yaklaşık 4 milyar USD'yi geçen TVL

Polygon ayrıca ekosisteme ve Ethereum ağına güvenilir bir alternatif olduğunu kanıtladı. DeFi dünyasını, işlem ücretlerinde yüzlerce dolar harcamak zorunda kalmadan merkezi olmayan finansmanı denemek isteyen küçük yatırımcılara açtı. Bu güven ve kullanım kolaylığı ile birçok şirket, varlıkları bir ağdan diğerine köprülemeyi kolaylaştırmak, güvenliği ve anonimliği artırmak ve nihayetinde ağı daha güçlü hale getirmek için Polygon'a geçiş yaptı.

## Cüzdan Oluşturma

Polygon Blockchain'i kullanmadan önce bir cüzdan adresi oluşturmanız gerekir. Farklı cüzdan türleri, yazılımlar (Metamask, TrustWallet...) ve donanımlar (Trezor veya Ledger) vardır. Ancak bu kılavuzda, Polygon Blockchain'e nasıl erişileceğini açıklamak için Metamask kullanacağız.

### Metamask'ı İndirme

Polygon Blockchain'i kullanmak için tamamlamanız gereken ilk adım, web tarayıcınıza Metamask uzantısını indirmektir. Resmi siteden indirebilirsiniz. Metamask, iOS ve Android cihazlarda da kullanılabilir.

Bunu yaptıktan sonra, tarayıcınızda Metamask logolu bir uzantınız olmalıdır. Metamask uzantısını ilk açtığınızda, size bir Metamask hesabınız olup olmadığını soracaktır. Eğer varsa **seed** kelimeleri yazmanız gerekir (**seed** kelimelerin önemine daha sonra geleceğiz) yüklemek istediğiniz hesabın. Hesabınız yoksa, yeni bir hesap oluşturmanız gerekir. İzlemeniz gereken adımlar:

1. Her şeyden önce, Metamask hesabınız için bir şifre seçmeniz gerekecek.
2. Daha sonra cüzdanınızı nasıl koruyacağınız ve **seed** kelimelerin önemi ile ilgili videoyu izlemelisiniz.
3. **Seed** kelimeleri göreceksiniz. Yeni bir cüzdan oluştururken Seed kelimeleriz en önemli şeydir, çünkü **seed** kelimelerinizi kaybederseniz ve bilgisayarınız bozulursa Metamask hesabınıza erişemezsiniz. Bu yüzden lütfen **seed** kelimelerinize dikkat edin ve kimseyle paylaşmayın. İşiniz bittiğinde, tarayıcınızda şunu görmelisiniz:

![Metamask'ın Arayüzü](<../../.gitbook/assets/image (18).png>)

### Polygon Blok Zincirini Ekleme

Yukarıdaki resimde de görebileceğiniz gibi Ethereum Mainnet kullanıyoruz, ancak farklı bir ağa geçmek için ortaya tıklarsak Polygon Mainnet'in olmadığını göreceksiniz. Endişelenmeyin, yapmamız gereken Polygon Mainnet'i manuel olarak eklemek, bunun için Custom RPC'ye tıklayıp şunu yazmanız gerekiyor:

![](<../../.gitbook/assets/image (20).png>)

İşiniz bittiğinde, Polygon Blockchain'deki Metamask cüzdanını kullanmaya neredeyse hazırsınız, geriye kalan tek adım Ethereum Mainnet'i Polygon Mainnet'e geçirmek. Bunu yapmak için Metamask'ın üstündeki açılır menüye tıklamanız gerekiyor.

## Ücretsiz MATIC Alma

Artık Polygon Blockchain'i kullanmak için ayarlanmış her şeye sahipsiniz, ancak cüzdanınızda herhangi bir MATIC yok. Bu nedenle Polygon blok zincirinde herhangi bir işlem yapamazsınız. Bir işlem, temelde 2 adres arasındaki, işlenmesi biraz zaman gerektiren (bu işlem, Polygon'un sahip olduğu farklı doğrulayıcılar tarafından yapılır) ve bir ücreti olan (**gas** olarak da bilinir ve MATIC tokenları ile ödenir) bir değişimdir.

Neyse ki, [bu sayfa](https://matic.supply) size Polygon ağındaki ilk işlemlerinizi yapmak için ücretsiz MATIC sağlar (bu tür sayfalara musluk denilebilir). Yapmanız gereken tek şey cüzdanınızı sayfaya bağlamak ve captcha'yı tamamlamak. Bu 0,002 MATIC (\~0,00223$), Polygon Ağı kullanarak birkaç işlem yapmamızı sağlayacaktır.

![ÜCRETSİZ MATIC Alma](<../../.gitbook/assets/image (23).png>)

Bazen ağ tıkanıklığı nedeniyle, sayfayı kullanırken bazı sorunlar yaşayabilirsiniz. Biraz bekleyin ve tekrar deneyerek ücretsiz MATIC talep edebileceksiniz. Ayrıca, diğerinin çalışmaması durumunda [burayı](https://macncheese.finance/matic-polygon-mainnet-faucet.php) kullanmayı deneyebilirsiniz.

Yazının bir sonraki bölümüne geçmeden önce, bu muslukların insanların onu boşaltması için yapılmadığını, cüzdanınızda çok fazla MATIC varsa veya daha fazlasını talep etmeye çalışırsanız hiçbir şey sağlamayacağını bilmelisiniz. 24 saat içinde birkaç kez tekrarlayabilirsiniz. Bu yüzden lütfen dikkatli olun ve bencil olmayın.

## Metamask'a Token Ekleme

Artık Metamask'ınızda biraz MATIC'e sahip olduğunuza göre, Polygon'un sahip olduğu farklı DApp'leri ve tokenları kullanmaya hazırsınız. [PolygonScan](https://polygonscan.com) kullanarak kullanmak istediğiniz tokenın adresini kopyalayabilirsiniz. İlgili kısımlara, eklemek istediğiniz tokenın adını yazmanız yeterlidir. Örneğin, Polygon üzerinde QiDAO'yu ararsak şunu elde ederiz:

![Results of writing QiDAO on PolygonScan](<../../.gitbook/assets/image (24).png>)

Şimdi, sözleşmenin adresini kopyalamanız ve Metamask'ta **Token Ekle**'ye tıklamanız gerekecek.

![Adding Qi on Metamask](<../../.gitbook/assets/image (25).png>)

## Polygon'da Token Nasıl Satın Alınır?

Artık Metamask'ımız ve gas ücretini ödemek için biraz MATIC'imiz hazır olduğuna göre, Polygon ağında bazı tokenlar satın almaya başlayabiliriz. Bunu yapmak için bir DEX (Merkeziyetsiz Borsa) kullanmanız gerekir, aralarından seçim yapabileceğiniz birçok DEX vardır [_Quickswap_](https://quickswap.exchange/#/swap), [_Slingshot_](https://app.slingshot.finance/trade/m/MATIC/USDC), [_Dexguru_](https://dex.guru), [_Sushiswap_](https://app.sushi.com/swap), gibi.

Hangi DEX'i kullanmak istediğinize karar verdikten sonra, Polygon Blockchain'de favori tokenlerinizi satın almaya başlayabilirsiniz.

![Buying Qi tokens using Quickswap](<../../.gitbook/assets/image (26).png>)

{% hint style="info" %}
Token satın almak istediğinizde kullanabileceğiniz bir diğer ilginç DApp ise [Zapper](https://zapper.fi/es/exchange)'dir. Zapper teorik olarak iki tokenın takasını gerçekleştirmek için en ucuz platformu arar.
{% endhint %}

## Cüzdan Geçmişinizi Kontrol Etme

Cüzdanınızın geçmişini nasıl kontrol edeceğinizi bilmek önemlidir, bunu yapmak için [DeBank](https://debank.com)'ı kullanabilirsiniz. Debank, Metamask hesabınızda yaptığınız farklı işlemleri kontrol etmenize ve kullandığınız tüm blok zincirlerdeki veya sahip olduğunuz NFT'lerdeki portföyünüzü kontrol etmenize izin verecektir. Bu, örneğin bazı Qi stake ederken aldığınız farklı Qi airdroplarını karşılaştırmak istiyorsanız faydalı olacaktır.

![All the transactions made in our new Metamask address](<../../.gitbook/assets/image (27).png>)

Gördüğünüz gibi, cüzdanımda 800.000 DxDex.io var ama bu cüzdanımda olması için hiçbir şey yapmadım. Bu tür dolandırıcılıkların farkında olmanız ve bilmediğiniz hiçbir coin ile asla etkileşime girmemeniz gerekir. Onlara erişim izni vermeniz durumunda, Debank bunu iptal etmenize izin verecektir. Lütfen dikkatli olun ve tokenı bilmiyorsanız ona dokunmayın.

## Yararlı Bağlantılar

Polygon blok zincirini kullanırken faydalı bulabileceğiniz bazı bağlantılar şunlardır:

* [Quickswap](https://quickswap.exchange/#/swap)
* [AAVE](https://app.aave.com)
* [PolygonScan](https://polygonscan.com/gastracker/)

## Sorumluluk Reddi

Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen gelişmelerden haberdar olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
