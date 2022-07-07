---
description: Trong hướng dẫn này, chúng tôi sẽ giải thích cách bắt đầu sử dụng Moonbeam.
---

# Khởi động trên Moonbeam

## Moonbean là gì?

Ra mắt vào tháng 1 năm 2020, Moonbeam là một nền tảng hợp đồng thông minh tương thích EVM (máy ảo Ethereum) chạy trên mạng Polkadot, khiến nó được gọi là Polkadot parachain. Parachains là tập hợp các chuỗi được kết nối với nhau được hưởng lợi từ chuỗi chuyển tiếp chính của Polkadot trong khi vẫn có thể tương tác, do đó tham gia vào lợi ích và bảo mật của chuỗi chính trong khi chạy song song với nó.

\
Polkadot mô tả những lợi ích của parachains như sau, “Parachains kết thúc kỷ nguyên của các blockchain bị che khuất, tạo ra một mạng lưới blockchain được kết nối, phi tập trung mà trước đây chỉ tồn tại các mạng bị cô lập với các cộng đồng bộ lạc của riêng họ”.

![Moonbeam, a Polkadot parachain](<../../.gitbook/assets/moonbeam (1).jpg>)

Do lớp tương thích EVM của nó, Moonbeam giúp các nhà phát triển Solidity dễ dàng chuyển các ứng dụng hiện có của họ từ các mạng tương thích EVM khác sang Moonbeam với một vài thay đổi mã. Moonbeam hiện có TVL là 130 triệu đô la và một hệ sinh thái các [ứng dụng sôi động và phát triển mạnh.](https://defillama.com/chain/Moonbeam)

Moonbeat cũng cung cấp khả năng tương thích với Substrate. Substrate là một khuôn khổ blockchain mô-đun được các nhà phát triển sử dụng để xây dựng các blockchain phù hợp với nhu cầu của họ bằng cách sử dụng các thành phần có thể tái sử dụng được gọi là pallet. Nó sử dụng ngôn ngữ lập trình Rust và là khung mà hầu hết các nhà phát triển sử dụng khi xây dựng các parachains cho mạng Polkadot.

Vì Moonbeam là một blockchain dựa trên Substrate, các ứng dụng được tích hợp với mạng của nó được hưởng lợi từ khả năng tương tác giữa các chuỗi Polkadot và Ethereum, cũng như các chuỗi khác như Bitcoin.

Các nhà phát triển cũng có thể sử dụng các công cụ hệ sinh thái tương thích với Substrate thường được sử dụng trên Ethereum, bao gồm trình khám phá khối, thư viện phát triển front-end và ví, cũng như các công cụ phát triển như Truffle và Remix.

\
Mã thông báo gas gốc cho Moonbeam là GLMR.

## Khởi động trên Moonbeam

Trước khi sử dụng Moonbeam, bạn sẽ cần một địa chỉ ví. Vì Moonbeam là một mạng EVM, nó sẽ chấp nhận các ví giống như trên các chuỗi EVM khác, bao gồm ví web như Metamask hoặc Nifty và bạn sẽ có thể sử dụng ví phần cứng của mình như Trezor hoặc Ledger, nhưng bạn có thể phải thực hiện thêm các bước để có thể kết nối ví lạnh của bạn với mạng.

Đối với hướng dẫn này, chúng tôi sẽ gắn bó với Metamask giống như chúng tôi đã làm cho tất cả các hướng dẫn khác trên trang web này. Nếu bạn chưa cài đặt Metamask, bạn có thể tìm hướng dẫn về [Cách bắt đầu với Polygon.](../polygon/how-to-get-started-on-polygon.md)

### Thêm Moonbeam vào Metamask

Mở cửa sổ bật lên Metamask, nhấp vào biểu tượng ví của bạn, điều hướng đến Cài đặt, sau đó chọn Mạng và tìm Thêm mạng. Bạn sẽ sử dụng thông tin sau trong các trường văn bản có liên quan:

* **Network Name:** Moonbeam
* **New RPC URL:** [https://rpc.api.moonbeam.network](https://rpc.api.moonbeam.network)
* **Chain ID:** 128
* **Currency Symbol:** GLMR
* **Block Explorer URL:** [https://moonscan.io/](https://moonscan.io/)

Lưu các thay đổi và Metamask sẽ tự động chuyển bạn sang Moonbeam:

![Moonbeam on Metamask](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.34.43 PM.png>)

## Kết nối Moonbeam

### Faucets

GLMR là mã thông báo gas gốc của Moonbeam, vì vậy bạn sẽ cần có một số trong ví của mình để thực hiện các giao dịch trên chuỗi. May mắn thay, Faucet Moonbeam chính thức sẽ giúp bạn bắt đầu với một lượng nhỏ GLMR, mặc dù xin lưu ý rằng số lượng phân tán bằng mã thông báo đôi khi có thể không đủ để hoàn thành giao dịch nếu mạng bị tắc nghẽn.\
Để nhận được một số GLMR miễn phí, bạn cần xác minh bạn là người thông qua bot captcha và kết nối ví Metamask của bạn với trang web. Một số tiền nhỏ (0,007 GLMR) sau đó sẽ được gửi ngay lập tức vào ví của bạn.

![GLMR Faucet](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.57.39 PM.png>)

Ngoài ra, người dùng có thể muốn sử dụng tính năng "[Hoán đổi lấy phí gas](https://app.solarflare.io/bridge/gas-swap)" của Solarflare. Điều này cho phép người dùng hoán đổi các mã thông báo khác bao gồm WETH, WBTC, USDC, DAI, USDT, BUSD, FLARE và BNB thành GLMR, mã thông báo gas gốc của Moonbeam.

![Tính năng hoán đổi phí gas của Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.15.46 PM.png>)

### Cầu nối

* [Multichain](https://app.multichain.org/#/router) là cầu nối chính thức của MAI thông qua quan hệ đối tác với Qi Protocol, và bạn có thể dễ dàng gửi MAI của mình đến Moonbeam bằng cách sử dụng nó.

![Multichain trên Moonbeam](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.03.00 PM.png>)

* [Solarflare](https://app.solarflare.io/bridge) là một AMM (nhà tạo thị trường tự động) đầy đủ tính năng trên Moonbeam, rất giống với Uniswap. Solarflare có một cầu nối tích hợp cho phép người dùng kết nối tài sản từ mạng chính Ethereum cũng như chuỗi BNB với Moonbeam. Solarflare cũng có tính năng "Hoán đổi lấy phí gas" như đã đề cập trong phần Faucet ở trên.

![Kết nối với Solarflare](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.06.21 PM.png>)

* [Celer](https://cbridge.celer.network/#/transfer) là một cầu nối phổ biến cũng hỗ trợ Moonbeam. Xin lưu ý rằng bạn có thể không kết nối được từ mọi chuỗi vào Moonbeam (Ví dụ: Polygon to Moonbeam bắc cầu không được hỗ trợ).

![Kết nối với  Celer](<../../.gitbook/assets/Screen Shot 2022-06-24 at 6.10.32 PM.png>)

* Các cây cầu khác có sẵn nhưng có thể chỉ là chuỗi cụ thể như Nomad hoặc Axelar cho hệ sinh thái Cosmos.

## DeFi trên Moonbeam

[StellaSwap](https://app.stellaswap.com/farm) hiện là nguồn thanh khoản chính của MAI trên Moonbeam. MAI-Base4Pool bao gồm MAI, FRAX, USDT, USDC và DAI và hiện có TVL (tổng giá trị bị khóa) là $ 535 nghìn, mang lại APR 26% (tỷ lệ phần trăm hàng năm) trên stablecoin của bạn.

![MAI-Base4Pool on StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.22.32 PM.png>)

Moonbeam có một hệ sinh thái DeFi sôi động với hàng chục DApp (ứng dụng phi tập trung) có sẵn để sử dụng bao gồm các mặt hàng chủ lực của DeFi được tìm thấy trên các chuỗi khác như [Curve ](https://moonbeam.curve.fi/)và [Beefy Finance](https://app.beefy.com/). Để có danh sách đầy đủ các DApp hiện có, hãy xem [trang Moonbeam của DefiLlama.](https://defillama.com/chain/Moonbeam)

## Mai Finance trên Moonbeam

Mặc dù Mai Finance không có trên Moonbeam, bạn có thể tạo vault và vay MAI bằng xStella và wGLMR trên StellaSwap. Xin lưu ý rằng việc vay MAI trên StellaSwap sẽ phải chịu lãi suất - 12% đối với vault xStella và 8% đối với hầm wGLMR. Bạn có thể tìm hiểu thêm về cách sử dụng các vault MAI của StellaSwap trong phần tiếp theo có tiêu đề, [Chơi với MAI legos trên StellaSwap.](playing-with-mai-legos-on-stellaswap.md)

![Các vault trên StellaSwap](<../../.gitbook/assets/Screen Shot 2022-06-24 at 5.01.01 PM.png>)

## Từ chối trách nhiệm

Hướng dẫn này KHÔNG phải là lời khuyên tài chính, và chỉ nên được coi là một công cụ giáo dục. Luôn luôn làm nghiên cứu riêng của bạn. Thảo luận về một dự án trong hướng dẫn này không nên được coi là sự chứng thực của dự án.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
