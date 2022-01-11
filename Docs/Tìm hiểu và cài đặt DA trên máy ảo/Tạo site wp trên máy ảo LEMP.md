# Tạo site wp trên máy ảo cài LEMP
### 1. Chuẩn bị 1 máy cài sẵn LEMP
### 2. Tiến hành cấu hình WP
- **Bước 1**: Tạo cơ sở dữ liệu MariaDB
- 1. Đăng nhập vào MariaDB:
```
mysql -u root -p
```
    + Nhập mật khẩu root của MariaDB. Bạn sẽ nhận được lời nhắc của MariaDB.
- 2. Tạo cơ sở dữ liệu và người dùng mới có quyền sử dụng nó:
```
CREATE DATABASE wordpress;
GRANT ALL PRIVILEGES on wordpress.* to 'user' identified by 'password';
```
    + Trong ví dụ trên đây wordpress là tên của cơ sở dữ liệu, user tên người dùng và password mật khẩu (mạnh).
```
FLUSH PRIVILEGES;
```
- 3. Thoát khỏi MariaDB
```
Exit
```
- **Bước 2**: Tạo document root và log
    + Đây chính là nơi sẽ lưu trữ toàn bộ dữ liệu website của bạn nên bạn phải phân quyền thật cẩn thận.
``` 
mkdir /usr/share/nginx/quynhkkk.com
mkdir /usr/share/nginx/quynhkkk.com/logs
```
- **Bước 3**: Truy cập vào đường dẫn vi /etc/nginx/conf.d/default.conf, sau đó thay đổi các đoạn như bên dưới.
```
server {
        listen 80;
        server_name quynhkkk.com;

        access_log /usr/share/nginx/quynhkkk.com/logs/access.log;
        error_log /usr/share/nginx/quynhkkk.com/logs/error.log;

location / {
        root /usr/share/nginx/quynhkkk.com;
        index index.php index.html index.htm;

if (-f $request_filename) {
        expires 30d;
        break;
}

if (!-e $request_filename) {
        rewrite ^(.+)$ /index.php?q=$1 last;
        }
}

location ~ .php$ {
        fastcgi_pass   localhost:9000;  # port where FastCGI processes were spawned
        fastcgi_index  index.php;
        fastcgi_param  SCRIPT_FILENAME   /usr/share/nginx/quynhkkk.com$fastcgi_script_name;  # same path as above
        fastcgi_param PATH_INFO               $fastcgi_script_name;
        include /etc/nginx/fastcgi_params;
        }
}
```
- Xác minh các tập tin cấu hình.
```
nginx -t
```
- Nếu bạn nhận được sau đây, nó có nghĩa là các mục nhập trong virtual host đã chính xác.
```
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
```
- Khởi động lại
```
systemctl restart nginx
systemctl restart php-fpm
```
- **Bước 4**: Cài đặt WP
- Tải về WordPress mới nhất.
```
wget http://wordpress.org/latest.tar.gz
```
- Giải nén tập tin WordPress với đuôi *.tar.gz
```tar xzvf latest.tar.gz
```
- Di chuyển nó đến thư mục document root
```
mv wordpress/* /usr/share/nginx/quynhkkk.com
```
- Sao chép tệp wp-sample-config.php và thay đổi thành wp-config.php.
```
cp /usr/share/nginx/quynhkkk.com/wp-config-sample.php /usr/share/nginx/quynhkkk.com/wp-config.php
```
- Chỉnh sửa tệp wp-config.php cấu hình kết nối đến cơ sở dữ liệu.
```
vi /usr/share/nginx/quynhkkk.com/wp-config.php
```
```
// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'database_name_here');
/** MySQL database username */
define('DB_USER', 'username_here');
/** MySQL database password */
define('DB_PASSWORD', 'password_here');
/** MySQL hostname */
define('DB_HOST', 'localhost');
```
- Phân quyền cho user Nginx toàn quyền trên thư mực chứa wordpress.
```
chown -R nginx:nginx /usr/share/nginx/quynhkkk.com/
```
- Giờ ta truy cập vào trình duyệt bằng domain hoặc ip cua mình, chọn ngôn ngữ và cài đặt tùy chọn.

