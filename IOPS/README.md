# Note-IOPS-FIO
 Ghi chép tìm hiểu IOPS và sử dụng FIO để test. 
1. [What is IOPS ?](#1-what-is-iops)
1. [Giải thích IOPS, latency và throughput](#2-giải-thích-iops-latency-và-throughput)
1. [Đo lường IOPS](#3-đo-lường-iops)
1. [IOPS in SSDs vs. HDDs](#4-iops-in-ssds-vs-hdds)
1. [Chỉ số IOPS có quan trọng không?](#5-chỉ-số-iops-có-quan-trọng-không)
1. [Các thuật ngữ](#6-term)
1. [Làm cách nào để tính IOPS?](#7-làm-cách-nào-để-tính-iops)
## 1. What is IOPS ?
**IOPS ([input/output](/Terms/I-O.md) operations per second)**
* là đơn vị đo lường tiêu chuẩn cho số lần đọc và ghi tối đa cho các vị trí lưu trữ không liền kề. IOPS được phát âm là EYE-OPS
* IOPS mô tả hiệu suất trong ổ đĩa thể rắn (SSD), ổ đĩa cứng (HDD) và mạng vùng lưu trữ. Tuy nhiên, số IOPS không phải là điểm chuẩn thực tế và các số do nhà cung cấp quảng cáo có thể không tương ứng với hiệu suất trong thế giới thực
### Các yếu tố quan trọng của storage
Có 3 yếu tố quan trọng trong Storage:
* **IOPS**
* **Bandwidth** 
* **Latency**
### Giải thích IOPS, latency và throughput
* [**Bandwidth** - Throughput - Thông lượng](/Terms/throughput.md): 
    * Đo lường bao nhiêu đơn vị thông tin mà hệ thống có thể xử lý trong một khoảng thời gian. Nó có thể đề cập đến số lượng hoạt động I/O mỗi giây, nhưng thương được đo bằng Bytes trên giây. Riêng IOPS và throughput không thể cung cấp phép đo hiệu suất chính xác.
    * giá trị đại diện cho khối lượng dữ liệu có thể xử lý trong 1 thời điểm - có thể hiểu cách khác, nó là lượng dữ liệu được truyền đến hệ thống mỗi giây. Số liệu được do thường tính theo đơn vị MB/s hoặc GB/s
* [Latency - Độ trễ](/Terms/Latency.md) đo thời gian từ khi đưa ra yêu cầu đến khi nhận được phản hồi. Liên quan đến IOPS, độ trễ là thước đo khoảng thời gian cần thiết để hoàn thành một yêu cầu I / O đơn lẻ theo quan điểm của ứng dụng.

Mặc dù không cung cấp một bức tranh hoàn chỉnh, nhưng việc kết hợp các phép đo độ trễ, IOPS và thông lượng có thể giúp đánh giá hiệu suất
## 2. Tầm quan trọng
[Tại đây](/Docs/iops-latency-throughput.md)
## 3. Đo lường IOPS
IOPS thường được đo bằng 1 công cụ kiểm tra mã nguồn mở được gọi là lometer. Máy đo IOPS xác định IOPS đỉnh trong các điều kiện đọc/ghi khác nhau. Việc đo lường cả IOPS và độ trễ có thể giúp quản trị viên mạng dự đoán mức tải mà mạng có thể xử lý mà hiệu suất không bị ảnh hưởng. Lometer đã ngừng sx vào 2006

Có thể tính toàn IOPS mà không cần lometer, nhưng kết quả sẽ khác nhau tùy thuộc vào loại hiệu suất của khối lượng công việc. Nói chung, có 3 loại hiệu suất khối lượng công việc: Random, tuần tự & hỗn hợp. RAID cũng có thể ảnh hưởng đến các tính toán của IOPS, vì mỗi thao tác ghi dẫn dẫn đến nhiều lần ghi vào mảng lưu trữ(Storage array)

## 4. IOPS in SSDs vs. HDDs
Ổ cứng HDD sử dụng phương trình tiêu chuẩn để xác định IOPS, nhưng ổ SSD hoạt động khác. Với HDD, IOPS phụ thuộc vào thời gian tìm kiếm, nhưng SSD phụ thuộc vào bộ điều khiển bên trong thiết bị. Hiệu suất SSD thay đổi theo thời gian, đạt đỉnh điểm từ rất sớm. Tuy nhiên, ngay cả sau khi vào trạng thái ổn định, SSD vẫn vượt trội hơn HDD về IOPS. Các ổ cúng HDD cũng phải vật lộn với độ trễ cao hơn và thời gian đọc/ghi lâu hơn.

## 5. Chỉ số IOPS có quan trọng không?
Mặc dù được các nhà cung cấp lưu trữ chào mời, nhưng vấn đề đặt ra là có bao nhiêu IOPS để đo lường. Tùy thuộc vào khối lượng công việc, các con số có thể khác nhau rất nhiều, vì vậy việc phân loại hiệu suất chỉ dựa trên IOPS không có ý nghĩa gì.

Vì số IOPS bị ảnh hưởng bởi kích thước của khối dữ liệu và hiệu suất khối công việc, nên không có khả năng các nhà cung cấp sẽ sử dụng các biến chuẩn khi liệt kê IOPS. Ngay cả khi một hệ thống tiêu chuẩn được sử dụng để xác định IOPS, với kích thước khối đã đặt và kết hợp đọc/ghi, con số đó không có ý nghĩa trừ khi nó khớp với một khối lượng công việc cụ thể.
## 6. Term
1. [Driver type - FC](/Terms/Driver-type/FC.md)
1. [Driver type - SAS](/Terms/Driver-type/SAS.md)
1. [Driver type - SATA](/Terms/Driver-type/Sata.md)
1. [RPM](/Terms/RPM.md)
1. [QoS - Quality of service ](/Terms/QoS.md)
1. [Latency](/Terms/Latency.md)
1. [Throughput](/Terms/throughput.md)
1. [Jitter](/Terms/Jitter.md)
1. [Capacity](/Terms/Capacity.md)
1. [I/O Size](/Terms/IO-size.md)

## 7. Làm cách nào để tính IOPS?
IOPS là một hàm của **rotational speed** - tốc độ quay (còn gọi là tốc độ trục chính), **latency** độ trễ và **seek time** thời gian tìm kiếm. Phương trình rất đơn giản:
```
1 / (seek + latency) = IOPS.
```
## Bendmark by Fio 
Fio tạo ra một số luồng hoặc quy trình thực hiện một loại hành động I/O cụ thể do người dùng chỉ định. fio nhận một số tham số toàn cục, mỗi tham số được kế thừa bởi luồng trừ khi các tham số được cung cấp cho chúng ghi đè cài đặt đó được đưa ra. Việc sử dụng điển hình của fio là viết một tệp công việc phù hợp với tải I/O mà người ta muốn mô phỏng.

* Fio được viết bởi Jens Axboe
* Fio works on (at least) Linux, Solaris, AIX, HP-UX, OSX, NetBSD, OpenBSD, Windows, FreeBSD, and DragonFly

Hướng dẫn sử dụng Fio --> [Here](/FIO/README.md)
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()
1. []()