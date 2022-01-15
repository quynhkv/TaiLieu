# Cài đặt Let's Encrypt với certbot Apache
### I. Chuẩn bị
- Một máy chủ CentOS 7 đã cài đặt LAMP Stack.
- Đã trỏ tên miền về ip máy chủ.
### II. Các bước cài đặt
- **1. Cài đặt Certbot Let's Encrypt Client**
    + Tạo kho lưu trữ CentOS 7 EPEL
    ```yum install epel-release```
    + Cài đặt Certbot
    ```yum install certbot python2-certbot-apache mod_ssl```
- **2. Lấy chứng chỉ**
    + Sau khi cài đặt được Certboot ta có thể sử dụng nó để yêu cầu chứng chỉ SSL cho tên miền của mình.
    + Để thực hiện cài đặt tương tác và lấy chứng chỉ.
    ```sudo certbot --apache -d quynh2k.xyz```
        + Với quynh2k.xyz là tên miền.
        + --apache là plugin và chỉ định tên miền để cấu hình chứng chỉ với -d.
    ```sudo certbot --apache -d quynh2k.xyz -d www.quynh2k.xyz```
- **3. Kiểm tra trạng thái chứng chỉ của bạn**
    + Cách 1: Kiểm tra từ trình duyệt của bạn.
    + Cách 2: Check từ trang SSL Shopper.







# Cài đặt Let's Encrypt với certbot Nginx
### I. Chuẩn bị
- Một máy chủ CentOS 7 đã cài đặt LEMP Stack.
- Đã trỏ tên miền về ip máy chủ.
### II. Các bước cài đặt
- **1. Cài đặt Cerbot Let’s Encrypt Client.**
    + Đầu tiên bạn cần cài đặt EPEL repository: 
    ```sudo yum -y install epel-release```
    + Tiếp theo cài đặt certbot-nginx bằng câu lệnh sau: 
    ```sudo yum -y install certbot-nginx```
- **2. Cài đặt SSL Let’s Encrypt**
    + Để cài đặt SSL cho website , các bạn sử dụng câu lệnh sau.
    ```sudo certbot --nginx -d quynh2k.xyz -d www.quynh2k.xyz```
    + `(Nhập email của bạn)` ở câu hởi đầu tiên - ở câu hỏi thứ 2 `(Y)es/(N)o: Y   (Nhấn Y để đồng ý điều khoản)` - ở câu hỏi thứ 3 `(Y)es/(N)o: N   (Nhấn N để từ chối các thông tin, tin tức từ letsencrypt và Certbot )`
    + Như vậy đã cài đặt thành công SSL thông qua Certbot, đường đẫn lưu file chứng chỉ của website sẽ nằm tại đường dẫn tương ứng.

        ```Certificate: /etc/letsencrypt/live/quynh2k.xyz/fullchain.pem```

        ``` Private Key: /etc/letsencrypt/live/quynh2k.xyz/privkey.pem```
    + Chứng chỉ Let’s Encrypt chỉ có hiệu lực trong 90 ngày, do đó bạn có thể thiết lập cronjob  để chứng chỉ tự động gia hạn nếu như hết hạn.
    + Các bạn chạy câu lệnh sau để mở cửa sổ thêm Cronjob.
    `sudo export VISUAL=nano; crontab -e`
    + Copy nội dung bên dưới và dán vào cửa sổ Crontab.
    `00 6 * * * /usr/bin/certbot renew --quiet`
    > Chú thích: Cronjob này có nghĩa là cứ đúng 6:00 AM nó sẽ check chứng chỉ, nếu chứng chỉ hết hạn sẽ tự động gia hạn. Ngược lại, nếu còn hạn sẽ không thực hiện gia hạn.
- **3. Kiểm tra chứng chỉ sau cài đặt**
    + Cách 1: Kiểm tra từ trình duyệt của bạn.
    + Cách 2: Check từ trang SSL Shopper.