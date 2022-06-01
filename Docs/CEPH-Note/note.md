## File storage
### Object storage 
* Lưu trữ đối tượng (còn được gọi là **object-based storage**) là lưu trữ dữ liệu máy tính quản lý dữ liệu dưới dạng **object** . 
* 3 thành phần trong object 
    *  **data itself** - bản thân dữ liệu
    * Một lượng **metadata** thay đổi 
    * Một số nhận dạng duy nhất trên toàn cầu.
* Object Storage được triển khai ở nhiều cấp:
    * Device Level (Object-Storage device)
    * System level 
    * interface level
* Trong mỗi trường hợp, Object Storage tìm cách kích hoạt các khả năng không được giải quyết bởi các kiến ​​trúc lưu trữ khác, chẳng hạn như giao diện được ứng dụng lập trình trực tiếp, không gian tên có thể mở rộng nhiều phiên bản phần cứng vật lý và các chức năng quản lý dữ liệu như sao chép dữ liệu và phân phối dữ liệu tại mức độ chi tiết của object.

* Hệ thống Object Storage cho phép lưu giữ một lượng lớn dữ liệu phi cấu trúc trong đó dữ liệu được ghi một lần và đọc một lần (hoặc nhiều lần).
*  Object Storage được sử dụng cho các mục đích như lưu trữ các đối tượng như video và ảnh trên Facebook, bài hát trên Spotify hoặc tệp trong các dịch vụ cộng tác trực tuyến, chẳng hạn như Dropbox.  Một trong những hạn chế với Object Storage là nó không dành cho dữ liệu giao dịch, vì Object Storage không được thiết kế để thay thế quyền truy cập và chia sẻ tệp NAS; nó không hỗ trợ các cơ chế khóa và chia sẻ cần thiết để duy trì một phiên bản cập nhật chính xác, duy nhất của tệp