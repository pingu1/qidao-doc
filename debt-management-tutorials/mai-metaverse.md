---
description: >-
  Hướng dẫn này sẽ trình bày tổng quan về các chuỗi khối khác nhau mà đồng tiền
  stablecoin MAI có thể được sử dụng và cách bạn có thể kết nối đồng tiền này
  với các chuỗi khác nhau.
---

# Vũ trụ MAI

![Andy sees his future ](<../.gitbook/assets/Screen Shot 2021-09-13 at 1.06.42 PM.png>)

## Giới thiệu

MAI, đôi khi được gọi là miMATIC, là đồng tiền ổn định đầu tiên có nguồn gốc từ chuỗi Polygon. Nó được chốt ở mức $ 1,00 và giá trị của nó có thể dao động trong khoảng $ 0,99 đến $ 1,01. Bạn có thể biết thêm chi tiết về [cách neo duy trì](https://docs.mai.finance/stablecoin-economics#how-is-the-peg-maintained) trong tài liệu chính thức của Mai Finance. Nhưng không phải vì MAI có nguồn gốc từ Polygon mà nó chỉ được tìm thấy trên mạng đó. Thật vậy, giống như cách bạn có thể tìm DAI trên các mạng khác nhau (DAI thực sự là một đồng stablecoin đến từ Ethereum Mainnet), MAI cũng đang mở rộng dần một cách chắc chắn sang các chuỗi khác. Bài viết này sẽ nêu bật các mạng khác nhau mà bạn có thể tìm thấy nó và cách bạn có thể chuyển MAI của mình từ chuỗi này sang chuỗi khác.

## Polygon

### Cách có được MAI trên chuỗi Polygon

Như đã giải thích ở trên, MAI có nguồn gốc từ Polygon và đó là nơi duy nhất (vào tháng 9 năm 2021) nơi bạn có thể đúc MAI. Điều này được thực hiện bởi

* vay MAI đối với một số tài sản thế chấp mà bạn đã gửi trước đó vào một vault trên Mai Finance
* đổi USDC sang Mai trên [Mai Finance](https://app.mai.finance/anchor)
* bán một tài sản khác và mua MAI trên bất kỳ DEX nào (Sàn trao đổi phi tập trung) trên Polygon như [Zapper](https://zapper.fi/exchange), [Balancer](https://polygon.balancer.fi/#/trade) hoặc [1Inch](https://app.1inch.io/#/137/classic/swap).

### Sử dụng MAI trên Polygon

Đồng stablecoin MAI đang được sử dụng trong ngày càng nhiều dự án trên Polygon, đặc biệt là hiện nay nó được sử dụng như các đồng stablecoin khác trong các dự án lớn trên QuickSwap. Tính đến tháng 9 năm 2021, có 3 bể stablecoin trên QuickSwap với tổng số tiền là:

* MAI-DAI với $6,553,255
* MAI-USDT với $6,316,026
* MAI-USDC với $5,458,323

Các bể khác có thể được tìm thấy trên các dự án khác / yield farming / yield optimizer. Bạn có thể đọc thêm về cách sử dụng  với đồng tiền stablecoin MAI của mình trong [đoạn chi tiết này](how-to-use-mai-in-the-real-life.md).

## Solana

### Cách kiếm MAI trên Solana

Solana là một nền tảng blockchain cho các ứng dụng phi tập trung. Mục tiêu của mạng là đề xuất phí thấp (dưới 0,01 đô la) và giao dịch nhanh (dưới 400 mili giây). Ý tưởng đằng sau điều này là tạo ra một số thay thế cho Ethereum Mainnet và các chuỗi phụ của nó. Tuy nhiên, không phải vì Solana là đối thủ cạnh tranh trực tiếp với mạng Ethereum mà nó không hỗ trợ các tài sản tương tự. Thật vậy, Solana hiện hỗ trợ đồng tiền stablecoin MAI có thể được bắc cầu từ Polygon (nơi nó có thể được đúc).

Để gửi đồng MAI của bạn đến Solana, bạn có thể sử dụng [AllBridge](https://allbridge.io), một nền tảng cầu nối cho phép bạn chuyển tài sản từ chuỗi này sang chuỗi khác. AllBridge hỗ trợ các mạng sau:

* Ethereum Mainnet
* Polygon
* Solana
* Huobi
* Binance Smart Chain

Giao diện thực sự trực quan theo nghĩa bạn chỉ cần chọn hai mạng và tài sản bạn muốn chuyển giữa hai mạng.

![Đưa MAI từ polygon sang solana](<../.gitbook/assets/Screen Shot 2021-09-13 at 1.52.23 PM.png>)

Bước tiếp theo là điền địa chỉ ví Solana của bạn và số tiền bạn muốn chuyển. Lưu ý rằng MetaMask chưa hỗ trợ ví Solana. Do đó bạn sẽ phải tạo một ví riêng trên mạng đó. Nó có thể là ví web như MetaMask hoặc ứng dụng ví. Xin vui lòng đọc [tài liệu hướng dẫn setup ví chính thức của Solana ](https://docs.solana.com/wallet-guide)để có thể có lựa chọn phù hợp.

{% hint style="info" %}
Cần lưu ý rằng Solana không cung cấp bất kỳ faucet nào mà bạn sẽ nhận được SOL đầu tiên của mình (đồng bản vị được sử dụng để thanh toán cho các giao dịch). Bạn cần mua một ít SOL trước và có chúng sẵn trong ví để có thể chuyển MAI.
{% endhint %}

### Sử dụng Mai trên Solana 

Tương tự như cách bạn có thể sử dụng MAI trên Polygon để cung cấp  thanh khoản và yield farming, bạn cũng có thể làm tương tự trên Solana. Nơi mà bạn có thể sử dụng MAI là [Saber,](https://app.saber.so/#/swap) trong bể MAI / USDC.

![Trạng thái bể MAI/USDC tại thời điểm Sept. 2021](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.11.10 PM.png>)

Một trong những điều thuận lợi cần biết về bể MAI / USDC trên saber đó là, không giống như cặp LP (Cung cấp thanh khoản) trên QuickSwap, bạn không cần phải cung cấp cặp LP với tỷ lệ 1: 1. Bạn có thể chỉ cần gửi một tài sản duy nhất (MAI hoặc USDC) hoặc một tỷ lệ cân bằng (hoặc không) của cả hai đồng tiền stablecoin.

![MAI và USDC không cân bằng trong bể Saber](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.13.51 PM.png>)

Điều này có nghĩa là bạn thực sự có thể sử dụng 100% tiền gửi MAI từ Mai Finance mà không cần phải hoán đổi bất kỳ khoản nào để lấy USDC. Nó đặc biệt tiện lợi và tránh bị ảnh hưởng bởi sự khác biệt nhỏ về giá giữa 2 đồng. Lưu ý rằng bạn sẽ nhận được phần thưởng được trả bằng token của trang trại gốc, giống như cách bạn sẽ được trả trong QUICK nếu bạn đang farming ở QuickSwap trên Polygon. Sau đó, bạn có thể bán đồng bản vị của saber để tăng vị thế của LP MAI / USDC.

{% hint style="info" %}
Trên Solana, bạn cũng có thể sử dụng [Sunny](https://app.sunny.ag), một nền tảng tăng tốc tự động gộp phần thưởng từ Saber. Lưu ý rằng nền tảng Sunny không được xác thực bởi team Mai Finance. AllBridge và Saber đã là đối tác chính thức của Mai Finance, nhưng kết quả không được đảm bảo chắc chắn. Và vui lòng, như thường lệ, hãy tự nghiên cứu.
{% endhint %}

## Avalanche

### Cách đưa MAI lên Avalanche

Avalanche là một blockchain, được thiết kế để cung cấp một nền tảng mã nguồn mở và một giao thức lớp 1 để khởi chạy các ứng dụng DeFi và các giải pháp blockchain doanh nghiệp. Đó là một giải pháp thay thế khác cho Ethereum Mainnet cũng hỗ trợ các tài sản tương tự như Ethereum Mainnet, Polygon và Solana. Do đó, bây giờ bạn có thể gửi MAI của mình từ Polygon (nơi duy nhất, kể từ tháng 9 năm 2021, nơi bạn có thể đúc MAI) đến Avax bằng cách sử dụng [Relay Chain](https://app.relaychain.com/#/transfer).

Cũng giống với AllBridge, giao diện người dùng khá đơn giản. Bạn chỉ cần chọn mạng mà nội dung sẽ là cầu nối, điểm đến của nó và mã token cần chuyển.

![Đưa đồng MAI từ Polygon sang Avanlache bằng Relay](<../.gitbook/assets/Screen Shot 2021-09-13 at 2.52.31 PM.png>)

Metamask có hỗ trợ [Avax wallets](https://support.avax.network/en/articles/4626956-how-do-i-set-up-metamask-on-avalanche), vì vậy bạn không cần phải cài đặt hay mở một ví web khác nữa.

### Sử dụng MAI trên Avax

Tương tự như cách bạn có thể sử dụng MAI để tăng sản lượng trên Polygon, bạn có thể sử dụng MAI trên Avalanche. Nơi để làm như vậy là [Trader Joe](https://www.traderjoexyz.com/#/farm), nơi bạn sẽ tìm thấy một bể MAI / USDC

![State of the MAI/USDC pool on Trader Joe as of Sept. 2021](<../.gitbook/assets/Screen Shot 2021-09-13 at 3.07.19 PM.png>)

Các bể thanh khoản trên Avalanche hoạt động rất giống với những gì bạn có thể tìm thấy trên Polygon. Do đó, bạn có thể sử dụng  Trader Joe giống như cách bạn sử dụng với QuickSwap. Trước tiên, bạn cần tạo một cặp LP trên trang web bằng cách sử dụng cùng một tỷ lệ MAI và USDC, sau đó gửi cặp LP vào bể. Tương tự như cách bạn sẽ được trả đồng QUICK khi farm trên QuickSwap, bạn sẽ nhận được phần thưởng bằng đồng JOE khi farm trên Trader Joe. Sau đó, bạn có thể sử dụng số tiền này vào các bể khác hoặc bán chúng để tăng vị thế cặp MAI / USDC của mình.

## Fantom

### Cách đưa MAI lên  Fantom

Fantom là một nền tảng blockchain / hợp đồng thông minh với mục đích giải quyết các vấn đề về khả năng mở rộng của các mạng khác, cụ thể là chuỗi khối Ethereum. Các nhà phát triển có thể tạo DApp (Ứng dụng phi tập trung) của họ trên mạng đó và sử dụng các tài sản tương tự như trên mạng khác. Như vậy, bạn đã có thể bắc cầu MAI từ Polygon sang Fantom bằng cách sử dụng cầu nối [AnySwap](https://anyswap.exchange/#/bridge).

Nếu AnySwap là một giải pháp bắc cầu khác, thì giao diện người dùng của nó rất giống với giao diện của AllBridge và Relay Chain. Khi ở trên Polygon, bạn sẽ phải kết nối ví MetaMask của mình trước, sau đó chọn tài sản bạn muốn kết nối (MAI) và mạng đích (Fantom).

![Bridging MAI from Polygon to Fantom](../.gitbook/assets/image.png)

Metamask không hỗ trợ [ví fantom](https://docs.fantom.foundation/tutorials/set-up-metamask), vì vậy rất dễ dàng thiết lập nó để nhận MAI của bạn trên Fantom và bắt đầu sử dụng nó ngay lập tức.

### Sử dụng MAI trên Fantom

Hiện tại, team Mai Finance chưa có bất kỳ quan hệ đối tác nào với bất kỳ yield farms nào trên Fantom. Sau khi nhóm biết về các dự án đang sử dụng MAI, tài liệu này sẽ được cập nhật. Hãy đón chờ nhé.

## Tuyên bố từ chối trách nhiệm

Các chi tiết được trình bày trong hướng dẫn này hoàn toàn mang tính giáo dục và chưa được kiểm tra trực tiếp bởi nhóm. Một số người dùng trên Discord đã thử bắc cầu tài sản của họ với Solana và/hoặc Avalanche, vì vậy bạn có thể tham gia cộng đồng Discord để đặt câu hỏi. Xin đừng quên tự nghiên cứu, các mạng khác nhau sẽ có phí giao dịch và thời gian thực hiện khác nhau, các chương trình thưởng khác nhau, phí bắc cầu, v.v. Nếu bạn gửi MAI của mình đến các mạng khác, hãy đảm bảo rằng bạn có thể kết nối chúng trở lại trong trường hợp bạn cần trên Polygon.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự mình nghiên cứu.
{% endhint %}
