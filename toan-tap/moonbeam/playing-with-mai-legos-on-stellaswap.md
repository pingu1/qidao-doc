---
description: Sử dụng MAI trên Moonbeam để kiếm lợi nhuận với StellaSwap.
---

# Chơi với MAI lego trên StellaSwap

Mặc dù Mai Finance không cung cấp các kho tiền trên Moonbeam, bạn có thể sử dụng một số mã thông báo yêu thích của mình trên chuỗi để đúc MAI bằng cách sử dụng các hầm MAI mới của StellaSwap. Bằng cách tận dụng các mã thông báo thế chấp của bạn và vay MAI để chống lại nó, bạn có thể kiếm được lợi nhuận lớn thông qua chiến lược lặp liên quan đến xSTELLA và MAI.

_LƯU Ý: Hướng dẫn này không có nghĩa là lời khuyên tài chính. Nó được tạo ra với mục tiêu giáo dục. Mục tiêu của hướng dẫn này không phải là đề xuất một chiến lược để tuân theo một cách mù quáng, vì vậy hãy làm bài tập về nhà và mô phỏng của riêng bạn, và chỉ đầu tư những gì bạn sẵn sàng có thể mất._

[StellaSwap](https://stellaswap.com/) là DEX (sàn giao dịch phi tập trung) hàng đầu trên Moonbeam. Là một DEX đầy đủ tính năng, StellaSwap cung cấp cho người dùng khả năng hoán đổi mã thông báo, kiếm lợi nhuận trên các trang trại và tham gia vào quản trị giao thức. Điều làm cho StellaSwap trở nên khác biệt, đó là nó là giao thức đầu tiên cho phép người dùng khai thác MAI nguyên bản trực tiếp từ giao diện của nó thông qua quan hệ đối tác với Mai Finance.

![Đúc MAI trực tiếp trên StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 4.41.56 PM.png>)

### Đúc MAI trên StellaSwap

Không giống như các kho tiền MAI trên Mai Finance, các kho tiền MAI của StellaSwap tính lãi khi vay đối với tài sản của bạn. Hiện tại, người dùng có thể vay MAI đối với xStella, mã thông báo chia sẻ doanh thu của StellaSwap, với lãi suất 12% hoặc đối với wGLMR, một phiên bản được  bọc của mã thông báo gas gốc của Moonbeam, với lãi suất 8%. Mặc dù những người dùng quen thuộc với các khoản lãi suất 0% của Mai Finance có thể bị ngạc nhiên bởi lãi suất cao hơn, nhưng chúng tôi sẽ xem xét một chiến lược lặp lại trong hướng dẫn này để cho phép bạn kiếm được lợi suất cao trên các stablecoin đã vay của mình mà không cần rời khỏi StellaSwap.

![Vaults trên StellSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

1. Đầu tiên, hãy đến [giao diện đúc tiền MAI của StellaSwap.](https://app.stellaswap.com/mai)
2. Từ đây, bạn sẽ có thể tạo một kho tiền xStella hoặc wGLMR để vay MAI. Để tạo chiến lược lặp của chúng tôi, chúng tôi sẽ tạo một xStella vault.
3. Bây giờ hãy vào vault mới tạo của bạn và gửi xStella. Xin lưu ý rằng xStella vault có 40% LTV (tỷ lệ cho vay trên giá trị), có nghĩa là cứ mỗi xStella trị giá 100 đô la, bạn sẽ có thể vay MAI trị giá 40 đô la.
4. Tiếp theo, bạn sẽ muốn chuyển đến phần vay và vay MAI. Hãy lưu ý LTV của bạn để tránh bị thanh lý.

![xStella vault](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.05.01 PM.png>)

### Kết hợp các Legos lại với nhau

Bây giờ bạn đã vay MAI thành công, đã đến lúc đưa nó vào sử dụng! Chúng tôi sẽ tạo đòn bẩy với MAI của mình bằng cách gửi nó vào bể stablecoin MAI-Base4Pool của StellaSwap và sử dụng lợi tức để kiếm được nhiều mã thông báo Stella hơn bằng cách đặt cọc cho chúng. Hãy luôn nhớ rằng nếu bạn tham gia chiến lược này, bạn sẽ tự chịu rủi ro và kho tiền của bạn có thể bị thanh lý nếu bạn không thực hiện trách nhiệm giải trình của mình!\
\
Đầu tiên chúng ta hãy tìm MAI-Base4Pool trên trang StellaSwap [Farms.](https://app.stellaswap.com/farm)

![MAI-Base4Pool](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Bể thanh khoản này hiện đang cung cấp lợi suất 26% rất hấp dẫn trên các đồng tiền ổn định với một bể bao gồm MAI, FRAX, USDT, USDC và DAI với lợi suất được thanh toán bằng mã thông báo Stella. Lưu ý rằng lợi suất này chủ yếu bù đắp lãi suất mà chúng tôi hiện đang trả cho khoản vay MAI của chúng tôi (12%). Chúng ta có thể xem xét hiệu suất của chúng tôi cho đến nay:

$$effective interest = (collateral * borrow interest)-(mai*farmingyield)$$

Điều này mang lại cho chúng tôi lợi suất hiệu quả là 1,6% để vay MAI - không tệ, nhưng chúng tôi có thể làm tốt hơn. Giờ đây, chúng tôi có thể lấy mã thông báo Stella mà chúng tôi kiếm được từ việc tham gia MAI-Base4Pool và [đặt cược chúng để nhận xStella.](https://app.stellaswap.com/xstella)

![Đặt cọc xStella](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.33.31 PM.png>)

Đặt cọc xStella có hai lợi ích bổ sung. Đầu tiên, nó cung cấp tỷ lệ APR đặt cược là 70%, do đó cộng gộp lợi nhuận của chúng ta, nhưng quan trọng hơn, xStella tăng giá trị theo thời gian khi doanh thu hoán đổi từ giao thức được chia sẻ giữa những người dùng. Điều này có nghĩa là bất kỳ lợi suất nào chúng ta đang kiếm được từ vị trí tương đối an toàn của chúng ta trong một bể stablecoin sẽ liên tục tăng. Sau đó, chúng ta có thể sử dụng những lợi tức bổ sung này để gửi thêm xStella vào kho tiền của chúng ta để tăng LTV của chúng ta hoặc để vay thêm MAI.

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Keep in mind that a strategy that works well at a given time may perform poorly (or make you lose money) at another time. Please stay informed, monitor the markets, keep an eye on your investments, and as always, do your own research.
{% endhint %}
