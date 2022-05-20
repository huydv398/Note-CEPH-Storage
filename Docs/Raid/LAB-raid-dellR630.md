
# Cấu hình các mode RAID cho server Dell r630.
## Cấu hình RAID 0
### Cấu hình RAID O (2 DISK)
![Imgur](https://i.imgur.com/5Qvcsiz.png)

Khởi động Server, khi Server chạy đến dòng **PowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

![Imgur](https://i.imgur.com/uMraGPc.png)

Xóa cấu hình cũ Chọn:
* Nhấn **F2**  chọn **Clear Config** 


### Cấu hình RAID O (3 DISK)
![Imgur](https://i.imgur.com/l9y6G3d.png)

Khởi động Server, khi Server chạy đến dòng **PowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

Xóa cấu hình cũ Chọn:
* Nhấn **F2**  chọn **Clear Config** 

![Imgur](https://i.imgur.com/uMraGPc.png)

Nhấn **F2** => chọn **Create New VD**

![Imgur](https://i.imgur.com/EyCGRXt.png)

Config Virtual Disk
* 1: Chọn Chế độ Card RAID
* 2: Chọn Disk muốn RAID (chọn 3 DISK)
* 3: Tên của Virtual Disk
* 4: Chọn OK để hoàn thành

![Imgur](https://i.imgur.com/iiwyMSa.png)

Chọn OK để lưu cấu hình

![Imgur](https://i.imgur.com/FQbEt6O.png)

Nhấn **ESC** để lưu và reboot máy

![Imgur](https://i.imgur.com/FbqReCT.png)

### Cấu hình RAID 1 (3 DISK )
![Imgur](https://i.imgur.com/pGDa9S0.png)

Khởi động Server, khi Server chạy đến dòng **PowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

Xóa cấu hình cũ Chọn:
* Nhấn **F2**  chọn **Clear Config** 

![Imgur](https://i.imgur.com/uMraGPc.png)

Nhấn **F2** => chọn **Create New VD**

![Imgur](https://i.imgur.com/EyCGRXt.png)

Config Virtual Disk
* 1: Chọn Chế độ Card RAID
* 2: Chọn Disk muốn RAID (chọn 2 DISK)
* 3: Tên của Virtual Disk
* 4: Chọn OK để hoàn thành

![Imgur](https://i.imgur.com/kS86aXa.png) 

Không thể chọn 3 ổ vì nguyên lý hoạt động của RAID 1 là cần 2 ổ hoặc 4 ổ. Số ổ cứng phải là số chẵn.

### Cấu hình RAID 0 (4 DISK)

![Imgur](https://i.imgur.com/5HaJcec.png)

Khởi động Server, khi Server chạy đến dòng **PowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

Xóa cấu hình cũ Chọn:
* Nhấn **F2**  chọn **Clear Config** 

!Khởi động Server, khi Server chạy đến dòng **PowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

Xóa cấu hình cũ Chọn:
* Nhấn **F2**  chọn **Clear Config** 

![Imgur](https://i.imgur.com/uMraGPc.png)

Nhấn **F2** => chọn **Create New VD**

![Imgur](https://i.imgur.com/zk2mOjC.png)

Cấu hình Virtual Disk 
* 1: Chọn chế độ RAID (RAID-0)
* 2: Tích vào Disk cần RAID
* 3 Đặt tên cho VD
* 4: Nhấn OK để hoàn thành

![Imgur](https://i.imgur.com/PsoKMnI.png)

Nhấn ESC và chọn OK để lưu lại

![Imgur](https://i.imgur.com/il1FQ3Y.png)

Reboot hệ thống

## Cấu hình RAID 1
### Cấu hình RAID 1 (2 DISK)

![Imgur](https://i.imgur.com/m9Xlg3F.png)

Khởi động Server, khi Server chạy đến dòng **PoowerEdge Expandable RAID Controller BIOS**

Nhấn **Ctrl** + **R**

Để vào **Bios Configuration**

Chọn main và Nhấn **F2** Chọn **Clear Config** 
### Cấu hình RAID 1 (4 DISK)

## Cấu hình RAID 0 + 1
![Imgur](https://i.imgur.com/RNZCj0Z.png)

## Cấu hình RAID 5
![Imgur](https://i.imgur.com/S5QLl46.png)

### Cấu hình RAID 5 Add 1 Disk

### Cấu hình RAID 5 (added 1 Disk) -1 Disk
Khi RAID 5 đã Add 1 disk mà do không sử dụng hết tài nguyên muốn thu hồi lại 1 Disk 

## Cấu hình RAID 6 
![Imgur](https://i.imgur.com/zkGksag.png)
