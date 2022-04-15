# 
* **Latency** đo lường độ trễ của hệ thống, ở đây nó đại diện cho thời gian đáp ứng yêu cầu IO, độ trễ trung bình của 1 IO. Số liệu này đối với HDD thường được tính bằng millisecond, đối với SSD tính bằng microsecond.

* **IOPS (I/O Per Second)** tượng trưng cho số lượng hoạt động IO có thể diễn ra trong 1 giây. Số liệu IOP rất quan trọng trong các hệ thống lưu trữ, đặc biệt là số lượng và tính ngẫu nhiên. Khi đánh giá 1 thiết bị cần xem xét giá trị Mã IOPS, với kích cỡ, bản chất IO.

* **Băng thông** (Bandwidth hoặc cũng được biết là throughput), giá trị đại diện cho khối lượng dữ liệu có thể xử lý trong 1 thời điểm - có thể hiểu cách khác, nó là lượng dữ liệu được truyền đến hệ thống mỗi giây. Số liệu được do thường tính theo đơn vị MB/s hoặc GB/s. [IO Size](/Terms/IO-size.md) có thể là 4KB, 8KB, 32KB, ..

Throughput đơn giản là tích giá trình IOPS với IO size.
```
Throughput   =   IOPS   x   I/O size
```
Ví dụ:
```
VD: 2048 IOPS với 8k blocksize
Throughput = IOPS x IO size = 2048 * 8K = 16,384 KB/S

Giá trị Throughput tương đương 16 MB/S.
```

Latency cũng ảnh hướng tới hiệu năng, độ trệ hệ thống tăng khiến các tiến trình diễn ra chậm hơn.
```
Latency   ∝   IOPS
```