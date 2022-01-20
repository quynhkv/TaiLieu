# Các bước xử lý
- Đầu tiên ta đăng nhập vào trang quản trị của trang web muốn chuyển dữ liệu ví dụ ở đây khách hàng muốn chuyển dữ liệu từ Cpanel sang DA.
- Ở giao diện trang quản trị Cpanel ta kéo xuống và click vào Domain, chọn mục public_html

![q](https://f4-zpcloud.zdn.vn/5932031432396810003/638d49c0171fda41830e.jpg)

![q](https://f4-zpcloud.zdn.vn/1391896687330945106/acda0a9754489916c059.jpg)

- Sau đó ta chọn tất cả file và nén lại rồi tải file vừa nén về

![q](https://f5-zpcloud.zdn.vn/7388171205651171222/3f6ca18d5e5d9303ca4c.jpg)

- Tiếp đó login vào trang quản trị con DA, ta tạo user(lưu ý khi tạo phải thêm mail của khách hàng vào)

![q](https://f4-zpcloud.zdn.vn/2033591671765509815/89e8b8e1f53e3860612f.jpg)

![q](https://f5-zpcloud.zdn.vn/8223983375745621587/c432b03bfde430ba69f5.jpg)

- Truy cập list user


- Login với tài khoản user vừa tạo


- Truy cập MySQL Managerment


- Tạo data base mới


- Nhập các thông tin để tạo data base


- Truy cập phpadmin với data base vừa tạo và import bên Cpanel


- Quay lại giao diện DA truy cập file


- Click vào `public_html` và giải nén các file ta đã tải ở bước trên 


- Chỉnh sửa file `wp-config.php`


- Chỉnh sửa DB name, user name, password đúng với tài khoản vừa tạo ở trên


- Thêm tên miền vào file host để kiểm tra 


- Sau khi kiểm tra thấy web mới chưa có chứng chỉ SSL ta truy cập vào giao diện SSL/TLS của con Cpanel để mượn chứng chỉ cho web mới


- Truy cập giao diện SSL trên con DA để gắn key và chạy thử


- Sau khi chạy thử thành công ta quay lại check xem tên miền của web đang trỏ về đâu, nếu trỏ về DNS của Nhân Hòa thì đã hoàn tất