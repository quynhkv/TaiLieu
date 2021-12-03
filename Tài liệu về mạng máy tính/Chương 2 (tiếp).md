# TRUYỀN FILE FTP (FILE TRANSFER)
> FTP (File Transfer Protocol) là giao thức truyền file giữa các máy tính. Giao thức này xuất hiện từ những năm 1971 nhưng vẫn còn được sử dụng rộng rãi cho đến tận ngày nay. FTP được đặc tả trong RFC 959.
### 1. Các lện FTP (FTP Commands)
- Lệnh (yêu cầu) từ client đến server và kết quả (trả lời) từ server tới client được gửi thông qua kết nối điều khiển và được mã hóa bằng bảng mã ASCII 7 bit
**USER username:** sử dụng để gửi thông tin định danh người dùng cho server.
**PASS password:** dùng để gửi password cho server.
**LIST:** dùng để yêu cầu server gửi một danh sách các file trong thư mục hiện thời. Danh sách này được gửi thông qua một kết nối dữ liệu TCP
**RETR filename:** dùng để lấy một file từ thư mục hiện thời (trên máy ở xa)
**STOR filename:** dùng để tải một file vào thư mục hiện thời (trên máy ở xa)
# THƯ TÍN ĐIỆN TỬ TRÊN INTERNET (E-mail)
> Cùng với Web, thư điện tử là một trong những ứng dụng Internet thồn dụng nhất. Gần giống thư tín điện tử thông thường, e-mail là dịch vụ không đòi hỏi đồng bộ - nghĩa là mọi người gửi và đọc thư khi thấy thuận tiện, không cần theo kế hoạch trước.
### 1. SMTP
> SMTP (Simple Mail Transfer Protocol) là giao thức gửi thư điện tử của tầng ứng dụng. SMTP sử dụng dịch vụ truyền dữ liệu tin cậy của TCP để truyền thư từ mail server của người gửi đến mail server của người nhận.
> Là trái tim của dịch vụ gửi thư trên Internet và được đặc tả trong RFC 821.
### 2. So sánh SMTP với HTTP
- Cả hai giao thức đều được sử dụng để gửi file giữa các máy tính.
- Khi truyền file cả hai giao thức HTTP và SMTP cùng sử dụng kêt nối liên tục.
- Điểm khác biệt cơ bản giữa hai giao thức là:
    + HTTP là giao thức kiểu kéo(Pull protocol)- client kéo thông tin từ server về.
    + SMTP là giao thức theo kiểu đẩy(Push protocol)- client đẩy thông tin lên server.
### 3. Khuôn dạng thư và chuẩn MIME
