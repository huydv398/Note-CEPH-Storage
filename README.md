# Note-IOPS-FIO
 Ghi chép tìm hiểu IOPS và sử dụng FIO để test. 
## 1. What is IOPS
**IOPS (input/output operations per second)**
* là đơn vị đo lường tiêu chuẩn cho số lần đọc và ghi tối đa cho các vị trí lưu trữ không liền kề. IOPS được phát âm là EYE-OPS
* IOPS mô tả hiệu suất trong ổ đĩa thể rắn (SSD), ổ đĩa cứng (HDD) và mạng vùng lưu trữ. Tuy nhiên, số IOPS không phải là điểm chuẩn thực tế và các số do nhà cung cấp quảng cáo có thể không tương ứng với hiệu suất trong thế giới thực
## 2. Giải thích IOPS, latency và throughput
* [Throughput - Thông lượng](/Docs/throughput.md): Đo lường bao nhiêu đơn vị thông tin mà hệ thống có thể xử lý trong một khoảng thời gian. Nó có thể đề cập đến số lượng hoạt động I/O mỗi giây, nhưng thương được đo bằng Bytes trên giây. Riêng IOPS và throughput không thể cung cấp phép đo hiệu suất chính xác.
* [Latency - Độ trễ](/Docs/Latency.md) đo thời gian từ khi đưa ra yêu cầu đến khi nhận được phản hồi. Liên quan đến IOPS, độ trễ là thước đo khoảng thời gian cần thiết để hoàn thành một yêu cầu I / O đơn lẻ theo quan điểm của ứng dụng.

Mặc dù không cung cấp một bức tranh hoàn chỉnh, nhưng việc kết hợp các phép đo độ trễ, IOPS và thông lượng có thể giúp đánh giá hiệu suất
## 3. Đo lường IOPS
IOPS thường được đo bằng 1 công cụ kiểm tra mã nguồn mở được gọi là lometer. Máy đo IOPS xác định IOPS đỉnh trong các điều kiện đọc/ghi khác nhau. Việc đo lường cả IOPS và độ trễ có thể giúp quản trị viên mạng dự đoán mức tải mà mạng có thể xử lý mà hiệu suất không bị ảnh hưởng. Lometer đã ngừng sx vào 2006

Có thể tính toàn IOPS mà không cần lometer, nhưng kết quả sẽ khác nhau tùy thuộc vào loại hiệu suất của khối lượng công việc. Nói chung, có 3 loại hiệu suất khối lượng công việc: Random, tuần tự & hỗn hợp. RAID cũng có thể ảnh hưởng đến các tính toán của IOPS, vì mỗi thao tác ghi dẫn dẫn đến nhiều lần ghi vào mảng lưu trữ(Storage array)

## 4. IOPS in SSDs vs. HDDs
Ổ cứng HDD sử dụng phương trình tiêu chuẩn để xác định IOPS, nhưng ổ SSD hoạt động khác. Với HDD, IOPS phụ thuộc vào thời gian tìm kiếm, nhưng SSD phụ thuộc vào bộ điều khiển bên trong thiết bị. Hiệu suất SSD thay đổi theo thời gian, đạt đỉnh điểm từ rất sớm. Tuy nhiên, ngay cả sau khi vào trạng thái ổn định, SSD vẫn vượt trội hơn HDD về IOPS. Các ổ cúng HDD cũng phải vật lộn với độ trễ cao hơn và thời gian đọc/ghi lâu hơn.

## Chỉ số IOPS có quan trọng không?
Mặc dù được các nhà cung cấp lưu trữ chào mời, nhưng vấn đề đặt ra là có bao nhiêu IOPS để đo lường. Tùy thuộc vào khối lượng công việc, các con số có thể khác nhau rất nhiều, vì vậy việc phân loại hiệu suất chỉ dựa trên IOPS không có ý nghĩa gì.

Vì số IOPS bị ảnh hưởng bởi kích thước của khối dữ liệu và hiệu suất khối công việc, nên không có khả năng các nhà cung cấp sẽ sử dụng các biến chuẩn khi liệt kê IOPS. Ngay cả khi một hệ thống tiêu chuẩn được sử dụng để xác định IOPS, với kích thước khối đã đặt và kết hợp đọc/ghi, con số đó không có ý nghĩa trừ khi nó khớp với một khối lượng công việc cụ thể.
