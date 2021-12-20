---
description: >-
  Phần này chúng tôi sẽ trình bày cách kết hợp giữa phần thưởng từ các kho tiền
  trên Mai Finance và farming để tối đa hóa lợi nhuận tổng thể của bạn.
---

# Cách để kết hợp giữa phần thưởng đi vay và farming

## Giới thiệu

Vào tháng 9 năm 2021, Mai Finance đã giới thiệu phần thưởng kho tiền để thúc đẩy hoạt động kinh doanh đi vay của mình khi người dùng sử dụng mã thông báo của họ để vay MAI. Không chỉ vay lãi suất 0% với phí hoàn trả nhỏ, giờ đây mọi người còn có thể được trả thưởng khi vay tiền. Hướng dẫn này sẽ đề xuất một chiến lược dựa trên việc farming đồng ổn định bằng cách sử dụng Augury Finance làm nguồn đầu ra mã thông báo cung cấp cho các kho tiền trên Mai Finance, tạo ra các ưu đãi vay vốn cao và MAI bổ sung sau đó sẽ được bơm lại vào  các bể thanh khoản.&#x20;

![](<../../.gitbook/assets/image (29).png>)

## Trình bày ứng dụng và các bể&#x20;

### Augury Finance

Augury Finance là một nền tảng tổng hợp lợi nhuận không tập trung vào việc tự động cộng gộp các mã thông báo LP (Nhóm thanh khoản) của bạn. Thay vào đó, Augury sẽ tự động bán mã thông báo nền tảng của các bể thanh khoản mà nó sử dụng để mua các mã thông báo khác tại Infusion của họ.

Ví dụ, bạn có thể farm cặp DFYN-ETH

![Bể thanh khoản khai thác DFYN-ETH trên Augury ](<../../.gitbook/assets/image (30).png>)

Infusion này đang sử dụng DinoSwap làm thanh khoản nền tảng và một cặp thanh khoản LP mà một người có thể tạo được trên DFYN. Với APR là 123,43%, người dùng gửi thanh khoản vào bể này sẽ được thưởng

* 30%  WETH
* 20%  LINK
* 20%  WBTC
* 15%  USDT
* 15%  WMATIC

Nếu bạn cung cấp thanh khoản trên DinoSwap, bạn sẽ được trả bằng mã thông báo DINO, giá rất dễ biến động. Trên các nền tảng tổng hợp khác như Adamant hoặc Beefy, bạn sẽ tăng vị thế LP của mình, nhưng với Augury, bạn "đảm bảo" vị thế của mình bằng cách nhận được các mã thông báo ít có khả năng biến động. Hạn chế là vị thế ban đầu của bạn sẽ không tăng theo thời gian vì 100% DINO thu hoạch được chuyển đổi thành bộ mã thông báo tạo ra phần thưởng trên Augury.

{% hint style="info" %}
Augury Finance đang sử dụng 3 cấp có phí đặt cọc và phí thực hiện khác nhau. Vui lòng đọc về các loại cấp bạn muốn sử dụng và đảm bảo rằng bạn hiểu tác động của chúng đối với chiến lược của bạn.
{% endhint %}

Trong chiến lược này, chúng tôi sẽ sử dụng bể USDT-UST cấp 2 để thưởng cho người dùng kết hợp WETH / WBTC / LINK / WMATIC / USDC, vì Mai Finance đề xuất 4 kho tiền cho 4 trong số 5 mã thông báo mà chúng ta sẽ nhận được làm phần thưởng. Để tối đa hóa lợi nhuận của mình, chúng ta sẽ thêm AAVE giữa đầu ra của Augury và kho tiền trên Mai Finance vì 3 trong số 5 token mà chúng ta sẽ thu hoạch có thể được cho vay trên AAVE.

![Bể thanh khoản của USDT-UST trên Augury](<../../.gitbook/assets/image (31).png>)

### Curve

Curve là một dự án blue-chip sẽ thưởng cho người dùng cho vay blue-chip token. Phần thưởng bao gồm các mã thông báo tự động cộng dồn (được thêm lại vào khoản đầu tư), mã thông báo WMATIC và mã thông báo CRV, là 2 mã thông báo cũng được chấp nhận làm tài sản thế chấp trên Mai Finance.&#x20;

Một trong những điều rất thú vị cần lưu ý về Curve và các bể của nó là người ta không phải gửi một số tiền chính xác của mỗi mã thông báo cho một bể nhất định. Thay vào đó, một mã thông báo duy nhất có thể được cung cấp và thuật toán quản lý bể sẽ tự động điều chỉnh các mã thông báo khác bằng cách bán một phần tiền gửi và mua các mã thông báo khác để duy trì tỷ lệ chính xác trong bể.&#x20;

Chúng ta sẽ sử dụng bể atricrypto3 chấp nhận bất kỳ sự kết hợp nào của WBTC / WETH / USDC / USDT / DAI và chúng ta sẽ thêm vào bể này USDC sẽ được tạo bởi bể trên Augury.

![Thông tin chi tiết về bể atricrypto3 trên Curve kể từ tháng 9 năm 2021](<../../.gitbook/assets/image (32).png>)

### AAVE

Như đã đề cập trong đoạn về Augury, AAVE được sử dụng để thêm một phần thưởng nhỏ vào bể trên Augury trước khi chúng ta sử dụng chúng trên Mai Finance. Thay vì đặt WBTC, WETH và WMATIC trực tiếp trên Mai Finance, chúng ta sẽ gửi các mã thông báo này trên AAVE và sử dụng công cụ lợi nhuận của Mai Finance để tự động gộp phần thưởng từ AAVE trong các nhóm amToken và sử dụng camToken làm tài sản thế chấp trong kho tiền . Bạn có thể biết thêm chi tiết về phần này bằng cách đọc hướng dẫn về [mã thông báo AAVE.](how-to-combine-farming-and-borrowing-rewards.md#intro)

![Lãi suất huy động vốn trên AAVE tháng 9 năm 2021](<../../.gitbook/assets/image (33).png>)

### Balancer

Balancer là một dự án blue-chip khác như Curve. Bạn sẽ có thể gửi một số mã thông báo nhất định trong các bể bao gồm hơn 2 mã thông báo và bạn gửi một mã thông báo duy nhất. Bể sẽ tự động được cân bằng để có được tỷ lệ bằng nhau của mỗi mã thông báo tạo ra nhóm.&#x20;

Đối với chiến lược này, chúng ta sẽ sử dụng bể WETH / BAL / Qi / MAI / USDC. Bể này sẽ chấp nhận mã thông báo Qi sẽ được thu thập từ kho tiền trên Mai Finance và sẽ thưởng cho chúng ta bằng các mã thông báo Qi và BAL bổ sung mà chúng ta sẽ có thể gửi vào Mai Finance trong kho tiền BAL, cho phép chúng ta kiếm thêm MAI và tăng vị tnế thanh khoản của chúng ta trên Augury.

![Bể trên Balancer tháng 9](<../../.gitbook/assets/image (34).png>)

## Khởi động hệ thống

![](<../../.gitbook/assets/image (35).png>)

Sau đây là một mô phỏng được thực hiện với khoản đầu tư ban đầu trị giá 1.000 đô la ETH được gửi vào kho camWETH để vay MAI trị giá 500 đô la, được quy đổi bằng USDT-UST trị giá 500 đô la. Mô phỏng này giả định các phần thưởng sau cho các  nền tảng khác nhau

* USDT-UST farming APR là 22.53%
* amWBTC APR  0.39%
* amWETH APR  1.71%
* amWMATIC APR  3.80%
* atricrypto3 APR bao gồm 3.86% tự động cộng dồn LP token, 13.09% WMATIC và 17.63% CRV
* Bể 5-tokens Balancer với APR là 43.46% với tỷ lệ BAL:Qi là 1:6
* APR kho tiền bao gồm
  * 23.28% cho camWBTC
  * 21.52% cho  camWETH
  * 32.93% cho camWMATIC
  * 24.51% cho LINK
  * 116.71% cho CRV
  * 62.38% cho BAL

Các APR này đều có thể thay đổi trên các nền tảng khác nhau và không có gì đảm bảo rằng chúng sẽ ổn định trong cả năm, tuy nhiên, chúng ta vẫn sẽ xem xét chúng như là ví dụ đối với mô phỏng này để có được ý tưởng về APR tổng thể. Để tiếp tục "đơn giản hóa" mô phỏng, chúng ta sẽ không tính đến các biến thể giá tài khoản cũng như phí giao dịch. Cũng xin lưu ý rằng mô phỏng này có tính đến phần thưởng Vault trên Mai Finance và phần thưởng Balancer được cộng dồn hàng ngày thay vì hàng tuần, nhưng những phần thưởng này hiện được phát hàng tuần vào ví của người dùng. Cuối cùng, vì lợi ích của mô phỏng này, chúng ta sẽ giả định CDR (Tỷ lệ thế chấp trên nợ) luôn là 200%, có nghĩa là chúng ta chỉ vay một nửa số tiền trên tài sản thế chấp nhắm tránh bị thanh lý quá dễ dàng.

### Ngày thứ nhất

Nếu bạn vẫn còn WETH trị giá 1.000 đô la, hãy gửi vào AAVE để nhận amWETH, sau đó gửi tiền vào [Mai Finance](how-to-combine-farming-and-borrowing-rewards.md#augury-finance) để nhận lại camWETH và cuối cùng gửi camWETH của bạn vào kho tiền tương ứng để có thể vay 500 MAI.

Sử dụng [Anchor](how-to-combine-farming-and-borrowing-rewards.md#intro) để chuyển đổi MAI của bạn thành USDT (hoặc bạn có thể sử dụng một DEX khác như [QuickSwap](how-to-combine-farming-and-borrowing-rewards.md#intro) nếu không đủ thanh khoản), sau đó bạn có thể sử dụng [DFYN ](https://exchange.dfyn.network/#/swap)để hoán đổi 50% USDT của mình thành UST và tạo thành một cặp USDT-UST sau đó bạn có thể gửi tiền trên [Augury](https://augury.finance/infusions/). Lưu ý rằng bạn cũng sẽ cần một số OMEN mà bạn có thể mua trên QuickSwap ..

Do đó, vào cuối Ngày 1, chúng tôi thu hoạch các phần thưởng sau

| Dạng phần thưởng           | Giá trị bằng đô la |
| -------------------------- | ------------------ |
| WBTC từ farming            | 0.123              |
| WETH từ farming            | 0.031              |
| WMATIC từ farming          | 0.031              |
| LINK từ farming            | 0.031              |
| USDC từ farming            | 0.092              |
| Phần thưởng Qi từ kho tiền | 0.295              |

Đây chỉ là những phần thưởng chúng ta nhận được từ việc canh tác và vay mượn vào cuối ngày đầu tiên.

### Ngày thứ hai

Phần thưởng được thu hoạch, WBTC, WETH và WMATIC được gửi đến các kho tiền tương ứng trên Mai Finance sau khi thông qua AAVE và công cụ năng suất trên Mai. LINK được gửi trực tiếp vào kho LINK và USDC được gửi đến Curve trong bể atricrypto3. Phần thưởng Qi được gửi đến Balancer. Tại thời điểm này, chúng ta có thể mượn thêm MAI từ 3 kho camToken và kho tiền LINK (chính xác là $ 0,13 trị giá MAI) và chúng ta có thể tạo thêm cặp USDT-UST từ MAI

Do đó, vào cuối Ngày thứ 2, chúng ta thu hoạch được những phần thưởng sau

| Dạng phần thưởng            | Giá trị tính bằng đô la |
| --------------------------- | ----------------------- |
| WBTC từ farming             | 0.123                   |
| WETH từ farming             | 0.031                   |
| WMATIC từ farming + Curve   | 0.031                   |
| LINK từ farming             | 0.031                   |
| USDC từ farming             | 0.093                   |
| Phần thưởng CRV trên Curve  | 0.00004                 |
| Phần thưởng BAL             | 0.00005                 |
| Phần thưởng Qi tại kho tiền | 0.296                   |

Tại thời điểm này, hệ thống đã bắt đầu và phần thưởng đang chảy theo cách mà mỗi bước đang cung cấp cho bước tiếp theo, tạo ra một số vòng lặp

## Kết quả farming

### Công việc hàng ngày

Công việc hàng ngày bao gồm các giao dịch sau

* Thu hoạch phần thưởng trên Augury
* Gửi WBTC, WETH và WMATIC trên AAVE
* Gửi amWBTC, amWETH và amWMATIC trên Mai Finance tại công cụ lợi nhuận
* Gửi camWBTC, camWETH và camWMATIC trong các kho tương ứng trên Mai Finance&#x20;
* WMATIC từ Curve và sử dụng chúng trong vault camWMATIC
* Thu hoạch CRV từ Curve và sử dụng chúng trong vault CRV&#x20;
* Vay MAI từ các vault khác&#x20;
* Chuyển đổi MAI thành USDT trên Mai Finance qua Anchor
* &#x20;Chuyển đổi 50% USDT thành UST trên DFYNC&#x20;
* Tạo cặp USDT-UST LP mới trên DFY
* Thêm cặp thanh khoản  trên Augury

### Công việc hàng tuần

Ngoài ra, bạn sẽ nhận được phần thưởng hàng tuần bằng BAL (từ khoản tiền gửi Qi của bạn trên Balancer) và mã thông báo Qi (từ phần thưởng kho tiền). Bạn sẽ phải

* Gửi mã thông báo Qi trên Balancer&#x20;
* Gửi mã thông báo BAL trên Mai Finance trong kho tiền BAL
* Mượn MAI từ khoản tiền gửi BAL bổ sung của bạn và chuyển đổi chúng theo cặp USDT-UST để cung cấp trên Augury

### Kết quả hàng tháng

| Tháng | USDT-UST | atricrypto3 | Balancer | camWBTC | camWETH  | camWMATIC | LINK  | CRV   | BAL  |   |
| ----- | -------- | ----------- | -------- | ------- | -------- | --------- | ----- | ----- | ---- | - |
| 1     | 503.84   | 2.79        | 9.01     | 3.72    | 1,002.34 | 0.94      | 0.93  | 0.001 | 0.02 |   |
| 2     | 507.88   | 5.66        | 18.39    | 7.47    | 1,004.68 | 1.93      | 1.87  | 0.003 | 0.09 |   |
| 3     | 511.99   | 8.47        | 28.14    | 11.24   | 1,007.04 | 2.96      | 2.81  | 0.004 | 0.21 |   |
| 4     | 516.18   | 11.36       | 38.28    | 15.06   | 1,009.41 | 4.02      | 3.76  | 0.005 | 0.38 |   |
| 5     | 520.43   | 14.28       | 48.83    | 18.90   | 1,011.79 | 5.13      | 4.72  | 0.007 | 0.60 |   |
| 6     | 524.76   | 17.23       | 59.79    | 22.78   | 1,014.18 | 6.29      | 5.69  | 0.008 | 0.87 |   |
| 7     | 529.17   | 20.21       | 71.18    | 26.69   | 1,016.58 | 7.48      | 6.67  | 0.010 | 1.21 |   |
| 8     | 533.66   | 23.24       | 83.03    | 30.63   | 1,018,99 | 8.72      | 7.65  | 0.011 | 1.60 |   |
| 9     | 538.22   | 26.29       | 95.34    | 34.61   | 1,021.42 | 10.01     | 8.64  | 0.013 | 2.05 |   |
| 10    | 542.87   | 29.38       | 108.14   | 38.63   | 1,023.86 | 11.34     | 9.64  | 0.014 | 2.57 |   |
| 11    | 547.61   | 32.51       | 121.44   | 42.68   | 1,026.31 | 12.72     | 10.65 | 0.016 | 3.16 |   |
| 12    | 552.43   | 35.67       | 135.26   | 47.45   | 1,028.78 | 14.15     | 11.67 | 0.017 | 3.81 |   |

Một số lưu ý:

* Sự tăng trưởng của nhóm USDT-UST là kết quả duy nhất của việc MAI được vay thêm từ các kho tiền&#x20;
* &#x20;Bể CRV hầu như không tăng nhiều do số lượng USDC được gửi trên Curve rất thấp&#x20;
* Kho tiền BAL không quan trọng do thực tế là 14,28% phần thưởng Balancer được thanh toán bằng mã thông báo BAL, phần còn lại được thanh toán bằng mã thông báo Qi&#x20;
* Số tiền trong bể Balancer là khoản thu lớn nhất và chỉ là kết quả của phần thưởng Vault và phần thưởng của Balancer

### Ngày thứ 365

Sau một năm đầy đủ, trạng thái đầu tư cuối cùng của chúng tôi sẽ là

| Vị thế thanh khoản  | Giá trị bằng đô la |
| ------------------- | ------------------ |
| USDT-UST            | 553.24             |
| atricrypto3         | 36.20              |
| Balancer            | 137.62             |
| camWBTC             | 47.45              |
| camWETH             | 1,029.19           |
| camWMATIC           | 14.39              |
| LINK                | 11.84              |
| CRV                 | 0.017              |
| BAL                 | 3.93               |

Tổng số nợ thực sự là toàn bộ cặp USDT-UST, vì vậy, $ 553,24 và tổng phần thưởng được tạo ra là $ 280,63, tương ứng với APY cuối cùng là 28,06%.

### So sánh với các chiến lược khác

Lợi nhuận 28% APY khi thanh khoản đồng tiền ổn định không phải là quá tệ, nhưng  so với các chiến lược khác áp dụng với số ETH trị giá 1.000 đô la ban đầu sẽ như thế nào?&#x20;

* Sử dụng đòn bẩy amWETH 8 lần thông qua AAVE: quy trình cụ thể  được mô tả trong hướng dẫn [mã thông báo AAVE.](leverage-aave-tokens.md)&#x20;
* Cung cấp toàn bộ đồng ổn định trên Augury: đối với chiến lược này, chúng ta bán WETH và farm với USDT-UST trị giá 1.000 đô la trên cùng một khoản tiền trên Augury
* Cung cấp thanh khoản toàn bộ đồng ổn định trên QuickSwap: đối với chiến lược này, chúng tôi sẽ sử dụng kho camWETH để hưởng lợi từ phần thưởng kho và farm với MAI trị giá 500 đô la trên QuickSwap (MAI-DAI ở mức 19,78% APY), sử dụng kho tiền DQUICK trên Mai Finance vay thêm MAI và đầu tư lại vào bể (kho dQUICK với APR là 55,72%))

| Chiến lược                                    | APY cuối cùng |
| --------------------------------------------- | ------------- |
| Chiến lược được trình bày trong hướng dẫn này | 28.06%        |
| Tạo đòn bẩy trên AAVE 8 lần                   | 46.46%        |
| Chỉ farm đồng ổn định trên Augury             | 22.53%        |
| Farming Quickswap  + kho dQUICK               | 35.96%        |

## Disclaimer

Chiến lược này khá thú vị khi sử dụng hầu hết các kho tiền từ Mai Finance và hướng dẫn này được viết chủ yếu để giới thiệu rằng, kể từ tháng 9 năm 2021, đây là phần sẽ tạo ra nhiều phần thưởng hơn khi kiếm được các đồng tiền ổn định. Tuy nhiên, chiến lược này có thể không phải là chiến lược thú vị nhất và liên quan đến rất nhiều thao tác của một số nền tảng. Cuối cùng, Augury là một công cụ tuyệt vời tạo ra các mã thông báo cụ thể có thể được bao gồm trong một số chiến lược, nhưng có lẽ không phải chỉ farm đồng ổn định. Và như một lưu ý nhỏ, không có phí gửi cũng như phí thực hiện không được tính đến khi tính APY cuối cùng.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}
