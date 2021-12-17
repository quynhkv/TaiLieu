# Sơ lược về LEMP Stack
### 1. LEMP Stack là gì?
- Các thành phần cấu thành LEMP stack cũng gần tương tự với LAMP, chỉ khác là Apache sẽ được thay thế bởi Nginx. Nginx được đọc là "engine-x", giải thích cho chữ E trong "LEPM", nginx cũng là một ứng dụng HTTP proxy nhưng không có được danh tiếng ấn tượng như Apache, tuy nhiên, nó có ưu điểm là cho phép xử lý tốc độ tải cao hơn đối với các HTTP request.
![q](https://f5-zpcloud.zdn.vn/4547017683293779429/9259a7ed2299e8c7b188.jpg)
### 2. Điểm khác biệt với LAMP Stack.
> Như đã nói, khác biệt cơ bản giữa LAMP và LEMP stack là ở 2 thành phần Apache và Nginx. Vậy việc sử dụng nginx và Apache sẽ tạo ra những khác biệt gì? Chúng ta sẽ cùng so sánh riêng 2 phần mềm này để thấy được rõ hơn sự khác biệt:
- **Apache**
- ![q](https://f5-zpcloud.zdn.vn/5242279977837563195/3ba4e4116165ab3bf274.jpg)
    + Apache đã được sử dụng từ lâu (từ những năm 1995), có rất nhiều các module được viết và cả người dùng tham gia vào mở rộng hệ chức năng cho Apache.
    + Phương pháp process/thread-oriented – sẽ bắt đầu chậm lại khi xuất hiện tải nặng, cần tạo ra các quy trình mới dẫn đến tiêu thụ nhiều RAM hơn, bên cạnh đó, cũng tạo ra các thread mới cạnh tranh các tài nguyên CPU và RAM;
    + Giới hạn phải được thiết lập để đảm bảo rằng tài nguyên không bị quá tải, khi đạt đến giới hạn, các kết nối bổ sung sẽ bị từ chối;
    + Yếu tố hạn chế trong điều chỉnh Apache: bộ nhớ và thế vị cho các dead-locked threads cạnh tranh cho cùng một CPU và bộ nhớ.
- **Nginx**
- ![q](https://f5-zpcloud.zdn.vn/4537555151372491964/d7fc0c49893d43631a2c.jpg)
    + Ứng dụng web server mã nguồn mở được viết để giải quyết các vấn đề về hiệu suất và khả năng mở rộng có liên quan đến Apache.
    + Phương pháp Event-driven, không đồng bộ và không bị chặn, không tạo các process mới cho mỗi request từ web.
    + Đặt số lượng cho các worker process và mỗi worker có thể xử lý hàng nghìn kết nối đồng thời.
    + Các module sẽ được chèn vào trong thời gian biên dịch, có trình biên dịch mã PHP bên trong (không cần đến module PHP).
> **Để kết luận thì nginx nhanh hơn và có khả năng xử lý tải cao hơn nhiều so với Apache khi sử dụng cùng một bộ phần cứng. Tuy nhiên, Apache vẫn là tốt hơn nhiều khi nói đến chức năng và tính sẵn sàng của các module cần thiết để làm việc với các ứng dụng máy chủ back-end và chạy các ngôn ngữ kịch bản lệnh. Vậy nên việc lựa chọn sẽ phụ thuộc phần lớn vào những gì bạn muốn chạy trên web server của mình. Việc chạy cả Apache và nginx trên cùng một máy chủ vẫn có khả năng thực hiện được, và nó sẽ giúp người dùng có được lợi ích tốt nhất từ cả 2 phương pháp. Ví dụ, bạn có thể chạy nginx như reverse proxy trong khi để Apache chạy trong back-end.**