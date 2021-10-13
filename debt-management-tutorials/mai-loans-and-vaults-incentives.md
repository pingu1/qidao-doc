---
description: >-
  Bài viết này giải thích chi tiết cách bạn có thể sử dụng Mai Finance để vay
  MAI với lãi suất 0% và lại được trả tiền để thực hiện việc này, chuyển khoản
  vay lãi suất 0% thành khoản vay lãi suất âm.
---

# Khoản vay MAI và ưu đãi cho các kho tiền

## Giới thiệu

Hoạt động kinh doanh cốt lõi của Mai Finance là cho vay. Thay vì bán tiền mã hóa của họ để mua các tài sản khác, mọi người có thể khóa tiền của họ trên Mai Finance và vay ngược lại chúng. Điều này mang lại cơ hội để giữ các tài sản có giá trị cao \(WBTC, WETH ...\) trong khi vẫn có thể nhận được các tài sản khác và lãi suất farming. Trong trường hợp đó, khoản vay được sử dụng để sinh lời, trong khi tài sản thế chấp đang tăng giá trị.

Một trong những lợi thế lớn khác của việc sử dụng Mai Finance là không có lịch trả nợ. Nói cách khác, bạn vay đồng tiền ổn định MAI đối với tiền điện tử của mình, bạn không phải trả bất kỳ khoản lãi nào và bạn có thể trả nợ bất cứ khi nào bạn muốn. Xem các bài viết khác nhau về [quản lý nợ](../debt-management-tutorials/debt-repayment-why-and-when.md) để biết thêm chi tiết. Khoản phí duy nhất mà bạn phải trả là phí hoàn trả tương ứng với 0,5% số tiền bạn đã vay khi hoàn trả khoản vay của mình và số tiền đó sẽ được lấy ra khỏi tài sản thế chấp của bạn.

Ví dụ: nếu bạn gửi ETH trị giá 200 đô la để vay MAI trị giá 100 đô la, khi bạn hoàn trả khoản vay của mình, bạn sẽ phải trả một khoản phí 0,5 đô la trực tiếp lấy từ khoản thế chấp ETH của mình.

Mai Finance đã giới thiệu vào tháng 9 năm 2021 các ưu đãi cho các kho tiền được thanh toán bằng Qi, mã token bản vị của Mai Finance. Nói cách khác, bằng cách gửi tài sản của bạn vào Mai Finance trong kho tiền để vay MAI, bạn cũng sẽ được trả tiền để làm điều đó. Bài viết này trình bày chi tiết cách hoạt động của chức năng này.

## Kho tiền là gì và hoạt động như thế nào?

### Tạo lập kho tiền

Trên Mai Finance, kho tiền là kho lưu trữ đặc biệt, nơi người ta có thể gửi tài sản của mình. Hiện tại, có 10 loại loại:

![C&#xE1;c lo&#x1EA1;i vault kh&#xE1;c nhau tr&#xEA;n n&#x1EC1;n t&#x1EA3;ng Mai Finance](../.gitbook/assets/image%20%281%29.png)

Có 2 loại kho tiền khác nhau:

* WETH
* WBTC
* MATIC
* LINK
* CRV
* AAVE

và

* camWETH
* camWBTC
* camWMATIC
* camAAVE

6 kho đầu tiên trong danh sách dành cho các tài sản trong khi 4 hầm cuối cùng dành cho camTokens. camTokens đang gộp mã thông báo thị trường AAVE, đại diện cho một khoản tiền gửi mà bạn có thể đã thực hiện trên AAVE và sau đó gửi vào các bể Yield của Mai Finance. Trong khi tài sản của bạn đang tạo ra lợi suất trên AAVE \(và trong khi phần thưởng được tự động cộng gộp bởi bể Yield\), bạn vẫn có thể vay MAI đồng tiền ổn định dựa trên các mã token này.

Lưu ý thêm, bạn có thể thấy trên ảnh chụp màn hình ở trên rằng trang tạo hiển thị một số thông tin rất quan trọng:

* MAI khả dụng: điều này tương ứng với trần nợ tối đa, số lượng MAI tối đa có thể được đúc từ tiền gửi kho tiền.
* Min Coll. đây là tỷ lệ Tài sản đảm bảo trên Nợ \(CDR\) tối thiểu cho kho tiền đó.
* APR khuyến khích cho kho tiền

### Hiểu rõ về nợ trần

Số lượng MAI tối đa mà người ta có thể đúc trên một kho tiền cụ thể phụ thuộc vào số lượng tài sản được gửi vào kho tiền đó. Trần nợ được thực hiện để đảm bảo rằng thị trường không tràn ngập MAI trong thời gian rất ngắn, điều này có thể ảnh hưởng đến giá của đồng tiền ổn định

Ví dụ, nếu một tổ chức lớn gửi 5.000 WBTC cùng một lúc và có thể vay MAI trị giá 100.000.000 đô la, hoán đổi tổng số để lấy nhiều WBTC hơn, điều này có thể đẩy giá MAI xuống rất nhiều và giá sẽ chênh lệch quá nhiều so với chốt, khiến toàn bộ nền tảng gặp rủi ro. Trần nợ là cơ chế ngăn điều này xảy ra: có một lượng MAI tối đa có thể được đúc cho một loại kho tiền nhất định.

Khi đạt đến trần nợ, thời gian mà không còn MAI để đúc được ghi lại và hệ thống sẽ tự động tăng trần nợ sau 48 giờ. Đây được coi là thời gian đủ để giá MAI ổn định \(trong trường hợp áp lực bán cao sau đợt bán tháo lớn đối với MAI\)

Điều này có nghĩa là trong 48 giờ, không ai có thể vay thêm MAI từ một kho tiền đã đạt đến trần nợ của nó, trừ khi một khoản nợ được hoàn trả.

Xin lưu ý thêm, càng có nhiều MAI trên thị trường, giá càng ổn định. Thật vậy, việc bán một lượng lớn MAI sẽ ít xâm lấn hơn đến giá của MAI nếu có nhiều MAI đang lưu hành.

* Nếu ai đó bán 1,000 MAI trong khi chỉ có 10.000 MAI đang lưu hành, thì lượng bán tương ứng với 10%
* Nếu ai đó bán 1,000 MAI trong khi có 10.000.000 MAI đang lưu hành, lượng bán tương ứng với 0,01%

Do đó, trần nợ không tăng dần mà theo cấp số nhân: càng có nhiều MAI lưu thông, thì tác động của một đợt bán lớn càng ít, do đó, trần nợ có thể được tăng lên nhiều hơn nữa.

{% hint style="info" %}
Khi bạn vay MAI, có thể xảy ra trường hợp số tiền MAI tối đa mà bạn có thể vay bị giới hạn bởi trần nợ, bất kể giá trị hiện tại của tài sản thế chấp của bạn và số tiền MAI hiện tại mà bạn đã vay. Trong trường hợp đó, bạn có thể đợi 48h để có thể vay thêm MAI.
{% endhint %}

### Tìm hiểu về tài sản thế chấp trên nợ

CDR, hay Tỷ lệ tài sản đảm bảo trên Nợ là tỷ lệ giữa giá trị của tài sản ký gửi trong kho tiền của bạn so với số tiền MAI bạn đã vay.

Ví dụ: nếu bạn gửi ETH trị giá 200 đô la để vay MAI trị giá 100 đô la, CDR của bạn sẽ là

$$
CDR=\frac{Tài.sản.thế.chấp}{Giá.trị.nợ}=\frac{200}{100}=200\%
$$

Duy trì CDR trên 100% có nghĩa là, tại bất kỳ thời điểm nào sẽ có nhiều tài sản thế chấp hơn nợ. Điều này là bắt buộc để đảm bảo rằng đồng tiền ổn định MAI được thế chấp quá mức nhằm đảm bảo nền tảng của tokenomics Mai Finance. Bạn có thể biết thêm chi tiết từ [tài liệu chính thức ](https://docs.mai.finance/stablecoin-economics)của Mai Finance.

Mỗi loại kho tiền có tỷ lệ CDR tối thiểu được chấp nhận, một ngưỡng mà theo đó kho tiền được coi là có rủi ro vì số tiền đã vay có thể không được đảm bảo bằng đủ tài sản thế chấp. Tại thời điểm này, bất kỳ ai cũng có thể thanh lý kho tiền, có nghĩa là một phần của khoản nợ được người thanh lý thanh toán và sau đó có thể lấy một phần của tài sản thế chấp đã ký gửi để hoàn trả. Bạn có thể tìm thêm thông tin chi tiết về quy trình thanh lý trong tài liệu chính thức.

Khi bạn vay MAI với một tài sản thế chấp nhất định, bạn sẽ nhận được một số gợi ý về số tiền MAI tối đa bạn có thể vay là bao nhiêu và tác động đến tỷ lệ lành mạnh trong thanh khoản của bạn tùy thuộc vào số tiền đã vay là bao nhiêu, như bạn có thể thấy trong ảnh chụp màn hình bên dưới:

![T&#x1EF7; l&#x1EC7; l&#xE0;nh m&#x1EA1;nh t&#xF9;y thu&#x1ED9;c v&#xE0;o s&#x1ED1; ti&#x1EC1;n vay](../.gitbook/assets/image%20%284%29.png)

Rất quan trọng khi bạn luôn phải để ý tỷ lệ CDR và tỷ lệ lành mạnh với mục đích:

* tránh bị thanh lý tài sản
* tăng cường lành mạnh của toàn bộ nền tảng Mai Finance bằng cách đảm bảo khối lượng MAI được lưu hành với hỗ trợ thích hợp.  

CDR "lành mạnh", theo định nghĩa của Mai Finance là cao hơn giá trị CDR tối thiểu từ 25% đến 270%. Lưu ý thêm, bạn cũng có thể xem[ hướng dẫn chiến lược](../huong-dan/leverage-aave-tokens.md) của chúng tôi để xem cách bạn có thể sử dụng CDR để đầu tư vào các dự án khác hoặc [trả nợ ](../debt-management-tutorials/debt-repayment-how.md#hoan-tra-mot-phan)bằng cách sử dụng nợ của bạn.

## Các ưu đãi kho tiền

### Tìm hiểu APR ưu đãi kho tiền  

Vào tháng 9 năm 2021, Mai Finance giới thiệu các ưu đãi kho tiền. Đây là phần thưởng do nền tảng Tài chính Mai phân bổ cho bất kỳ ai vay MAI và tham gia vào sự phát triển của nền tảng.

Mỗi loại kho \(trong số 10 loại khác nhau\) nhận được 0,05 Qi trên mỗi khối, sau đó được phân phối giữa tất cả những người dùng có Tỷ lệ tài sản đảm bảo trên Nợ lành mạnh. APR của kho tiền được xác định bởi số tiền hiện tại MAI đã vay.

Ví dụ, Ben và Kila là 2 người bạn đã gửi ETH của họ vào các hầm WETH trên Mai Finance.

* Ben đã gửi số ETH trị giá tương đương 2.000 đô la và vay 1.000 MAI
* Kila đã gửi số ETH trị giá tương đương 10.000 đô la và vay 6.000 MAI

Số tiền MAI hiện tại mà người dùng đã gửi WETH vào kho tiền là 1.000.000 MAI.

Cả Ben và Kila đều đủ điều kiện nhận ưu đãi kho tiền vì Ben có CDR là 200% và Kila có CDR là 166,67%. Ben, với khoản vay của mình, sở hữu 0,1% tổng số tiền đã vay, trong khi Kila sở hữu 0,6%.

Tổng lượng Qi được phân bổ cho kho WETH \(hoặc bất kỳ kho tiền nào\) là

$$
Qi=0.05*\frac{86400}{2}=2160
$$

{% hint style="info" %}
86.400 là số giây trong một ngày và trên Polygon, thời gian khối là 2 giây, có nghĩa là số khối dự kiến ​​mỗi ngày là 86.400 / 2 = 43.200. Do đó, phát thải cho mỗi Vault là 2.160 Qi / ngày.

**Lưu ý**: Thời gian khối trên Polygon gần đây đã tăng lên và khoảng 2,6 giây. Tuy nhiên, tất cả các APR và APY được hiển thị trên tất cả các ứng dụng đều giả định thời gian khối là 2 giây. Vui lòng DYOR và kiểm tra [thời gian khối hiện tại trên PolygonScan](https://polygonscan.com/chart/blocktime).
{% endhint %}

Do đó, nếu trạng thái của Vault vẫn giữ nguyên, Ben sẽ nhận được 0,1% trong số 2.160 Qi được phân phối, trong khi Kila sẽ nhận được 0,6%.

* Ben sẽ nhận được 2,16 Qi mỗi ngày, đây là phần thưởng hàng ngày là 0,216% hoặc APR là 78,84%
* Kila sẽ nhận được 12,96 Qi mỗi ngày, đây cũng là phần thưởng hàng ngày là 0,216% hoặc APR là 78,84%

Lưu ý nhỏ, 2.160 Qi cho 1.000.000 MAI là phần thưởng hàng ngày 0,216% hoặc 78,84%, là APR của Vault.

{% hint style="info" %}
Dễ dàng nhận thấy rằng APR của Vault được liên kết trực tiếp với số tiền MAI đã vay. Vay càng nhiều MAI thì APR càng thấp. Cũng cần lưu ý thêm, số tiền MAI có thể vay cũng bị giới hạn bởi nợ trần, điều này sẽ tăng lên cùng với nhu cầu về MAI.
{% endhint %}

Để xác minh, chúng ta có thể tính toán APR lý thuyết cho kho tiền MATIC dựa trên các con số được công bố trên [trang phân tích ](https://app.mai.finance/analytics)trên Mai Finance. Số tiền MAI vay từ kho tiền MATIC là 799.328. Phần thưởng là 2.160 Qi mỗi ngày cho kho tiền đó. Điều đó tương ứng với APR là

$$
APR=\frac{Phần .thưởng Qi}{MAI_{đã.mượn}}*365=\frac{2160}{799328}*365=44,29\%
$$

Điều này ít nhiều tương ứng với APR được hiển thị trên kho tiền MATIC đã được quảng cáo trong hội thảo QiDAO vào ngày 13 tháng 9, như được hiển thị trong ảnh chụp màn hình sau:

![](../.gitbook/assets/image%20%2823%29%20%282%29%20%283%29%20%281%29.png)

### Tính toán APR của hầm tiền bắt đầu

Với dữ liệu tương tự như ví dụ trên, có thể tính toán APR bắt đầu cho tất cả các vault như sau

| Dạng vault | APR bắt đầu |
| :--- | :--- |
| MATIC | 44.29% |
| WETH | 24.03% |
| LINK | 27.41% |
| AAVE | 164.14% |
| CRV | 159.96% |
| WBTC | 36.92% |
| camWETH | 25.46% |
| camWMATIC | 44.33% |
| camAAVE | 167.23% |
| camWBTC | 47.38% |

{% hint style="info" %}
Như bạn có thể thấy, một số hầm sẽ tạo ra nhiều phần thưởng hơn những hầm khác. Ngoài ra, bạn có thể thấy rằng điều cực kỳ quan trọng là phải gửi tài sản của mình càng sớm càng tốt để hưởng lợi từ APR cao trước khi tăng trần nợ và vay nhiều hơn \(làm giảm APR\).

Bạn cũng có thể thấy rằng nếu bạn giữ khoản vay của mình trong hơn một năm, phí hoàn trả hơn 0,5% sẽ dễ dàng được bù đắp bởi chương trình thưởng này.
{% endhint %}

### Phân phối thưởng

Phần thưởng được phân bổ bởi các ưu đãi kho tiền sẽ được phân phối theo cách tương tự như đối với Qi đặt cổ phần. Có nghĩa là mỗi thứ Tư hàng tuần, Qi được phân bổ bởi chương trình ưu đãi Vaults sẽ được airdrop / nhận cho tuần trước ngày trả lương

## Hỏi đáp về phần thưởng Qi.

*  **Kho tiền nào thì nhận được phần thưởng Qi?**

Hiện tại thì tất cả kho tiền đều nhận được 

*  **Bao nhiêu Qi được dùng để khuyến  khích hoạt động cho vay?**

0.05 Qi/khối cho mỗi loại kho tiền

*  **Bao nhiêu MAI tôi cần phải mượn để nhận được phần thưởng?**

Đối với ưu đãi vay tiền của Vault, hãy cao hơn tỷ lệ thanh lý từ 25% đến 270% để nhận được airdrop mã token Qi. Điều này có nghĩa là:

*  _Matic_ - Tỷ lệ thanh lý 150% - Điều kiện để nhận khuyến khích giữa 175% và 420% 
* _Tokens_: - Tỷ lệ thanh lý  130% - Điều kiện để nhận khuyến khích giữa 155% và 400% 
* _CamTokens_: - Tỷ lệ thanh lý 135% - Điều kiện để nhận khuyến khích giữa 160% và 405%



*  **Làm sao tôi biết được rằng kho tiền có đang được nhận thưởng hay không?**

 Nếu bạn thấy biểu tượng cảm xúc lửa trên trang tổng quan về vault của mình, điều đó có nghĩa là vault đang kiếm được phần thưởng

*  **Tôi sẽ nhận được khoảng bao nhiêu?**

Phần trăm tổng phần thưởng của bạn dựa trên phần trăm MAI bạn đã vay so với tổng số tiền MAI đã vay từ loại kho tiền đó.

*  **Chương trình ưu đãi diễn ra trong bao lâu?**

Thời gian dự kiến của chương trình ưu đãi vay là kéo dài 3 tháng. DAO có thể bỏ phiếu để ngừng khuyến khích trước khi hết 3 tháng hoặc bỏ phiếu để gia hạn chương trình.

* **Tôi sẽ nhận thưởng bằng cách nào?**

Qi sẽ được airdrop cho những chủ sở hữu kho tiền đủ điều kiện.

* **Tính đủ điều kiện nhận phần thưởng được thu thập như thế nào?**

Tính đủ điều kiện cho phần thưởng được tính trên mỗi khối. Bạn sẽ kiếm được phần thưởng cho các khối bạn đủ điều kiện trong tuần.

* **Khi nào phần thưởng theo dõi trong tuần bắt đầu?**

Chúng tôi sẽ tuân theo lịch trình tương tự như eQi. Bạn có thể tìm thấy số khối trên trang Boost.

## Tuyên bố từ chối trách nhiệm 

Hướng dẫn này đã được viết trước khi ra mắt các ưu đãi của Vault, có nghĩa là các APR được quảng cáo trong tài liệu này  có thể được sửa đổi và / hoặc có thể không chính xác. Số tiền MAI đã vay, trần nợ và giá trị của mã token Qi sẽ ảnh hưởng lớn đến APR cuối cùng của mỗi loại kho tiền. Hãy đảm bảo rằng bạn đầu tư có trách nhiệm.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém \(hoặc khiến bạn mất tiền\) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}

