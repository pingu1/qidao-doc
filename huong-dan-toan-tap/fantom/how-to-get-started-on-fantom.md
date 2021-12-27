---
description: >-
  Trong hướng dẫn này chúng tôi sẽ giải thích tất cả những gì bạn cần phải biết
  để bắt đầu trên mạng Fantom.
---

# Cách bắt đầu trên mạng Fantom

## Fantom là gì?

Fantom là một giải pháp thay thế Ethereum cho các nhà thiết kế blockchain. Là một blockchain hỗ trợ hợp đồng thông minh mã nguồn mở, nó cho phép các nhà thiết kế phát triển an toàn, toàn diện và mô-đun DApps (Ứng dụng phân cấp).

Chuỗi đã được thiết kế để khắc phục tất cả các hạn chế của thế hệ nền tảng blockchain trước đây, đôi khi được coi là thế mắc kẹt blockchain bao gồm: phân quyền, bảo mật và khả năng mở rộng. Để cải thiện một trong những khía cạnh này, sẽ phải trả giá bằng một trong hai khía cạnh còn lại. Fantom đã cố gắng giải quyết vấn đề này nhờ cơ chế đồng thuận Lachesis aBFT (Byzantine Fault Tolerant không đồng bộ) dựa trên DAG (Đồ thị Acyclic), cho phép nó có hiệu suất cao, có thể mở rộng và an toàn. Các tiêu chuẩn ban đầu cho thấy Fantom có thể dễ dàng xử lý hơn 20.000 giao dịch mỗi giây.

Cuối cùng, Fantom tương thích 100% EVM (Máy ảo Ethereum), có nghĩa là các DApp đã được phát triển trên các mạng tương thích EVM cũng sẽ có thể triển khai trên Fantom. Điều này cũng mang lại một lợi thế khác cho người dùng vì MetaMask và các ứng dụng web3 khác cũng tương thích với Fantom. Bạn sẽ có thể chuyển đổi liền mạch từ Polygon hoặc Avalanche sang Fantom trong cùng một ví.

## Khởi động trên Fantom

Fantom tương thích với EVM, nếu bạn đã có ví cho các chuỗi EVM khác (Ethereum Mainnet, Polygon hoặc Avalanche), bạn sẽ có thể sử dụng nó. Nếu không, đã đến lúc tạo một địa chỉ ví. Có thể sử dụng các loại ví khác nhau: ví phần mềm như Metamask hoặc [fWallet](https://pwawallet.fantom.network/#/), hoặc ví phần cứng như [Trezor](https://trezor.io/coins/) hoặc [Ledger.](how-to-get-started-on-fantom.md#what-is-fantom)

Bởi vì chúng tôi đang sử dụng Metamask trong tất cả các hướng dẫn khác, chúng ta sẽ sử dụng Metamask, nhưng hãy thoải mái sử dụng bất kỳ ví phần mềm / phần cứng nào khác mà bạn thích. Nếu bạn cần hướng dẫn về cách cài đặt Metamask, bạn có thể tìm hướng dẫn trên các bước [bắt đầu tại Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Thêm mạng Fantom vào Metamask

Để sử dụng mạng Fantom, bạn sẽ cài đặt cấu hình thủ công nó vào Metamask. Để làm như vậy, hãy nhấp vào menu thả xuống ở đầu cửa sổ Metamask (nơi nó cho biết mạng bạn hiện đang sử dụng, Ethereum Mainnet theo mặc định), sau đó chọn RPC tùy chỉnh. Các thông tin sau là những thông tin sẽ cho phép bạn kết nối với Fantom:

* **Network Name**: Fantom Opera
* **RPC URL**: https://rpc.ftm.tools/
* **ChainID**: 250
* **Symbol**: FTM
* **Explorer**: https://ftmscan.com

Sau khi lưu các thay đổi của bạn, Metamask sẽ tự động chuyển sang mạng Fantom.

![Good job! You're on Fantom!](../../.gitbook/assets/ftm-mm0.png)

Nếu bạn cần thêm chi tiết để thiết lập Metamask, bạn sẽ tìm thấy thông tin bổ sung trên[ hướng dẫn Fantom chính thức .](how-to-get-started-on-fantom.md#what-is-fantom)

### FTM faucet

Bây giờ bạn đang sử dụng FTM, bạn sẽ cần một số FTM (mã thông báo gốc được sử dụng để tphí gas ban đầu). Bạn có thể kết nối một số mã thông báo FTM từ các chuỗi khác hoặc sử dụng faucet sẽ gửi đủ mã thông báo FTM vào ví của bạn để thực hiện một số giao dịch. [Faucet trên Fantom ](how-to-get-started-on-fantom.md#bridging-to-fantom)có thể được tìm thấy trên SpookySwap, một trong những DEX chính ở đó (Sàn giao dịch phi tập trung). Lưu ý rằng đó là một dịch vụ do SpookySwap cung cấp dựa trên Discord và điều đó sẽ yêu cầu Tài khoản Discord hợp lệ hoạt động trong hơn 30 ngày (tuy nhiên, nó không bắt buộc phải ở trên máy chủ SpookySwap Discord trong 30 ngày).

* Sau khi bạn tham gia máy chủ [SpookySwap Discord ](https://docs.spookyswap.finance/getting-started/how-to-get-fantom-gas)và xác minh tài khoản của mình, hãy chuyển đến phần #faucet.

![](<../../.gitbook/assets/image (42).png>)

* Trong kênh #faucet, chỉ cần nhập lệnh! Faucet và bot sẽ gửi cho bạn một số $ FTM. Lưu ý rằng bạn sẽ bị giới hạn 1 lần tương tác sau mỗi 30 ngày.
* Nếu bạn muốn xác minh rằng bạn đã nhận đúng mã thông báo FTM của mình, bạn có thể nhấp vào tên Fantom Tip Bot để tương tác trực tiếp với nó và nhập !balance

![Thank you Fantom Tip Bot and SpookySwap](<../../.gitbook/assets/image (45).png>)

* Tất cả những gì bạn cần làm bây giờ là gửi mã thông báo FTM đến địa chỉ ví của bạn bằng lệnh! Withdraw<địa chỉ ví của bạn>. Bạn sẽ tìm thấy địa chỉ ví của mình ở đầu cửa sổ Metamask.

![Rút từ tài khoản Discord](../../.gitbook/assets/ftm-faucet.png)

![Tiền gửi mới nhận trên ví Metamask](../../.gitbook/assets/ftm-mm.png)

## Kết  nối tới Fantom

### Cầu nối đồng ổn định / ETH / BTC

Nếu bạn muốn kết nối các đồng tiền ổn định với Fantom, bạn có thể sử dụng danh sách các cầu nối sau:

* [AnySwap](https://anyswap.exchange/#/bridge): Đây là cầu nối chính thức được hỗ trợ để gửi MAI mà bạn đã đúc trên Polygon đến Fantom (xem [hướng dẫn MAI](how-to-get-started-on-fantom.md#what-is-fantom) để biết chi tiết). Giải pháp này hỗ trợ nhiều tài sản và nhiều chuỗi để bạn dễ dàng gửi tiền điện tử của mình đến Fantom. Vui lòng kiểm tra ghi chú Nhắc nhở ở cuối giao diện bắc cầu để biết chi tiết phí giao dịch và thời gian thực hiện dự kiến.

![Mang MAI sang Fantom](<../../.gitbook/assets/image (43).png>)

* [Celer Bridge](https://cbridge.celer.network/#/): cung cấp dịch vụ cầu nối cho nhiều chuỗi đối với hầu hết các đồng tiền ổn định, với phí dao động từ 0,04% đến 0,19% để kết nối với Fantom (DYOR).
* [xpollinate](https://www.xpollinate.io): phí thấp và đảm bảo rằng có đủ thanh khoản trên chuỗi mục tiêu cho mã thông báo bạn muốn làm cầu nối. Thanh khoản càng thấp (hoặc số lượng cầu nối càng lớn), thời gian chuyển càng dài.

### Cầu nối cho một số tài sản khác

* Binance CEX: Bạn sẽ có thể mua mã thông báo FTM trên Binance và kết nối trực tiếp với Fantom, nhưng đây là mã thông báo duy nhất bạn có thể chuyển.
* [SpookySwap](https://spookyswap.finance/bridge): hỗ trợ nhiều mạng và nhiều mã thông báo mà bạn sẽ có thể gửi đến Fantom.
* AnySwap: xem mô tả được thực hiện trong phần đồng ổn định.

## DeFi trên Fantom

Fantom đã chứng kiến sự mở rộng khá ấn tượng vào cuối mùa hè năm 2021, đặc biệt là với các chương trình kích thích đã giúp thu hút các nhà đầu tư và nhà phát triển trên chuỗi. Sự tăng trưởng cũng được hỗ trợ bởi các dự án blue chip đã triển khai DApp của họ trên Fantom vào tháng 9 năm 2021, bao gồm Curve và SushiSwap.

* [BeethovenX](https://app.beethovenx.io/#/): Ứng dụng này rất giống với Balancer. Bạn sẽ có thể giao dịch một số mã thông báo cho những người dùng khác và cũng có thể tham gia các bể cân bằng bao gồm nhiều mã thông báo. Đây cũng là đối tác chính thức đầu tiên của Mai Finance trên Fantom và là nơi duy nhất mà bạn có thể hoán đổi MAI của mình hoặc sử dụng chúng trong nhóm MAI-USDC.

![Đổi MAI thành FTM](<../../.gitbook/assets/image (44).png>)

* [SpookySwap](https://spookyswap.finance): Đây là DEX (Sàn giao dịch phi tập trung) lớn nhất trên Fantom, nơi bạn sẽ có thể hoán đổi mã thông báo của mình cho người dùng khác, ký gửi thanh khoản  và canh tác lợi nhuận, giống như cách bạn làm trên QuickSwap trên Polygon. SpookySwap sẽ thưởng cho bạn bằng cách sử dụng mã thông báo BOO, mã thông báo gốc của nền tảng. Lưu ý thêm, khi bạn đặt cọc mã thông báo BOO của mình, bạn sẽ nhận được xBOO, một mã thông báo lợi nhuận, để đổi lại và bạn có thể sử dụng chúng để kiếm thêm phần thưởng (nguyên tắc giống như Dragon's Syrup trên QuickSwap).
* [SpiritSwap](https://app.spiritswap.finance): AMM truyền thống và nền tảng canh tác lợi suất, nơi bạn sẽ có thể hoán đổi mã thông báo, tạo mã thông báo LP và canh tác lợi nhuận trong các bể thanh khoản. SpiritSwap sẽ thanh toán cho bạn bằng mã thông báo SPIRIT mà bạn có thể đặt cọc trên nền tảng và nhận mã thông báo inSPIRIT (SPIRIT sẽ bị khóa trong một khoảng thời gian nhất định), chủ yếu của mã thông báo veCRV. Bạn cũng có thể sử dụng SpiritSwap để cho vay và mượn trong khi chờ Mai Finance trên Fantom.
* [Tarot](https://www.tarot.to): Tarot là phiên bản Fantom của Impermax, nơi bạn sẽ có thể sử dụng mã thông báo LP của mình từ SpookySwap (hoặc các DEX / AMM khác) và sử dụng chúng để farm trên nền tảng. Bạn cũng có thể gửi các mã thông báo đơn lẻ và cho vay chúng trên các bể cụ thể, nơi mọi người sẽ có thể vay chúng để tạo mã thông báo LP mới và tận dụng số tiền thanh khoản của họ. Hãy lưu ý về việc thanh lý nếu bạn tạo đòn bẩy LP của mình trong một bể mà khả năng sử dụng cao.
* [Scream](https://scream.sh): Đây là một bản sao của Compound, nơi bạn có thể cho mượn mã thông báo của mình và vay ngược lại chúng. Việc cho mượn mã thông báo của bạn sẽ khiến bạn kiếm được phần thưởng bằng mã thông báo bạn cho mượn, cũng như mã thông báo SCREAM mà bạn sẽ có thể sử dụng trên các nền tảng khác.
* [Curve](how-to-get-started-on-fantom.md#bridging-stable-coins-eth-btc): Curve là dự án blue chip mà mọi người đều biết rõ, nơi bạn sẽ có thể gửi mã thông báo của mình vào các bể cụ thể (không cần gửi số tiền cân bằng) và bạn sẽ được thưởng bằng mã thông báo bạn cho vay, cũng như mã thông báo CRV và wFTM.

![Bể kép DAI + USDC trên Curve on Fantom](../../.gitbook/assets/ftm-crv.png)

Có rất nhiều cơ hội khác trên Fantom sẽ được mô tả trong các hướng dẫn khác.

## Một số liên kết hữu ích khác

* [Fantom explorer](https://explorer.fantom.network)
* [Fantom gas checker](https://ftmscan.com/gastracker)
* Official [Fantom Discord](how-to-get-started-on-fantom.md#ftm-faucet) server
* [DeBank](https://debank.com) portfolio managed

## Tuyên bố từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Các dự án được trình bày trong hướng dẫn này hoặc chỉ giới thiệu các khả năng trên mạng Fantom và bạn không nên coi đó là chứng thực tin cậy cho dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
