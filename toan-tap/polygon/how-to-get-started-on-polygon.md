---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ trình bày tất cả mọi thứ bạn cần biết để sử
  dụng các Dapps khác nhau trên chuỗi khối Polygon
---

# Các bước bắt đầu trên mạng Polygon

## Polygon là gì?

Mạng lưới Polygon là một mạng lưới được xây dưng trên nền tảng của chuỗi khối Ethereum, được thiết kế để giải quyết các vấn đề về khả năng mở rộng mà chuỗi Ethereum đang gặp phải. Một giao dịch trung bình trên mạng Polygon chỉ mất 3 đến 5 giây với chi phí giao dịch 1 xu, cho phép người dùng thực hiện được hàng chục giao dịch mỗi ngày với ngân sách hợp lý.

Polygon cũng là một trong những " side chain" đầu tiên có những tiến bộ đáng kể so với các chuỗi hiện tại, có thể kể đến như.

* Cơ sở người dùng ngày càng tăng
* Số lượng ứng dụng ngày càng tăng
* TVL bền vững ổn định vào khoảng 4 tỷ USD

Polygon cũng bắt đầu xây dựng lòng tin như là một thay thế đáng tin cậy của chuỗi Ethereum, mở ra thế giới Defi cho những nhà đầu tư  nhỏ mà không phải chi hàng trăm đô la cho phí giao dịch. Với sự tin cậy cũng như tính thân thiện của Polygon, rất nhiều công ty đã chuyển sang Polygon để tạo điều kiện kết nối tài sản từ mạng này sang mạng khác, tăng cường bảo mật và tính ẩn danh, cùng lúc đó làm mạng lưới trở nên vững mạnh hơn.&#x20;

## Tạo một ví&#x20;

Trước khi bắt đầu với chuỗi khối Polygon , bạn cần tạo một địa chỉ ví, có nhiều loại ví khác nhau bao gồm phần mềm (Metamask, TrustWallet ...) và phần cứng (Trezor hoặc Ledger). Tuy nhiên, trong hướng dẫn này, chúng tôi sẽ sử dụng Metamask để giải thích cách truy cập vào Polygon.

### Tải Metamask

Bước đầu tiên bạn cần hoàn thành để sử dụng chuỗi Polygon là tải xuống tiện ích mở rộng Metamask trong trình duyệt web của bạn. Bạn có thể tải xuống trên[ trang web ](https://metamask.io/index.html)của họ. Metamask cũng có thể được sử dụng trên các thiết bị IOS và Android.

Khi hoàn thành bạn sẽ thấy một tiện ích mở rộng trên trình duyệt của mình với biểu tượng của Metamask. Khi bạn mở tiện ích mở rộng Metamask lần đầu tiên, nó sẽ hỏi bạn xem bạn có tài khoản Metamask hay không, nếu có, bạn cần viết seed phrase (chúng ta sẽ nói về tầm quan trọng của seed phrase sau) của tài khoản bạn muốn sử dụng. Nếu chưa có tài khoản, bạn sẽ phải tạo một tài khoản mới. Sau đây là một số bước cụ thể:

1. Trước hết, bạn cần chọn mật khẩu cho tài khoản Metamask của mình.&#x20;
2. Sau đó, bạn nên xem video về cách bảo vệ ví của bạn và tầm quan trọng của cụm từ seed phrase.
3. Seed phrase của bạn là điều quan trọng nhất khi tạo ví mới, vì nếu bạn mất cụm từ này và máy tính của bạn bị hỏng, bạn sẽ không thể truy cập vào tài khoản Metamask của mình. Vì vậy, hãy giữ cẩn thận với cụm từ này và tuyệt đối không chia sẻ nó với bất kỳ ai.

![Giao diện của Metamask](<../../.gitbook/assets/image (18).png>)

### Thêm chuỗi Polygon

Như bạn thấy ở trên, chúng ta bắt đầu với mạng Ethereum mặc định, để có thể sử dụng mạng Polygon, chúng ta cần thêm thủ công bằng cách nhấp vào RPC tùy chọn và thiết lập mạng  Polygon với các thông số kỹ thuật như hình dưới:

![](<../../.gitbook/assets/image (20).png>)

Sau khi hoàn tất, bạn gần như đã sẵn sàng để sử dụng ví Metamask trên Polygon , bước duy nhất còn lại là chuyển Ethereum Mainnet sang Polygon, để làm như vậy bạn cần nhấp vào menu mạng thả xuống ở đầu tiện ích Metamask.

## Cách nhận MATIC miễn phí

Bây giờ bạn đã thiết lập mọi thứ để sử dụng Polygon, tuy nhiên bạn không có bất kỳ MATIC nào trên ví của mình, vì vậy bạn không thể thực hiện bất kỳ giao dịch nào trên Polygon cả. Về cơ bản, một giao dịch là sự trao đổi giữa 2 địa chỉ, cần một thời gian để được xử lý (điều này được thực hiện bởi các node xác thực khác nhau mà Polygon có) và có phí (phí này còn được gọi là gas và được thanh toán bằng mã thông báo MATIC).

May mắn thay, [trang này](https://matic.supply/) cung cấp cho bạn MATIC miễn phí để thực hiện các giao dịch đầu tiên của bạn trên mạng Polygon (những loại trang đó có thể được gọi là faucet). Điều duy nhất bạn cần làm là kết nối ví của bạn với trang đó và hoàn thành hình ảnh xác thực. 0,002 MATIC này (\~ 0,00223 $) sẽ cho phép bạn thực hiện một số giao dịch sử dụng trên mạng Polygon.

![Nhận miễn phí MATIC](<../../.gitbook/assets/image (23).png>)

Đôi khi do tắc nghẽn mạng, bạn có thể gặp một số vấn đề khi sử dụng trang, vì vậy chỉ cần đợi một chút là bạn sẽ có thể yêu cầu một số MATIC miễn phí. Ngoài ra, bạn có thể thử sử dụng [trang này](https://macncheese.finance/matic-polygon-mainnet-faucet.php) trong trường hợp trang kia không hoạt động.

Trước khi chúng ta chuyển sang phần tiếp theo của bài viết, bạn cần lưu ý rằng những trang faucets này không được thực hiện để mọi người rút nó cạn ra, nó sẽ không mang lại bất cứ gì nếu ví của bạn có quá nhiều MATIC hoặc nếu bạn cố gắng yêu cầu nhiều hơn một vài lần trong vòng 24h. Vì vậy, xin hãy cẩn thận và đừng ích kỷ.

## Thêm token vào Metamask

Bây giờ bạn đã có một số MATIC miễn phí trong Metamask để sẵn sàng sử dụng các DApp và mã thông báo khác nhau mà Polygon. Bạn có thể sao chép địa chỉ của mã thông báo mà bạn muốn sử dụng bằng [PolygonScan](https://polygonscan.com/). Khi bạn ở đó, bạn chỉ cần viết tên của mã thông báo mà bạn muốn thêm. Ví dụ: nếu chúng ta tìm kiếm QiDAO trên Polygon, chúng ta sẽ thấy:

![Kết quả của QiDao trên Polygonscan](<../../.gitbook/assets/image (24).png>)

Bây giờ, bạn sẽ cần sao chép địa chỉ của hợp đồng và nhấp vào thêm mã thông báo trên Metamask.

![Thêm Qi vào trong Metamask](<../../.gitbook/assets/image (25).png>)

## Cách mua token trên Polygon

Bây giờ đã có Metamask và một số MATIC để thanh toán gas, chúng ta có thể bắt đầu mua một số mã thông báo trên mạng Polygon. Để làm như vậy, bạn cần sử dụng DEX (Sàn giao dịch phi tập trung), có rất nhiều DEX mà bạn có thể lựa chọn, như [_Quickswap_](https://quickswap.exchange/#/swap)_,_ [_Slingshot_](https://app.slingshot.finance/markets)_,_ [_Dexguru,_](https://dex.guru/token/0x76bf0c28e604cc3fe9967c83b3c3f31c213cfe64-polygon) __ [_Sushiswap_](https://app.sushi.com/vi/swap)_, v.v.._&#x20;

Khi bạn quyết định DEX nào bạn muốn sử dụng, bạn có thể bắt đầu mua các mã thông báo yêu thích của mình trên Polygon.

![Buying Qi tokens using Quickswap](<../../.gitbook/assets/image (26).png>)

{% hint style="info" %}
Một DApp thú vị khác để sử dụng khi bạn muốn trao đổi tiền mã hóa là [Zapper](https://zapper.fi/). Về mặt lý thuyết, Zapper tìm kiếm nền tảng rẻ nhất để thực hiện hoán đổi hai mã thông báo, vì vậy đó là một cách tốt để tiết kiệm một số MATIC nhất định.
{% endhint %}

## Kiểm tra ví của bạn

Điều quan trọng là phải biết cách kiểm tra lịch sử ví của bạn, để làm như vậy, bạn có thể sử dụng [DeBank](https://debank.com/). Debank sẽ cho phép bạn kiểm tra các giao dịch khác nhau mà bạn đã thực hiện trong tài khoản Metamask của mình, cũng như kiểm tra danh mục đầu tư của bạn trong tất cả các blockchain mà bạn sử dụng hoặc NFT mà bạn sở hữu. Điều này sẽ hữu ích nếu bạn muốn so sánh, chẳng hạn như các airdrop Qi khác nhau mà bạn nhận được khi đặt một số cổ phần Qi.

![Tất cả các giao dịch được hiển thị trên ví Metamask mới ](<../../.gitbook/assets/image (27).png>)

Như bạn có thể thấy, tôi có trong ví 800.000 DxDex.io nhưng tôi chưa làm bất cứ điều gì để có những mã thông báo đó trong ví của mình. Bạn cần lưu ý những kiểu lừa đảo này và không bao giờ tương tác với bất kỳ đồng tiền nào mà bạn không biết. Trong trường hợp bạn cấp cho họ quyền truy cập, Debank sẽ cho phép bạn thu hồi quyền truy cập đó. Hãy cẩn thận và nếu bạn không biết mã thông báo đó, đừng chạm vào nó.

## Một số liên kết hữu ích

Dưới đây là một số liên kết mà bạn có thể thấy hữu ích khi sử dụng chuỗi khối Polygon:

* [Quickswap](https://quickswap.exchange/#/swap)
* &#x20;[AAVE](https://app.aave.com/)
* [PolygonScan](https://polygonscan.com/gastracker/): liên kết này sẽ hữu ích để quan sát giá gas giao dịch trên chuỗi khối Polygon

## Tuyên bố từ chối trách nhiệm

Hướng dẫn này chắc chắn không phải là lời khuyên tài chính, nó được thực hiện với mục tiêu giáo dục.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}

