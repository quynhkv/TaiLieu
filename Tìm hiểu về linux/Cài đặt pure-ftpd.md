# Cài đặt và cấu hình pure-ftpd trên máy ảo
### 1. Cài đặt pure-ftpd
- **Bước 1**
- Ta cài pure-ftpd từ epel với lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/6457156679370377515/ec07bb2f660dac53f51c.jpg)
> ![q](https://f5-zpcloud.zdn.vn/8727750898602879367/4ce1d0c80deac7b49efb.jpg)
- **Bước 2**
- Sau khi cài đặt ta sử dụng lệnh sau để khởi động dịch vụ pure-ftpd:
> ![q](https://f5-zpcloud.zdn.vn/3533357901366229790/ac563f78e25a2804714b.jpg)
- Kiểm tra trạng thái của dịch vụ:
> ![q](https://f5-zpcloud.zdn.vn/3636408464658698235/e88545aa988852d60b99.jpg)
- **Bước 3**
- Cho phép pure-ftpd đi qua firewall của CentOS 7:
> ![q](https://f5-zpcloud.zdn.vn/3304630208255450279/4c6ae79f3abdf0e3a9ac.jpg)
### 2. Cấu hình pure-ftpd
- **Bước 1**
- Ta cần chỉnh sửa một vài thông số trong file config của pure-ftpd với lệnh:
> ![q](https://f4-zpcloud.zdn.vn/5482926265919690191/470815cdc8ef02b15bfe.jpg)
- **Bước 2**
- Chỉnh sửa các thông số sau:
+ Cho phép các user ftp sử dụng toàn quyền trong thư mục gốc mà user đó được phân quyền, hạn chế không cho những tài khoản này hoạt động bên ngoài thư mục gốc được phân quyền:
> ![q](https://f4-zpcloud.zdn.vn/2706928136590067474/cdff6767ba45701b2954.jpg)
+ Chỉ cho phép truy cập bằng user đã được cấp quyền:
> ![q](https://f5-zpcloud.zdn.vn/3858558430956265869/055789d654f49eaac7e5.jpg)
+ Chỉ định đường dẫn nơi chứa file dữ liệu của các tài khoản ftp:
> ![q](https://f5-zpcloud.zdn.vn/1035274446838900372/d9f4217cfc5e36006f4f.jpg)
- **Bước 3**
- Sau khi chỉnh sửa ta khởi động lại dịch vụ:
> ![q](https://f4-zpcloud.zdn.vn/7582731231261124802/606cd2e20fc0c59e9cd1.jpg)
- Kiểm tra trạng thái của dịch vụ:
> ![q](https://f5-zpcloud.zdn.vn/1767108058614785644/d36a62e5bfc775992cd6.jpg)
### 3. Quản lý user
- **3.1** Tạo user
- Thực hiện tạo user ftp với lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/6377750526961522405/8feab3666e44a41afd55.jpg)
+ Ở đây ta nhập password muốn đặt:
> ![q](https://f5-zpcloud.zdn.vn/7125383491136920984/10e0216dfc4f36116f5e.jpg)
> **Các thông số :**
+ **-u testftp**: Đây là user được tạo trên hệ thống linux.
+ **-g testftp**: Là group của user trên.
+ **quynhkv**: Đây là user ftp được tạo thuộc sở hữu của user quynhkvftp.
+ **-d**: Là tham số cho đường dẫn tới thư mục home dành cho user quynhkv.
- Muốn xóa user thì ta dùng lệnh sau:
> ![q](https://f4-zpcloud.zdn.vn/308451436086393700/9c38194ac7680d365479.jpg)

> Thay tên user muốn xóa vào **“username”**
- **3.2** Kiểm tra
- Kiểm tra thông số user FTP vừa tạo bằng lệnh:
> ![q](https://f5-zpcloud.zdn.vn/2707089362650540567/3069ab1b7539bf67e628.jpg)