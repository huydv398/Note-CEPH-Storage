# Throughput - Thông lượng
* Là thước đo hệ thống có thể xử lý được bao nhiêu đơn vị thông tin trong một khoảng thời gian nhất định. 
* Các thước đo liên quan về năng suất hệ thống bao gồm tốc độ hoàn thành một số khối lượng công việc cụ thể và thời gian phản hồi, khoảng thời gian giữa một yêu cầu của từng người dùng tương tác và nhận được phản hồi.

## Các loại througput
* Trong lịch sử, Throughput là thước đo hiệu quả so sánh của các máy tính thương mại lớn chạy nhiều chương trình đồng thời. Một thước đo throughput ban đầu là số lượng công việc hàng loạt được hoàn thành trong một ngày.
* Một Benchmark có thể được sử dụng để đo throughput.
* **Trong truyền dữ liệu**, Network throughput là lượng dữ liệu được di chuyển thành công từ nơi này tới nơi khác trong một khoảng thời gian nhất định và thường được đo bằng bit/giây(bps), như megabits trên giây(Mbps) hoặc gigabits per second (Gbps).
* **Trong hệ thống lưu trữ**, throughput đề cập đến lượng dữ liệu có thể nhận và ghi vào phương tiện lưu trữ hoặc đọc từ phương tiện và trả về hệ thống yêu cầu, thường được đo bằng bytes trên giây (Bps). Nó cũng có thể đề cập đến số lượng các hoạt động đầu vào hoặc đầu ra(I/O) được phản hồi trong 1 giây (IOPS)
* Thông lượng cũng áp dụng ở các cấp cao hơn của cơ sở hạ tầng CNTT. Cơ sở dữ liệu hoặc phần mềm trung gian khác có thể được thảo luạn về "Giao dịch mỗi giây"(transactions per second - TPS); Máy chủ web có thể được thảo luận về số lượt xem site mỗi phút
## Throughput, bandwidth và letancy
Một số thuật ngữ liên quan - Throughput, bandwidth và letancy - đôi khi bị nhầm lẫn với nhau. Tóm lại,
* **Network bandwidth** đề cập đến dung lượng của mạng để dữ liệu được di chuyển trong một thời điểm.
* Throughput thể hiện lượng dữ liệu
* letancy đề cập đến tốc độ truyền dữ liệu

throughput và latency cùng phản ánh hiệu suất của mạng
## Throughput vs network Bandwidth
Bandwidth là dung lượng của liên kết truyền thông mạng có dây hoặc không dây để truyền lượng dữ liệu tối đa từ điểm này tới điểm khác qua một mạng máy tính hoặc kết nối internet trong một khoảng thời gian nhất định - thường là một giây. Đồng nghĩa với **capacity**, băng thông mô tả tốc độ truyền dữ liệu. Băng thông không phải là thước đo tốc độ mạng - một quan niệm sai lầm phổ biến

Trong khi băng thông truyền thống được biểu diễn bằng bit trên giây(bps), các liên kết mạng hiện đại có dung lượng lớn hơn, thường được đo bằng hằng triệu bit trên giây(megabits trên giây hoặc Mbps) hoặc hằng tỷ bit trên giây(gigabit trên giây hoặc Gbps).

Throughput nhất thiết phải thấp hơn băng thông vì băng thông thể hiện khả năng tối đa của mạng của bạn hơn là tốc độ truyền thực tế.

## Throughput vs network letancy
### Network letancy 
- độ trễ của mạng là một biểu hiện về thời gian để một gói dữ liệu đi từ điểm này tới điểm khác. Trong một số môi trường, độ trễ được đo bằng cách gửi một gói tin được trả lại cho người gửi; thời gian khứ hồi được coi là độ trễ, càng gần bằng 0 càng tốt.

### Các yếu tố làm Network throughput - thông lượng mạng bị suy giảm bao gỗm:
* Sự cố phần cứng: nếu routers và các thiết bị khác đã cũ hoặc gặp lỗi.
* Traffic: nếu lưu lượng mạng lớn, nó có thể dẫn đến mất gói. 

### Các yếu tố góp phần vào network letancy - độ trễ của mạng
* Propagation - truyền: Đây chỉ đơn giản là thời gian để một gói tin di chuyển giữa nơi này và nơi khác với tốc độ ánh sáng
* Transmission - Quá trình truyền: Bản thân phương tiện (Cho dù là cáp quang, không dây hay phương tiện khác) tạo ra một số độ trễ, thay đổi từ phương tiện này sang phương tiện khác. Kích thước của gói dẫn đến sự chậm trễ trong một chuyến đi khứ hồi vì gói lớn hơn sẽ mất nhiều thời gian hơn để nhận và trả so với gói ngắn. Ngoài ra, khi tín hiệu phải được tăng cường bởi repeater, điều này cũng tạo ra độ trễ bổ sung.
* Router và các bộ sử lý khác: Mỗi gateway cần có thời gian để kiểm tra và có thể thay đổi tiêu đề trong một gói
* Sự chậm trễ của máy tính và storage: Trong các mạng ở mỗi điểm cuối của hành trình, một gói tin có thể phải chịu sự chậm trễ về lưu trữ và truy cập hard disk ở các thiết bị trung gian như switch và bridges. 

### Đo lường và giám sát network throughput
Có nhiều công cụ chủ động và thụ động khác nhau để đo lưu lượng mạng. Chúng bao gồm Simple Network Management Protocol (SNMP), Windows Management Instrumentation (WMI),Tcpdump, và những thứ khác.

SNMP là một giao thức lớp ứng dụng, được sử dụng để quản lý và giám sát các thiết bị mạng cũng như chức năng của chúng. SNMP cung cấp một ngôn ngữ chung cho các thiết bị mạng để chuyển tiếp thông tin quản lý trong môi trường trong mạng LAN hoặc WAN 

WMI là một tập hợp các thông số kỹ thuật của Mcrosoft để hợp nhất việc quản lý các thiết bị và ứng dụng trong mạng từ các hệ thống máy tính windows. WMI cung cấp cho người dùng thông tin về trạng thái máy tính cục bộ từ xa. Nó cũng hỗ trợ các hành động như cáu hình bảo mật, thiết lập thay đổi thuộc tính hệ thống, thiết lập và thay đổi quyền cho người dùng và nhóm người dùng được ủy quyền, gán thay đổi nhãn ổ đĩa

TCPdump là một công cụ dòng lệnh mã nguồn mở để giám sát lưu lượng mạng. Tcpdump hoạt động bằng cách chụp và hiển thị các tiêu đề gói(packet hesder) và đối sánh với một bộ tiêu chí. Nó hiểu các toán tử tìm kiếm boolean và có thể sử dụng tên máy chủ, địa chỉ IP, tên network và giao thức làm đối số.