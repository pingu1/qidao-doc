---
description: >-
  Trong hướng dẫn này, chúng tôi sẽ giải thích mọi thứ bạn cần biết để bắt đầu
  sử dụng chuỗi Harmony.
---

# Khởi động trên Harmony

## Harmony là gì ?

Harmony là một blockchain cố gắng giải quyết các vấn đề mà Ethereum Mainnet đangphải đối mặt: đạt được mức độ cân bằng thỏa mãn giữa phân cấp và khả năng mở rộng. Trọng tâm chính của chuỗi là tập trung vào thông lượng giao dịch cao, tốc độ và hiệu quả năng lượng. Điều này được thực hiện bằng cách tận dụng lợi thế cao của các trình xác thực sẽ được nhóm lại để xử lý các giao dịch đồng thời. Hỗ trợ khả năng mở rộng chỉ đơn giản là tăng số lượng phân đoạn, điều này cũng giúp đạt được giao dịch nhanh hơn. Vui lòng tìm hiểu thêm về Harmony và công nghệ của nó [trong tài liệu chính thức của họ.](https://docs.harmony.one/home/general/technology)

## Khởi động trên Harmony

Để sử dụng mạng Harmony, bạn sẽ cần một địa chỉ ví. Vì Harmony là mạng tương thích với EVM (Máy ảo Ethereum), nó sẽ chấp nhận các ví tương tự như trên các chuỗi tương thích với EVM khác, bao gồm ví web như Metamask hoặc Nifty và bạn sẽ có thể sử dụng ví phần cứng của mình như Trezor hoặc Ledger.

Đối với hướng dẫn này, chúng tôi sẽ gắn bó với Metamask giống như tất cả các hướng dẫn khác trên trang web này. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về [Cách bắt đầu trên mạng Polygon](how-to-get-started-on-harmony.md#harmony).

### Thêm Harmony vào Metamask

Nếu bạn đã cài đặt phiên bản mới nhất của Metamask, bạn đã có quyền truy cập vào chuỗi Harmony và không có gì khác để bạn thực hiện ngoài việc chọn Harmony One trong menu thả xuống mạng ở đầu Metamask. Bạn cũng có thể tự thiết lập một RPC mới để truy cập Harmony bằng các bước sau. Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Harmony One. Dữ liệu bạn sẽ nhận được như sau:

* **Tên mạng:** Harmony One
* **RPC URL mới:** https://api.harmony.one
* **ID chuỗi:** 1666600000
* **Biểu tượng tiền tệ:** ONE
* **Trình khám phá chuỗi URL:** https://explorer.harmony.one/

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang mạng Harmony:

![Xin chúc mừng!! bạn đã trên Harmony](../../.gitbook/assets/Harmony-onboarding-1.png)

## Cấu nối tới Harmony One

### Faucets

Không có bất kỳ faucet chính thức nào để nhận ONE mã thông báo đầu tiên của bạn cho một vài giao dịch đầu tiên của bạn. Bạn hầu như sẽ phải bắc cầu một số mã thông báo từ một chuỗi khác bằng cách sử dụng [cầu Harmony](https://bridge.harmony.one/erc20) chính thức cho phép bạn kết nối một số tài sản cụ thể từ Ehtereum Mainnet hoặc Binance sang Harmony. Bạn cũng có thể nhận được danh sách các dự án sẽ cho phép bạn nhận được ONE thông qua Fiat Gateways hoặc Exchange Gateways từ [danh sách này](https://docs.harmony.one/home/developers/harmony-stack#bridges-fiat-gateways-exchanges) do nhóm Harmony quản lý.

Như mọi khi, bạn cũng có thể sử dụng [ElkNet ](https://app.elk.finance/#/elknet)để chuyển một số mã thông báo ELK từ các chuỗi khác sang Harmony. Nếu bạn làm như vậy, hãy đảm bảo chọn tag đổi $ ELK 1 lấy gas sẽ hoán đổi một phần mã thông báo đã chuyển của bạn thành mã ONE, điều này cũng sẽ cho phép bạn hoán đổi phần còn lại của mã thông báo ELK của mình sang nhiều ONE hoặc tài sản khác.

### Các cầu nối

* [Multichain.org](https://app.multichain.org/#/router) (được biết trước đây AnySwap) là đối tác chính thức của Mai Finance sẽ cho phép bạn kết nối các mã thông báo MAI của bạn từ Polygon và các chuỗi khác với Harmony. Lưu ý thêm, Multichain đã hợp tác với các nhà phát triển của Mai Finance để đảm bảo rằng MAI mà bạn làm cầu nối với Harmony cũng giống như những gì bạn sẽ có thể vay từ nền tảng cho vay. Không cần phải có Hub trên Harmony. Chỉ cần đi đến bộ định tuyến Multichain, chọn mạng gốc, mã thông báo bạn muốn chuyển và mạng đích là xong. Hãy chú ý đến số tiền tối thiểu để chuyển, phí chuyển và thời gian chuyển tiền, nhưng sau khi hoàn tất, bạn sẽ nhận được tài sản của mình trên Harmony.

![Đưa MAI từ Polygon tới Harmony One](../../.gitbook/assets/Harmony-onboarding-2.png)

* [Official Harmony Bridge](https://bridge.harmony.one/erc20), như đã giải thích trong đoạn trước, sẽ cho phép bạn chuyển các tài sản cụ thể từ Ethereum Mainnet hoặc BSC.
* [RelayChain](https://app.relaychain.com/#/cross-chain-bridge-transfer) là một giải pháp khác nếu bạn muốn chuyển một thứ gì đó sang Harmony. Kiểm tra ứng dụng của họ để xem tài sản nào có thể bắc cầu.
* [ElkNet](https://app.elk.finance/#/elknet) là một trường hợp cụ thể vì cầu nối từ Elk Finance sẽ cho phép bạn kết nối mã thông báo ELK từ bất kỳ chuỗi tương thích EVM nào với bất kỳ chuỗi tương thích EVM nào khác, nơi chúng được triển khai với khả năng hoán đổi một phần nhỏ số tiền đã chuyển thành phí gas (xem phần dành riêng cho faucets ở trên).

## DeFi trên Harmony

Bởi vì Harmony One là một mạng có giao dịch nhanh chóng và an toàn, cũng như giá gas rất rẻ, rất nhiều DApp tương thích với EVM (Ứng dụng phi tập trung) đã được triển khai cho mạng này. Danh sách sau không trình bày tất cả, hãy tự khám phá mạng và danh sách DApps. Bạn có thể tham khảo danh sách [đầy đủ hơn trên DefiLlama](https://defillama.com/chain/Harmony).

* [ViperSwap](https://viper.exchange/#/swap): Đây là đối tác đầu tiên của Mai Finance trên Harmony One. Đây là bản fork Uniswap v2, một DEX (Sàn giao dịch phi tập trung) và AMM (Nhà tạo thị trường tự động), nơi bạn có thể hoán đổi tài sản của mình, tạo mã thông báo LP (Cung cấp thanh khoản) và nhận phần thưởng bằng cách cung cấp thanh khoản cho các nhà giao dịch. Phần thưởng được trả bằng mã thông báo VIPER, bạn sẽ có thể đặt cọc vào nền tảng để nhận được nhiều phần thưởng hơn. Đây là DEX nơi bạn sẽ tìm thấy một số bể thanh khoản với MAI.&#x20;

![Các bể MAI-ONE và MAI-VIPER trên ViperSwap kể từ tháng 12 năm 2021](../../.gitbook/assets/Harmony-onboarding-3.png)

Bạn sẽ lưu ý rằng APR (Tỷ lệ phần trăm hàng năm) trên các bể rất cao. Điều này chủ yếu là do cách phân phối phần thưởng trên ViperSwap: khi bạn nhận phần thưởng của mình, 5% mã thông báo VIPER có thể được sử dụng trực tiếp, trong khi 95% nếu bị khóa cho đến năm 2021-12-25. Sau đó, phần thưởng sẽ khóa trong một năm đầy đủ, có nghĩa là bạn sẽ không thể truy cập ngay lợi nhuận từ việc trồng trọt của mình và nó sẽ nhỏ giọt rất chậm. Có một bước ngoặt khác đối với các bể ViperSwap: bạn sẽ phải trả phí rút tiền sẽ giảm xuống nếu bạn đặt cọc các token LP của mình trong một thời gian dài. Phí chuyển từ 25% nếu bạn rút trong cùng một khối với giao dịch gửi tiền (để chống lại các hoạt động flashloan) thành 0,01% nếu bạn rút sau 1 tháng. Thêm chi tiết trong [tài liệu chính thức](https://docs.venomdao.org/viper/tokenomics#bbd0) của họ về phần thưởng và [phí rút LP](https://docs.venomdao.org/viper/fees).

* [DeFi Kingdom](https://game.defikingdoms.com/#/): Đây là một dự án đặc biệt thú vị được kết hợp giữa DeFi và Gamification. Mã thông báo gốc của nó JEWEL, được sử dụng làm phần thưởng cung cấp thanh khoản cho những người dùng đang cung cấp tính thanh khoản, nhưng nó có thể được sử dụng trong trò chơi hoặc trên thị trường. Việc giải thích toàn bộ vũ trụ của DeFi Kingdom (hoặc DFK) sẽ mất quá nhiều thời gian cho hướng dẫn này, vì vậy chúng tôi đặc biệt khuyên bạn nên đọc tài liệu chính thức.

![Bản đồ chính của DeFi Kingdom tại thời điểm tháng 11 2021](../../.gitbook/assets/Harmony-onboarding-4.png)

* [SushiSwap](https://app.sushi.com) là DEX / AMM nổi tiếng cũng có mặt trên nhiều chuỗi khác. Hoán đổi, cung cấp thanh khoản, cung cấp thanh khoản ONE và lợi nhuận SUSHI.
* [Curve Finance](https://harmony.curve.fi/) là một ứng dụng chuỗi chéo khác sẽ cho phép bạn cung cấp thanh khoản (3pool và tricrypto) và sẽ thưởng cho bạn các mã thông báo cộng dồn, cũng như ONE và CRV.
* [Beefy Finance](https://app.beefy.finance/#/harmony) là một công cụ tối ưu hóa lợi nhuận mà chúng tôi đã trình bày trong nhiều hướng dẫn trước vì nó có mặt trên nhiều chuỗi. Hiện tại, bạn sẽ có thể gửi mã thông báo LP của mình từ Curve và SushiSwap, đồng thời để công cụ cộng dồn Beefy tổng hợp phần thưởng do nền tảng canh tác cung cấp thành nhiều mã thông báo LP hơn.
* [Euphoria DAO](https://app.euphoria.money/#/dashboard) hiện là Ohm-fork lớn nhất trên Harmony và được phát triển bởi Venom DAO cũng đứng sau ViperSwap. Bạn có thể phát hành trái phiếu một số tài sản khác nhau và nhận tài sản gốc của chúng, mã thông báo WAGMI. Đặt cọc WAGMI để có thêm WAGMI với APY điên rồ (Tỷ lệ phần trăm hàng năm) như đối với hầu hết các dự án OHM.

## Mai Finance trên Harmony

Mai Finance đã ra mắt trên Harmony One vào tháng 12 năm 2021 và hướng dẫn này khá gần với ngày ra mắt nên ứng dụng có thể đã được cập nhật.&#x20;

Bạn sẽ có thể gửi WETH hoặc ONE token của mình trên Mai Finance (https://app.mai.finance/vaults/create) để vay đồng tiền ổn định MAI. Sau đó, bạn sẽ có thể hoán đổi MAI để tận dụng tài sản của mình, giao dịch ký quỹ hoặc canh tác lợi tức trên ViperSwap.

![Hầm tiền MAI Finance tại thời điểm tháng 12 năm 2021](../../.gitbook/assets/Harmony-onboarding-5.png)

## Tuyên bố từ chối trách nhiệm

Như thường lệ, hướng dẫn này không phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
