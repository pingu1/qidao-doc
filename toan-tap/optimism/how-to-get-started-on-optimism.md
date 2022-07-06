---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ giải thích mọi thứ cần phải biết để bắt đầu
  trên mạng Optimism và sử dụng các dAPP trên đó.
---

# Khởi động trên mạng Optimism

## Optimism là gì?

Optimism hay còn gọi là Optimistic Ethereum hay đôi khi được gọi là giải pháp mở rộng quy mô cho mạng Ethereum cho phép người dùng được hưởng lợi thì phí giao dịch thấp và tốc độ ngay trong khi bảo mật vẫn được đảm bảo bởi mạng Ethereum. Chính vì lý do này nên Optimistic còn được coi là Ethereum lớp 2 (hay L2 cho ngắn gọn). Tên gọi Optimistic xuất phát từ việc giải pháp này sử dụng công nghệ Optimistic Rollup đề cập đến việc sử dụng loại bằng chứng mà nó sử dụng để hoạt động song song với mạng chính (Ethereum L1). Tìm hiểu thêm về giải pháp này cũng như công ZK rollup vui lòng theo đường [liên kết này](https://support.deversifi.com/en/article/deversifi-what-is-the-difference-between-zk-rollup-and-optimistic-rollup-3gf3bw/).

Bởi vì nó là một công nghệ Rollup, Optimistic không tạo ra các khối của riêng nó và do đó không phải là một chuỗi khối. Ngoài ra, API mạng Optimism phần lớn sử dụng đặc điểm kỹ thuật JSON-RPC tương tự như Ethereum và do đó về cơ bản tương đương EVM (Máy ảo Ethereum), cho phép các ứng dụng được tạo cho mạng chính Ethereum chạy trên Optimism về cơ bản mà không có thay đổi nào đối với cơ sở mã của chúng.\
\
Xin lưu ý rằng vì điều này, Optimistic không sử dụng mã thông báo gas của riêng mình mà sử dụng Ether như phí gas để thanh toán cho các giao dịch.

## Khởi động trên mạng Optimism

Trước khi sử dụng Optimism, bạn sẽ cần một địa chỉ ví. Vì Optimism là một mạng EVM, nó sẽ tương thích với các ví giống như trên các chuỗi EVM khác, bao gồm ví web như Metamask hoặc Nifty hoặc bạn có thể sử dụng ví phần cứng của mình như Trezor hoặc Ledger, nhưng bạn có thể phải theo dõi thêm các bước để có thể kết nối ví lạnh của bạn với mạng.

Đối với hướng dẫn này, chúng ta sẽ sử dụng với Metamask giống như chúng ta đã làm cho tất cả các hướng dẫn khác trên trang web này. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về [Cách bắt đầu trên Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Thêm Optimism vào Metamask

Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Thêm mạng. Bạn sẽ sử dụng thông tin sau trong các trường cần điền:

* **Network Name:** Optimism
* **New RPC URL:** [https://mainnet.optimism.io](https://mainnet.optimism.io)
* **Chain ID:** 10
* **Currency Symbol:** ETH
* **Block Explorer URL:** [https://optimistic.etherscan.io/](https://optimistic.etherscan.io/)

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang Optimism:

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.40.30 PM.png>)

## Kết nối tới Optimism

### Faucets

Không có bất cứ nguồn Faucets nào trên Optimism, nhưng nếu bạn sử dụng DApp như [ElkNet](https://app.elk.finance/#/elknet), bạn có thể chọn hoán đổi một số mã thông báo Elk của mình thành gas khi bắc cầu từ bất kỳ mạng nào được hỗ trợ.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.36.40 PM.png>)

### Các cầu nối

* [Multi Chain](https://app.multichain.org/#/router) là đối tác chính thức của Mai Finance nếu bạn muốn chuyển MAI hoặc QI của mình sang Optimism từ bất kỳ mạng nào khác. Từ mạng đã chọn của bạn, bạn chỉ cần chọn chuỗi đích (Optimism) và tài sản bạn muốn gửi (MAI hoặc ETH với số tiền chính xác và nhấp vào nút Chuyển. Hãy chú ý đến phí chuyển trực tiếp trên tài sản bạn đang chuyển.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.14.42 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) là một cầu nối phổ biến và là một trong những đối tác cầu nối chính thức cho mạng Optimism.
* [Hop Protocol](https://app.hop.exchange/#/send?token=ETH\&sourceNetwork=polygon\&destNetwork=optimism) là một cầu nối phổ biến khác cũng là đối tác chính thức của mạng Optimism. Chỉ có một số lượng nhỏ mã thông báo được hỗ trợ bao gồm ETH và các loại tiền ổn định khác nhau như USDC, DAI và USDT, nhưng nó cung cấp phí bắc cầu thấp hơn hầu hết các giải pháp khác.
* [Hashflow](https://app.hashflow.com/) là một công nghệ bắc cầu mới hơn, hoạt động về cơ bản như một DEX crosschain (trao đổi phi tập trung) cho bất kỳ mã thông báo nào có đủ thanh khoản. Ngoài ra, người dùng Hashflow hiện có thể kiếm được HFT (mã thông báo Hashflow) để hoán đổi hoặc cung cấp tính thanh khoản cho mã thông báo. Chuỗi hiện được giới hạn ở Ethereum, Avalanche, Arbitrum, Optimism, Polygon và BNB.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.51.25 PM.png>)

* [Elknet](https://app.elk.finance/#/elknet) sẽ hoạt động như một cầu nối và một faucet khi bạn chuyển mã thông báo ELK giữa 2 mạng. Bạn sẽ có thể bắc cầu ELK của mình và ở đầu nhận, bạn có thể có một phần nhỏ ELK của mình trực tiếp dưới dạng mã thông báo gas, ETH trong trường hợp của chúng tôi, như đã giải thích trong phần trên.

## DeFi trên Optimism

Để bắt đầu Optimism, đây là một số DApp mà bạn có thể thấy hữu ích để sử dụng MAI và QI của mình, bao gồm:

* [Curve](https://optimism.curve.fi/factory/4/deposit): Đây là nơi mà phần lớn thanh khoản MAI hiện đang tồn tại trên Optimism vì Curve cực kỳ hiệu quả trong việc thực hiện hoán đổi stablecoin.

Bằng cách gửi MAI vào Curve LP, sau đó bạn sẽ nhận được mã thông báo LP có thể được gửi vào hầm tiền Curve trên trang Farm của Mai Finance để kiếm được lợi nhuận từ mã thông báo QI.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.58.06 PM.png>)

* [Arrakis](https://beta.arrakis.finance/#/vaults/0x65Fbf30f29C7626385f78Dbc41702d97b9cD486a) gần đây đã ra mắt trên Optimism và đây là nơi bạn sẽ tìm thấy nhóm thanh khoản QI / WETH. Giao thức này hiện chưa được khởi động thanh khoản, nhưng sẽ cung cấp một trường hợp sử dụng bổ sung cho QI cho đến khi việc đặt cọc QI ra mắt trên mạng. Xin lưu ý rằng Arrakis sử dụng bể Uniswap nên bạn sẽ phải đặt cọc cả QI và WETH theo tỷ lệ được chỉ định vào bể thanh khoản.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.07.37 PM.png>)

* [BeethovenX](https://op.beets.fi/#/pool/0x3dc09db8e571da76dd04e9176afc7feee0b89106000000000000000000000019), một fork Balancer chính thức được chấp nhận, ra mắt trên Optimism vào tháng 6 năm 2022 và cung cấp một bể stablecoin thanh khoản cao hoàn toàn mới có tên là "Come Together", bao gồm FRAX, USDC và MAI. Do phần thưởng lớn bao gồm mã thông báo QI, BEETS và BAL, nó chắc chắn sẽ trở thành bể stablecoin trên thực tế cho MAI trên Optimism.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 10.09.43 PM.png>)

## Mai Finance trên Optimism

Nền tảng cho vay đã có sẵn trên Optimism, nơi bạn sẽ có thể gửi mã thông báo WETH (Ether được bọc) hoặc WBTC (Bitcoin được bọc) vào một kho tiền làm thế chấp và mượn thêm MAI. MAI có thể được gửi vào bể thanh khoản Curve để kiếm QI hoặc bể ổn định FRAX / USDC / MAI mới trên BeethovenX mới ra mắt gần đây để kiếm phần thưởng là các mã thông báo QI, BEETS và BAL.

![](<../../.gitbook/assets/Screen Shot 2022-06-17 at 9.56.07 PM.png>)

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
