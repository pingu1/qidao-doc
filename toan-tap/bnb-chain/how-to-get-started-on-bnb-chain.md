---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ giải thích mọi thứ bạn cần biết để bắt đầu
  sử dụng các DApp khác nhau mà chuỗi BNB cung cấp.
---

# Khởi động trên chuỗi BNB

## Chuỗi BNB là gì?

BNB Chain là mạng tương thích EVM (Máy ảo Ethereum), là phiên bản nâng cấp của BSC ban đầu, cung cấp phí giao dịch thấp và thời gian khối nhanh hơn nhiều so với Ethereum.\
\
Bởi vì điều này, BNB Chain là một trong những chuỗi phổ biến nhất trên thế giới với hơn 4,5 tỷ giao dịch hàng năm và một hệ sinh thái DApp cực kỳ sôi động.

BNB Chain sử dụng mã thông báo BNB của Binance để thanh toán phí gas, vì vậy hãy đảm bảo có một số trong ví của bạn để thực hiện các giao dịch. Binance cung cấp các hướng dẫn đơn gian làm theo về cách mua hoặc chuyển token vào [chuỗi BNB của mình.](https://www.binance.com/en/support/faq/85a1c394ac1d489fb0bfac0ef2fceafd)

## Khởi động trên chuỗi BNB

Trước khi sử dụng BNB Chain, bạn sẽ cần địa chỉ ví. Vì BNB Chain là mạng EVM nên nó sẽ chấp nhận các ví tương tự như trên các chuỗi EVM khác, bao gồm ví web như Metamask hoặc Nifty và bạn sẽ có thể sử dụng ví phần cứng của mình như Trezor hoặc Ledger, nhưng bạn có thể phải tuân theo các bước bổ sung để có thể kết nối ví lạnh của bạn với mạng.

Đối với hướng dẫn này, chúng tôi sẽ gắn bó với Metamask giống như chúng tôi đã làm cho tất cả các hướng dẫn khác trên trang web này. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về [Cách bắt đầu trên Polygon](../polygon/how-to-get-started-on-polygon.md).&#x20;

Ngoài ra, bạn có thể sử dụng Ví Binance của riêng Binance để bắt đầu sử dụng mạng một cách dễ dàng hơn.

### Thêm chuỗi BNB vào Metamask

Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Thêm mạng. Bạn sẽ sử dụng thông tin sau trong các trường văn bản có liên quan dưới đây.

* **Network Name:** BNB Chain
* **New RPC URL:** [https://docs.binance.org/smart-chain/developer/rpc.html](https://docs.binance.org/smart-chain/developer/rpc.html)
* **Chain ID:** 0x38
* **Currency Symbol:** BNB
* **Block Explorer URL:** [**https://bscscan.com/**](https://bscscan.com/)\*\*\*\*

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang BNB:

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.28.44 AM.png>)

Nếu bạn muốn tìm kiếm các RPC bổ sung có độ trễ thấp hơn, hãy xem [ChainList ](https://chainlist.org/)để biết các điểm cuối bổ sung.

## Kết nối với chuỗi BNB

### Faucets

Có các nguồn faucets miễn phí có sẵn trên BNB Chain, nhưng theo ý kiến của tác giả rằng sẽ an toàn hơn khi sử dụng [ElkNet](https://app.elk.finance/#/elknet) để nhận mã thông báo gas miễn phí. Nếu bạn chọn sử dụng một vòi bạn tìm thấy trực tuyến, vui lòng tự chịu rủi ro. Với ElkNet, bạn có thể chọn hoán đổi một số mã thông báo Elk của mình dưới dạng khí khi bắc cầu từ bất kỳ mạng nào được hỗ trợ.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.29.50 AM.png>)

### Cầu nối

* [Multi Chain](https://app.multichain.org/#/router)là đối tác chính thức của Mai Finance nếu bạn muốn chuyển MAI hoặc QI của mình sang BNB Chain từ bất kỳ mạng nào khác. Từ mạng đã chọn của bạn, bạn có thể chỉ cần chọn chuỗi đích (Chuỗi BNB) và tài sản bạn muốn gửi (ví dụ: MAI hoặc QI) với số tiền chính xác và nhấp vào nút Chuyển. Chú ý đến phí chuyển khoản được tính trực tiếp trên tài sản bạn đang chuyển.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.32.07 AM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) là một cầu nối phổ biến và cho phép bạn chuyển mã thông báo từ khoảng 15 mạng khác nhau sang Chuỗi BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.31.15 AM.png>)

* [Hashflow](https://app.hashflow.com/) là một công nghệ bắc cầu mới hơn, hoạt động về cơ bản như một DEX xuyên chuỗi (trao đổi phi tập trung) cho bất kỳ mã thông báo nào có đủ thanh khoản. Ngoài ra, người dùng Hashflow hiện có thể kiếm được HFT (mã thông báo Hashflow) để hoán đổi hoặc cung cấp tính thanh khoản cho mã thông báo. Chuỗi hiện được giới hạn ở Ethereum, Avalanche, Arbitrum, Optimism, Polygon và BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.33.51 AM.png>)

* [Elknet](https://app.elk.finance/#/elknet) sẽ hoạt động như một cầu nối và một nguồn faucets khi bạn chuyển mã thông báo ELK giữa 2 mạng. Bạn sẽ có thể kết nối ELK của mình và ở đầu nhận, bạn có thể có một phần nhỏ ELK của mình trực tiếp dưới dạng mã thông báo gas, BNB trong trường hợp của chúng tôi, như đã giải thích trong phần trên.

## DeFi trên chuỗi BNB

* [Ellipsis Finance](https://ellipsis.finance/pool/0x68354c6E8Bbd020F9dE81EAf57ea5424ba9ef322) là lựa chọn phù hợp cho thanh khoản MAI trên Chuỗi BNB. Nhóm MAI trên Ellipsis (MAI + val3EPS) bao gồm bốn loại tiền ổn định bao gồm BUSD (Binance USD), USDC, USDT (Tether) và MAI. Bằng cách gửi các stablecoin, và sau đó đặt LP vào Ellipsis, người dùng có thể kiếm được lợi nhuận thay đổi từ 6 đến 15% được thanh toán bằng mã thông báo EPS của Ellipsis, mã thông báo VAL của Vallas, cũng như phí giao dịch.

![Bể MAI+val3EPS trên Ellipsis](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.07.42 AM.png>)

## Mai Finance trên chuỗi BNB

Nền tảng cho vay đã có sẵn trên Chuỗi BNB, nơi bạn sẽ có thể gửi mã thông báo WBNB (Wrapped BNB) và CAKE (PancakeSwap) vào một kho tiền làm thế chấp và mượn MAI. Sau đó, bạn có thể gửi MAI đã vay của mình trên Ellipsis để kiếm được lợi nhuận từ MAI của bạn.

![](<../../.gitbook/assets/Screen Shot 2022-06-18 at 11.11.26 AM.png>)

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
