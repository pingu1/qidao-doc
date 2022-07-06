---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ giải thích mọi thứ bạn cần biết để bắt đầu
  sử dụng các DApp khác nhau mà Arbitrum cung cấp.
---

# Khởi động trên mạng Arbitrum

## Arbitrum là gì?

Arbitrum là một giải pháp mở rộng quy mô cho phép người dùng gửi các giao dịch trên mạng Ethereum và thực hiện chúng nhanh hơn với chi phí gas thấp hơn nhiều. Vì lý do này, Arbitrum được biết đến như một Ethereum lớp 2 (viết tắt là L2). Giống như mạng anh em của nó, Optimism, Arbitrum cũng sử dụng công nghệ Optimistic Rollup đề cập đến loại bằng chứng mà mạng sử dụng để hoạt động song song với chuỗi Ethereum chính (lớp 1 hoặc L1). Để đọc thêm về Optimistic rollups và các giải pháp tổng hợp khác như ZK rollups, vui lòng truy cập [liên kết này](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Bởi vì nó là một công nghệ rollups, Arbitrum không tạo ra các khối của riêng mình và do đó không thực sự là một blockchain. Offchain Labs, các nhà phát triển đằng sau Arbitrum, nhằm mục đích làm cho mạng EVM (Máy ảo Ethereum) tương đương với các bản nâng cấp trong tương lai.\
\
Xin lưu ý rằng vì lý do này, Arbitrum không sử dụng mã thông báo gas của riêng mình mà sử dụng Ether làm gas để thanh toán cho các giao dịch.

## Khởi động trên Arbitrum

Trước khi sử dụng Arbitrum, bạn sẽ cần một địa chỉ ví. Vì Arbitrum là một mạng EVM, nó sẽ chấp nhận các ví giống như trên các chuỗi EVM khác, bao gồm ví web như Metamask hoặc Nifty và bạn sẽ có thể sử dụng ví phần cứng của mình như Trezor hoặc Ledger, nhưng bạn có thể phải theo dõi thêm các bước để có thể kết nối ví lạnh của bạn với mạng.&#x20;

Đối với hướng dẫn này, chúng tôi sẽ gắn bó với Metamask giống như chúng tôi đã làm cho tất cả các hướng dẫn khác trên trang web này. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về [Cách bắt đầu trên Polygon](../polygon/how-to-get-started-on-polygon.md).

### Thêm Arbitrum vào Metamask

Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Thêm mạng. Bạn sẽ sử dụng thông tin sau trong các trường văn bản có liên quan:

* **Network Name:** Arbitrum
* **New RPC URL:** [https://arb1.arbitrum.io/rpc](https://arb1.arbitrum.io/rpc)
* **Chain ID:** 4216
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://arbiscan.io/](https://arbiscan.io/)

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang Arbitrum:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.27.21 PM.png>)

## Kết nối tới Arbitrum

### Faucets

Không có faucet cho phí gas nào trên Arbitrum, nhưng nếu bạn sử dụng DApp như [ElkNet](https://app.elk.finance/#/elknet), bạn có thể chọn hoán đổi một số mã thông báo Elk của mình thành gas khi bắc cầu từ bất kỳ mạng nào được hỗ trợ.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.31.52 PM.png>)

### Cầu nối

* [Multi Chain](https://app.multichain.org/#/router) là đối tác chính thức của Mai Finance nếu bạn muốn chuyển MAI hoặc QI của mình sang Arbitrum từ bất kỳ mạng nào khác. Từ mạng đã chọn của bạn, bạn có thể chỉ cần chọn chuỗi đích (Arbitrum) và tài sản bạn muốn gửi (MAI hoặc ETH với số tiền chính xác và nhấp vào nút Chuyển. Hãy chú ý đến phí chuyển trực tiếp trên tài sản bạn đang chuyển.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.33.02 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) là một cầu nối phổ biến và cho phép bạn chuyển các mã thông báo từ khoảng mười lăm mạng khác nhau sang Arbitrum.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.35.44 PM.png>)

* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) là một cây cầu phổ biến khác. Chỉ có một số lượng nhỏ mã thông báo được hỗ trợ bao gồm ETH và các loại tiền ổn định khác nhau như USDC, DAI và USDT, nhưng nó cung cấp phí bắc cầu thấp hơn hầu hết các giải pháp khác.
* [Hashflow](https://app.hashflow.com/) là một công nghệ bắc cầu mới hơn, hoạt động về cơ bản như một DEX xuyên chuỗi (trao đổi phi tập trung) cho bất kỳ mã thông báo nào có đủ thanh khoản. Ngoài ra, người dùng Hashflow hiện có thể kiếm được HFT (mã thông báo Hashflow) để hoán đổi hoặc cung cấp tính thanh khoản cho mã thông báo. Chuỗi hiện được giới hạn ở Ethereum, Avalanche, Arbitrum, Optimism, Polygon và BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) sẽ hoạt động như một cầu nối và một faucet khi bạn chuyển mã thông báo ELK giữa 2 mạng. Bạn sẽ có thể bắc cầu ELK của mình và ở đầu nhận, bạn có thể có một phần nhỏ ELK của mình trực tiếp dưới dạng mã thông báo gas, ETH trong trường hợp của chúng ta, như đã giải thích trong phần trên.

## DeFi trên Arbitrum

* [Balancer](https://arbitrum.balancer.fi/#/pool/0x0510ccf9eb3ab03c1508d3b9769e8ee2cfd6fdcf00000000000000000000005d) hiện có bể duy nhất trên Arbitrum có thanh khoản MAI. Bằng cách gửi MAI của bạn vào nhóm MAI / USDC / USDT, người dùng có thể kiếm được khoảng 13% lợi nhuận trên stablecoin của họ. Xin lưu ý rằng nhóm này sẽ sớm được di chuyển để khắc phục lỗi thanh khoản hiện có.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.43.57 PM.png>)

## Mai Finance trên Arbitrum

Nền tảng cho vay đã có sẵn trên Arbitrum, nơi bạn có thể gửi mã thông báo WETH (Ether được bọc) hoặc WBTC (Bitcoin được bọc) vào một kho tiền làm thế chấp và mượn MAI. Sau đó, bạn có thể gửi MAI đã vay của mình trên Balancer để kiếm lợi nhuận.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.38.15 PM.png>)

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
