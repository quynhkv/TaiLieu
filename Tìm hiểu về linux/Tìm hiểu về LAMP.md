# TÌM HIỂU SƠ LƯỢC VỀ LAMP
### 1. LAMP là gì?
- ### **Khái niệm**
    + ![m](https://f4-zpcloud.zdn.vn/4610653278723357913/74e424a197fe5da004ef.jpg)
    + LAMP là viết tắt của các từ Linux, Apache, MySQL và PHP, là giải pháp máy chủ kết hợp từ 4 giải pháp phần mềm: Linux - Apache - MySQL - PHP. Đa số các Linux hosting hiện nay sử dụng công nghệ này. Các phần mềm này kết hợp với nhau tạo thành các stack phần mềm, từ đó giúp các thành phần Website hoạt động trên nền tảng này hiệu quả.
- ### **Các phần mềm này tạo thành các stack và các stack này được sắp xếp theo trình từ như sau:**
    + Linux: là stack đầu tiên, hệ điều hành này là hệ điều hành mã nguồn mở được sử dụng rộng rãi, và được nhiều lập trình viên biết đến và áp dụng.
    + ![m](https://f4-zpcloud.zdn.vn/4089657186315589042/0bf35db6eee924b77df8.jpg)
    + Apache:  Lớp thứ 2 bao gồm phần mềm Web Server, thường là Apache Web (HTTP) Server, lớp này nằm trên Linux. Web Server chịu trách nhiệm chuyển đổi các web browser sang các website chính xác của chúng. Apache đã (và vẫn) là ứng dụng web server phổ biến nhất trên public Internet hiện nay. Trên thực tế, Apache được ghi nhận là đóng một vai trò quan trọng trong sự phát triển ban đầu của World Wide Web.
    + ![m](https://f5-zpcloud.zdn.vn/416668236745324230/a3288c6b3f34f56aac25.jpg)
    + MySQL: Lớp thứ ba là nơi cơ sở dữ liệu database được lưu trữ. MySQL lưu trữ các chi tiết có thể được truy vấn bằng script để xây dựng một website. MySQL thường nằm trên Linux và cùng với Apache /lớp 2. Trong cấu hình highend, MySQL có thể được off load xuống 1 máy chủ lưu trữ riêng biệt.
    + ![m](https://f4-zpcloud.zdn.vn/4712790608911325047/c217a8551b0ad154881b.jpg)
    + PHP: Là lớp trên cùng của stack. Lớp script bao gồm PHP và / hoặc các ngôn ngữ lập trình web tương tự khác. Các website và ứng dụng web chạy trong lớp này. Hầu hết các. Developer nên biết về LAMP stack truyền thống vì nó đã được sử dụng làm web từ rất lâu rồi. Tất cả các công nghệ backend như PHP và Mysql đều rất phổ biến và được hỗ trợ bởi các nhà cung cấp hosting lớn. Do đó, ưu điểm lớn nhất của LAMP stack là bảo mật và sự hỗ trợ rộng rãi. Các CMS phổ biến nhất như WordPress, Joomla, Drupal.. đều được phát triển trên nền PHP và MySQL. Cả Apache, PHP và Mysql đều có mã nguồn mở, đó là lý do tại sao Linux là lớp nền tảng cho môi trường này. Đây cũng là môi trường đơn giản nhất để các developer làm web trực tuyến.
    + ![m](https://f5-zpcloud.zdn.vn/6270168104305626388/e797aed61d89d7d78e98.jpg)
### 2. Apache là gì?
- ![m](https://f5-zpcloud.zdn.vn/416668236745324230/a3288c6b3f34f56aac25.jpg)
- ### **Khái niệm.**
    + Apache - tên chính thức là Apache HTTP Server - đây là một phần mềm web server miễn phí có mã nguồn mở. Một sản phẩm được phát triển và điều hành bởi hệ thống Apache Software Foundation. Và đây cũng một trong những web server được sử dụng phổ biến nhất hiện nay chiếm khoảng 54%.Các yêu cầu được gửi tới máy chủ sử dụng dưới phương thức HTTP. Khi bạn sử dụng trình duyệt này, bạn chỉ cần nhập địa chỉ IP hoặc URL và nhấn ENTER. Sau đó, máy sẽ tiếp nhận địa chỉ IP hoặc URL mà bạn đã nhập vào. Chức năng này có được là do cài đặt trên web server.
- ### **Cách thức hoạt động**
    + Apache Web Server chạy trên chính phần mềm của mình chứ không phải là server vật lý. Với nhiệm vụ chủ yếu là thiết lập kết nối, liên kết giữa server và browser rồi chuyển file giữa chúng (cấu trúc hai chiều client - server). Ngoài ra, Apache  - một phần mềm đa nền tảng được hoạt động khá mượt với cả server Unix và Windows.
    + Khi người dùng tiến hành tải site lên web, trình duyệt sẽ gửi đi 1 request tải trang lên phía server. Apache có nhiệm vụ trả lại kết quả đầy đủ các file, thành phần để hiển thị các trang About Us. Server và client giao tiếp qua HTTP protocol.
    + Không dừng lại ở đó, apache còn là một nền tảng module với độ tùy biến cao và chuẩn xác. Modules sẽ cho phép admin của server thực hiện các chế độ như tắt hoặc thêm vào các chức năng. Apache với công dụng sở hữu các chức năng modules mang tính bảo mật caching, chứng thực mật khẩu tuyệt đối.
- ### **Ưu điểm**
    + Là một phần mềm mã nguồn mở miễn phí phục vụ được cho nhiều mục đích ngoài về công nghệ mà còn có thể trên cả lĩnh vực thương mại, kinh doanh.
    + Là một phần mềm đáng tin cậy, chất lượng ổn định.
    + Được cập nhật một cách thường xuyên, phát hiện báo lỗi và lỗi bảo mật liên tục giúp người dùng ngăn chặn nguy cơ bị xâm phạm thông tin.
    + Linh hoạt về các thể thức cấu trúc module.
    + Hoạt động hiệu quả, nhanh nhạy với WordPress sites.
    + Sở hữu một cộng đồng lớn nhằm tương trợ, giải đáp thắc mắc trong mọi vấn đề.
    + Cấu hình đơn giản, thân thiện với những người mới bắt đầu sử dụng ứng dụng này.
- ### **Nhược điểm**
    + Do nhiều người có thể truy cập vào cùng một lúc nên đôi khi quá trình truy vấn còn gặp trục trặc, chậm hoặc thông tin đến người dùng có sự nhầm lẫn làm ảnh hưởng đến hiệu năng làm việc của Apache Web.
    + Vì app miễn phí nên người dùng có thể lựa chọn sử dụng nhiều cách thiết lập khác nhau và chính vì vậy dẫn đến tình trạng bảo mật đôi khi còn kém.
### 3. MySQL là gì?
- ![m](https://f4-zpcloud.zdn.vn/4712790608911325047/c217a8551b0ad154881b.jpg)
- ### **Khái niệm.**
    + MySQL là một hệ thống quản trị cơ sở dữ liệu mã nguồn mở (gọi tắt là RDBMS) hoạt động theo mô hình client-server. Với RDBMS là viết tắt của Relational Database Management System.
    + MySQL quản lý dữ liệu thông qua các cơ sở dữ liệu. Mỗi cơ sở dữ liệu có thể có nhiều bảng quan hệ chứa dữ liệu. MySQL cũng có cùng một cách truy xuất và mã lệnh tương tự với ngôn ngữ SQL.
- ### **Ưu điểm**
    + Dễ sử dụng.
    + Độ bảo mật cao.
    + Đa tính năng.
    + Khả năng mở rộng và mạnh mẽ.
    + Nhanh chóng.
- ### **Nhược điểm**
    + Có giới hạn.
    + Độ tin cậy thấp.
    + Dung lượn hạn chế.
### 4. PHP là gì?
- ### **Khái niệm**
- ![m](https://f5-zpcloud.zdn.vn/6270168104305626388/e797aed61d89d7d78e98.jpg)
    + Là ngôn ngữ script được tạo cho các giao tiếp phía server. Do đó, nó có thể xử lý các chức năng phía server như thu thập dữ liệu biểu mẫu, quản lý file trên server, sửa đổi cơ sở dữ liệu và nhiều hơn nữa.
- ### **Ưu điểm**
    + Nó phổ biến rộng rãi do tính chất nguồn mở và chức năng linh hoạt. Nó cũng đủ đơn giản cho người mới sử dụng nhưng các lập trình viên chuyên nghiệp cũng có thể dùng các tính năng nâng cao hơn.
### 5. Linux là gì?
- ![m](https://f4-zpcloud.zdn.vn/1625366133524342696/36ef08adbbf271ac28e3.jpg)
- ### **Khái niệm**
    + Là một hệ điều hành máy tính đang được sử dụng rộng rãi trong thời gian gần đây. Trong đó có 2 khách hàng lớn là IBM và Dell. Linux đồng thời cũng là tên hạt nhân của hệ điều hành này.
- ### **Ưu điểm**
    + Không tốn nhiều chi phí mua bản quyền.
    + Tính bảo mật tương đối cao.
    + Tính linh hoạt.
    + Có thể hoạt động tốt trên các máy tính cấu hình yếu.
- ### **Nhược điểm**
    + Số lượng ứng dụng được hỗ trợ trên Linux còn hạn chế.
    + Một số nhà sản xuất không phát triển driver hỗ trợ nền tảng Linux.
