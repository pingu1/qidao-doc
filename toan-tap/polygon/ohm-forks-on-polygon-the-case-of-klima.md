---
description: >-
  Hướng dẫn này sẽ trình bày đơn giản hóa các bản fork của Olympus DAO và cách
  bạn có thể hưởng  lợi từ chúng bắng cách sử dụng MAI Finance và trường hợp cụ
  thể là KlimaDAO trên Polygon.
---

# Bản sao chép OHM trên Polygon: Trường hợp của KlimaDAO

Nếu bạn theo dõi tin tức tiền điện tử trong vài tháng gần đây, bạn chắc chẵn đã nghe qua dự án Olympus DAO và các bản fork của nó trên các hệ sinh thái khác nhau. Tôi sẽ cố trình bày nhanh các dự án này là gì, các giao thức cốt lõi của chúng cũng như cách mà bạn có thể sử dụng chúng như một phần trong chiến lược đầu tư của mình. Đến phần cuối của phần này, chúng ta sẽ tập trung vào một trường hợp cụ thể là Klima DAO, một trong những bản fork thành công nhất của Olympus DAO trên mạng  lưới Polygon. &#x20;

## Những bản nhánh của Olympus DAO là gì?

### OHM là gì và bản nhánh là gì?

Tất cả mọi thứ bắt đầu trên Ethereum Mainnet với sự ra đời của Olympus DAO. Mục tiêu của họ ra tạo ra một loại tiền tệ mới có thể cạnh tranh với đồng USD với giá trị được thả nổi theo thị trường. Đồng bản vị của Olympus DAO là OHM được hỗ trợ hoàn toàn bởi tập hợp các loại tài sản mã hóa khác nhau.

Olympus DAO được ra mắt vào tháng 3 năm 2021 và hiện vẫn là một dự án thành công trên mainnet với TVL lên đến hàng chục triệu đô trong khi giá của token OHM vẫn ở mức cao. Chính vì sự thành công này nên đã có rất nhiều bản sao chép của Olympus DAO xuất hiện ở nhiều chuỗi khác nhau.&#x20;

### Tổng quan về Tokenomics

Phần này sẽ có lượng kiến thức kỹ thuật nhiều hơn những hướng dẫn trước đây tuy nhiên để có thể hiểu được thành công của Olympus DAO, chúng ta phải hiểu được cách nó hoạt động.

Ý tưởng cơ bản của giao thức Olympus là tăng kho bạc nhiều nhất có thể bằng cách bán mã thông báo gốc với giá chiết khấu, đồng thời duy trì nguồn cung lưu hành ở mức thấp nhất có thể để duy trì mức giá cao. Điều này được thực hiện bằng cách cung cấp phần thưởng rất cao cho các nhà đầu tư và có gần như toàn quyền kiểm soát thanh khoản.

* **Trái phiếu:** giao thức sẽ đề xuất các mã thông báo gốc ở mức giá chiết khấu. Giá được trả bằng cách sử dụng các tài sản cụ thể được sử dụng để hỗ trợ mã thông báo gốc. Trong ví dụ về Olympus DAO, mã thông báo OHM được hỗ trợ 100% bởi một số mã thông báo bao gồm chủ yếu là DAI, do đó, trái phiếu có thể được mua trực tiếp bằng DAI hoặc sử dụng cặp DAI-OHM LP (và gần đây là các mã thông báo FRAX). Khi mọi người mua mã thông báo gốc bằng cách sử dụng tài sản hỗ trợ hoặc mã thông báo LP, khoản thanh toán sẽ được chuyển trực tiếp vào kho bạc, cho phép giao thức đúc nhiều mã thông báo hơn, do đó có thể chạy trong một khoảng thời gian dài hơn. Điều duy nhất là mã thông báo chiết khấu được phát hành trong thời gian vesting, có nghĩa là người dùng đã mua mã thông báo gốc bằng cách sử dụng trái phiếu sẽ không thể sử dụng ngay lập tức.
* **Gửi cố phần:** sau khi mua trái phiếu, người dùng sẽ thu thập các mã thông báo gốc và sẽ có sự lựa chọn giữa việc bán chúng hoặc đặt cố phần. Để đảm bảo rằng tùy chọn thứ hai sẽ được chọn, giao thức cung cấp phần thưởng cực kỳ cao cho những người đặt cược (chúng ta đang nói về mức lãi lên đến 1,2% hàng ngày !!!). Mục tiêu đằng sau những APR cao này là đạt được tỷ lệ đặt cổ phần gần 100% nhất có thể. Nếu không có nhiều token lưu hành, giá sẽ tăng và cùng với phần thưởng cao, thì việc đặt cổ phần thậm chí còn hấp dẫn hơn thế. Một lưu ý nhỏ là giá tăng cũng sẽ giúp giữ tỷ lệ phần thưởng cao.
* **Tăng ngân quỹ và kiểm soát thanh khoản:** Lưu trữ kho bạc được tăng lên từ việc bán trái phiếu và từ thực tế là các mã thông báo gốc có thể được liên kết với các mã thông báo LP hầu như được kiểm soát hoàn toàn bởi giao thức. Các mã thông báo LP này được sử dụng để thu phí hoán đổi cho những người dùng thích mua mã thông báo gốc trên thị trường với giá đầy đủ so với việc mua bằng trái phiếu (xem chương tiếp theo để biết chi tiết).
* **Mua lại và đốt:** Hầu hết các dự án giống OHM bao gồm một cơ chế sẽ mua lại các mã thông báo gốc và đốt chúng vào những dịp rất cụ thể. Vấn đề xảy ra khi người dùng bắt đầu bán các mã thông báo gốc, khiến giá bắt đầu giảm xuống. Tuy nhiên, nếu mọi người bán mã thông báo của họ, APY sẽ tăng lên vì số lượng mã thông báo được đúc vẫn giữ nguyên đối với các mã thông báo đặt cổ phần ít hơn. Nhưng ngay cả với APY cao hơn, nếu không có ai mua và đặt cổ phần các mã thông báo đã bán, giao thức cũng có thể mua lại chúng từ thị trường để tạo áp lực mua, đẩy giá lên và giữ cho nguồn cung lưu hành ở mức thấp. Các token được mua lại chỉ đơn giản là bị đốt. Thật vậy, vì một phần của kho bạc đã được sử dụng để mua những mã thông báo này, việc giữ chúng trong kho bạc hoặc phân phối chúng sẽ thực sự làm loãng kho bạc, điều này sẽ làm giảm tỷ lệ phần thưởng hoặc ảnh hưởng đến khoảng thời gian mà giao thức có thể chạy.

Bạn có thể tìm thấy nguồn thông tin bổ sung về Olympus DAO tại đây:

* [DeFi 2.0 - A new Narrative? Olympus DAO, Tokemak Explained](https://www.youtube.com/watch?v=l0vRTi8\_FRk)
* [WTF is Olympus DAO](https://newsletter.banklesshq.com/p/wtf-is-olympus-dao)

### Trái phiếu VS Gửi cổ phần

Tại sao ai đó sẵn sàng mua một mã thông báo trong khi có một phiên bản có giá thấp hơn bằng trái phiếu. Đây hoàn toàn là câu hỏi chính đáng và câu trả lời phụ thuộc vào mức chiết khấu mà trái phiếu đưa ra.

Vì chúng ta đang làm việc với Klima DAO, hãy so sánh giữa mua và đặt cổ phần với trái phiếu:

![Phần thưởng đặt cổ phần Klima tháng 11 năm 2021](../../.gitbook/assets/Klima-1.png)

![Mức ROI của trái phiếu trên Klima tại thời điểm 11/2021](../../.gitbook/assets/Klima-2.png)

Nếu một người mua trực tiếp Klima từ thị trường và đặt cổ phần trong 5 ngày (thời gian thực tế của trái phiếu, ROI (Lợi tức đầu tư) sẽ là 8,51%. Nếu một người mua trái phiếu thay thế, ROI tối đa sẽ là 5,47% bằng cách cung cấp cặp BCT / KLIMA.

Điều này có nghĩa là, với số tiền tương đương 100 đô la, bạn sẽ nhận được sau 5 ngày

* $108.51 với lựa chọn 1
* $105.47 với lựa chọn 2

Tuy nhiên, điều quan trọng là phải hiểu rằng trái phiếu Klima được phát hành trong thời gian chuyển biến. Do đó, bạn có thể thu hoạch Klima được trao và đặt cược nó để kiếm lợi nhuận từ các đợt phân phối phần thưởng. Vì bạn sẽ chỉ nhận được phần thưởng cho bất cứ thứ gì bạn đã đặt cược trong thời gian chuyển biến và vì có 15 đợt phân phối phần thưởng trong 5 ngày để trái phiếu được phát hành hoàn toàn, chúng ta có thể giả định rằng bạn có khả năng thu được 6,67% trước mỗi một trong số 15 khoản bồi hoàn. Giả sử bạn sẽ thu hoạch và đặt cổ phần vào đầu mỗi đợt bồi hoàn, bạn sẽ nhận được:

| # Các đợt trả thưởng | Số lượng được đặt  | Phần thưởng  | Tổng phần thưởng |
| -------------------- | ------------------ | ------------ | ---------------- |
| 1                    | 7.031              | 0.038        | 0.038            |
| 2                    | 14.063             | 0.077        | 0.116            |
| 3                    | 21.094             | 0.116        | 0.232            |
| 4                    | 28.125             | 0.155        | 0.397            |
| 5                    | 35.157             | 0.193        | 0.580            |
| 6                    | 42.188             | 0.232        | 0.812            |
| 7                    | 49.219             | 0.271        | 1.083            |
| 8                    | 56.251             | 0.309        | 1.392            |
| 9                    | 63.282             | 0.348        | 1.740            |
| 10                   | 70.313             | 0.387        | 2.127            |
| 11                   | 77.345             | 0.425        | 2.552            |
| 12                   | 84.376             | 0.464        | 3.016            |
| 13                   | 91.407             | 0.503        | 3.519            |
| 14                   | 98.439             | 0.514        | 4.061            |
| 15                   | 105.470            | 0.580        | 4.651            |

Vào cuối mỗi giai đoạn chuyển đổi, ROI 5,47% được ghi nhận, nhưng phần thưởng đặt cổ phần cũng tăng thêm 4,65% (chưa được cộng lại), dẫn đến ROI 10,12%. Điều này có nghĩa là trái phiếu thực sự thú vị hơn đặt cổ phần trực tiếp, ngay cả khi ROI trái phiếu có vẻ thấp hơn ROI đặt cổ phần.

Tổng phần thưởng bạn sẽ nhận được khi đặt cược N lần trong khoảng thời gian chuyển đổi (với Nmax tối đa = 15) là:

$$Tổng_{phần.thưởng} = \sum_{i=1}^{N}{\frac{Vốn.đầu.tư * i * (1 + APR_{Thời.gian.chuyển.đỏi})}{N} * APR_{Đặt.cổ.phần}}$$

Sau đó, bạn có thể chạy các mô phỏng của riêng mình để xác minh xem liệu tốt hơn nên mua và đặt cược hay gửi trái phiếu. Trong ví dụ, với ROI đặt cược là 8,51% trong 5 ngày, chiết khấu liên kết 3,95% với 15 lần tăng giá sẽ tốt hơn (cho ROI tương đương là 8,52%).

{% hint style="info" %}
Bạn có thể chạy mô phỏng tương tự với thu hoạch + đặt cổ phần chỉ một lần một ngày thay vì 3 lần một ngày trước mỗi lần rebase. Đối với cùng một APY như trên, bạn sẽ cần chiết khấu trái phiếu là 6,76% để có được ROI tốt hơn so với đặt cổ phần.
{% endhint %}

{% hint style="success" %}
Bạn có thể tìm thấy một trình mô phỏng để tính toán gửi trái phiếu VS đặt cổ phần của mình dưới [dạng bảng tính google](https://docs.google.com/spreadsheets/d/1MTKTbf-ZAihGbEax3WEwkxToG7IlPKlwmYq59O3KG2o/edit#gid=0), bạn có thể sao chép và chỉnh sửa theo ý mình. Lưu ý rằng trang này KHÔNG được duy trì cũng như không được cung cấp bởi cộng đồng QiDAO.
{% endhint %}

### Trường hợp đặc biệt của Klima DAO

Đặc điểm cụ thể khiến Klima DAO khác với các Ohm-fork khác là tài sản chính hỗ trợ mã thông báo gốc Klima: mã thông báo BCT, được cung cấp bởi [Toucan Protocol](https://toucan.earth). BCT (Base Carbon Tonne) thực sự đại diện cho các khoản đầu tư vào thế giới thực để khử carbon trên trái đất, biến lượng carbon bù đắp từ thế giới thực thành token. Bạn có thể đọc thêm nhiều điều về cách nó hoạt động trong [tài liệu chính thức ](https://docs.toucan.earth/protocol/introduction/defi-refi)của Toucan

BCT sau đó được [ứng dụng Klima DAO ](https://dapp.klimadao.finance/#/stake)sử dụng để đúc mã thông báo KLIMA, giống như cách DAI được Olympus DAO sử dụng để đúc OHM. Nói cách khác, Klima hoạt động giống như một bể chứa Carbon, cung cấp nguồn vốn thực tế để chống lại biến đổi khí hậu. Bạn có thể tìm thấy thêm thông tin trên [trang web ](https://www.klimadao.finance)và [tài liệu ](https://docs.klimadao.finance)của Klima, đồng thời bạn có thể đến và thảo luận về các cách làm cho tiền điện tử trở nên xanh hơn trên máy chủ Discord của QiDAO.

{% hint style="info" %}
Một trong những điểm khác biệt chính giữa Olympus và Klima là BCT không có giá ổn định. Điều này mang lại rủi ro cao hơn so với các fork sử dụng tiền xu ổn định để xây dựng kho bạc của họ, tuy nhiên, người ta cho rằng các vấn đề môi trường sẽ ngày càng quan trọng hơn và sẽ có ngày càng nhiều dự án cố gắng khai thác carbon từ khí quyển, điều này sẽ làm tăng giá trị tổng thể của BCT.
{% endhint %}

## Chiến lược 1: Tạo đòn bẩy chosKLIMA , or full (9,9)

Nếu không đi sâu vào[ lý thuyết trò chơi (3,3)](https://en.wikipedia.org/wiki/Nash\_equilibrium), (9,9) đại diện cho một tình huống trong đó một người đang tận dụng một vị thế đặt cược. Điều này thực sự có thể thực hiện được vì Klima DAO sẽ cung cấp mã thông báo sKLIMA làm bằng chứng ký quỹ mà một số nền tảng sẽ chấp nhận làm tài sản thế chấp cho một khoản vay khả thi. Hãy cùng xem chi tiết.

### Vòng lặp đòn bẩy sử dụng Klima và MarketXYZ

![Tạo đòn bẩy cho vị thế Klima ](../../.gitbook/assets/Klima-3.png)

Ý tưởng là nhận được một lượng mã thông báo KLIMA ban đầu mà bạn có thể gửi trên Klima DAO. Điều này sẽ cho phép bạn nhận được APY rất cao (kể từ khi viết, APY là 38.873,08%, hoặc 601% APR hoặc mức lợi nhuận hàng ngày là 1,68%) và bằng cách gửi mã thông báo KLIMA của bạn, bạn sẽ nhận được sKLIMA làm bằng chứng gửi tiền.

Mã thông báo sKLIMA này có thể được sử dụng trên Market XYZ trong [Tủ khóa đòn bẩy xanh](https://polygon.market.xyz/pool/5), điều này sẽ cho phép bạn vay theo khoản tiền gửi này.

{% hint style="info" %}
Xin lưu ý thêm, Mai Finance đã hợp tác với Market XYZ và tạo ra quỹ khóa xanh với 1M MAI để đảm bảo lãi suất thấp khi bạn vay MAI đối với sKLIMA của mình.
{% endhint %}

![Tủ khóa màu xanh lá cây trên MarketXYZ tháng 11 năm 2021](../../.gitbook/assets/Klima-Marketxyz.png)

Bạn không có nghĩa vụ phải vay MAI, bạn thực sự có thể vay bất kỳ mã thông báo nào với lãi suất thấp nhất, nhưng bạn cần lưu ý rằng bạn sẽ phải trả phí cho khoản vay của mình và bạn trả khoản vay càng nhanh thì càng ít phí bạn sẽ trả.

Với khoản vay của mình, bạn sẽ có thể mua thêm mã thông báo KLIMA và lặp lại vòng lặp.

Bạn sẽ nhận thấy rằng APY trên sKLIMA sẽ bù đắp phần lớn các khoản lãi cho khoản vay của bạn.

{% hint style="warning" %}
Có một số tiền tối thiểu để vay trên Market.xyz, vui lòng kiểm tra giới hạn khi bạn muốn áp dụng chiến lược này.
{% endhint %}

### Kết quả mong đợi

Thị trường XYZ cũng sẽ có một số mức thanh lý, có nghĩa là nếu giá trị tài sản thế chấp của bạn thấp hơn mức thanh lý, bạn sẽ có nguy cơ mất tài sản thế chấp của mình. Để giảm rủi ro thanh lý, mô phỏng sau giả định rằng bạn sẽ giữ tỷ lệ C / D là 250% và bạn đầu tư 1.000 đô la ban đầu của mã thông báo KLIMA ở mức 38,873% APY để vay MAI với lãi suất 20,49%

| sKLIMA ($) | MAI loan ($) | eq. APY (%) | interests ($) |
| ---------- | ------------ | ----------- | ------------- |
| 1,000.00   | 400.00       | 38,873      | 81.96         |
| 1,500.00   | 560.00       | 54,455      | 114.74        |
| 1,560.00   | 624.00       | 60,642      | 127.86        |
| 1,624.00   | 649.60       | 63,129      | 133.10        |
| 1,649.60   | 659.84       | 64,125      | 135.20        |
| 1,659.84   | 663.94       | 64,523      | 136.04        |
| 1,663.94   | 665.57       | 64,682      | 136.38        |

Tất nhiên, nó có thể đủ để dừng sau 3 vòng vì APY tương đương sẽ không tăng quá nhiều so với thời gian đó.

Lưu ý thêm, vì khoản đầu tư ban đầu là 1.000 đô la, giá trị bạn sẽ nhận được vào cuối 1 năm sẽ là 646.820,00 đô la, giả sử mọi thứ vẫn như cũ. Nói cách khác, bạn đầu tư 1.000 đô la, bạn sẽ cần phải trả lại 665,57 đô la và thêm 136,38 đô la (khoản nợ tích lũy là 801,95 đô la) nhưng bạn cũng sẽ kiếm được 646.820 đô la.

Bạn cũng có thể thấy rằng giá trị của vị thế sKLIMA của bạn đang tăng rất nhanh (khoảng 8% sau mỗi 5 ngày), có nghĩa là bạn cũng có thể tăng khoản nợ của mình tại thời điểm này và tận dụng nhiều hơn nữa để có thêm lợi nhuận.

### Nhận lợi ích và hoàn trả khoản vay của bạn

Một trong những vấn đề chính của các dự án OHM-fork là nó giả định rằng mọi người đều đặt cổ phần và không ai bán. Nhưng, nếu không ai bán, thì không ai nhận được bất kỳ lợi ích nào, và trong hầu hết các trường hợp, người bán đầu tiên sẽ nhận được nhiều lợi ích nhất.

Đối với bất kỳ chiến lược đầu tư nào, điều quan trọng là phải nắm bắt được giá trị thu được của bạn. Bạn có thể làm điều đó bằng cách rút một phần vị trí sKLIMA của mình trên MarketXYZ và nhận lại KLIMA mà bạn có thể bán.

Nếu bạn đầu tư 100 đô la và vận hành 7 vòng  lặp như trên, khoản đầu tư của bạn vào KLIMA sẽ tạo ra 67,11 đô la sau 31 ngày, có nghĩa là bạn có thể hoàn trả đầy đủ khoản vay của mình với lãi suất trong 1 tháng. Nếu bạn làm như vậy, bạn sẽ bắt đầu lại với 166 đô la vào tháng tiếp theo và không còn nợ. Chỉ cần theo dõi lãi suất đi vay có thể khá cao trên Market XYZ.

## Chiến lược 2: Đầu tư liên tục, hoặc toàn bộ (4,4)

Một lần nữa, (4,4) có liên quan đến lý thuyết trò chơi và tiền tệ dự trữ, và những người mua trái phiếu mã thông báo của họ sau đó đặt cổ phần chúng. Trong chiến lược này,  chúng ta có thể sử dụng Klima và Augury để mua trái phiếu và đặt cổ phần liên tục.

### Vòng lặp đầu tư sử dụng Augury và Mai Finance

![Đầu tư liên tục bằng Augury Finance và Mai Finance](../../.gitbook/assets/Klima-4.png)

Chúng ta vẫn đang sử dụng Klima, nhưng lần này chúng ta đang sử dụng nguồn cung cấp từ Augury Finance để tự động hóa việc trích xuất giá trị của Klima. Bằng cách gửi mã thông báo KLIMA của bạn vào [Infusion](https://augury.finance/infusions), thuật toán phụ trách sẽ thực hiện các tác vụ sau sau mỗi lần rebase:

* 50% KLIMA thu hoạch được đặt lại để tăng vị thế sKLIMA của bạn
* 50% KLIMA thu được được bán với USDC được thêm vào bể NFTM trên Augury và được phân phối cho bạn dưới dạng mã thông báo NFTM

![Augury Infusion với 0% phí thực hiện và 0% phí gửi](../../.gitbook/assets/Klima-Augury.png)

NFTM sau đó có thể được giữ lại khi nó tăng giá trị hoặc đổi lấy USDC của nó. Nói cách khác, không quan trọng nếu mã thông báo KLIMA mất giá trị sau khi rebase vì giá trị của nó được ghi lại và lưu trữ dưới dạng NFTM.

Sau khi quy đổi giá trị USDC của phần thưởng NFTM, bạn có thể mua mã thông báo mà mình chọn và cất giữ trong kho của Mai Finance. Ví dụ trên đang sử dụng một vault camWETH, nhưng bạn thực sự có thể sử dụng bất kỳ vault nào bạn thích. Ý tưởng là có thể sử dụng kho tiền trên Mai Finance để vay MAI và mua trái phiếu mới trên Klima DAO để lặp lại vòng lặp. Sau đó, bạn có thể thu hoạch mã thông báo KLIMA và đưa chúng trở lại trong Augury. Hãy nhớ rằng trái phiếu đang cạnh tranh rất ít tại một thời điểm, vì vậy bạn hoàn toàn có thể thu hoạch thường xuyên và đặt vào Augury trước khi trái phiếu của bạn được trao hoàn toàn.

### Kết quả mong đợi

Giả sử bạn đầu tư 100 đô la như trong ví dụ trước và đặt nó trực tiếp vào Infusion trên Augury, APR của  Klima Infusion là 552,94% (giá trị hiện tại khi viết bài) và bạn muốn giữ tỷ lệ C / D trên camWETH vault là 240% và APY là 2,19% trên camWETH vault, đây là kết quả trong một năm:

| day | sKLIMA ($) | wETH ($)  | MAI loan ($) |
| --- | ---------- | --------- | ------------ |
| 30  | 137.751    | 27.708    | 11.545       |
| 60  | 189.776    | 64.883    | 27.035       |
| 90  | 261.474    | 116.150   | 48.396       |
| 120 | 360.282    | 186.835   | 77.848       |
| 150 | 496.453    | 284.283   | 118.451      |
| 180 | 684.115    | 418.613   | 174.422      |
| 210 | 942.737    | 603.771   | 251.571      |
| 240 | 1,299.152  | 858.978   | 357.907      |
| 270 | 1,790.339  | 1,210.720 | 504.466      |
| 300 | 2,467.258  | 1,695.500 | 706.458      |
| 330 | 3,400.140  | 2,363.625 | 984.844      |
| 360 | 4,685.775  | 3,284.424 | 1,368.510    |

Một lần nữa, giả sử rằng tất cả các tỷ giá và giá cả không đổi, vào cuối năm, bạn sẽ có

* $4,684.775 giá trị của mã thông báo KLIMA
* $3,284.424 giá trị của wETH
* và dư nợ của $1,368.510

Đó là một APY tương đương là 6,866,46%. Con số này khác xa so với 38,705,13% được quảng cáo bởi KLIMA, nhưng vẫn khá ấn tượng đối với khoản đầu tư 100 đô la. Ngoài ra, phần lớn lợi nhuận của bạn đã được chuyển đổi thành WETH trong một kho tiền trên Mai Finance và khoản vay của bạn trên ứng dụng này sẽ giúp bạn nhận được một số Token Qi bổ sung.

{% hint style="info" %}
Nếu chiến lược này có APY thấp hơn nhiều so với thuần túy (9,9), thì nó cũng là một chiến lược tương đối hợp lý vì bạn có thể tham gia vòng lặp với bao nhiêu KLIMA bạn muốn.
{% endhint %}

## Tuyên bố từ chối trách nhiệm

Mọi thứ được trình bày trong tài liệu này là lý thuyết thuần túy và được đề xuất cho các mục đích giáo dục. Vấn đề lớn nhất với các dự án như Olympus và Klima là, một lần nữa, người dùng đầu tiên bán sẽ thu được lợi nhuận từ mức giá cao. Nếu lần bán đầu tiên là lớn (vì lợi nhuận thu được là lớn), nó có thể tạo ra hiệu ứng cầu tuyết nhanh chóng thành hiệu ứng hoảng sợ, rất có thể giết chết giá của mã thông báo KlIMA. Tuy nhiên, trong trường hợp này, APY sẽ tăng vọt, có nghĩa là những người dùng không bán hàng sẽ được hưởng lợi từ phần thưởng rất cao, do đó khi APY thu hút người dùng mới, những người nắm giữ sẽ là người chiến thắng lớn.

Cũng cần lưu ý rằng dự án chỉ có thể tiếp tục in mã thông báo miễn là có thêm tiền vào kho bạc.

Vì vậy, rủi ro có thể rất cao nếu bạn không trích xuất một số lợi ích theo thời gian để giảm rủi ro.

Lưu ý cuối cùng, hãy chú ý rằng ohm-fork là xu hướng mới, nhưng hầu hết các dự án có thể thất bại và rất nhiều fork trong số này không phải là những dự án vững chắc. Vì bản chất của chúng, chúng chưa được RugDoc xác minh và có thể rất phức tạp để xác định các ứng dụng thực sự từ lừa đảo thuần túy.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
