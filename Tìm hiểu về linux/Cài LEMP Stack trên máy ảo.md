# Cài LEMP Stack trên máy ảo CentOS 7
### 1. Cài đặt Nginx Web Server
- **Bước 1**
  + Vì NGINX không có sẵn repository của CentOS vì vậy chúng ta phải cài repository EPEL​ với câu lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/6925063237124805802/58dfc3bcc1a90bf752b8.jpg)
- **Bước 2**
  + Cài đặt Nginx với lệnh sau:
> ![q](https://f4-zpcloud.zdn.vn/7086798801051696369/caa783c981dc4b8212cd.jpg)
- **Bước 3**
  - Sau khi cài đặt hoàn tất, các bạn có thể sử dụng các lệnh sau để quản lý Nginx:
> ![q](https://f4-zpcloud.zdn.vn/7777833804115080965/b2a99bde99cb53950ada.jpg)
- **Bước 4**
  - Mặc định trên Centos 7 sẽ sử dụng tường lửa là Firewalld, nên các bạn cần thực hiện mở Port dịch vụ với Firewalld theo các cách sau:
> ![q](https://f4-zpcloud.zdn.vn/6621412947217809234/7fb982c980dc4a8213cd.jpg)
### 2. Cài đặt MariaDB
- **Bước 1**
  - Để cài đặt MariaDB các bạn chạy lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/7062171643618811251/d6b992c490d15a8f03c0.jpg)
  - Sau khi cài đặt hoàn tất, các bạn có thể sử dụng các lệnh sau để quản lý MariaDB:
> ![q](https://f4-zpcloud.zdn.vn/5056829290209438505/dd1d946196745c2a0565.jpg)
- **Bước 2**
  - Thiết lập bảo mật MariaDB Server:
> ![q](https://f5-zpcloud.zdn.vn/5787828424287119963/2d38b247b0527a0c2343.jpg)
### 3. Cài đặt PHP-FPM và các Module
- **Bước 1**
  - Để cài đặt kho Remi các bạn chạy lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/1812633192686679754/61a1aedaaccf66913fde.jpg)
- **Bước 2**
  - Sau khi cài đặt gói Remi xong, các bạn cần chọn phiên bản PHP mà mình cần cài đặt và kích hoạt gói chứa phiên bản PHP đó. Ở hướng dẫn này mình sẽ cài đặt PHP 8.0 nên sẽ kích hoạt gói bằng lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/843867848909743116/7c65e5c5ced0048e5dc1.jpg)
- **Bước 3**
  - Khi module remi-80 của PHP đã được bật, bạn có thể tiến hành cài đặt PHP và các PHP Extension cần thiết bằng lệnh bên dưới:
> ![q](https://f5-zpcloud.zdn.vn/4557670494626381487/4017431741028b5cd213.jpg)
- **Bước 4**
  - Kiểm tra phiên bản PHP vừa cài đặt bằng lệnh:
> ![q](https://f4-zpcloud.zdn.vn/750536942741704089/61db58d95acc9092c9dd.jpg)
> Hiển thị như trên là đã thành công.
- **Bước 5**
  - Mặc định PHP sẽ thực thi file PHP gần nhất nếu không tìm thấy file php được request. Để ngăn chặn việc thực thi PHP không mong muốn các bạn thay đổi cấu hình như sau:
  - **sudo nano /etc/php.ini**
  - Các bạn tìm và thay thế các dòng sau:
> ![q](https://f5-zpcloud.zdn.vn/7897459242625096707/3206360b341efe40a70f.jpg)
- **Bước 6**
  - Mở và chỉnh sửa file cấu hình **/etc/php-fpm.d/www.conf** bằng lệnh sau:
  - **sudo nano /etc/php-fpm.d/www.conf**
  - Các bạn tìm và thay thế các dòng sau:
> ![q](https://f5-zpcloud.zdn.vn/6755846294550853713/56d546d944cc8e92d7dd.jpg)
- **Bước 7**
  - Bảo mật php_fpm.sock với câu lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/8452775495522364073/ffc621c923dce982b0cd.jpg)
- **Bước 8**
  - Khởi động PHP-FPM sau khi đã hoàn tất chỉnh sửa cấu hình bằng lệnh:
> ![q](https://f5-zpcloud.zdn.vn/1234967697169720254/8f87cd89cf9c05c25c8d.jpg)
### 4. Cấu hình VHost(Nginx)
- **Bước 1**
  - Virtual Host là file cấu hình cho phép nhiều domain cùng chạy trên một máy chủ. Tất cả các file vhost sẽ nằm trong thư mục **/etc/nginx/conf.d/**. Để tiện quản lý mỗi website nên có một vhost riêng, ví dụ: **quynhkv.com.conf**
  - Trong ví dụ này sẽ tạo website **quynhkv.com** với vhost tương ứng là **/etc/nginx/conf.d/quynhkv.com.conf** với nội dung sau:
> ![q](https://f5-zpcloud.zdn.vn/1909443430835972058/d6878754c841021f5b50.jpg)
> ![q](https://f5-zpcloud.zdn.vn/7304688539253888883/a357b584fa9130cf6980.jpg)
- **Bước 2**
  - Tiếp theo các bạn cần tạo thư mục chứa mã nguồn website và thư mục chứa file log bằng các lệnh sau:
> ![q](https://f5-zpcloud.zdn.vn/4592219336466905227/7ecfa31dec0826567f19.jpg)
- **Bước 3**
  - Khởi động lại Nginx để load cấu hình:
> ![q](https://f5-zpcloud.zdn.vn/7512144705153774447/176c59b116a4dcfa85b5.jpg)
- **Bước 4**
  - Sau khi cấu hình hoàn tất các bạn trỏ tên miền về vps sau đó tạo **file /home/quynhkv.com/public_html/index.php** với nội dung sau và gõ tên miền của bạn vào thanh địa chỉ của trình duyệt để kiểm tra:
> ![q](https://f5-zpcloud.zdn.vn/316320780515424286/c81c793a4a1a8044d90b.jpg)
> ![q](https://f4-zpcloud.zdn.vn/4032564261379063770/6df3252e6a3ba065f92a.jpg)

> Hiển thị như trên là đã thành công.
