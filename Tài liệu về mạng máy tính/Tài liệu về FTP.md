# FTP
### 1. FTP là gì?
> FTP - File Transfer Protocol (Giao thức truyền tải tập tin) được dùng trong việc trao đổi dữ liệu trong mạng thông qua giao thức TCP/IP, thường hoạt động trên 2 cổng là 20 và 21. Với giao thức này, các máy client trong mạng có thể truy cập đến máy chủ FTP để gửi hoặc lấy dữ liệu. Điểm nổi bật là người dùng có thể truy cập vào máy chủ FTP để truyền và nhận dữ liệu dù đang ở xa.
![email](https://www.totolink.vn/public/uploads/img_article/giaothucftplaginhungdieubanchuabietvegiaothucftp-1.png)
### 2. Mô hình hoạt động của giao thức FTP
- Giao thức FTP hoạt động dựa trên mô hình cơ bản của việc truyền và nhận dữ liệu từ máy Client đến máy Server. Quá trình truyền nhận dữ liệu giữa máy Client và Server lại được tạo nên từ 2 tiến trình TCP logic là Control Connection và Data Connection.
![email](https://www.totolink.vn/public/uploads/img_article/giaothucftplaginhungdieubanchuabietvegiaothucftp-2.png)
- **Control Connection:** Đây là phiên làm việc TCP logic đầu tiên được tạo ra khi quá trình truyền dữ liệu bắt đầu. Tuy nhiên, tiến trình này chỉ kiểm soát các thông tin điều khiển đi qua nó, ví dụ như các tập lệnh. Quá trình này sẽ được duy trì trong suốt quá trình phiên làm việc diễn ra.
- **Data Connection:** Khác với tiến trình Control Connection, Data Connection là một kết nối dữ liệu TCP được tạo ra với mục đích chuyên biệt là truyền tải dữ liệu giữa máy Client và máy Server. Kết nối sẽ tự động ngắt khi quá trình truyền tải dữ liệu hoàn tất.
### 3. Các phương thức truyền dữ liệu trong giao thức FTP
> Khi quá trình truyền dữ liệu được thiết lập, dữ liệu sẽ được truyền từ máy Client đến máy Server hoặc có thể ngược lại. Dựa trên việc truyền dữ liệu này, FTP có 3 phương thức truyền tải dữ liệu là stream mode, block mode, và compressed mode.
- **Stream mode:** Phương thức này hoạt động dựa vào tính tin cậy trong việc truyền dữ liệu trên giao thức TCP. Dữ liệu sẽ được truyền đi dưới dạng các byte có cấu trúc không liên tiếp. Thiết bị gửi chỉ đơn thuần đẩy luồng dữ liệu qua kết nối TCP tới phía nhận mà không có một trường tiêu đề nhất định.
- **Block mode:** Là phương thức truyền dữ liệu mang tính quy chuẩn hơn. Với phương thức này, dữ liệu được chia thành nhiều khối nhỏ và được đóng gói thành các FTP blocks. Mỗi block sẽ chứa thông tin về khối dữ liệu đang được gửi.
- **Compressed mode:** Phương thức truyền sử dụng kỹ thuật nén dữ liệu khá đơn giản là “run-length encoding”. Với thuật toán này, các đoạn dữ liệu bị lặp sẽ được phát hiện và loại bỏ để giảm chiều dài của toàn bộ thông điệp khi gửi đi.
![email](https://www.totolink.vn/public/uploads/img_article/giaothucftplaginhungdieubanchuabietvegiaothucftp-3.png)
### 4. Một số thiết bị Router Wifi hỗ trợ FTP Service
- TOTOLINK A3000RU
- TOTOLINK A3002RU - V1
- TOTOLINK A3002RU - V2
- TOTOLINK A6004NS
- TOTOLINK A8000RU
> TOTOLINK mong rằng các thông tin trong bài viết này sẽ giúp người dùng hiểu và vận dụng tốt hơn máy chủ FTP để phục vụ cho nhu cầu sử dụng của chính mình.
- ![email](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvWhXa-GN_skUn_0OXhHGTpflgfX3GaTogug&usqp=CAU)