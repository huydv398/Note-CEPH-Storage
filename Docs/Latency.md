# Latency 
Latency là một từ đồng nghĩa với delay. Trong telecommunications - Viễn thông, đỗ trễ thấp có liên quan đến trải nghiệm người dùng (user experience - UX) tích cực trong khi độ trễ cao liên quan đến trải nghiệm người dùng kém

Trong computer networking, latency là biểu hiện của khoảng thời gian để một gói dữ liệu di chuyển từ điểm chỉ định đến điểm khác. Lý tưởng nhất là độ trễ bằng 0 thì càng tốt. Độ trễ của mạng có thể được đo bằng các xác định round-trip time (RTT) - thời gian khứ hồi để một gói dữ liệu di chuyển đến một điểm đến và quay lại một lần nữa.

Độ trễ mạng cao có thể làm tăng đáng kể thời gian tải web, làm gián đoạn các luồng video và âm thanh, đồng thời khiến ứng dụng không thể sử dụng được. Tùy thuộc vào ứng dụng, ngay cả một sự gia tăng tương đối nhỏ về đọ trễ cũng có thể làm hỏng Trải nghiệm người dùng.

Một trong những lý do chính cho độ trễ kém là do địa lý. Các mạng Giao thức Internet(IP) được phân phối cao đi qua những khoảng cách xa, tăng thêm thời gian truyền dẫn có thể khiến ứng dụng lỗi.

## Nguyên nhân của độ trễ trong viễn thông
Độ trễ có thể do nhiều nguyên nhân, bao gồm:
* **Transmission media** - Phương tiện truyền dẫn: Độ trễ có thể bị ảnh hưởng bởi loại phương tiện sử dụng để truyền dữ liệu, thoại và video. 
* **Packet size** - Kích thước gói: Một gói lớn sẽ mất nhiều thời gian hơn để gửi khứ hồi một gói nhỏ
* **Packet loss and jitter** - Mất gói và chập chờn: độ trễ cũng có thể do tỷ lệ phần trăm cao các gói không đến được đích của chúng hoặc có quá nhiều thay đổi về thời gian để một số gói truyền từ hệ thống này qua hệ thống khác
* **Signal strength** - Cường độ tín hiệu: Nếu tín hiệu yếu và phải được tăng cường bằng repeater
* **Propagation delays** - sự chậm trễ lan truyền: Nếu mỗi nút gateway phải mất thời gian để kiểm tra và có thể thay đổi tiêu đề trong một gói- ví dụ: Thay đổi số hop count - bước nhảy trong trường time-to-live (TTL) - thời gian tồn tại thì độ trễ này sẽ cao hơn.
* **Máy tính và lưu trữ**
## Các loại độ trễ
* **Interrupt latency**- Độ trễ gián đoạn là khoảng thời gian cần thiết để máy tính hoạt động theo một tín hiệu thông báo cho OS dùng cho đến khi nó có thể quyết định làm gì cho một sự kiện
* **Fiber optic latency** - Độ trễ của sợi quang là thời gian ánh sáng truyền đi một khoảng cách xác định qua một sợi cáp quang. Đối với mỗi KM, độ trễ 3,33 micro giây (μs) tự nhiên xảy ra, theo tốc độ ánh sáng. Tuy nhiên, trong thực tế độ trễ mỗi km là 4,9 μs - do ánh sáng truyền chậm hơn trong cáp. Các chỗ uống cong hoặc các điểm không hoàn hảo khác trong cáp có thể làm cho độ trễ cao hơn.
* **Internet latency times** - Thời gian độ trễ mạng internet phụ thuộc vào khoảng cách. Một gói tin di chuyển qua mang càng lâu thì độ trễ càng cao.
* **WAN latency** có thể là một yếu tố quan trọng trong việc xác định độ trễ internet. 
* **Audio latency** là độ trễ giữa âm thanh được tạo ra và nghe thấy. 
* **Operational latency** - Độ trễ hoạt động có thể được xác định là tổng thời gian của các hoạt động nếu chúng được thực hiện trong quy trình làm việc tuyến tính
* **Mechanical latency** - Độ trễ cơ học là độ trễ đầu vào của hệ thống hoặc thiết bị cơ khí đến đầu ra mong muốn. 
* **Computer and OS latency** là độ trễ giữa đầu vào hoặc lệnh và đầu ra mong muốn. Các yếu tố góp phần làm tăng độ trễ của máy tính bao gồm không đủ data bufers - bộ đệm dữ liệu và tốc độ dữ liệu giữa bộ vi xử lý và thiết bị đầu vào/đầu ra không khớp.
## Kiểm tra và đo lường latency
Kiểm tra độ trễ có thể khác nhay giữa các ứng dụng. Trong một số ứng dụng, việc đo độ trễ yêu cầu thiết bị đặc biệt và phức tạp hoặc kiến thức về các lệnh và chương trình máy tính đặc biệt; trong các trường hợp khác, độ trễ có thể được đo bằng đồng hồ bấm giờ . Các nhà quản lý mạng có một số công cụ để thực hiện việc này, bao gồm traceroute, t traceroute(MTR) và ping.

Các lệnh Ping được sử dụng để xác định xem máy tính mà người dùng đang cố truy vấn có đang hoạt động không. Để đánh giá độ trễ, admin gửi yêu cầu gửi lại giao thức thông báo điều khiển Internet(Internet Control Message Protocol - ICMP) tới một địa chỉ mạng và chờ phản hồi

Thông tin độ trễ cũng có thể thu thập bằng cách sử dụng lệnh traceroute. Lệnh trực quan hóa đường dẫn mà các gói đi qua mạng IP, ghi lại độ trễ giữa  các thiết bị trên đường dẫn và tổng thời gian vận chuyển.

Để đánh giá độ trễ cơ học, máy ảnh tốc độ cao có thể được sử dụng để ghi lại sự khác biệt từng phút trong thời gian phản hồi từ đầu vào đến tác vụ cơ học
## Giảm độ trễ
Latency có thể được giảm bớt bằng cách điều chỉnh, tinh chỉnh và nâng cấp phần cứng, phần mềm và hệ thống cơ học của máy tính. Trong máy tính, độ trễ có thể được loại bỏ hoặc ẩn bằng kỹ thuật nạp trước - dự đoán nhu cầu về các yêu cầu đầu vào dữ liệu và đa luồng hoặc bằng cách sử dụng song song trên nhiều luồng thực thi.

Để giảm độ trễ và tăng hiệu suất bao gồm gỡ cài đặt các chương trình không cần thiết, tối ưu hóa cấu hình mạng và phần mềm cũng như nâng cấp hoặc ép xung phần cứng.
## Latency vs throughput
Latency và throughput thường được sử dụng để đo hiệu suất mạng và cải thiện thời gian tải.

Latency có thể được gọi là thời gian cần thiết để thực hiện hành động, trong khi thông lượng có thể được coi là số lượng hành động có thể được thực hiện trong một đơn vị thời gian. Nói cách khác, độ trễ đo lường tốc độ truyền dữ liệu, trong khi throughput là lượng dữ liệu có thể gửi đi.

Bandwidth là một khái niệm khác thường được kết hợp với latency. Băng thông mô tả  dung lượng tối đa của kết nối mạng/kết nối internet. Mạng càng ít băng thông thì độ trễ càng nhiều.

Để hiểu mối quan hệ của băng thông với độ trễ, hãy hình dung băng thông dưới dạng đường ống và thông lượng như lượng nước mà đường ống có thể vận chuyển trong một thời gian cụ thể. Độ trễ trở thành thời gian cần thiết để nước về đến đích. Đường ống càng nhỏ thì mất nhiều thời gian để nước về đến đích. Băng thông và độ trễ có mối quan hệ nguyên nhân và kết quả theo cách này.