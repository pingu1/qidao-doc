---
description: >-
  Hướng dẫn này đề xuất phân tích đầy đủ về các lựa chọn sử dụng đòn bẩy khác
  nhau trên chuỗi khối Fantom bằng cách sử dụng các hầm tiền trên Yearn và
  Beefy.
---

# Chiến lược tạo đòn bẩy trên Fantom

## Giới thiệu

Mai Finance đã ra mắt nền tảng cho vay của mình trên Fantom với nhiều loại hầm tiền khác nhau cho phép đúc đồng ổn định MAI bằng tài sản mã hóa được dùng làm thế chấp trong kho tiền. Ý tưởng là bạn vẫn có thể giữ tài sản mã hóa của bạn để hưởng lợi từ việc tăng giá trong khi vẫn có thể mua những tài sản khác hoặc canh tác lợi nhuận. Bạn có thể mua thêm tài sản mã hóa để tiếp tục gửi vào kho tiền nhằm tạo đòn bẩy tối đa cho khoản đầu tư của bạn. Trong hướng dẫn này chúng tôi sẽ sử dụng 2 nền tảng cho vay khác nhau để tạo đòn bẩy cho DAI của bạn.

## Tạo đòn bằng token từ Yearn Finance

### Gửi tài sản trên Yearn Finance

[Yearn Finance](https://beta.yearn.finance/#/home) là một nhóm giao thức chạy trên mạng Ethereum và một số mạng khác cho phép người dùng tối đa hóa tài sản mã hóa thông qua hoạt động cho vay và giao dịch. Tại hướng dẫn này, chúng tôi sẽ gửi mã token đơn lẻ vào các hầm tiền trên Yearn để nhận lại yvToken như là bằng chứng cho việc gửi tiền. Tại trường hợp này, chúng ta sẽ nhận lại yvDAI khi ký gửi DAI

<img src="../../.gitbook/assets/ftm-leverage-yv1.png" alt="yearn vaults on Fantom network" data-size="original">

{% hint style="info" %}
Trang web của Yearn hiện tại đang trong giai đoạn thử nghiệm trên chuỗi khối Fantom nên chỉ số APR/APY không được hiển thị trên giao diện. Tuy nhiên, bạn có thể thấy APR của DAI trên tab Iron Bank là 8%. Hãy luôn nghiên cứu trước khi đầu tư.
{% endhint %}

### Gửi yvToken vào Mai Finance

Khi bạn đã gửi DAI của mình vào Yearn Finance, bạn sẽ có yvDAI trong ví của mình. Đây là những gì chúng tôi gọi là mã thông báo mang lại lợi nhuận: đó là mã thông báo không có bất kỳ giá trị nào, nhưng đại diện cho phần của bạn trong bể cụ thể nơi tài sản của bạn đang kiếm được lợi nhuận và trong đó phần thưởng được tự động cộng lại. Nói cách khác, nếu DAI của bạn không thay đổi giá trị vì DAI được gắn với đô la Mỹ, thì giá trị cơ bản của mã thông báo yvDAI của bạn vẫn tăng.

Mai Finance chấp nhận rất nhiều mã thông báo lợi nhuận đến từ các hầm tiền của Yearn như một loại thế chấp để có thể vay MAI từ đó.&#x20;

<img src="../../.gitbook/assets/ftm-leverage-yv2 (1).png" alt="Deposit your yvToken on Mai Finance" data-size="original">

Hiện tại kho tiền yvDAI có ngưỡng thanh lý là 110%, điều này có nghĩa là bạn có thể vay MAI để tỷ lệ giữa giá trị tài sản thế chấp của bạn và giá trị nợ là 110%. Hãy cẩn thận rằng 110% thực sự là tỷ lệ mà kho tiền của bạn sẽ được thanh lý. Bạn cần giữ tỷ lệ trên ngưỡng tối thiểu này. Vì DAI không thay đổi nhiều về giá (lên hoặc xuống dưới vài xu) nên có thể giữ CDR (Tỷ lệ tài sản đảm bảo trên nợ) "an toàn" là 115%, nhưng hãy thoải mái giữ mức cao hơn nếu bạn muốn.

Như thường lệ, để tính toán giá trị khoản vay mà chúng ta có thể nhận được dựa trên giá trị tài sản thế chấp và CDR mục tiêu chúng ta sẽ sử dụng công thức sau:



$$
MAI_{Khả.dụng} = \frac{Giá.trị_{Thế.chấp} - Giá.trị_{Nợ} * CDR_{Mục.tiêu}}{CDR_{Mục.tiêu}}
$$

​Với giá trị tài sản thế chấp là 100 đô la và không có nợ, nếu chúng ta muốn giữ CDR hợp lý là 115%, chúng ta có thể vay tối đa

$$
MAI_{khả.dụng}=\frac{100-0*1.15}{1.15}=86.95
$$

​Trong khi số DAI trên Yearn vẫn đang sinh lời, chúng ta có thể swap số MAI sang DAI và tiếp tục vòng lặp.

### Hoán đổi MAI trên BeethovenX

Trên mạng Fantom [BeethovenX](https://app.beets.fi/#/trade) là nguồn thanh khoản chính của MAI. Tại đây bạn có thể hoán đổi số MAI sang DAI với tỷ lệ trượt giá thấp.

![Hoán đổi MAi sang DAI](../../.gitbook/assets/ftm-leverage-yv3.png)

Đây là bước cuối cùng của vòng lặp để có nhiều DAI hơn, bạn có thể gửi chúng vào kho tiền của Yearn và lặp lại vòng lặp. Làm như vậy sẽ tăng số lượng tài sản bạn có trong kho tiền của Yearn nhiều hơn, vì vậy bạn kiếm được nhiều lợi nhuận hơn và nếu bạn so sánh với khoản đầu tư ban đầu, thì APR của bạn sẽ tăng lên. Nếu bạn muốn có thêm ví dụ về APR bạn có thể đạt được bằng cách sử dụng vòng lặp yvDAI, vui lòng đọc hướng dẫn camDAI trên mạng Polygon sử dụng cùng một chiến lược nhưng các công cụ khác nhau.

{% hint style="success" %}
BeethovenX thực sự là một cơ hội tuyệt vời để canh tác với MAI, chỉ cần gửi MAI của bạn vào bể MAI-DAI-USDC (APR \~ 30% tính đến tháng 11 năm 2021) nếu bạn không thể đạt được APR tốt hơn bằng cách sử dụng các vòng đòn bẩy.
{% endhint %}

$$
MAI_
$$

## Tạo đòn bẩy với mooScreamTokens trên Mai Finance

### Gửi tài sản của bạn trên Beefy Finance

[Beefy Finance](https://app.beefy.finance/#/fantom) là một nền tảng  tối ưu hóa lợi nhuận đa chuỗi, phi tập trung cho phép người dùng kiếm được lãi kép từ việc nắm giữ tiền điện tử của họ. Nói cách khác, bạn có thể ký gửi một số tài sản hoặc mã thông báo LP từ các nền tảng khác trên Beefy Finance và để Beefy tự động cộng dồn mã thông báo trang trại và kết hợp chúng thành nhiều tài sản ký gửi / mã thông báo LP của bạn. Đối với hướng dẫn này chúng ta sẽ sử dụng các khoản tiền gửi DAI duy nhất trên Beefy và sử dụng Scream làm nền tảng farming. Scream là một nền tảng cho vay trên mạng Fantom mà trên đó bạn có thể cho mượn tài sản của mình và thu thập mã thông báo SCREAM. Beefy sau đó sẽ bán mã thông báo SCREAM để có thêm DAI

Để gửi DAI chúng ta sẽ truy cập ứng dụng Beefy Finance và chọn Scream làm nền tảng mà chúng tôi sẽ thu được lợi nhuận.&#x20;

![Gửi DAI trên Beefy bằng Scream](../../.gitbook/assets/ftm-leverage-beefy1.png)

Như bạn có thể thấy, Beefy đã mang lại một APY không thể tin được cho các khoản tiền gửi  DAI. Khi bạn đã gửi DAI của mình trên Beefy, bạn được cung cấp bằng chứng gửi tiền trong ví của mình dưới dạng mã thông báo mooScreamDAI. Đối với mã thông báo yvDAI, mã thông báo mooScreamDAI là một khoản tiền gửi mang lại lợi nhuận, có nghĩa là tài sản của bạn vẫn được sử dụng trên Scream và được kết hợp trên Beefy, kiếm được lợi nhuận. Nhưng bạn sẽ có thể sử dụng mã thông báo này trên Mai Finance để vay MAI.

### Gửi mooScreamToken trên Mai Finance

Sau khi bạn gửi DAI của mình trên tài chính Beefy, bạn sẽ có mooScreamDAI trong ví của mình. Bạn có thể sử dụng các bước tương tự như đối với chiến lược Yearn Vault ở trên, điểm khác biệt duy nhất là tỷ lệ thanh lý của mooScreamDAI là 135%. Vì DAI là một đồng tiền ổn định, nên vẫn có thể vay MAI và giữ một CDR rất gần với tỷ lệ thanh lý. Đối với ví dụ này chúng ta sẽ nhắm đến CDR 140% và với công thức tương tự như trên, chúng ta có thể tính số lượng MAI mà chúng tôi có thể đúc với DAI trị giá 100 đô la.

$$
MAI_{available}=\frac{100-0*1.4}{1.4}=71.43
$$

​Vì chúng ta vay ít hơn, chúng ta sẽ có thể thực hiện ít vòng lặp hơn và APY tương đương cuối cùng cũng sẽ thấp hơn, tuy nhiên đây vẫn là một chiến lược khá tốt cho người mới bắt đầu.&#x20;

Phần còn lại của vòng lặp tương tự như đối với yvDAI, có nghĩa là bạn sẽ phải hoán đổi MAI của mình cho DAI trên BeethovenX và lặp lại cho đến khi bạn hài lòng.

## Một số chú ý cho chiến lược dùng đòn bẩy  trên Fantom

Tạo đòn bẩy cho DAI được coi là một chiến lược khá an toàn  dành cho người mới bắt đầu và bạn có thể nhận được một số lợi suất tốt bằng cách sử dụng nhiều nhất 3 giao thức. Tuy nhiên, vẫn có một số _rủi ro_ cần lưu ý.&#x20;



### Rủi ro thanh lý&#x20;

Bạn càng thực hiện nhiều vòng, rủi ro thanh lý càng cao. Thật vậy, ngay cả một sự thay đổi nhỏ của giá DAI cũng sẽ được tăng lên bởi đòn bẩy bạn đã áp dụng và ngay cả khi bạn giữ CDR cao hơn 5 điểm so với tỷ lệ thanh lý, kho tiền của bạn có thể gặp rủi ro. Bạn nên dừng các vòng lặp đòn bẩy ở bước mà bạn gửi tài sản của mình vào tài chính MAI và không vay thêm MAI để giữ CDR tốt hơn.&#x20;

Ngoài ra, trong trường hợp thanh lý, vì kho tiền của bạn trên tài chính MAI chứa nhiều tài sản hơn, nên việc thanh lý cũng sẽ có tác động lớn hơn so với việc bạn không cho mượn vị trí của mình, đơn giản vì khoản nợ bạn phải trả cũng lớn hơn nhiều. ..

### Rủi ro kỹ thuật

Nếu bạn sử dụng nhiều giao thức cho hợp đồng đầu tư của mình, bạn cần đảm bảo rằng các giao thức này an toàn.  Trong chiến lược đòn bẩy của chúng ta, nếu một giao thức duy nhất bị tấn công, toàn bộ chiến lược có thể sụp đổ. Đảm bảo rằng bạn đã thẩm định trước khi đầu tư vào các dự án DeFi.

### Chạm mức nợ trần

Bởi vì những chiến lược này dễ thiết lập và ít rủi ro, nên có nhu cầu sử dụng rất cao. Tuy nhiên, bạn chắc chắn nhận thấy rằng trong quá trình đòn bẩy, MAI mượn được đổi lấy DAI (hoặc các mã thông báo khác). Nếu quá nhiều MAI được bán trên Beethoven, giá của nó sẽ giảm từ từ và có nguy cơ MAI mất chốt, điều này khá tệ đối với một đồng tiền ổn định. Để có thời gian bình ổn giá, Tài chính Mai có cơ chế bảo đảm, trong đó quan trọng nhất là trần nợ cho từng kho tiền.

Mức trần nợ đại diện cho số lượng MAI tối đa có thể được đúc cho một kho tiền nhất định. Khi đã đạt đến mức trần, không thể mượn MAI nữa. Sau đó, nhóm cốt lõi phụ trách tài chính của MAI có thể quyết định tăng trần hoặc đợi thêm một chút để MAI có thể điều chỉnh về mức giá tốt hơn.

Bạn luôn có thể xác minh số lượng MAI có thể được đúc trên trang tạo vault, nhưng bạn thường sẽ nhận thấy rằng không còn MAI nữa nếu bạn nhận được thông báo lỗi sau:

![Tin nhắn báo lỗi khi chạm nợ trần](../../.gitbook/assets/ftm-leverage-error.png)

Trong hầu hết các trường hợp, chờ đợi tăng trần là giải pháp duy nhất. Hãy theo dõi twitter hoặc Discord để biết khi nào điều này xảy ra.

## Tuyên bố từ chối trách nhiệm

Hướng dẫn này đã trình bày một số cách bạn có thể sử dụng tài sản của mình trên Fantom và đưa Mai Finance vào chiến lược nhằm tăng lợi nhuận của bạn. Tuy nhiên, như thường lệ, hướng dẫn này không phải là một lời khuyên tài chính và bạn phải luôn nghiên cứu kỹ lưỡng trước khi áp dụng chiến lược đầu tư và đầu tư một cách có trách nhiệm.

Cũng nên nhớ rằng chiến lược này có thể không phải là chiến lược tốt nhất tùy thuộc vào thời điểm bạn định sử dụng. Chúng tôi vừa nhấn mạnh rằng BeethovenX cũng có APR khá thú vị cho MAI của bạn và bạn cũng có thể sử dụng Beefy Finance để gộp phần thưởng BEETS thành các đồng tiền ổn định hơn.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
