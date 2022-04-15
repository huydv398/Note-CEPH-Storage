# IO Size.
## Kích thước io là gì?
* Kích thước yêu cầu IO có ảnh hưởng đến thông lượng hiệu suất - nói chung, kích thước IO càng lớn, băng thông lưu trữ càng cao. Điều rất thường bị bỏ qua là trong hầu hết các trường hợp, các công cụ đang hiển thị kích thước IO trung bình. Hãy nhớ rằng hầu hết các khối lượng công việc sản xuất có sự kết hợp của các kích thước IO.
* Kích thước IO lưu trữ điển hình nằm trong khoảng từ 512 byte đến 256 KB hoặc thậm chí 1 MB cho các thiết bị mới hơn.
## Tính IO Size
Để tính toán kích thước I/O trung bình của mỗi đĩa, tổng số byte đọc và ghi được chia cho tổng số I / O trong khoảng thời gian thu thập.
## IO latency?
Độ trễ là thời gian I/O thực hiện từ khi yêu cầu đến khi hoàn thành. Độ trễ được đo bằng ms (milliseconds - mili giây) hoặc msec (microseconds - micro giây). I/O 512 kB. Theo ý kiến ​​của tôi, hầu hết các nhà cung cấp nói quá nhiều về IOPS, Thông lượng và Độ trễ cho một trường hợp sử dụng rất cụ thể.
##  block size in storage?
Là lượng không gian đĩa liền kề lớn nhất có thể được phân bổ cho một tệp và do đó là lượng dữ liệu lớn nhất có thể được truy cập trong một thao tác I/O đơn lẻ. Một khối con là đơn vị nhỏ nhất của không gian đĩa liền kề có thể được cấp phát. Các tệp nhỏ hơn một kích thước khối được lưu trữ trong các phân đoạn.
