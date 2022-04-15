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