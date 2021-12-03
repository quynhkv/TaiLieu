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
![email](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSEYQfXZBYTQI3zD2bxKlSICR1USdttgsZdBw&usqp=CAU)
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
- 5 nhóm dữ liệu chính:
    + **Văn bản (Text)**
    + **Ảnh (Image)**
    + **Âm thanh (Audio)**
    + **Video**
    + **Kiểu ứng dụng (Application)**
### 4. Giao thức truy cập mail
- **POP3**
    + POP3 được đặc tả trong RFC 1939 là giao thức lấy thư cực kỳ đợn giản và có ít chức năng.
    + POP3 gồm 3 giai đoạn: kiểm chứng, tiến hành xử lý và cập nhật.
- **IMAP**
    + Giống như POP3, IMAP cũng là giao thức lấy thư nhưng nó có nhiều đặc tính phức tạp hơn.
    + IMAP được thiết kế cho phép người dùng thao tác trên những hộp thư ở xa một cách dễ dàng; cho phép Bob tạo ra những thư mục thư khác nhau trong mailbox. Bob có thể đặt thư vào thư mục hay dịch chuyển thư từ thư mục này đến thư mục khác. IMAP cũng có lệnh cho phép tìm kiếm trên thư mục theo tiêu chí xác định.
    + IMAP có một đặc tính quan trọng là có những lệnh cho phép user agent chỉ lấy một số thành phần trong thư.
    + Phiên làm việc IMAP gồm 3 giai đoạn: giai đoạn thiết lập kết nối giữa client(user agent) và IMAP server, giai đoạn server chấp nhận kết nối và giai đoạn tương tác client/server.
- **HTTP**
    + Ngày nay, nhiều người sử dụng Webmail - dịch vụ có thể truy cập email qua trình duyệt (Hotmail hay Yahoomail). Khi đó, user agent là trình duyệt Web thông thường và mọi người kết nối tới hộp thư của mình trên mail server qua HTTP.
# DỊCH VỤ TÊN MIỀN - DNS
### 1. Các dịch vụ của DNS
> DNS là cơ sở dữ liệu phân tán được đặt trên một hệ thống phân cấp các máy phục vụ tên(nameserver) và giao thức thuộc tầng úng dụng cho phép máy tính và máy chủ thông tin phục vụ mục đích xách định địa chỉ IP. Máy chủ tên miền thường là các máy UNIX có cài đặt phần mềm Berkely Internet Name Domain (BIND). Giao thức DNS chạy trên nền UDP với số hiệu cổng là 53.
> - *Bên cạnh dịch vụ xác định địa chỉ IP từ tên máy, DNS cung cấp một số dịch vụ quan trọng sau:*
- **Dịch vụ đặt bí danh cho máy tính (Host aliasing):**
    + Máy tính có tên phức tạp có thể có một hoặc nhiều bí danh (alias).
    + Tên bí danh thường dễ nhớ hơn tên đầy đủ
    + Một ứng dụng có thể yêu cầu DNS xác định tên đầy đủ cũng như địa chỉ IP của một tên bí danh.
- **Dịch vụ đặt tên bí danh cho mail server (Mail server aliasing)**
    + Hiển nhiên địa chỉ email cần dễ nhớ. Ví dụ Bob có tài khoản trên Hotmail, địa chỉ của Bob có thể đơn giản là bob@hotmail.com. Tuy nhiên tên máy tính của máy phục vụ thư tại Hotmail phức tạp và vì thế khó nhớ hơn so với hotmail.com. Ứng dụng có thể sử dụng DNS để xác định tên đầy đủ của một bí danh cũng như đại chỉ IP của máy tính đó. Trên thực tế, DNS cho phép mail server và Webserver của các công ty có tên (bí danh) giống nhau.
- **Phân tán tải(load distribution):**
    + DNS thực hiện việc phân tán tải cho các server, đặc biệt là các Webserver "nhân bản" (replicated) (là các server có nội dung giống hệt nhau).
### 2. Cơ chế hoạt động của DNS
![email](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQwmRZwWiuxxBnith5vGIwJJlEChW_Mc6WSsA&usqp=CAU)
> Với client, DNS là một "hộp đen". Client gửi thông điệp truy vấn DNS vào hộp đen đó, trong thông điệp chứa tên máy cần xác định địa chỉ IP. Với hệ điều hành Unix, gethostname() là một hàm mà úng dụng có thể gọi để gửi thông điệp truy vấn. Sau một khoảng thời gian nào đó - từ vài phần nghìn giây đến vài chục giây, client nhận được thông điệp trả lời của DNS chứa địa chỉ IP cần xác định. Vì vậy, với client thì DNS là một dịch vụ xác định IP đơn giản và dễ hiểu. Nhưng "hộp đen" triển khai dịch vụ đó thực sự phức tạp, bao gồm nhiều máy chủ tên (nameserver) đặt khắp nơi trên thế giới và một giao thức ở tầng ứng dụng xác định cách thức trao đổi thông tin giữa các nameserver và giữa nameserver với máy tính.
