# Tutorial FIO
## Install 
By centos:
```
yum install -y fio
```

By Ubuntu:
```
apt-get install -y fio
```

## FIO làm việc như thế nào?
* Để mô phỏng khối lượng công việc I/O
* Viết một tệp công việc mô tả thiết lập cụ thể đó. Tệp công việc có thể chứa bất kỳ số lượng chuỗi và/hoặc tệp nào - nội dung điển hình của tệp công việc là phần chung xác định các thông số được chia sẻ và một hoặc nhiều phần công việc mô tả các công việc liên quan. 
* Chạy tệp fio, fio phân tích cú pháp tệp này và thiết lập mọi thứ như được mô tả. Nếu chúng ta chia nhỏ một công việc từ trên xuống dưới, nó chứa các thông số cơ bản sau:
    * I/O type: Xác định kiểu I/O được cấp cho (các) tệp.
    * Block size: một giá trị đơn lẻ hoặc nó có thể mô tả một loạt các kích thước khối.
    * I/O size: Chúng ta sẽ đọc/ghi bao nhiêu dữ liệu.
    * I/O engine: Làm thế nào để chúng tôi phát hành I/O? Chúng tôi có thể ánh xạ bộ nhớ tệp, chúng tôi có thể sử dụng đọc/ghi thông thường, chúng tôi có thể sử dụng mối nối, I/O không đồng bộ, hoặc thậm chí SG (SCSI generic sg).
    * I/O depth: Nếu I / O engine không đồng bộ, chúng ta muốn duy trì độ sâu xếp hàng lớn đến mức nào?
    * Target file/device: Có bao nhiêu tệp mà chúng tôi đang dàn trải khối lượng công việc.
    * Threads, processes and job synchronization: trải rộng khối lượng công việc này lên bao nhiêu luồng hoặc quy trình.





https://fio.readthedocs.io/en/latest/fio_doc.html#job-file-parameters

https://github.com/congto/FIO-TEST

https://github.com/benschweizer/iops
https://github.com/lacoski/ceph-note/blob/0d9ebffb2a/docs/terms/fio.md

https://www.digitalocean.com/community/tutorials/how-to-benchmark-digitalocean-volumes