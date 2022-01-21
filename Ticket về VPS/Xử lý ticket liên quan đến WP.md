### Cài WP trên Cpanel
- Đầu tiên ta truy cập vào trang quản trị Cpanel

![q](https://f5-zpcloud.zdn.vn/6276924542981904293/6e3a99338bd2468c1fc3.jpg)

- Kéo xuống tìm và click vào mục Wp toolkit

![q](https://f6-zpcloud.zdn.vn/8824655528289882006/878025d43735fa6ba324.jpg)

- Ở đây công cụ WP toolkit của Cpanel sẽ hỗ trợ ta cài đặt WP nhanh chóng do nó sẽ tạo sẵn cho ta DB cũng như 1 số setting rồi, ta tiến hành click vào install và bước vào quá trình điền thông tin

![q](https://f5-zpcloud.zdn.vn/8168553395886956018/459e37c92528e876b139.jpg)

- Trong phần này ta cần chú ý một số thông tin như sau:
    + 1. Installation path(đường dẫn cài đặt): mục này ta có thể bỏ trống hoặc nếu muốn / đến đâu thì có thể thêm vào tùy ý.
    + 2. Website title(tiêu đề website): mục này ta nhập tên tiêu đề nào mà ta muốn.
    + 3. Plugin/theme set(tùy chọn phiên bản cài đặt plugin/theme): ở đây ta chọn None nếu muốn cài plugin/theme theo mặc định.
    + 4. Ngôn ngữ: tùy chọn
    + 5. Version(phiên bản): ta để mặc định
    + 6. Username: nhập username muốn đặt
    + 7. Password: nên đặt mật khẩu có tính bảo mật mạnh
    + 8. Email: tùy chọn

![q](https://f5-zpcloud.zdn.vn/4782570254607472933/8e7c92c39522587c0133.jpg)

- Tiếp đến phần DB và Automatic update settings như đã nói ở trên thì công cụ WP toolkit đã hỗ trợ tạo sẵn rồi ta chỉ việc click vào install và cài đặt thôi.

![q](https://f6-zpcloud.zdn.vn/5981921766316598854/e508e15ff3be3ee067af.jpg)

- Đợi quá trình cài đặt hoàn tất sau khoảng 3-5p ta đã có 1 site WP mới.

![q](https://f6-zpcloud.zdn.vn/7162011369464214129/147842421aa3d7fd8eb2.jpg)

- Tiếp theo ta cài đặt và sử dụng Plugin Duplicator WordPress Để Backup Và Restore Website, ở bước này ta có thể làm theo trang hướng đã sau `https://blog.vinahost.vn/plugin-duplicator-wordpress`
- Lưu ý ở bước này ta nên tạo một DB mới trên Cpanel như sau:
    + Trở lại giao diện trang quản trị, tìm đến và click vào mục MySQL Database

![q](https://f6-zpcloud.zdn.vn/5062179987779937713/d790317a489b85c5dc8a.jpg)

+ Trong giao diện này ta tạo một DB mới, nhập tên muốn đặt và click Create

![q](https://f4-zpcloud.zdn.vn/1458540368250371637/5f34fede873f4a61132e.jpg)

+ Tiếp đến ta tạo user mới và add nó vào DB vừa tạo ở trên

![q](https://f6-zpcloud.zdn.vn/8046518068224041942/91a0ea4d93ac5ef207bd.jpg)

+ Tạo xong DB mới ta quay lại trang cài đặt theo hướng dẫn ở trên, nhập thông tin DB, user, password ứng với DB ta mới tạo và làm các bước tiếp tục theo hướng dẫn
- Sau khi làm theo hướng dẫn vậy là ta đã có 1 website hoàn chỉnh.
### Lưu ý
> Khi tạo website xong mà login vào trang quản trị báo sai mật khẩu thì ta làm theo hướng dẫn sau để đổi mật khẩu.
- Đầu tiên ta trở lại giao diện trang quản trị Cpanel tìm và click vào mục phpMyAdmin

![q](https://f6-zpcloud.zdn.vn/7491407991759176691/b38f2597b97674282d67.jpg)

- Ở đây ta click vào tên DB mới tạo ở phần trước

![q](https://f4-zpcloud.zdn.vn/345822531451860323/f9c242dade3b13654a2a.jpg)

- Tìm đến mục wpnh_user và click vào

![q](https://f6-zpcloud.zdn.vn/7939995364647410830/8b9b3580a961643f3d70.jpg)

- Ở đây ta thấy giao diện này hiển thi toàn bộ thông tin về DB, ở mục user_pass đó không phải là mật khẩu mà đó là một mã hóa 

![q](https://f5-zpcloud.zdn.vn/2305652460121969257/687a2860b48179df2090.jpg)

- Để thay đổi mật khẩu ta tích chọn và nhấn Edit

![q](https://f6-zpcloud.zdn.vn/4741381777728232802/6bb91da481454c1b1554.jpg)

- Trong giao diện Edit ở mục Value ta nhập mật khẩu mới và ở mục Funtion chọn MD5 rồi click Go để hoàn tất

![q](https://f6-zpcloud.zdn.vn/1870593319291391844/acb822a5be44731a2a55.jpg)

