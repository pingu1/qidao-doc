---
description: >-
  Hướng dẫn này sẽ trình bày một cách farming một cặp thanh khoản duy nhất với
  sự khác biệt giữa đặt cọc và lãi kép.
---

# Một cách mới để farm cặp ELK-MAI

## Giới thiệu

Cung cấp thanh khoản trên các sàn DEX (Sàn giao dịch phi tập trung) và canh tác lợi nhuận là những cách phổ biến nhất đến kiếm lợi nhuận trong DeFi. Tuy nhiên, nhiều người dùng chỉ chú ý đến tỷ lệ của bể thanh khoản mà không thực sự biết đó là APR(Lãi suất phần trăm hàng năm) hay APY(Lãi suất cộng dồn hàng năm). Có nhiều cách để canh tác lợi nhuận một bể thanh khoản và quản lý mã thông báo phần thưởng. Trong hướng dẫn này, chúng tôi xin giới thiệu một cách mới nhất để canh tác lợi nhuận bể ELK-MAI và tận dụng mã thông báo phần thưởng ELK trên Harmony.

{% hint style="info" %}
Hướng dẫn này chắc chắn không phải là lời khuyên tài chính, nó được thực hiện với mục tiêu giáo dục. Bạn cần chú ý đến sự thay đổi giá cả, cung và cầu, chương trình thưởng, ngày kết thúc, khoản lỗ tạm thời, v.v. và chỉ đầu tư những gì bạn sẵn sàng để có thể mất.
{% endhint %}

![](../../.gitbook/assets/elk-farming-1.png)

## Elk Finance

[Elk Finance](https://app.elk.finance/#/) là một bản sao chép của Uniswap V2 cũng như một nhà tạo lập thị trường tự động (AMM). Bạn có thể tìm thấy những tính năng thông thường như với các bản sao chép Uniswap khác như hoán đổi tài sản, kết hợp các cặp tài sản khác nhau, canh tác lợi suất và đặt cọc mã thông báo phần thưởng ELK.

Điều làm cho Elk Finance trở thành một dự án hoàn toàn khác là sự hiện diện của nó trên nhiều blockchain và không chỉ các chuỗi tương thích EVM (Máy ảo Ethereum). Elk Finance hiện có mặt trên 16 chuỗi và họ có kế hoạch mở rộng sang nhiều chuỗi khác. Họ đã quản lý để xây dựng một cầu nối giữa tất cả các chuỗi đó để cho phép người dùng chuyển mã thông báo ELK chính là ELKNET.

![Kết nối ELK từ Harmony sang Moonriver bằng ElkNet](../../.gitbook/assets/elk-farming-2.png)

Ngoài ra, một tính năng thú vị do ElkNet đề xuất là khả năng hoán đổi một phần tài sản được chuyển thành mã thông báo phí gas tại chuỗi khối đích. Điều này đặc biệt hữu ích nếu bạn lần đầu tiên sử dụng chuỗi khối mà không có sẵn faucets.

{% hint style="success" %}
Ngoại trừ các chuỗi có gas cao (chỉ có Avalanche và Cronos tại thời điểm viết bài), việc sử dụng ElkNet để kết nối các mã thông báo ELK của bạn từ chuỗi này sang chuỗi khác được thực hiện miễn phí. Bạn không nghe sai đâu, bạn không phải trả bất kỳ khoản phí kết nối nào cả!
{% endhint %}

Cuối cùng, Elk Finance cung cấp tính năng bảo vệ Tổn thất tạm thời. Bạn có thể đọc tất cả thông tin chi tiết về chương trình Tổn thất tạm thời trong [tài liệu chính thức ](https://docs.elk.finance/features/impermanent-loss-protection)của họ, nhưng về cơ bản, tất cả những gì bạn cần biết là nếu giá ELK thay đổi giữa thời điểm bạn gửi tiền và thời điểm bạn rút tiền, bạn sẽ được trả thêm ELK nhằm trang trải mất mát tạm thời. Vì MAI được chốt bằng 1 USD, khoản lỗ tạm thời chỉ liên quan đến biến động giá của ELK.

## Canh tác lợi suất cặp MAI-ELK

Elk Finance đã hợp tác với Mai Finance vào tháng 1 năm 2022 để đề xuất canh tác lợi suất bằng cách sử dụng cặp MAI-ELK LP trên DEX của họ. Hiện tại, cặp MAI-ELK có thể được sử dụng trên 3 chuỗi khối khác nhau: Harmony, Moonriver và Gnosis. Một số bể bổ sung có thể được khởi chạy sau này trên Polygon, Cronos và Fantom. Hãy xem các chiến lược khác nhau mà bạn có thể áp dụng cho bể mới này.

{% hint style="info" %}
Chúng tôi đang đề xuất hướng dẫn này cho Harmony vì phí gas rất rẻ, cho phép bạn cộng dồn phần thưởng của mình theo cách thủ công hàng ngày. Điều này làm cho nó trở thành một chuỗi khối rất tốt cho những người mới bắt đầu chỉ có một vài đô la để đầu tư dưới dạng trải nghiệm. Tuy nhiên, mọi thứ được trình bày trong hướng dẫn này cũng có thể được áp dụng cho bất kỳ chuỗi nào khác.
{% endhint %}

### Canh tác lợi suất và đặt cọc

Chiến lược đầu tiên khác đơn giản và trực diện:

* kết hợp cặp thanh khoản của bạn
* gửi cặp thông báo Elk-MAI vào bể để nhận 200% APR
* thu hoạch phần thưởng hàng ngày
* gửi chúng để nhận phần thưởng 32.53% APR

Nếu bạn khởi đầu với 100 đô la, đây là kết quả bạn có thể nhận được hàng tháng cho một năm hoàn chỉnh, giả sử tỷ lệ được đưa ra ở trên vẫn giữ nguyên trong toàn bộ thời gian.

| ngày | MAI-ELK ($) |  ELK đã gửi ($) |
| ---- | ----------- | --------------- |
| 30   | 100.000     | 16.653          |
| 60   | 100.000     | 33.756          |
| 90   | 100.000     | 51.323          |
| 120  | 100.000     | 69.366          |
| 150  | 100.000     | 87.897          |
| 180  | 100.000     | 106.930         |
| 210  | 100.000     | 126.479         |
| 240  | 100.000     | 146.557         |
| 270  | 100.000     | 167.180         |
| 300  | 100.000     | 188.360         |
| 330  | 100.000     | 210.115         |
| 360  | 100.000     | 232.458         |

Vào cuối năm, bạn sẽ có

* $100.00 MAI-ELK LP
* $236.24 ELK đã gửi

Tương ứng với APY là 236,24%. Đó chính xác không phải là APR c vì một phần của phần thưởng được cộng dồn (ELK gửi).

{% hint style="info" %}
Bạn có thể tìm thấy tất cả các kết quả và công thức được sử dụng để tạo bảng này trong [Google Trang](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit#gid=0) tính sau trong tab đầu tiên. Bạn có thể sao chép tệp này vào ổ đĩa của riêng mình và điều chỉnh tỷ giá cũng như khoản đầu tư ban đầu để xem APY tổng thể thay đổi theo số bạn nhập.
{% endhint %}

### Canh tác lợi suất và cộng dồn trực tiếp

Cộng dồn có nghĩa là bạn thu thập phần thưởng của mình và sử dụng nó để tạo thêm mã thông báo LP. Trong trường hợp này, bạn sẽ:

* thu thập phần thưởng ELK
* hoán 50% thành MAI
* kết hợp thành cặp ELK-MAI bổ sung thêm
* gửi vào bể

Nếu bạn khởi đầu với cùng một khoản đầu tư là 100 đô la, thì kết quả bạn có thể mong đợi cho một năm canh tác lợi suất hoàn chỉnh, giả sử tỷ lệ đưa ra vẫn giữ nguyên trong toàn bộ thời gian canh tác, như sau:

| ngày | MAI-ELK ($) |
| ---- | ----------- |
| 30   | 117.172     |
| 60   | 138.044     |
| 90   | 162.635     |
| 120  | 191.607     |
| 150  | 225.739     |
| 180  | 265.952     |
| 210  | 313.328     |
| 240  | 369.143     |
| 270  | 434.901     |
| 300  | 512.374     |
| 330  | 603.647     |
| 360  | 711.179     |

Tại thời điểm cuối năm bạn sẽ có

* $730.878 trị giá mã thông báo MAI-ELK LP trong bể

Tương ứng với khoản đầu tư ban đầu là 100 đô la, với APY tổng thể là 630,88%. Vì chúng tôi đang cộng gộp phần thưởng, đây là APY chính xác mà bạn sẽ nhận được từ APR là 200%.

Xin lưu ý thêm, các công thức để tính APY từ APR với lãi kép hàng ngày (hoặc APR từ APY) như sau:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

$$
APR = N * (( 1 + APY)^\frac{1}{N} - 1)
$$

Với N là số lần bạn gộp phần thưởng của mình. Trong trường hợp của chúng tôi, công thức 2 sẽ cung cấp cho chúng tôi

$$
APY = ( 1 + \frac{2}{365})^{365}-1 = 634.88\%
$$

$$
APR = 365 * (( 1 + 6.3488)^\frac{1}{365} - 1) = 199.99\%
$$

Dễ thấy rằng nếu bạn áp dụng APR là 200% (APR của bể LP) cho phần thưởng của mình, bạn sẽ nhận được lợi suất tốt hơn so với nếu bạn áp dụng APR là 32,53% (đặt cược APR). Theo nghĩa đó, tính lãi kép tốt hơn so với đặt cược trong khi APR canh tác lợi suất vẫn cao hơn APR đặt cược. Điều này rõ ràng có thể thay đổi theo số lượng thanh khoản trong bể.

{% hint style="info" %}
Đối với phần trước, bạn có thể tìm thấy mô phỏng trong cùng [Bảng tính Google](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit#gid=0) trong tab thứ hai.
{% endhint %}

### Canh tác lợi suất và cộng dồn với Mai Finance

Nếu đặt cược và lãi kép đang mang lại lợi nhuận tốt, cả hai phương pháp đều được liên kết trực tiếp với giá của mã thông báo ELK, vì vậy giá trị khoản đầu tư của bạn sẽ thay đổi theo giá của ELK. Chúng tôi đã thấy rằng lãi kép cung cấp các tùy chọn tốt hơn so với đặt cược. Bây giờ chúng ta sẽ xem cách bạn có thể thu được một số giá trị từ phần thưởng canh tác của mình và tiếp tục đầu tư vào cùng một bể bằng cách sử dụng Mai Finance. Các thao tác hàng ngày sẽ như sau:

* Thu hoạch phần thưởng ELK
* Bán 66% phần thưởng để mua một số mã thông báo blue chip được chấp nhận làm tài sản thế chấp trên Mai Finance. Đối với ví dụ của chúng tôi, chúng tôi sẽ sử dụng ONE mã thông báo ở đây
* Gửi mã thông báo ONE vào kho tiền trên Mai Finance
* Vay thêm MAI với 200% CDR (Tỷ lệ thế chấp trên Nợ), giá trị này sẽ tương ứng với các mã thông báo ELK còn lại của bạn
* kết hợp thêm mã thông báo MAI-ELK
* gửi vào bể

{% hint style="info" %}
Chuyển đổi mã thông báo phần thưởng của bạn thành ONE không phải là cách an toàn nhất để bảo vệ tài sản của bạn, một trong những cách tốt nhất để làm điều đó là chuyển đổi sang các đồng ổn định. Tuy nhiên, các tùy chọn về Mai Finance trên Harmony khi viết bài này là khá hạn chế. Bạn có thể nhận được các lựa chọn tốt hơn trong tương lai (sau tháng 1 năm 2021), chẳng hạn như đặt cọc Stake DAO LP làm tài sản thế chấp (xem [bài viết dành riêng](../polygon/the-elephant-and-the-otter.md) của chúng tôi cho Polygon để biết cách bạn có thể sử dụng mã Stake DAO trên Mai Finance).
{% endhint %}

Nếu bạn bắt đầu với cùng một khoản đầu tư ban đầu là 100 đô la, kết quả bạn có thể mong đợi cho một năm canh tác lợi suất hoàn chỉnh, giả sử tỷ lệ đưa ra vẫn giữ nguyên trong toàn bộ thời gian này và kho tiền của bạn không bị thanh lý là như sau:

| ngày | MAI-ELK ($) | ONE ($) | Mai debt ($) |
| ---- | ----------- | ------- | ------------ |
| 30   | 111.154     | 11.560  | 5.780        |
| 60   | 124.003     | 24.456  | 12.228       |
| 90   | 138.337     | 38.842  | 19.421       |
| 120  | 154.328     | 54.892  | 27.446       |
| 150  | 172.168     | 72.797  | 36.398       |
| 180  | 192.070     | 92.772  | 46.386       |
| 210  | 214.273     | 115.055 | 57.528       |
| 240  | 239.042     | 139.915 | 69.958       |
| 270  | 266.674     | 167.648 | 83.824       |
| 300  | 297.501     | 198.588 | 99.294       |
| 330  | 331.891     | 233.106 | 116.552      |
| 360  | 370.257     | 271.609 | 135.805      |

Vào cuối năm bạn sẽ có:

* $377.069 trị giá mã thông báo MAI-ELK LP trong bể
* $278.446 giá trị của mã thông báo ONE trong ONE vault của bạn
* $139.223 giá trị của món nợ
* tỷ lệ CDR là 200%, như dự định

Bắt đầu từ vị trí ban đầu với MAI-ELK trị giá 100 đô la, điều này tương ứng với APY tổng thể là 416,29%. Ở đây, chúng tôi nhận được ít lợi nhuận hơn một chút so với lãi kép thuần túy, tuy nhiên chúng tôi cũng trích một phần lợi nhuận tốt thành ONE, có thể ít biến động hơn ELK, do đó có thể ít rủi ro hơn.

{% hint style="info" %}
Một lần nữa, mô phỏng có thể được tìm thấy trong cùng một [Bảng tính Google](https://docs.google.com/spreadsheets/d/1Vva5dhjYix0g4bMZRSAMIutDgbT08TsTLhVJE0TUrF8/edit#gid=0) trong tab thứ ba.
{% endhint %}

Ngoài ra, bạn cũng có thể bán tất cả phần thưởng ELK của mình cho các mã thông báo được chấp nhận trên Mai Finance, vay thêm MAI và bán một phần của nó để mua thêm ELK nhằm tăng vị thế của bạn trong bể MAI-ELK. Bằng cách đó, bạn sử dụng ONE nhiều hơn, nhưng cũng đồng thời tăng nợ của bạn. Bạn sẽ nhận được MAI-ELK trị giá 270,715 đô la, ONE trị giá 352,913 đô la và khoản nợ trị giá 171,457 đô la cho APY tổng thể là 342,17%.

## Ảnh hưởng của tần suất cộng dồn

Cho dù bạn quyết định đặt cọc hay cộng dồn phần thưởng của mình, điều quan trọng là phải hiểu rằng phần thưởng của bạn sẽ thay đổi tùy thuộc vào tần suất bạn thực hiện quy trình thu hoạch + tái đầu tư của mình. Xin nhắc lại, công thức tính APY và APR như sau:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Trong phương trình này, N đại diện cho số lần bạn gộp phần thưởng của mình trong một năm. Vì vậy, và APR là 200% như trên sẽ cung cấp cho bạn APY sau tùy thuộc vào tần suất bạn cộng dồn:

| Tần suất cộng dồn | APY tương ứng |
| ----------------- | ------------- |
| hàng ngày         | 634.88 %      |
| 2 lần mỗi tuần    | 625.01 %      |
| hàng tuần         | 611.71 %      |
| 2 lần mỗi tháng   | 609.55 %      |
| hàng tháng        | 535.86 %      |
| hàng quý          | 406.25 %      |
| 2 lần mỗi năm     | 300.00 %      |

Thực hiện cộng dồn theo cách thủ công nhiều hơn một lần một ngày có thể tốn kém tùy thuộc vào chuỗi khối bạn đang hoạt động. Nhưng về cơ bản, rõ ràng là bạn càng cồng dồn thường xuyên thì phần thưởng càng tốt. Điều này cũng giải thích lý do tại sao trình tối ưu hóa lợi suất / trình cộng dồn tự động lại phổ biến. Hãy nhớ rằng bằng cách tính lãi kép, bạn tăng thêm áp lực bán vào mã thông báo bạn sử dụng để canh tác lợi suất, điều này sẽ có tác động tiêu cực đến giá của mã thông báo đó. Nếu đó cũng là mã thông báo bạn đang sử dụng để canh tác lợi suất (trong ELK ví dụ của chúng tôi), bạn có thể bị ảnh hưởng bởi tổn thất tạm thời, trừ khi bạn đang sử dụng Elk Finance DEX, bảo vệ bạn khỏi tổn thất tạm thời.

## Chọn đúng bể&#x20;

Cặp MAI-ELK đã được triển khai cho một số chuỗi, vì vậy bạn có thể triển khai trên chuỗi có tỷ giá tốt nhất.

![Bể MAI-ELK trên Gnosis (trên), Moonriver (giữa) và Harmony (dưới) tại thời điểm tháng 1 năm 2021](../../.gitbook/assets/elk-farming-3.png)

{% hint style="info" %}
Bể MAI-ELK cũng có thể được triển khai cho các chuỗi khác trong tương lai gần, có thể trên Polygon, Cronos và Fantom. Điều này không được đảm bảo và không có ETA cho điều đó, vì vậy hãy cập nhật bằng cách kiểm tra các máy chủ Discord khác nhau của cả hai dự án, theo dõi chúng trên twitter.
{% endhint %}

Bên cạnh tỷ lệ phần thưởng trên mỗi chuỗi, bạn cũng có thể phải xem xét giá của mã thông báo ELK trên mỗi chuỗi. Nếu giá gần như giống nhau trên tất cả các chuỗi, thì sự khác biệt nhỏ cũng có thể là một yếu tố để bạn chọn chuỗi nơi bạn muốn canh tác lợi suất mã thông báo ELK.

![Giá của mã thông báo ELK trên tất cả các chuỗi](../../.gitbook/assets/elk-farming-4.png)

Như bạn có thể thấy, bể MAI-ELK trên Moonriver mang lại tỷ lệ phần thưởng tốt hơn và mã thông báo ELK cũng có giá cao hơn trên chuỗi đó. Điều này có nghĩa là, tại thời điểm viết bài, có thể tốt hơn nếu canh tác lợi suất bể MAI-ELK trên Moonriver hơn là trên Harmony hoặc Gnosis, đặc biệt nếu bạn định bán một phần của các mã thông báo được nuôi. Lưu ý rằng điều này có thể không đúng mọi lúc, vì vậy hãy đảm bảo rằng bạn chọn chuỗi của mình đúng cách và bạn tự nghiên cứu trước khi tham gia nhóm LP. Cuối cùng, chúng tôi khuyên bạn nên đọc tài liệu về [bảo vệ IL](https://docs.elk.finance/features/impermanent-loss-protection) vì bảo hiểm phụ thuộc nhiều vào số ngày mã thông báo LP của bạn được gửi vào bể.

Một lưu ý nhỏ, vì ELK bắc cầu là miễn phí, bạn có thể chuyển từ chuỗi này sang chuỗi khác để luôn được hưởng lợi từ tỷ lệ tốt nhất. Đảm bảo rằng bạn hiểu rằng bạn cũng sẽ ảnh hưởng đến tỷ lệ phần thưởng của bể bạn thoát và bể bạn tham gia (ít thanh khoản hơn sẽ làm tăng APR, thanh khoản nhiều hơn sẽ làm giảm nó).

## Tuyên bố từ chối trách nhiệm

Hướng dẫn này đã được viết để minh họa các cách khác nhau để tạo ra lợi nhuận bằng cách sử dụng thanh khoản mã thông báo được cung cấp. Bạn sẽ ảnh hưởng rất nhiều đến lợi nhuận của mình với chiến lược mà bạn chọn, cũng như mức độ rủi ro. Tất nhiên, tất cả các khái niệm được chỉ ra trong tài liệu này cũng có thể áp dụng cho bất kỳ cặp LP nào và bạn rất nên thử nghiệm của riêng mình trước khi chọn chiến lược, cặp LP, bể hoặc thậm chí là DEX.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
