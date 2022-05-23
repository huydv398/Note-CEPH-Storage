# Note-STORAGE
Ghi chép tìm hiểu STORAGE

Các tài liệu được note lại trong quá trình tìm hiểu bộ nhớ. Lộ trình xây dựng các kiến thức phần cứng đến phần mềm bao gồm các thông số cơ bản đến cấu hình cài đặt các phần mềm lưu trữ chuyên dụng trong lĩnh vực storage và cloud computing.
## I. Vấn đề cơ bản	
1. [Các loại thiết bị Lưu trữ cơ bản](/Docs/1.Types-of-storage-devices.md)
1. [Tìm hiểu **Ổ cứng HDD**](/Docs/2.1hard-disk-drive.md)
    * [Nguyên lý hoạt động đọc - ghi vào Ổ cứng HDD](/Docs/2.2-Write-Read-HDD.md)
1. [Tìm hiểu **Ổ cứng SSD**](/Docs/3.SSD.md)
    * [Nguyên lý hoạt động đọc ghi vào  Ổ cứng SSD](/Docs/3.2-ssd-work.md)
1. [Thông số cần chú ý trong Datasheet của từng loại](/Docs/4.data-sheet-drive.md)
1. [Block size & Hiệu suất Disk liên tục](/Docs/5.performance&block.md)
1. [Thông số hiệu suất Disk: IOPS, Throughput, Legacy](/IOPS/README.md)
1. [Drive interface FC, SAS, SATA, NVME(PCIe)](/Docs/6.drive-interfaces.md)
## II. ỨNG DỤNG
1. [File system](/Docs/Filesystem/1.file-system.md)
    1. [File system Windows](/Docs/Filesystem/1.1.File-system-Windows.md)
    1. [File system Linux - part 1](/Docs/Filesystem/1.2.File-system-Linux.md)
    1. [File system Linux - part 2](/Docs/Filesystem/1.3.File-system-Linux2.md)
1. [Các loại File system in linux](/Docs/Filesystem/2.types-file-linux.md)
1. [Cấu trúc File system](/Docs/Filesystem/3.Structure-FS.md)
1. [File system in Userspace](/Docs/Filesystem/4.FUSE.md)
1. [File system - Truy cập Filesystem](/Docs/Filesystem/5.access-fs.md)
1. [File system - Kiểm soát quyền truy cập](/Docs/Filesystem/6.permission-access.md)
1. [File system](/Docs/Filesystem/7.fs-struc.md)
1. [RAID](/Docs/Raid/raid.md)
1. [RAID Type](/Docs/Raid/type-raid.md)
1. [RAID thực hành RAID trên Dell R630](/Docs/Raid/LAB-raid-dellR630.md)
1. [Partition Table](/Docs/PartitionTable/Partition-Table.md)
    * [Phân vùng GPT](/Docs/PartitionTable/GPT.md)
    * [Phân vùng MBR](/Docs/PartitionTable/MBR.md)
    * [Chuẩn BIOS](/Docs/PartitionTable/BIOS.md)
    * [Chuẩn UEFI](/Docs/PartitionTable/UEFI.md)
1. [`/etc/fstab`](https://imgur.com/OdT8JwX)
1. [LVM](/Docs/LVM/README.md)
    1. [Thông tin cơ bản về quản lý khối- **LVM** (Logical Volume Manger)](/Docs/LVM/lvm.md)
    1. [LVM - Các loại Logical Volume](/Docs/LVM/2.Type-lv.md)
    1. [LVM - Cấu hình cơ bản. Tạo LVM](/Docs/LVM/3.config-basic.md)
    1. [LVM - Cấu hình cơ bản phần 2](/Docs/LVM/4.config-basic-2.md)
    1. [LVM - Snapshot](/Docs/LVM/5.lvm-snapshot.md)
    1. [LVM - Thin Provisioning Volume](/Docs/LVM/6.Thin-Provisioning-Volume.md)
    1. [LVM](/Docs/LVM/7.Striped-lvm.md)
    1. [LVM](/Docs/LVM/8.Mirrored-LVM.md)
    1. [LVM](/Docs/LVM/9.Cache-LVM.md)
## III. Tìm hiểu các thuật ngữ	
1. [SLA,SLO](/Docs/)
1. [QoS - Quality of service](/Docs/)
1. [Latency](/Docs/)
1. [Throughput](/Docs/)
1. [Jitter](/Docs/)
1. [Capacity](/Docs/)
1. [I/O Size](/Docs/)
## IV. THÔNG SỐ	
1. [Độ quan trọng latency](/Docs/)
1. [Tìm hiểu về các thông số: IOPS, Latency và Throughput](/Docs/)
1. [Mối quan hệ; IOPS latency và bandwidth](/Docs/)
1. [Ý nghĩa các thông số: IOPS, Latency và Throughput](/Docs/)
## V. Bench mark ổ đĩa	
1. [Thực hành lệnh `dd` trong linux](/Docs/)
1. [Ý nghĩa tham số FIO bench mark](/Docs/)       
1. [FIO bench mark](/Docs/)   
## VI. Cloud and Storage
1. [CEPH](/)
1. [SAN](/)
1. [vSAN](/)
1. [OWNCLOUD](/) 
1. [NEXTCLOUD](/)




    1. [ext3,ext4,lvm,đ fio,]()
    1. [s]()
    1. [s]()
    1. [s]()
    1. [s]()
    1. [s]()