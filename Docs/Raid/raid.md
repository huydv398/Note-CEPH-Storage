# RAID
RAID là viết tắt của Redundant Array of Inexpensive Disks (Hệ thống đĩa dự phòng).
## RAID là gì?
* Hình thức ghép nhiều ổ đĩa cứng vật lý thành một hệ thống ổ đĩa cứng có chức năng gia tăng tốc độ đọc/ghi dữ liệu hoặc nhằm tăng thêm sự an toàn của dữ liệu chứa trên hệ thống đĩa hoặc kết hợp cả yếu tố an toàn và tốc độ.

* RAID là một giải pháp để lưu trữ dữ liệu trên nhiều ổ cứng hoặc đĩa cứng để bảo vệ dữ liệu trong trường hợp rủi ro hỏng ổ cứng.
## Lợi thế của RAID

Có 3 lý do chính để áp dụng RAID:

* Dự phòng
* Hiệu quả cao
* Giá thành thấp
### So với ổ cứng thông thường thì RAID giải quyết gì?
* Giải quyêt được lỗi hỏng hóc của một hoặc nhiều ổ cứng trong RAID. RAID cho phép 1 số lượng ổ nhất định hư hại về phần cứng.

* Tăng hiệu suất đọc/ ghi trên RAID với tốc độ ổ cứng.
* Dung lượng lớn: Tổng dung lượng ổ lớn hơn là sử dụng duy nhất 1 ổ và khi 1 ổ duy nhất đó gặp vấn đề thi cả máy chủ gặp vấn đề.

#### RAID 0
![Imgur](https://i.imgur.com/5Qvcsiz.png)
RAID 0 là cấp độ cơ bản. Các dữ liệu cần chứa trên hệ thống RAID 0 được phân tách thành hai thành phần để chứa trên hai ổ cứng khác nhau. RAID cho phép ghi dữ liệu lên lên theo 1 phương thức được gọi là Striping với tối thiểu là hai đĩa cứng. RAID 0 thích hợp cho người dùng cần truy nhanh dữ liệu lớn.

* Ưu điểm: Tăng tốc độ đọc ghi của đĩa (gấp đôi bình thường theo lý thuyết)
* Nhược điểm: Tính an toàn thấp. Nếu một đĩa bị hỏng thì dữ liệu trên các đĩa còn lại sẽ không sử dụng được
* Đối tượng sử dụng: Thích hợp với những dịch vụ cần lưu trữ và truy xuất với tốc độ cao. Chẳng hạn như dịch vụ video streaming, chạy cơ sở dữ liệu.

#### RAID 1
![Imgur](https://i.imgur.com/m9Xlg3F.png)

Có khả năng đảm bảo an toàn dữ liệu từ ổ cứng, Nó cần 2 ổ cứng để làm việc. Dữ liệu sẽ được ghi vào hai ổ đĩa giống nhau.

Trong trường hợp bị trục trặc, ổ còn lại sẽ tiếp tục hoạt động bình thường. Có thể thay thế ổ đĩa bị hỏng mà không cần lo lắng đến vấn đề mất thông tin

Dung lượng cuối cùng của hệ thống RAID 1 bằng dung lượng của ổ đơn(hai ổ 100GB chay RAID sẽ cho hệ thống nhìn thấy duy nhất một ổ RAID 100GB).

#### RAID 1+0 hay RAID 0+1
![Imgur](https://i.imgur.com/RNZCj0Z.png)

Là sự kết hợp giữa RAID 0 và RAID 1. Chi phí khá đắt do cần ít nhất 4 Ổ cứng để hoạt động được RAID 0+1, dung lượng cuối cùng sẽ bằng dung lượng của tổng 2 ổ, ví dụ chạy 4 ổ 100GB thì lượng dữ liệu được hiển thị là 200GB

#### RAID 2
RAID 2 gồm 2 cụm ổ đĩa, cụm thứ nhất chứa các dữ liệu được phân tác giống như RAID 0, cụm 2 chứa các mã ECC dành cho sửa chữa lỗi ở cụm thứ nhất. Sự hoạt động của các ổ đĩa ở RAID 2 đồng thời để đảm bảo rằng các dữ liệu được đọc đúng, chính do vậy chúng không hiệu quả và không còn được sử dụng
#### RAID 3 RAID4
Là sự cải tiến của RAID 0 nhưng có thêm ít nhất một ổ cứng chứa thông tin có thể khôi phục lại dữ liệu đã hư hongwr của các ổ cứng RAID 0. 

2 ổ cứng chứa thông tin được phân tán và ổ cứng thứ 3 chứa tất cả dữ liệu.

#### RAID 5 
![Imgur](https://i.imgur.com/S5QLl46.png)

RAID 5 thực hiện chia đều dữ liệu trên các ổ đĩa giống như RAID 0 nhưng với một cơ chế phức tạp hơn.

Là dạng RAID mạnh mẽ nhất cho người dùng văn phòng và gia đình với 3 hoặc 5 ổ cứng riêng biệt. Dữ liệu và bản sao lưu được chia lên tất cả các ổ cứng. 

RAID 5 vừa đảm bảo tốc độ có cải thiện, vừa giữ được tính an toàn cao. Dung lượng đĩa cứng: nếu bạn dùng 3 ổ 100GB thì dung lượng cuối dùng là 200GB

RAID 5 cần ít nhất 3 ổ cứng

#### RAID 6

![Imgur](https://i.imgur.com/zkGksag.png)

Một phần giống RAID 5 nhưng lại được sử dụng lặp lại nhiều hơn số lần sự phân tách dữ liệu vào các đĩa cứng khác nhau. Ví dụ RAID 5 thì mỗi lần phân tách thành hai vị trí lưu trữ trên 2 đĩa cứng lưu trữ khác nhau nhưng RAID 6  thì mỗi dữ liệu lưu ở 3 vị trí trở lên

RAID 6 yêu cầu ít nhất 4 ổ cứng

Khả năng chịu rủi ro cao. nếu 4 ổ cứng thì cho phép hỏng 2 ổ cứng máy vẫn hoạt động bình thường.

### Cần gì để chạy RAID?

Để chạy RAID, bạn cần 1 card RAID điều khiển và 2 ổ cứng có dung lượng giống nhau. 

Xác định kiểu RAID muốn sử dụng

Bộ điều khiển RAID (RAID Controller) là nơi tập chung các cáp dữ liệu kết nối các đĩa cứng trong hệ thống RAID và nó được xử lý toàn bộ dữ liệu đi qua nó. Bộ điều khiển này có nhiều dạng khác nhau, từ Card tách rời cho đến chip tích hợp.
