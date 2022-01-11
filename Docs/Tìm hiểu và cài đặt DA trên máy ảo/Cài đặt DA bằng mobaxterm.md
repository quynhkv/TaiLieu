# Cài đặt DA bằng mobaxterm
### Bước 1.
- Update các bản vá mới nhất cho hệ thống.
```
yum update -y
```
### Bước 2.
- Tải bản cài đặt từ Direct Admin.
```
wget http://www.directadmin.com/setup.sh
```
> ![q](https://f5-zpcloud.zdn.vn/3613223220959783749/85938a38226eef30b67f.jpg)
### Bước 3.
- Phân quyền cho file cài đặt.
```
chmod 755 setup.sh
```
### Bước 4.
- Chạy file setup.sh để bắt đầu cài đặt.
```
./setup.sh
```
- Tiến trình cài đặt bắt đầu, bạn vui lòng chờ 30 phút để hệ thống tự động cài đặt, cho đến khi nhận đươc thông báo như bên dưới là thành công, bạn lưu lại các thông tin quan trọng:
> ![q](https://f5-zpcloud.zdn.vn/3356728277337764351/b5a0a70b0f5dc2039b4c.jpg)
### Bước 5.
- Mở các port trên Firewall để chạy các dịch vụ HTTPD; FTP; Mail ...v...v
```
firewall-cmd --permanent --add-port=2222/tcp
firewall-cmd --permanent --add-port=21/tcp
firewall-cmd --permanent --add-port=25/tcp
firewall-cmd --permanent --add-port=80/tcp
```
- Khi add xong các port thì reload lại firewall:
```
firewall-cmd –reload
```
### Bước 6.
- Tiến hành đăng nhập thử.
> ![q](https://f4-zpcloud.zdn.vn/4721178333079645197/cae90a41a2176f493606.jpg)
- Vậy là đã thành công.
