---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ giải thích tất cả những gì bạn cần phải biết
  để bắt đầu trên mạng Moonriver.
---

# Các bước bắt đầu trên Moonriver

## Moonriver là gì?

Sẽ rất phức tạp để hiểu rõ Moonriver là gì nếu không đề cập đến Polkadot, Moonbeam và Kusama.

Polkadot là chuỗi khối lớp 1 được tạo nhằm cạnh tranh trực tiếp với Ethereum, Cosmos hay EOS trong việc phát triển và hoàn thiện hệ sinh thái hoàn chỉnh cho tiền điện tử và các ứng dụng liên quan. Một trong những khác biệt chính khiến Polkadot khác biệt với các chuỗi khối lớp 1 khác là sự tách biệt giữa chuỗi chính, chuỗi chuyển tiếp(relay chain) và các chuỗi khối do người dùng tạo nên (Parachains). Chuỗi chuyển tiếp thừa hưởng từ các lợi thế từ các yêu cầu thấp về tài nguyên tính toán vì hầu hết các phát triển và nâng cấp được thực hiện trên các parachain này. Mặt khác, các parachain này thừa hưởng trọn vẹn tính bảo mật từ mạng chuyển tiếp. Điều này cũng tạo ra các môi trường biệt lập có thể hoạt động độc lập mà không cần thiết phải tiết lộ thông tin người dùng cho chuỗi chính.&#x20;

Kusama là môi trường tiền thử nghiệm cho cho chuỗi Polkadot,  một chuỗi tách biệt được mô phỏng chuỗi chuyển tiếp của Polkadot nơi tất cả các phát triển và nâng cấp cho chuỗi chính được thử nghiệm đầu tiên. Tuy nhiên Kusama vận hành bằng tiền thực và các giao dịch cũng là thực nhưng với quy tắc "dễ thở" hơn so với Polkadot. Tuy nhiên, mục tiêu cuối cùng của các ứng dụng là được chuyển sang Polkadot tại một thời điểm nào đó. Với các nguyên tắc "dễ thở" này, các dự án vẫn có thể thử nghiệm giao thức của mình trong khi xây dựng cộng đồng. Một khi sản phẩm cuối cùng được hoàn thiện thì nó sẽ được chuyển sang môi trường chính.&#x20;

Moonriver thực sự là một parachain trên Kusama. Các mã triển khai trên Moonriver chính là bản thử nghiệm có thể được triển khai chính thức trên Moonbeam, sản phẩm hoàn thiện trên Polkadot. Bởi vì cả Moonbeam và Moonriver là 2 chuỗi tương thích với EVM nên sẽ chấp nhận tất cả các hợp đồng thông minh từ các chuỗi tương thích với Ethereum. Chính đặc trưng này khiến Moonriver và Moonbeam trở thành điểm đến của nhiều Daap từ các chuỗi tương thích với Ethereum khác như Polygon, Avalanche, Fantom để mở rộng sang Polkadot thông qua các parachain này.&#x20;

Cũng như các chuỗi khối EVM tương thích khác, Moonriver sử dụng mã thông báo MOVR làm phí gas để xác nhận giao dịch.&#x20;

## Bắt đầu trên Moonriver

Trước khi sử dụng Moonriver bạn cần một địa chỉ ví, bởi vì chuỗi Moonriver là EVM tương thích nên nó chấp nhận các ví tương tự trên các chuỗi EVM khác bao gồm cả ví mềm như Metamask hoặc Nifty và ví cứng như Trezor và Ledger. Tuy nhiên bạn cần một số bước để kết nối ví lạnh.  Bạn có thể tìm thấy hướng dẫn từng bước rất rõ ràng trên [tài liệu của Moonbeam.](https://moonbeam.foundation/tutorials/how-to-create-moonriver-ethereum-address/)

Đối với hướng dẫn này, chúng ta sẽ sử dụng Metamask giống như tất cả các hướng dẫn khác. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về[ Cách bắt đầu với Polygon.](how-to-get-started-on-moonriver.md#moonriver-la-gi)

### Thêm Moonriver vào Metamask

Về lý thuyết, Moonriver được cài đặt sẵn MetaMask, có nghĩa là bạn không cần phải thêm thông tin chuỗi để Metamask hoạt động. Tuy nhiên, có thể là một ý tưởng hay để xác minh rằng thiết lập của bạn là chính xác bằng cách kiểm tra kỹ các giá trị được lưu vào ví cục bộ của bạn. Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Moonriver. Dữ liệu bạn sẽ nhận được như sau:

* **Tên mạng:** Moonriver
* **New RPC URL:** https://rpc.moonriver.moonbeam.network
* &#x20;**ID chuỗi:** 1285
* **Mã thông báo:** MOVR
* **Trình khám phá chuỗi URL:** https://blockscout.moonriver.moonbeam.network/

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang mạng Moonriver:

![Xin chúc mứng. Bạn đã ở mạng Moonriver](../../.gitbook/assets/Moonriver-setup-MM.png)

## Bắc cầu sang Moonriver

### Faucets

Một trong những DEX lớn nhất trên Moonriver, SolarBeam, cung cấp [hoán đổi giao dịch không cần gas](how-to-get-started-on-moonriver.md#moonriver-la-gi) trong trường hợp bạn không có gas. Điều này cũng giả sử bạn có một số tiền trên Moonriver, nhưng không thể làm gì vì bạn có 0 MOVR trong ví của mình.

![Giao dịch không cần gas cho phép bạn đổi lấy gas](../../.gitbook/assets/Moonriver-faucet.png)

Lưu ý rằng chỉ một số tài sản nhất định mới được chấp nhận cho giao dịch không cần gas này và MAI không phải là một phần của các đồng tiền được hỗ trỗi

### Các cầu nối

* [Relay Chain](https://app.relaychain.com/transfer#/) là đối tác chính thức của Mai Finance nếu bạn muốn chuyển MAI của mình sang Moonriver từ Polygon. Khi bạn đã kết nối với Polygon, bạn có thể chỉ cần chọn chuỗi đích (Moonriver) và tài sản bạn muốn gửi (MAI hoặc miMATIC) với số tiền chính xác và nhấp vào nút Transfer. Cần lưu ý đến phí chuyển tiền.

![Bắc cầu MAI từ Polygon sang Moonriver](../../.gitbook/assets/Moonriver-relaychain.png)

* Nếu bạn cần kết nối các tài sản khác từ mạng khác, bạn có thể sử dụng Relay Chain (xem ở trên),[ AnySwap](https://anyswap.exchange/#/bridge) nếu bạn muốn kết nối từ ETH Mainnet đến Moonriver và tất nhiên bạn cũng có thể sử dụng tính năng [cầu nối](https://app.solarbeam.io/bridge) từ Solarbeam.
* Một lưu ý đặc biệt cho [Elknet](https://app.elk.finance/#/elknet) sẽ hoạt động như một cầu nối và một nguồn faucet khi bạn chuyển mã thông báo ELK giữa 2 mạng. Bạn sẽ có thể làm cầu nối ELK của mình và ở đầu nhận, bạn có thể có một phần nhỏ ELK của mình trực tiếp dưới dạng mã thông báo gas, MOVR trong trường hợp của chúng tôi.

### Trung tâm trung chuyển

Trong trường hợp bạn bắc cầu một số MAI từ Polygon đến Moonriver thông qua Relay Chain, bạn sẽ nhận được phiên bản RelayChain của MAI thay vì MAI gốc do ứng dụng trên Moonriver tạo ra. Hai mã thông báo (một từ RelayChain và một từ Mai Finance) có cùng giá trị và cùng tên, nhưng địa chỉ hợp đồng khác nhau, và mã duy nhất sẽ được chấp nhận để farming trên Moonriver là từ Mai Finance.

Bạn có thể hoán đổi MAI của mình từ Relay Chain bằng cách sử dụng [trung tâm trung chuyển](https://app.mai.finance/hub) trên Mai Finance với tỷ lệ 1: 1, sau đó bạn sẽ có thể sử dụng MAI thực sự của mình trên các nền tảng khác.

![Sử dụng trung tâm trung chuyển để chuyển MAI (RelayChain) thành MAI từ Mai Finance](../../.gitbook/assets/Moonriver-hub.png)

{% hint style="info" %}
Xin lưu ý thêm, nếu bạn muốn chuyển MAI của mình từ Moonriver sang Polygon hoặc các chuỗi khác, trước tiên bạn sẽ phải chuyển đổi chúng thành phiên bản RelayChain.
{% endhint %}

## DeFi trên Moonriver

Moonriver đang nhận được rất nhiều sức hấp và ngày càng có nhiều ứng dụng chuyển sang chuỗi mới này, với tiềm năng chuyển hoàn toàn sang Polkadot. Như vậy, bạn sẽ có thể cung cấp thanh khoản trên nền tảng sau (danh sách hiện chưa đầy đủ):

* [Solarbeam](https://app.solarbeam.io): Đây là DEX và AMM chính trên Moonriver. Bạn sẽ có thể hoán đổi tài sản của mình, tham gia khai thác thanh khoản bằng cách cung cấp các cặp LP (Cung cấp tính thanh khoản) trong các bể hoặc gửi cổ phần mã thông báo gốc của nền tảng. Solarbeam cũng là một trong những đối tác đầu tiên của Mai Finance trên Moonriver, và bạn sẽ có thể farm cặp MAI-MOVR. Bạn cũng sẽ tìm thấy nhóm MAI-USDC không nhận được bất kỳ phần thưởng nào nhưng có thể nhận được một số phí giao dịch.

![Các bể LP bao gồm MAI trên Solarbeam kể từ tháng 12 năm 2021](../../.gitbook/assets/Moonriver-solarbeam.png)

Khi bạn farm trên Solarbeam, bạn sẽ được thưởng bằng mã thông báo SOLAR mà sau đó bạn có thể đặt  vào Vault trong một khoảng thời gian nhất định và nhận thêm mã thông báo SOLAR hoặc đặt cổ phần để đạt được các mã thông báo khác trên nền tảng.

* [Huckleberry Finance](https://www.huckleberry.finance): Đây là một DEX / AMM khác trên Moonriver, nơi bạn sẽ có thể thu được sản lợi nhuận và có thể sử dụng Beefy để cộng dồn lợi nhuận.
* [Beefy Finance](https://app.beefy.finance/#/moonriver): Công cụ cộng dồn tự động nổi tiếng cũng có trên Moonriver và sẽ giúp bạn gộp số tiền kiếm được từ cả Solarbeam và Huckleberry. Lưu ý thêm, Beefy không đề xuất cặp MAI-MOVR khi viết bài, nhưng bạn có thể sớm sử dụng Beefy để thu thập mã thông báo SOLAR và nhận thêm MAI-MOVR.
* [Sushiswap](https://app.sushi.com): Không cần trình bày nhiều về SushiSwap! Bạn sẽ có thể hoán đổi tài sản và cung cấp thanh khỏa của mình cho một số mã thông báo LP nhất định giống như bạn làm trên bất kỳ chuỗi nào khác. Phần thưởng được cấp trong SUSHI và MOVR.
* [Rome DAO](https://romedao.finance): Đây là OHM-fork đầu tiên trên Moonriver. Liên kết tài sản của bạn để nhận mã thông báo ROME chiết khấu mà bạn có thể đặt cổ phầntrên để đạt được APY rất cao. Tại thời điểm viết bài, ROI trong 5 ngày là khoảng 10,6%. RomeDAO hiện chấp nhận FRAX và MIM trong kho quỹ của mình, nhưng cũng có thể sớm chấp nhận MAI.

## Mai Finance trên Moonriver

Nền tảng cho vay đã có sẵn trên Moonriver, nơi bạn sẽ có thể đặt mã thông báo mooSolarETH-USDC của mình vào một kho tiền và mượn MAI. Để làm như vậy

* Tạo một cặp ETH-USDC trên Solarbeam
* Gửi cặp ETH-USDC trên Beefy và nhận mã thông báo mooSolarETH-USDC
* Gửi số mooToken của bạn trên Mai Finance tại hầm tiền thích hợp

![Hầm tiên Mai Finance  Moonriver kể từ tháng 12 năm 2021](../../.gitbook/assets/Moonriver-vaults.png)

Hầm ETH cũng là một lựa chọn tốt.

Trong khi tài sản thế chấp của bạn đang kiếm được 44,08% APY từ Beefy Finance (tính đến thời điểm viết bài), bạn sẽ có thể vay MAI và farming cặp MAI-MOVR và nhận được 128% APR trên Solarbeam, hoặc 158,058% APY trên RomeDAO.

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
