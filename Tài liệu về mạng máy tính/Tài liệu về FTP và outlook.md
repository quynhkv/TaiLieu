# OUTLOOK
### 1. Outlook là gì?
![email](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRl529QAQ2Lq7K0XVf-L_i7DS2B_vLu2mwR2g&usqp=CAU)
> **Outlook** là phần mềm quản lý thông tin cá nhân của Microsoft, bao gồm các công cụ: e-mail, lịch, công việc quản lý, quản lý liên lạc, ghi chú, tạp chí và duyệt web.
- Outlook có thể được sử dụng như một ứng dụng độc lập, hoặc có thể làm việc với các ứng dụng kết hợp khác cho nhiều người dùng trong một tổ chức, chẳng hạn như chia sẻ các hộp thư và lịch biểu, trao đổi thư mục công cộng, danh sách SharePoint và lịch trình cuộc họp.
- Không phải là công cụ miễn phí, bạn sẽ phải mua phiên bản hoàn chỉnh hoặc trả cước để sử dụng khi có nhu cầu.
### 2. Ưu điểm của outlook
- **Tốc độ truy cập nhanh, không gian lưu trữ rộng mở.**
![email](https://cdn.tgdd.vn/Files/2018/12/07/1136233/outlook-la-gi-cach-cai-dat-va-su-dung-outlook-cho-nguoi-moi-bat-dau--7.jpg)
    + Hỗ trợ việc gửi mail đính kèm tập tin có dung lượng lớn kết hợp với OneDrive, Skype Drive và khôi phục email đã xóa (trong phạm vi và thời gian cho phép) ngay cả khi bạn đã hoàn tất thao tác xóa email trong thùng rác.
- **Tính bảo mật và khả năng chống spam cao.**
![email](https://cdn.tgdd.vn/Files/2018/12/07/1136233/outlook-la-gi-cach-cai-dat-va-su-dung-outlook-cho-nguoi-moi-bat-dau--8.jpg)
    + Có thể tạo, xóa và thay đổi các địa chỉ mail hay đăng nhập bằng mật khẩu tạm thời một cách dễ dàng.
- **Đa dạng kết nối.**
    + Tích hợp với các trang mạng xã hội đang chiếm ưu thế hiện nay như Facebook, Twitter, Skype...
# POP - IMAP - SMTP
### 1. POP
- ### **Khái niệm**
> POP – Post Office Protocol hay Giao thức Bưu điện là một giao thức tầng ứng dụng, dùng để lấy thư điện tử từ server mail, thông qua kết nối TCP/IP.
- Mặc định port POP3 là:
    + **Port 110** - port không mã hóa.
    + **Port 995** - SSL/TLS port, cũng có thể được gọi là OP3S.
- ### **Cách thức hoạt động**
    + **Bước 1:** Kết nối đến server.
    + **Bước 2:** Nhận toàn bộ mail.
    + **Bước 3:** Lưu cục bộ như mail mới.
    + **Bước 4:** Ngắt kết nối.
> Giống như một người đưa thư thông thường, giao thức POP sẽ xóa mail của bạn khỏi server và bạn có thể lựa chọn việc lưu trữ email trên thiết bị của mình, hoặc tạo 1 bản sao trên server đến khi cần, bạn có thể tải lại.
![email](https://lh5.googleusercontent.com/tM7JL-25VZ2p4_THsbBmhNjSCdtqBAoZOw7UlTjJa8LBTUOZ5XVM0_fvuYicit8GwrfkdrHSlxDBzOlv9q2308sf216M-7DD_IjyZ7-71n_Rpcxa1xCNdt5fKZHK8aQ5TF1gvYVV=s0)
- ### **Ưu điểm**
    + Chỉ một máy khách yêu cầu truy cập mail trên server và việc lưu trữ mail cục bộ là tốt nhất.
    + Mail luôn sẵn sàng có thể truy cập ngay cả khi không có kết nối Internet.
    + Kết nối Internet chỉ dùng để gửi và nhận mail.
    + Tiết kiệm không gian lưu trữ trên server.
    + Được lựa chọn để lại bản sao mail trên server. Thư đã gửi được lưu trữ cục bộ trên PC hoặc máy Mac, chứ không phải trên máy chủ email.
    + Hợp nhất nhiều tài khoản email và nhiều server vào một hộp thư đến.
- ### **Nhược điểm**
    + Không thể truy cập email từ xa, từ các máy tính khác.
    + Việc xuất folder lưu trữ mail cục bộ sang máy khác hoặc client hay một thiết bị vật lý khác sẽ khá khó khăn.
    + Có khả năng mất toàn bộ mail nếu folder mail bị hỏng.
    + Dễ nhận phải các mail có chứa virus, khiến máy tính bị tấn công.
### 2. IMAP
- ### **Khái niệm**
> IMAP – Internet Message Access Protocol hay Giao thức truy cập tin nhắn Internet cho phép người dùng đọc các email cục bộ bằng một ứng dụng trung gian như OutLook,...
- Port IMAP mặc định:
    + Port 143 – port không mã hóa.
    + Port 993 – SSL/TLS port, cũng có thể được gọi là IMAPS.
- ### **Cách thức hoạt động**
    + **Bước 1:** Kết nối đến server.
    + **Bước 2:** Lấy nội dung được yêu cầu từ người dùng và lưu đệm cục bộ, tổng kết tin nhắn hay nội dung của những email được chọn lựa kỹ càng.
    + **Bước 3:** Xử lý các biên tập từ người dùng. Ví dụ: đánh dấu email – mail để đọc, lưu hay xóa…
    + **Bước 4:** Ngắt kết nối.
- ### **Ưu điểm**
    + Là một dạng của lưu trữ đám mây, IMAP có thể tiết kiệm không gian lưu trữ cục bộ.
    + Mail được dự phòng tự động trên server.Vì mail được lưu trên server đầu xa nên ta có thể kiểm tra mail từ các thiết bị khác nhau ở khắp nơi trên thế giới.
    + Không giống với POP3, IMAP cho phép bạn truy cập, sắp xếp đọc thư ở bất cứ đâu mà không cần tải xuống trước điều này giúp bạn linh động hơn.
    + IMAP chỉ tải xuống thư khi ta bấm vào nó và phần đính kèm không tự động được tải xuống.
- ### ** Nhược điểm**
    + Chỉ sử dụng được khi có kết nối Internet.
    + Dung lượng lưu trữ email bị phụ thuộc vào nhà cung cấp dịch vụ.
    + Khó kiểm soát toàn bộ email nếu lượng lưu trữ quá lớn.
> # Nên sử dụng POP hay IMAP?
> ### Ta nên chọn IMAP nếu muốn:
- Truy cập email từ nhiều thiết bị khác nhau.
- Có một kết nối Internet thường xuyên và tin cậy.
- Xem nhanh các email mới hoặc những email trên server.
- Không phải lo lắng về vấn đề dự phòng dữ liệu do không gian lưu trữ cục bộ hạn chế.
> ### Ngược lại, ta nên chọn POP nếu muốn:
- Truy cập mail chỉ từ một thiết bị.
- Có thể truy cập email thường xuyên dù có kết nối Internet hay không.
- Không yêu cầu nhiều về không gian lưu trữ  do không gian lưu trữ trên server của POP khá hạn chế.
### 3. SMTP
- ### **Khái niệm**
> SMTP (Simple Mail Transfer Protocol, tạm dịch: Giao thức truyền tải thư tín đơn giản hóa) là giao thức thực hiện nhiệm vụ chính là gửi mail.
- ### **Nguyên lý hoạt động**
> SMTP liên lạc với server từ xa và gửi email từ mail client tới mail server. Sau đó được gửi đến server mail của email nhận.
- SMTP ports: 
    + Port 25 – port không mã hóa.
    + Port 465 – SSL/TLS port, cũng có thể được gọi là SMTPS.
- ### **SMTP khác POP và IMAP ở chỗ:**
> Nhiệm vụ của SMTP là gửi mail đi, còn nhiệm vụ của POP3 và IMAP là lấy mail về.