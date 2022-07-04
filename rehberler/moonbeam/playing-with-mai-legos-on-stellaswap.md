---
description: Bu kılavuzda StellaSwap ile verim elde etmek için Moonbeam'de MAI kullanımından bahsedeceğiz.
---

# StellaSwap'te MAI legoları ile oynamak

Mai Finance, Moonbeam'de kasa sunmasa da StellaSwap'in yeni MAI kasalarını kullanarak zincirdeki istediğiniz tokenlardan bazılarını MAI'ye mint’lemek için kullanmak mümkündür. Teminat tokenlarınızı kullanarak ve buna karşı MAI ödünç alarak xSTELLA ve MAI'yi içeren bir döngü stratejisi aracılığıyla büyük verim elde edebilirsiniz.

_NOT: Bu rehber kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Amaç körü körüne takip edilebilecek stratejiler önermek değildir. Bu yüzden lütfen kendi simülasyonunuzu yapın ve sadece kaybetmeyi göze aldığınız kadar yatırım yapın._

[StellaSwap](https://stellaswap.com/) Moonbeam'deki lider DEX'tir (merkeziyetsiz borsa). Tam özellikli bir DEX olarak StellaSwap, kullanıcılara token takas etme, çiftliklerde verim kazanma ve protokol yönetişimine katılma olanağı sunar. StellaSwap'i diğerlerinden ayıran özellik, kullanıcıların MAI'yi, Mai Finance ile ortaklık yoluyla doğrudan arayüzünden yerel olarak mint’lemesine izin veren bu tür ilk protokol olmasıdır.

![MAI'yi direkt StellaSwap üzerinden mint’leyin](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### MAI'yi StellaSwap üzerinden mint’lemek

Mai Finance'deki MAI kasalarının aksine, StellaSwap'in MAI kasaları varlıklarınıza karşı borçlanma için faiz alır. Şu anda kullanıcılar MAI'yi StellaSwap'in gelir paylaşımı stake token'ı xStella'ya %12 faizle veya Moonbeam'in yerel gas tokenının wrapped versiyonu olan wGLMR'ye %8 faizle ödünç alabilirler. Mai Finance'in %0 faiz kasalarına aşina olan kullanıcılar, yüksek faiz oranları karşısında şaşırmış olsalar da bu kılavuzda, StellaSwap'ten hiç ayrılmadan ödünç aldığınız stablecoin'lerinizden yüksek getiriler elde etmenize olanak tanıyan bir döngü stratejisinden geçeceğiz.

![StellSwap'teki Kasalar](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. İlk önce StellaSwap'in [MAI mintleme bölümüne](https://app.stellaswap.com/mai) gidin.
2. Buradan MAI ödünç almak için bir xStella veya wGLMR kasası oluşturabileceksiniz. Döngü stratejimizi oluşturmak için bir xStella kasası oluşturacağız.
3. Şimdi yeni oluşturduğunuz kasanıza girin ve xStella yatırın. Lütfen xStella kasalarının %40 LTV'ye (kredi/değer oranı) sahip olduğunu unutmayın; bu, her 100$ değerindeki xStella için 40$ değerinde MAI ödünç alabileceğiniz anlamına gelir.
4. Ardından, ödünç alma bölümüne gidip MAI'yi ödünç alabilirsiniz. Lütfen likidasyondan kaçınmak için LTV'nizi unutmayın.

![xStella kasası](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### Legoları bir araya getirmek

MAI'yi başarıyla ödünç aldığınıza göre şimdi onu kullanma zamanı! MAI'mizi StellaSwap'in MAI-Base4Pool stablecoin çiftliğine yatırarak güçlendireceğiz ve getirileri stake ederek daha fazla Stella tokenı kazanmak için kullanacağız. Bu stratejiyi kendi sorumluluğunuzda yaptığınızı ve gerekli özeni göstermezseniz kasanızın tasfiye edilebileceğini asla unutmayın! \
\
İlk olarak StellaSwap Çiftlikleri sayfasında MAI-Base4Pool'u bulalım. [Farm](https://app.stellaswap.com/farm) sayfası.

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Bu çiftlik şu anda MAI, FRAX, USDT, USDC ve DAI'den oluşan bir havuza sahip, Stella tokenlarında ödenen bir getiri ile stablecoinler üzerinde çok cazip bir %26 verim sunuyor. Bu verimin, şu anda ödünç alınan MAI'mize (%12) ödediğimiz faizi çoğunlukla dengelediğini unutmayın. Şimdiye kadarki performansımıza bir göz atalım:

$$effective interest = (collateral * borrow interest)-(mai*farmingyield)$$

Bu bize MAI'yi ödünç almak için %1,6'lık etkili bir verim sağlıyor - fena değil, ama daha iyisini yapabiliriz. Artık MAI-Base4Pool'da bulunarak kazandığımız Stella tokenlarını alıp [xStella almak için onları stake edebiliriz.](https://app.stellaswap.com/xstella).&#x20;

![Staking xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

xStella'yı stake etmenin iki ek avantajı vardır. Birincisi, %70'lik bir stake APR'si sağlayarak getirilerimizi birleştirir, ancak daha da önemlisi, protokolden elde edilen takas geliri kullanıcılar arasında paylaşıldığından xStella'nın değeri zaman içinde artar. Bu, bir stablecoin çiftliğinde nispeten güvenli konumumuzdan kazandığımız her türlü verimin sürekli olarak artacağı anlamına gelir. Daha sonra bu ek getirileri, LTV'mizi artırmak için kasamıza ek xStella yatırmak veya buna karşı ek MAI ödünç almak için kullanabiliriz.

## Sorumluluk Reddi

Bu kılavuz kesinlikle finansal tavsiye değildir, eğitim amaçlı hazırlanmıştır. Her zaman kendi araştırmanızı yapın. Bu kılavuzda bir projenin tartışılması, projenin onaylanması olarak değerlendirilmemelidir.

{% hint style="info" %}
Belirli bir zamanda iyi çalışan bir stratejinin başka bir zamanda kötü performans gösterebileceğini (veya para kaybetmenize neden olabileceğini) unutmayın. Lütfen güncel olun, piyasaları takip edin, yatırımlarınızı takip edin ve her zaman olduğu gibi kendi araştırmanızı yapın.
{% endhint %}
