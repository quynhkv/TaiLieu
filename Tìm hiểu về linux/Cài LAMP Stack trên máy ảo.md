# Cài đặt LAMP Stack trên máy ảo CentOS 7
### 1. Cài đặt Apache Web Server
> Máy chủ web Apache là một trong những máy chủ web phổ biến nhất trên thế giới. Nó đã được ghi chép đầy đủ và được sử dụng rộng rãi trong một thời gian dài, điều này khiến cho Apache trở thành một lựa chọn mặc định tuyệt vời để lưu trữ một website.
- **Bước 1.**
    +	Khởi động máy ảo CentOS.
    +	Ở màn hình giao diện chính kích chuột phải chọn Open Terminal.
![e](https://f4-zpcloud.zdn.vn/2267294275458379350/32e8c651bf32756c2c23.jpg)
- **Bước 2.**
    + Bây giờ để cài Apache Web Server ta cần thêm quyền sudo cho user, ở giao diện Terminal gõ lệnh sau để login vào user root:
![q](https://f5-zpcloud.zdn.vn/6102214719221088462/fca7a620384af214ab5b.jpg)
- **Bước 3.**
    + Sau khi login vào user root ta mở file /etc/sudoers bằng lệnh:
    ![q](https://f5-zpcloud.zdn.vn/9104067148528139137/7fa57721e94b23157a5a.jpg)
- **Bước 4.**
    + Chỏ xuống và bạn sẽ tìm thấy dòng có nội dung như sau:
    ![q](https://f5-zpcloud.zdn.vn/6047691853607194630/c2dcb624284ee210bb5f.jpg)
- **Bước 5.**
    + Gõ thêm vào tên group mà bạn muốn. Ở đây, vì đã tạo user quynhkv nên máy cũng đã tự tạo group quynhkv, nên ta sẽ dùng sử dụng group quynhkv luôn.
    ![q](https://f5-zpcloud.zdn.vn/7938207791596051715/a9a67e54e03e2a60732f.jpg)
    + Sau đó dùng tổ hợp phím Ctrl + S
    ![q](https://f5-zpcloud.zdn.vn/4105645777178984643/166105979bfd51a308ec.jpg)
    + Tiếp theo gõ Ctrl + X để lưu file lại
- **Bước 6.**
    + Sau khi lưu file gõ exit để thoát ra
    ![q](https://f5-zpcloud.zdn.vn/3739122400658896925/df7ecc8b52e198bfc1f0.jpg)
- **Bước 7.**
    + Giờ ta gõ lệnh sau rồi nhập pass user để tiến hành cài Apache Web Server
    ![q](https://f5-zpcloud.zdn.vn/1854139507075499642/ab14b7ff2995e3cbba84.jpg)
- **Bước 8.**
    + Sau khi cài đặt hoàn tất, các bạn có thể sử dụng các lệnh sau để quản lý Apache
    ![q](https://f5-zpcloud.zdn.vn/4307911791870693317/1eb1ea587432be6ce723.jpg)
    + Giờ ta khởi động và xem trạng thái của dịch vụ Apache
    ![q](https://f4-zpcloud.zdn.vn/8616156899430155565/db9fbe70201aea44b30b.jpg)
- **Bước 9.**
    + Mặc định trên Centos 7 sẽ sử dụng tường lửa là Firewall, nên ta cần thực hiện mở Port dịch vụ Apache với Firewall theo 2 lệnh sau:
    ![q](https://f5-zpcloud.zdn.vn/175595081751757660/400c28ecb6867cd82597.jpg)
### 2. Cài đặt MariaDB
- **Bước 1.**
    + Để cài đặt MariaDB ta chạy lệnh sau:
    ![q](https://f5-zpcloud.zdn.vn/3467746179891902444/e6281cf0829a48c4118b.jpg)
- **Bước 2.**
    + Sau khi cài đặt hoàn tất, các bạn có thể sử dụng các lệnh sau để quản lý MariaDB:
    ![q](https://f4-zpcloud.zdn.vn/4802316549595847676/6ec2971f0975c32b9a64.jpg)
    + Giờ ta lại khởi động và xem trạng thái của dịch vụ mariadb
    ![q](https://f5-zpcloud.zdn.vn/4171382287581246057/12b85e69c0030a5d5312.jpg)
> Lưu ý: File cấu hình chính của MariaDB là file /etc/my.conf
- **Bước 3.**
    + Thiết lập bảo mật MariaDB Server
    + Như vậy ta đã cài đặt thành công MariaDB Server . MariaDB Server  bao gồm một tập lệnh bảo mật để thay đổi một số tùy chọn mặc định kém an toàn như Remote Connect và user test. Các bạn sử dụng lệnh sau để chạy tập lệnh bảo mật:
    ![q](https://f5-zpcloud.zdn.vn/5709137418231323744/f27f00b09eda54840dcb.jpg)
    ![q](https://f5-zpcloud.zdn.vn/6921717041116730556/530e07c299a853f60ab9.jpg)
### 3. Cài đặt PHP
> Phiên bản PHP có sẵn CentOS 7 là các bản cũ và đã lỗi thời và vì lý do đó, các bạn nên cài đặt kho lưu trữ gói của bên thứ ba để có thể sử dụng các phiên bản PHP mới nhất . Và Remi là kho lưu trữ gói phổ biến cung cấp các bản phát hành PHP mới nhất cho các máy chủ CentOS.
- **Bước 1.**
    + Để cài đặt kho Remi ta chạy lệnh sau:
    ![q](https://f5-zpcloud.zdn.vn/6479925469342808779/0c5bc3995df397adcee2.jpg)
- **Bước 2.**
    + Sau khi cài đặt gói Remi xong, ta cần chọn phiên bản PHP mà mình cần cài đặt và kích hoạt gói chứa phiên bản PHP đó. Ở đây ta sẽ cài đặt PHP 8.0 nên sẽ kích hoạt gói bằng lệnh sau:
    ![q](https://f5-zpcloud.zdn.vn/270335491224982942/04889a4c0426ce789737.jpg)
> Lưu ý: Ở số 80 (tương ứng PHP 8.0), bạn có thể thay thế bằng phiên bản PHP bạn muốn (Ví dụ: 72 – 73 –74 tương ứng 7.2 –7.3 – 7.4..)
- **Bước 3.**
    + Khi module remi-80 của PHP đã được bật, ta có thể tiến hành cài đặt PHP và các PHP Extension cần thiết bằng lệnh bên dưới:
    ![q](https://f5-zpcloud.zdn.vn/4293954668191014619/a9e50bd894b25eec07a3.jpg)

- **Bước 4.**
    + Kiểm tra phiên bản PHP vừa cài đặt bằng lệnh:
    ![q](https://f4-zpcloud.zdn.vn/8828577552192254613/08e8b4d92bb3e1edb8a2.jpg)
    + Hiển thị như trên thì đã cài đặt thành công PHP 8.0 rồi nhé.
### 4. Cấu hình Virtual Host(Apache)
- **Bước 1.**
    + Tạo Folder chứa code cho website web1 bằng lệnh:
    ![q](https://f5-zpcloud.zdn.vn/3867290298147261209/9c97b6a329c9e397bad8.jpg)
- **Bước 2.**
    + Chỉnh sửa quyền truy cập sao cho quyền đọc được chấp nhận với tất cả các file và thư mục bên trong /var/www bằng lệnh:
    ![q](https://f5-zpcloud.zdn.vn/5777653898534874047/4677def3438689d8d097.jpg)
- **Bước 3.**
    + Tạo ra file index.html đơn giản cho website để kiểm tra thử hoạt động của Virtual host bằng lệnh:
    ![q](https://f4-zpcloud.zdn.vn/6692698396740004802/2088bca723cde993b0dc.jpg)
- **Bước 4**
    + Tạo 2 thư mục lưu trữ File cấu hình Virtual host cho apache bằng lệnh:
    ![q](https://f5-zpcloud.zdn.vn/7926345836455271465/e7cbe0376d42a71cfe53.jpg)
- **Bước 5.**
    + Gõ lệnh sau để Apache nhận cấu hình những virtual host trong sites-enabled
    ![q](https://f5-zpcloud.zdn.vn/8327466010273906174/39528c70131ad944800b.jpg)
    + Thêm dòng sau vào cuối file sau đó lưu lại và thoát: IncludeOptional sites-enabled/*.conf
- **Bước 6.**
    + Tạo File Virtual host cho web1.com bằng lệnh:
    ![q](https://f5-zpcloud.zdn.vn/2603924293052470676/167cb75c2836e268bb27.jpg)
    + Thêm nội dung sau vào file sau đó lưu và thoát:
        + < VirtualHost *:80 >
            + ServerAdmin admin@web1.com
            + ServerName web1.com
            + ServerAlias www.web1.com
            + DocumentRoot /var/www/web1
            + DirectoryIndex index.php index.html
            + ErrorLog /var/www/web1/error.log
            + CustomLog /var/www/web1/requests.log combined 
        + < /VirtualHost >
    + **Trong đó:**
        + ServerAdmin: khai báo email của quản trị viên.
        + ServerName khai báo domain mà website sẽ lắng nghe.
        + ServerAlias  (tuỳ chọn) khai báo Alias của domain, thương là www.
        + DirectoryIndex loại file sẽ được tìm đến để khởi chạy.
        + DocumentRoot khai báo đường dẫn chứa code của website.
        + ErrorLog và CustomLog khai báo đường dẫn lưu file log của website.
- **Bước 7.**
    + Như đã để cập ở trên, Apache sẽ chỉ nhận những cấu hình Virtual host trong thư mục sites-enabled. vì vậy ta sẽ tạo một liên kết ( symbolic link) vào thư mục sites-enabled của mỗi virtual host:
    ![q](https://f5-zpcloud.zdn.vn/5628032350672214511/222a13a0a4d56e8b37c4.jpg)
- **Bước 8.**
    + Restart Apache để lưu thay đổi:
    ![q](https://f5-zpcloud.zdn.vn/5672954032991802399/7351ef765f03955dcc12.jpg)
    + Như vậy ta đã cấu hình xong Virtual host cho website.
- **Bước 9.**
    +   Kiểm tra hoạt động:
        + Trên trình duyệt web của User, bạn vào web1.com để kiểm tra, nếu ra nội dung như ta setup ban đầu thì đã thành công.
        + Truy cập web1.com:
        ![q](https://f5-zpcloud.zdn.vn/1090504420018895590/a60b5d385f4c9512cc5d.jpg)
> Trong khuôn khổ bài lab này bạn sẽ cần phải trỏ ip trong file hosts của windows để có thể phân dải tên miền web1.com về ip của Web server.
- Để trỏ về ip trong file hosts về ip của Web server ta làm như sau:
    + Kiểm tra địa chỉ IP của bạn:117.4.255.125 là ip của bạn,
    ![q](https://f5-zpcloud.zdn.vn/3115018012628678427/ac68c355c1210b7f5230.jpg)
    + Tiếp theo ta gõ lệnh sau:
    + ![q](https://f5-zpcloud.zdn.vn/445404288923061463/7fd8c4e5c6910ccf5580.jpg)
    + Ở đây ta thêm ip và tên miền vào rồi save file
    ![q](https://f4-zpcloud.zdn.vn/5256698511515839821/ffb6428b40ff8aa1d3ee.jpg)
- Vậy là đã xong.