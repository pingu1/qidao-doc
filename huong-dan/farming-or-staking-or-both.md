---
description: >-
  Hướng dẫn này sẽ trình bày một chiến lược làm nhấn mạnh những tương tác tuyệt
  vời giữa Mai Finance, QuickSwap và Adamant sau khi ra mắt bể LP mới trên Mai
  Finance và QuickSwap.
---

# Farming hoặc Staking? Hoặc cả hai?

![](../.gitbook/assets/screen-shot-2021-09-03-at-9.24.12-am.png)

## Intro

Khi bạn đang sử dụng các ứng dụng DeFi \(Tài chính phân quyền\), đặc biệt là khi bạn đang yield farming, bạn có xu hướng kết thúc với một loạt các token bản vị của farm đó. Nếu hầu hết mọi người chỉ đơn giản là bán những token này để mua thêm hoặc những đồng tiền yêu thích của họ, chúng tôi sẽ cố gắng giới thiệu một số cách để thực sự giữ và đưa chúng vào hoạt động nhằm tăng doanh thu của bạn.

Để làm như vậy, chúng tôi sẽ sử dụng các bể LP mới \(Nhóm cung cấp tính thanh khoản\) được ra mắt trên QuickSwap vào đầu tháng 9 năm 2021, đang sử dụng mã token Qi từ Mai Finance. Nếu bạn cần hiểu rõ các ứng dụng QuickSwap và Adamant là gì, vui lòng đọc hướng dẫn [Xếp chồng DApps.](stack-dapps-like-lego-bricks.md)

## Trình bày ứng dụng và các bể 

### Farming

Để tối đa hóa lợi nhuận, chúng tôi sẽ sử dụng 3 ứng dụng khác nhau

* Mai Finance
* QuickSwap
* Adamant

Chúng ta cũng sẽ sử dụng các bể như sau:

* Qi/MATIC trên Mai Finance để tạo ra Qi
* Qi/WETH trên QuickSwap để tạo ra QUICK và ADDY
* Qi/QUICK trên Adamant để tạo ra ADDY và MATIC

Bạn đã có thể thấy rằng mỗi nền tảng đang tạo ra các mã token có thể cung cấp đầu vào cho các bể khác trên các nền tảng khác. Ý tưởng là sử dụng mã token Qi thu được trên Mai Finance kết hợp với mã token QUICK thu được trên QuickSwap và sử dụng 2 trên Adamant. Adamant sẽ tạo mã ADDY cho phép bạn nhận cổ tức WMATIC. Mã token WMATIC có thể được khóa trên Mai Finance trong kho tiền WMATIC để mượn MAI, sau đó mua MATIC và WETH mà sau đó chúng ta có thể sử dụng với  Qi để tăng vị thế của bạn trên cả Mai Finance và QuickSwap

### Staking 

Bạn cũng cần biết rằng các token dư ra có thể stake trên Mai Finance và Quickswap:

* Qi trên Mai Finance **VÀ** QuickSwap có thể dùng bình chọn  trên QIP \(Đề xuất cải tiến QiDao\).
* Qi trên Mai Finance có thể được khóa. Nếu bạn khóa số Qi của mình lại, bạn sẽ có đủ điều kiện để nhận cổ tức trả bằng Qi phân phối vào thứ Tư hàng tuần. Chi tiết sẽ tại phần tiếp theo
* QUICK trên QuickSwap có thể stake và tạo ra thêm token QUICK tại Dragon's Lair.
* khóa QUICK \(dQUICK\) có thể cũng được sử dụng trên QuickSwap để tạo ra các token khác tại Dragon's Syrup, và bể mà chúng ta chọn sẽ là bể ADDY.
* ADDY trên Adamant được tự đông khóa trong vòng 90 ngày nhưng sẽ được chia cổ tức bằng WMATIC
* ADDY trên Adamant cũng  có thể được khóa nhằm tăng tỷ lệ APRs/APYs \(**Lãi suất hàng năm** / **Lãi suất cộng dồn hàng năm**\) trong bể mà bạn đã tham gia vào, cũng như tạo thêm ADDY và tăng cổ tức MATIC của bạn.

## Khởi động hệ thống

![](../.gitbook/assets/screen-shot-2021-09-08-at-6.54.08-am.png)

Những gì sau đây là một mô phỏng được thực hiện với khoản đầu tư ban đầu trị giá 1000 đô la cho các cặp Qi / MATIC và Qi / WETH LP và các APR / APY hiện tại được cung cấp bởi các nền tảng khác nhau vào ngày 9 tháng 9 năm 2021. Trên thực tế tỷ giá sẽ khác nhau, giá mã token sẽ thay đổi, một số chương trình sẽ kết thúc, v.v. vì vậy kết quả cuối cùng chỉ là ước tính bạn có thể nhận được gì nếu mọi thứ vẫn ổn định \(không bao giờ xảy ra\).

### Ngày 1

{% hint style="info" %}
**CHÚ Ý:** Các bể được sử dụng trong hướng dẫn này đã hoạt động vài giờ trước khi phát hành. APR và APY rõ ràng sẽ không giữ nguyên và một số bản sửa đổi đối với tài liệu sẽ được thực hiện sau một vài ngày. Xin vui lòng, DYOR và đầu tư một cách thận trọng.
{% endhint %}

Vì chúng ta có 500$ của mỗi cặp Qi/MATIC và cặp Qi/ETH, chúng ta sẽ gửi chúng trên Mai Finance và QuickSwap. Cần lưu ý thêm là bạn thích Qi hay QUICK thì bạn chỉ cần gửi thêm cặp thanh khoản vào nền tảng tương ứng để tạo ra nhiều token ưa thích hơn và stake nhiều hơn. Đối với trường hợp này chúng ta sẽ theo tỷ lệ 50/50.

* $500 của cặp Qi/MATIC sẽ ở trên Mai Finance với APR là 1160.65%
* $500 của cặp Qi/WETH sẽ trên QuickSwap với APR là 1817.44%

Chúng ta cũng sẽ sử dụng các APR sau cho phần còn lại của minh họa

* dQUICK APR từ Dragon's Lair là 17.28%
* ADDY APR từ Dragon's Syrup là 17.08%
* Qi/QUICK APR trên Adamant tự động cồng dồn cặp thanh khoản là 133%
* Qi/QUICK APR trên Adamant cho ADDY là 131%
* WMATIC APR trên Adamant là 35% của số token ADDY đã khóa

Vì APR trên Mai Finance thấp hơn APR trên QuickSwap, nên chúng ta sẽ sử dụng 100% Qi được tạo trên Mai Finance để tạo thêm mã Qi / QUICK \(không bán nhưng kết hợp với mã QUICK nhận được trên QuickSwap\), nghĩa là tại cuối ngày, chúng ta còn lại 0 Qi. Tất nhiên, nếu bạn cân đối khoản đầu tư ban đầu của mình theo cách khác, bạn có thể nhận được Qi còn lại và còn lại 0 QUICK.

Ở cuối ngày thứ nhất chúng ta sẽ có

| Dạng phần thưởng | Giá trị bằng dollars |
| :--- | :--- |
| dQUICK trên QuickSwap | 8.997 |
| ADDY trên QuickSwap | 0 |
| Qi/QUICK trên Adamant | 31.799 |
| ADDY trên Adamant | 0 |
| WMATIC trên Adamant | 0 |

### Ngày 2

Vào ngày 2, dQUICK được gửi trên QuickSwap Dragon's Syrup bắt đầu tạo ra các token ADDY, cũng như cặp Qi / QUICK LP trên Adamant. Vào cuối Ngày 2, chúng tôi sẽ nhận được

| Dạng phần thưởng | Giá trị bằng dollar |
| :--- | :--- |
| dQUICK trên QuickSwap | 17.998 |
| ADDY trên QuickSwap | 0.0042 |
| Qi/QUICK trên Adamant | 63.713 |
| ADDY trên Adamant | 0.114 |
| WMATIC trên Adamant | 0 |

Đừng quên nhận thưởng ADDY hàng ngày để có thể tạo ra cổ tức WMATIC

### Ngày 3

Vào ngày thứ 3, các token ADDY thu thập trên Adamant bắt đầu tạo ra cổ tức WMATIC. Có nghĩa cuối ngày thứ 3, danh mục đầu tư của chúng ta sẽ có

| Dạng phần thưởng | Giá trị bằng $ |
| :--- | :--- |
| dQUICK trên QuickSwap | 27.004 |
| ADDY trên QuickSwap | 0.025 |
| Qi/QUICK trên Adamant | 95.743 |
| ADDY trên Adamant | 0.343 |
| WMATIC trên Adamant | 0.0001 |

Bắt đầu ngày thứ 4, chúng ta sẽ có thể

* thu cổ tức WMATIC 
* gửi một phần WMATIC vào Mai Finance và vay MAI 
* bán MAI để mua thêm WETH 
* ghép MATIC còn lại với Qi và WETH với một số Qi khác được tạo trên Mai Finance 
* gửi thêm cặp Qi / WMATIC trên Mai Finance và cặp Qi / WETH trên QuickSwap

Tại thời điểm này, vòng quay của chúng ta thực sự bắt đầu và chúng ta có thể ước lượng doanh thu như sau:

## Kết quả farming

### Công việc hàng ngày

Thao tác hàng ngày sẽ bao gồm các giao dịch sau đây:

* Thu hoạch Qi trên Mai Finance
* Thu hoạch WMATIC trên Adamant 
* Gửi 66% WMATIC vào Mai Finance 
* Vay MAI 50% số tiền đặt cọc 
* Đổi MAI lấy WETH 
* Tạo cặp Qi / WMATIC trên QuickSwap 
* Gửi Qi / WMATIC vào Mai Finance 
* Tạo cặp Qi / WETH trên QuickSwap 
* Gửi tiền Qi / WETH trên QuickSwap 
* Thu hoạch QUICK trên QuickSwap 
* Tạo cặp Qi / QUICK trên QuickSwap 
* Gửi  QUICK  còn lại vào Dragon's Lair 
* Gửi  dQUICK vào Dragon's Syrup 
* Thu hoạch mã token ADDY từ Dragon's Syrup 
* Thu hoạch mã token ADDY từ Adamant 
* Nạp Qi / QUICK mới trên Adamant 
* Tiền gửi thu được ADDY trên Adamant \(khóa\)

### Kết quả sơ bộ sau 1 tháng

| Tháng | dQUICK | Qi/QUICK | ADDY | Qi/MATIC  Qi/WETH |
| :--- | :--- | :--- | :--- | :--- |
| 1 | $280.96 | $1,040.78 | $54.97 | $0.91 |
| 2 | $557.79 | $2,162.98 | $224.36 | $7.89 |
| 3 | $842.08 | $3,413.73 | $521.09 | $27.85 |
| 4 | $1,138.60 | $4,816.62 | $960.17 | $68.48 |
| 5 | $1,454.30 | $6,405.18 | $1,559.60 | $138.44 |
| 6 | $1,798.77 | $8,224.86 | $2,341.64 | $247.49 |
| 7 | $2,184.58 | $10,335.38 | $3,334.13 | $406.84 |
| 8 | $2,627.76 | $12,813.60 | $4,572.23 | $629.47 |
| 9 | $3,148.40 | $15,757.01 | $6,100.39 | $930.60 |
| 10 | $3,771.42 | $19,288.05 | $7,974.83 | $1,328.32 |
| 11 | $4,527.47 | $23,559.40 | $10,266.47 | $1,844.31 |
| 12 | $5,454,16 | $28,760.60 | $13,064.51 | $2,504.79 |

### Day 365

Sau 1 năm, trạng thái cuối cùng của số vốn của chúng ta sẽ là

| Dạng phần thưởng | Giá trị bằng dollar |
| :--- | :--- |
| dQUICK trên QuickSwap | 5,628.29 |
| ADDY trên QuickSwap | 365.25 |
| Qi/QUICK trên Adamant | 29,733.58 |
| ADDY trên Adamant | 13,587.56 |
| Qi/MATIC + Qi/WETH bổ sung | 2,631.07 |

Lưu ý rằng ADDY đã được tạo thông qua  QuickSwap chưa được thu hoạch hàng ngày và được thêm vào để tăng phần thưởng ADDY trên Adamant trong minh họa này. Ngoài ra, chúng ta chỉ stake số ADDY được thưởng. Sau khoảng thời gian 90 ngày, nếu bạn nhận ADDY và khóa chúng, bạn sẽ tăng phần thưởng ADDY nhiều hơn và tạo ra nhiều WMATIC hơn.

Cuối cùng, sau một năm, doanh thu được tạo ra trị giá là 51.580,50 đô la. Nếu chúng ta coi khoản đầu tư ban đầu là $ 1.000 cho Qi / MATIC và Qi / WETH, thì  APY cuối cùng là 5,087,39%.

## Tuyên bố từ chối trách nhiệm

Hướng dẫn này chắc chắn không phải là lời khuyên tài chính, nó được thực hiện với mục tiêu giáo dục. Bạn cần chú ý đến sự thay đổi giá cả, cung và cầu, ngày kết thúc chương trình thưởng, tổn thất tạm thời, v.v. đầu tư những gì bạn sẵn sàng những gì có thể mất.

{% hint style="info" %}
Hãy nhớ rằng một chiến lược hoạt động tốt tại một thời điểm nhất định có thể hoạt động kém \(hoặc khiến bạn mất tiền\) vào một thời điểm khác. Hãy cập nhật thông tin, theo dõi thị trường, theo dõi các khoản đầu tư của bạn và như mọi khi, hãy tự nghiên cứu.
{% endhint %}

