# Một số giao diện liên quan đến công việc
### 1. CRM
- Dùng để kiểm tra các Ticket.
- Check email của khách hàng.
- Check đơn hàng.
### 2. WHOIS
- Dùng để kiểm tra tên miền đang trỏ DNS về đâu.
### 3. ZONEDNS
- Quản lý, thêm khách hàng.
- Quản lý, thêm domain.
- Một số lưu ý:
+ Domain name: là thông tin của khách hàng cung cấp.
> ![q](https://f5-zpcloud.zdn.vn/274349040894188458/7863f809b4d27e8c27c3.jpg) 
+ Email kỹ thuật: là 1 email khác do khách hàng cung cấp - là email của người mà khách hàng cho phép người này thay họ quản lý tiên miền đã đăng ký.
> ![q](https://f5-zpcloud.zdn.vn/8804171176462593927/39172f7e63a5a9fbf0b4.jpg)
+ Mật khẩu: ta sẽ đặt mật khẩu cho khách hàng ở đây.
> ![q](https://f4-zpcloud.zdn.vn/7360093148707768085/1ac65da81173db2d8262.jpg)
+ Khách hàng: đây là email chính của khách hàng.
> ![q](https://f5-zpcloud.zdn.vn/4836113868840032731/a1ac80c0cc1b06455f0a.jpg)
+ Ở phần thông tin thêm: thường thì khi ta lấy lại thông tin tên miền cho khách hàng thì ta sẽ tích “có” ở cả 2 mục này sau đó “Cập nhật domain”.
> ![q](https://f5-zpcloud.zdn.vn/8436650447860782858/37a3facfb6147c4a2505.jpg)
+ Với yêu cầu muốn lấy lại thông tin tên miền đơn lẻ thì ta có thể kiểm tra tên miền – lấy lại password và gửi về mail cho khách hàng.
+ Còn với yêu cầu muốn lấy lại thông tin của nhiều tên miền cùng lúc thì ta hướng dẫn khách hàng chuyển đến cho bộ phận kinh doanh xử lý.
- Khi muốn tạo hoặc chỉnh sửa bản ghi cho tên miền ta search tên miền đó ra và click vào,
> ![q](https://f5-zpcloud.zdn.vn/9007983806295589677/36640a0146da8c84d5cb.jpg)
+ Và đây là giao diện để ta chỉnh sửa
> ![q](https://f5-zpcloud.zdn.vn/6061261009724162119/0069fa12b6c97c9725d8.jpg)
### 4. MXTOOLBOX
- Dùng để kiểm tra tên miền ở loại mx.
> ![q](https://f4-zpcloud.zdn.vn/7940498099898648721/8a137d6031bbfbe5a2aa.jpg)
- Ở đây ta có thể kiểm tra bằng rất nhiều loại bản ghi.
> ![q](https://f5-zpcloud.zdn.vn/2218326936886464191/9e7eaf0fe3d4298a70c5.jpg)
### 5. Một số phương pháp check ip tên miền bằng lệnh cmd
- **nslookup**
> ![q](https://f5-zpcloud.zdn.vn/2336378549210701117/11906be0273bed65b42a.jpg)
- **set type=ns**
> ![q](https://f5-zpcloud.zdn.vn/6074232719240654952/8c2d745a3881f2dfab90.jpg)
- **set type=a**
> ![q](https://f5-zpcloud.zdn.vn/1740591237557215895/1cc2b0b4fc6f36316f7e.jpg)
- **set type=mx**
> ![q](https://f5-zpcloud.zdn.vn/263091189205207762/30d29aa4d67f1c21456e.jpg)