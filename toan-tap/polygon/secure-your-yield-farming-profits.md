---
description: >-
  TPhần này trình bày một cách chi tiết một chiến lược an toàn cho việc tối ưu
  thanh khoản ít sinh lợi hơn nhưng an toàn hơn rất nhiều.
---

# Tối ưu thanh khoản chỉ bằng stablecoin

## Ý tưởng chung

Khi bạn tham gia tối ưu thanh khoản (yield farming) tại một farm nào đó trên Polygon, bạn đưa số vốn đầu tư của bạn cho sự thành công hoặc thất bại của farm đó. Hướng dẫn này không trình bày chi tiết farm là gì và làm thế nào để farm. Nếu bạn cần hướng dẫn chi tiết bạn có thể tìm trên internet hoặc bạn cũng có thể hỏi cộng đồng [Discord](https://discord.gg/mQq55j65xJ) Mai Finance.

Vấn đề chính khi bạn farming là bạn phải lựa chọn giữa:

* Bán đồng bản vị của farm thành những đồng an toàn hơn.
* Tái đầu tư để tiếp tục sinh lời nhiều hơn ( còn được gọi là siêu lãi kép).

Hướng dẫn dưới đây sẽ trình bày từng bước các tận dụng nền tảng Mai Finance để thực sự đảm bảo được lợi nhuận thu được trong khi vẫn tái đầu tư một phần vào farm.

{% hint style="info" %}
Để minh họa chi tiết hơn làm thế nào bạn có thể làm điều đó, chúng ta sẽ dùng [farm mới nhất ](https://ball.polypup.finance/)của Polypup. Xin lưu ý đây chỉ là ví dụ cho mục đích giáo dục nên tuyệt đối không sử dụng như là một lời khuyên tài chính. Ngoài ra, thuật ngữ "an toàn" cũng chỉ mang tính chủ quan cá nhân.
{% endhint %}

![](<../../.gitbook/assets/Screen Shot 2021-08-09 at 10.20.26 AM.png>)

## Vòng đời farming

### Chuẩn bị

Một trong những farmer kỳ cựu từng nói rằng

> Đừng bao giờ mua những thứ có thể kiếm được

Trong nội dung hướng dẫn này, vì chúng ta ưu tiên sự an toàn tài chính là quan trọng hàng đầu cho nên cặp stablecoin được lựa chọn để tiến hành farm nhằm bảo vệ số vốn đầu tư tránh được tổn thất tạm thời. Hầu hết các farm đều có các cặp stable coin trong bể thanh khoản của họ. Cặp MAI/USDC cũng được tìm thấy trên nền tảng của Mai Finance và đây cũng sẽ là cặp ví dụ cho minh họa này.

Để bắt đầu farm bằng cặp MAI/USDC, bạn cần phải có stablecoin. Trên nền tảng của Mai Finance, bạn có thể vay được stable Mai bằng cách dùng những đồng coin ưa thích của bạn làm tài sản thế chấp. Trong trường hợp này, chúng ta sẽ lấy MATIC làm tài sản thế chấp để vay MAI bằng cách gửi vào các vault tại mục Vault của trang web. Nếu bạn cần hỗ trợ, vui lòng tham gia Discord và đặt câu hỏi cho cộng đồng. Ngoài ra, bạn cũng dễ dàng tìm thấy những hướng dẫn cần thiết tại các mục trên trang web này.

{% hint style="info" %}
Bạn có thể gửi trực tiếp đồng MATIC của mình vào vault MATIC hoặc bạn có thể gửi chúng vào Aave để nhận amWMATIC sau đó gửi lên Mai Finance để nhận về camWMATIC và dùng chúng như là tài sản thế chấp để vay MAI. Bạn sẽ thấy rằng với cùng số lượng MAI vay được bạn còn nhận được thêm lợi nhuận từ đồng MATIC trên các nền tảng Aave và Mai Finance. Để biết thêm chi tiết và hướng dẫn cụ thể bạn có thể tham khảo tại phần [Tạo đòn bẩy cho các token từ thị trường Aave](leverage-aave-tokens.md).
{% endhint %}

Khi vay đã vay stablecoin MAI, bạn có thể sử dụng mục [Anchor](https://app.mai.finance/anchor) trên app Mai Finance để chuyển một nửa MAI thành USDC với tỷ lên là 1:1.&#x20;

![Sử dụng mục Swap để chuyển một nửa MAI thành USDC](<../../.gitbook/assets/Screen Shot 2021-08-09 at 6.28.28 AM.png>)

Bây giờ, phụ thuộc vào farm cụ thể bạn muốn tham gia, bạn cần ghép 2 đồng này với nhau để tạo ra một cặp thanh khoản LP trên các nền tảng DEX. Vì dự định ban đầu của chúng ta là Polypup mà farm này chấp nhận cặp thanh khoản của Quickswap LPs, nên chúng ta đi tới trang chính của Quickswap vào mục [Pool](https://quickswap.exchange/#/add/0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174/0xa3Fa99A148fA48D14Ed51d610c367C61876997F1) để tạo cặp MAI-USDC

![Tạo LP token bằng MAI và USDC](<../../.gitbook/assets/Screen Shot 2021-08-09 at 6.29.16 AM.png>)

Vậy là bạn đã sẵn sàng

### Ký gửi và thu hoạch đồng coin của farm

Bây giờ bạn có một số token LP, bạn truy nhập vào website và gửi chúng vào bể thanh khoản để bắt đầu thu hoạch đồng coin Ball của Polypup.

![Nhận BALL trong bể](<../../.gitbook/assets/Screen Shot 2021-08-09 at 10.58.19 AM.png>)

Như bạn thấy ở trên hình, farming cặp MAI/USDC cho chúng ta mức lãi suất 176% một năm. Tùy vào dung lượng bể và giá của token BALL mà APR sẽ thay đổi theo thời gian.&#x20;

{% hint style="info" %}
Có một điều quan trọng cần đặc biệt lưu ý là khi bạn gửi LP vào các farm thì hầu hết sẽ bị tính phí từ 2 đến 4% trực tiếp lấy từ LP của bạn. Hãy hết sức lưu ý điều này và đảm bảo rằng bạn chuẩn bị tâm lý có thể sẽ mất phí mà không lấy lại được.
{% endhint %}

Giờ đây cặp stablecoin đã được gửi vào bể thanh khoản và bạn nhận được đồng coin của farm mà bạn có thể thu hoạch bất cứ khi nào. Chú ý rằng giá của đồng coin sẽ rất biến động, vì vậy cần chắc chắn rằng bạn thu hoạch thường xuyên khi đồng coin này còn có giá. Để càng lâu thì nguy cơ càng lớn vì khả  năng bạn nhận được một đống coin không có giá trị. Trên hình, chỉ cần nhấp vào harvest và nhận đồng coin BALL.

### Tạo đòn bẩy cho các đồng coin farm

Bây giờ bạn có một số token farm được, bạn sẽ lựa chọn giữa:

* bán chúng để mua những đồng coin ưa thích &#x20;
* tái đầu tư vào trong bể thanh khoản khác

Mai Finance giới thiệu cho bạn lựa chọn thứ ba cho phép bạn thực hiện cả hai điều này. Một khi bạn nhận được đồng coin mà bạn đã farm được, bạn chuyển chúng lên các sàn DEX mà hỗ trợ bán đồng coin này. Thông thường bạn sẽ tìm thấy liên kết với DEX chấp nhận trao đổi đồng coin này tại menu của farm. Trong link sẽ có địa chỉ hợp đồng giúp bạn dễ dàng hơn.

![Swapping phần thưởng thành MATIC](<../../.gitbook/assets/Screen Shot 2021-08-09 at 11.14.29 AM.png>)

Tại thời điểm đó,  chúng ta đã quay lại bước mà chúng ta có token MATIC trong ví, sẵn sàng được gửi vào Mai Finance làm tài sản thế chấp để vay MAI, hoán đổi một phần của nó thành USDC, tạo một cặp LP và gửi lại vào trang trại. Bằng cách thực hiện chuyển đổi này, chúng ta "đảm bảo" 100% phần thưởng của mình bằng cách hoán đổi chúng thành một loại đồng coin ổn định hơn (ở đây là MATIC) và chúng ta gửi tiếp 50% phần thưởng của mình bể farming (hoặc thực tế, trong ví dụ này là 46% vì phí gửi là 4%).

Từ một góc độ khác, APR được áp dụng 100% cho số stablecoin bạn gửi vào bể, nên nếu bạn tiếp tục cộng dồn bạn sẽ nhận được số APY chỉ bằng một nửa số APY mà farm đã quảng cáo.

## Ước tính lợi nhuận

Tất cả kết quả trình bày dưới đây dựa vào một số giả định sau:

* Chúng ta bắt đầu với số tiền tương đương 60 MAI đã vay so với số tiền MATIC trị giá 120$
* APR của farm giữ ở mức 176,99% trong khoảng thời gian này, tương ứng với mức tăng là 0,484% hàng ngày
* Giá trị của MATIC và BALL giữ nguyên trong khoảng thời gian này.

Những giả định này rõ ràng là không áp dụng được với thực tế, APR sẽ giảm dần theo thời gian khi thanh khoản nhiều hơn được cung cấp cho bể và khi token của farm biến động về giá.

### Kết quả ước tính sơ bộ

| Ngày | Giá trị LP  | Giá trị thưởng | Số MATIC cộng dồn | LP mới tạo ra |
| :--: | ----------: | -------------: | ----------------: | ------------: |
|   1  |      $57.60 |         $0.279 |            $0.279 |        $0.139 |
|   2  |     $57.734 |         $0.280 |            $0.559 |        $0.140 |
|   3  |     $57.874 |         $0.280 |            $0.840 |        $0.140 |
|   4  |     $58.014 |         $0.281 |            $1.121 |        $0.141 |
|   5  |     $58.155 |         $0.282 |            $1.403 |        $0.141 |
|   6  |     $58.296 |         $0.282 |            $1.686 |        $0.141 |
|   7  |     $58.437 |         $0.283 |            $1.969 |        $0.142 |
|   8  |     $58.579 |         $0.284 |            $2.253 |        $0.142 |
|   9  |     $58.721 |         $0.285 |            $2.538 |        $0.142 |
|  10  |     $58.863 |         $0.285 |            $2.823 |        $0.143 |
|  11  |     $59.006 |         $0.286 |            $3.109 |        $0.143 |
|  12  |     $59.149 |         $0.287 |            $3.396 |        $0.143 |
|  13  |     $59.292 |         $0.287 |            $3.684 |        $0.144 |
|  14  |     $59.436 |         $0.288 |            $3.972 |        $0.144 |
|  15  |     $59.580 |         $0.289 |            $4.261 |        $0.144 |
|  16  |     $59.725 |         $0.289 |            $4.551 |        $0.145 |
|  17  |     $59.870 |         $0.290 |            $4.841 |        $0.145 |
|  18  |     $60.015 |         $0.291 |            $5.132 |        $0.145 |

* Vào ngày 1, phí 4% được áp dụng cho cặp MAI / USDC trị giá 60 đô la ban đầu của chúng ta.
* Vào cuối ngày 1, doanh thu đã tạo (0,279 đô la) được chuyển toàn bộ vào vault MATIC.&#x20;
* Vào cuối ngày 1, vì chúng ta đã thêm một số tiền vào kho tiền, chúng ta có thể vay thêm MAI.Để giữ tỷ lệ Tài sản đảm bảo trên Nợ là 200%, chúng ta chỉ vay 50% MATIC đã ký gửi (0,139 đô la)&#x20;
* Vào đầu ngày thứ 2, chúng ta cộng dồn $ 0,139 vào bể (và farm sẽ tính phí gửi 4%)&#x20;
* Vào đầu ngày 3, chúng ta bắt đầu lại với số token LP trị giá 0,134 đô la bổ sung

### Ước lượng APR, APY và doanh thu tăng trưởng

Số liệu ước lượng ở bảng trên dừng lại ở ngày thứ 18 vì chúng ta đã quay về điểm xuất phát ban đầu là 60$. Điều này có nghĩa là chúng ta đã hoàn vốn đủ, đây cũng là mục tiêu tối thiểu cho bất cứ farmer nào cần hướng tới.&#x20;

Khi đã qua ngày hoàn vốn, thì số tiền thưởng bạn mà bạn thu được khi tiếp tục farm sẽ là lợi nhuận của bạn. Bởi vì chúng ta chỉ farm stablecoin nên tổn thất tạm thời là không có.

Tuy nhiên, chúng ta cũng nên cân nhắc hoàn trả số phí ban đầu là 2.4$ vào ngày thứ 9 vì đó là thời điểm giá trị lợi  nhuận trong ví dưới dạng MATIC đạt tới số lượng đó. Nếu chúng ta chỉ bán số đồng coin farm để kiếm lợi nhuận và không tái đầu tư vào trong bể thì thời điểm đó khoản đầu tư của chúng ta sinh lời.

Về lợi nhuận, phần thưởng được cộng dồn vào bể chỉ bằng 50% APR. Điều này có nghĩa là với APR của farm được quảng cáo là 176,99%, tuy nhiên tốc độ tăng trưởng thực tế chỉ là 88,495% hàng năm, hay 0,242% hàng ngày.

Cũng có thể tính toán lợi nhuận chính xác được tích lũy vào ngày cụ thể trong farm, giả sử bạn đang cộng dồn hàng ngày, sử dụng công thức dưới đây cho Lợi tức đầu tư

$$
ROI_{NgàyN}=Vốn .đầu.tư.ban.đầu*(1+APRHàng.ngày)^{NgàyN}-Vốn.đầu.tư.ban.đầu
$$

Trong trường hợp farm có phí gửi là 4%, bạn cần nhân kết quả trên với 96%. Trong trường hợp cụ thể trên, chúng ta có thể nhanh chóng xác nhận rằng công thức có chuẩn xác hay không bằng cách so sánh kết quả của nó với bảng trên.

$$
ROI_{Ngày1} = [60 * (1+0.00242)^{1}-60]*0.96=$0.1396523836
$$

$$
ROI_{Ngày365}=[60*(1+0.00242)^{365}-60]*0.96=$81.80752927
$$

Bắt đầu từ $ 60,00 và tạo ra $ 81,81 sau 1 năm tạo ra tỷ lệ APY là 136,34%.

Nếu chúng ta so sánh điều này với APY lý thuyết được đưa ra bởi 88,495% APR bằng cách sử dụng công thức sau:

$$
APY = ( 1 + \frac{APR}{N})^N-1
$$

Với APR là 88.495% và N = 365 (cộng dồn hàng ngày)

$$
APY = ( 1 + \frac{0.88495}{365})^{365}-1=142.02\%
$$

Lưu ý rằng ước tính ở trên không tính đến phí gửi 4%, do đó có sự chênh lệch nhỏ.

Lợi nhuận trong ví MATIC chỉ đơn giản là gấp đôi lợi nhuận từ trang trại và chúng tôi có thể tính ROI vào một ngày nhất định bằng cách sử dụng cùng một công thức như trên và nhân kết quả với 2.

$$
ROI_{Day365} = [60 * (1 + 0.00242)^{365} - 60]*0.96*2=$163.6150585
$$

Đây là số MATIC mà chúng ta sẽ tạo ra bằng cách farming trong một năm, với khoản đầu tư ban đầu là 60 đô la trị giá MAI / USDC, giả sử APR của trang trại không đổi. Điều này cũng mang lại APY là 272,69%, gần bằng APR mà farm đã quảng cáo (farm thường không tính đến phí gửi 4% trong APR được hiển thị).

### Tổng kết sau một năm farming với stablecoin

Tại thời điểm cuối năm ta sẽ có

* $283.62 MATIC trong Vault (ban đầu là $120.00 + $163.62 lợi nhuận từ farming).
* $141.82 nợ (ban đầu $60.00 + $81.82 mượn và tái đầu tư).
* $141.82  MAI/USDC LP có trong farm

## Tuyên bố từ chối trách nhiệm

Tất cả được trình bày trong chiến lược này dựa vào các giả thuyết:

* Farm giữ mức APR liên tục trong vòng 1 năm (chắc chắn là sai)
* Có thể farm trong vòng cả năm (điều  này gần như không thể, tất cả farm đều kết thúc vòng farming sớm hay muộn).

Lưu ý thêm, APR của bể MAI / USDC trên Polypup sau 24h farming là 128,13%, chủ yếu là do giá BALL giảm dần.

Ngoài ra, farming với các cặp stablecoin có thể là cách "an toàn" nhất để kiếm lợi nhuận mà tránh được tổn thất tạm thời. Tuy nhiên không có gì đảm bảo rằng bạn có thể lấy lại 4% số tiền phí gửi ban đầu. Bạn cũng có thể tìm thấy các website mà ở đó có các bể cho stablecoin với mức phí chỉ 0% đến 1%, ngay cả với những bể không cặp với đồng bản vị của farm.

Thu hoạch phần thưởng và đổi lấy những tài sản có giá trị ổn định được coi là chiến lược farming tốt nhất. Việc vay MAI nhằm tái đầu tư một phần vào bể stablecoin để tăng doanh thu farming, mang lại lợi ích của bạn với 4% phí gửi mà farm đã lấy từ cặp LP của bạn, đây có thể không phải là điều tốt nhất nên làm nếu bạn không chắc chắn để lấy lại và có lẽ tốt hơn nên sử dụng một chiến lược khác để đầu tư lại thu nhập của bạn (đầu tư vào các bể bản vị của farm với lãi suất 0% và có APR cao).

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém (hoặc khiến bạn mất tiền) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự mình nghiên cứu.
{% endhint %}
