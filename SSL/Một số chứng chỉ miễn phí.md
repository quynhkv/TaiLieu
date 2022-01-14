# I. Một số chứng chỉ miễn phí của SSL
### 1. Chứng chỉ Let's Encrypt
- Let’s Encrypt là chứng chỉ tiêu chuẩn an ninh công nghệ toàn cầu miễn phí. Được quản lý bởi Internet Security Research Group (ISRG) - tập đoàn phi lợi nhuận của California. Với sứ mệnh nâng cao bảo mật trên môi trường internet, phá bỏ các rào cản về tài chính, công nghệ,....hướng tới mục đích an toàn chung.

![q](https://f5-zpcloud.zdn.vn/7379321608015647574/6998e6c71fd5d28b8bc4.jpg)

- Nguyên tắc của Let's Encrypt:
    + Let’s Encrypt hoạt động dựa trên 6 nguyên tắc Miễn phí - Tự động - An toàn - Minh bạch - Mở - Hợp tác.
    + Let’s Encrypt cung cấp chứng chỉ an ninh mạng hoàn toàn miễn phí cho các website sau khi yêu cầu thông tin xác minh. Chứng chỉ này có giá trị như SSL tính phí, đảm bảo trang web này chính chủ và an toàn với người dùng.
    + Các phần mềm chạy trên máy chủ web sở hữu Let’s Encrypt có thể tự động tương tác để lấy chứng chỉ một cách dễ dàng, tự động gia hạn.
    + Let’s Encrypt cung cấp chứng chỉ cho các trang web an toàn dựa trên những tiêu chuẩn bảo mật TLS và qua bên xét duyệt thứ ba - CA.
    + Các chứng chỉ Let’s Encrypt sau khi cấp phát và thu hồi đều được ghi lại công khai với tất cả người sử dụng. Giúp bạn có thể dễ dàng kiểm tra về độ an toàn của website trong những khoảng thời gian trước đây.
    + Let’s Encrypt là chứng chỉ cung cấp cho tất cả các website có nhu cầu. giao thức phát hành và gia hạn tự động sẽ được công bố như một tiêu chuẩn công khai.
    +   Let’s Encrypt là sản phẩm phi lợi nhuận hướng tới mục đích an toàn chung trên không gian mạng, được sự quan tâm và hợp tác cùng phát triển của các tập đoàn lớn như facebook, mozilla, Cisco,... nỗ lực đem lại lợi ích cho cộng đồng.
### 2. Chứng chỉ OpenSSL
- OpenSSL là một thư viện phần mềm có mã nguồn mở được sử dụng để mã hóa dữ liệu và triển khai các giao thức mạng. Công cụ này dùng cho toàn bộ các ứng dụng bảo mật truyền thông qua mạng máy tính để phòng chống nghe trộm hoặc cần phải xác định phe truyền thống ở phía đầu bên kia.
- OpenSSL ra mắt vào năm 1998 và có sẵn trong các hệ thống Linux, Windows, macOS và BSD. Với OpenSSL, người dùng có thể thực hiện các tác vụ liên quan đến SSL khác nhau như CSR (Yêu cầu ký chứng chỉ), tạo khóa riêng và cài đặt chứng chỉ SSL. Vì vậy, khi nhắc tới chứng chỉ SSL/TLS và cách thức triển khai chúng thì đây chính là công cụ thích hợp nhất.
- Hiện nay, chúng đang được ứng dụng rộng rãi trong các máy chủ web Internet nhằm phục vụ cho hầu hết các trang web.

![q](https://f5-zpcloud.zdn.vn/2992913659695958912/134787187e0ab354ea1b.jpg)

- OpenSSL được sử dụng để:
    + Tạo các tham số chính RSA, DH và DSA
    + Tạo chứng chỉ X.509, CSR và CRL
    + Mã hóa và giải mã bằng mật mã
    + Kiểm tra máy khách và máy chủ SSL/TLS
    + Xử lý email đã ký hoặc mã hóa S/MIME
### 3. Chứng chỉ Cloudflare
- Cloudflare là dịch vụ DNS trung gian, giúp điều phối lượng truy cập giữa máy chủ và các client qua lớp bảo vệ CloudFlare. Hay nói một cách dễ hiểu thì thay vì bạn truy cập trực tiếp vào Website thông qua máy chủ phân giải tên miền DNS (Domain Name Server) thì bạn sẽ sử dụng máy chủ phân giải tên miền của CloudFlare. Các truy cập sẽ phải đi qua máy chủ của CloudFlare để xem dữ liệu website thay vì truy cập trực tiếp.

![q](https://f5-zpcloud.zdn.vn/6467156513868441785/4c3777688e7a43241a6b.jpg)

- Mục đích của CloudFlare:
    + Dừng các cuộc tấn công nhắm vào trang web.
    + Tự động sửa đổi nội dung để cải thiện hiệu suất.
    + Chèn ứng dụng vào các trang web.
    + Cung cấp phân tích phong phú về tất cả các yêu cầu cho trang web của bạn.
    + Tự động xác định đối tượng nào là tĩnh và có thể lưu vào bộ nhớ cache ở cạnh của mạng mà không có bất kỳ cấu hình người dùng nào.
    + Cung cấp cổng mạng giữa các giao thức như IPv6 \ IPv4.
    + Giúp cài đặt SSL linh hoạt và dễ dàng nhấp một lần.
    + Và nhiều thứ khác mà CDN truyền thống không thể cung cấp.
# II. So sánh SSL miễn phí và SSL mất phí

![q](https://f5-zpcloud.zdn.vn/8420823772557690212/7ece0e4f2552e80cb143.jpg)

### 1. Chi phí
- Từ tên gọi ta cũng đã nhận thấy sự khác biết giữa 2 loại SSL.
### 2. Tính an toàn
> Đối với những doanh nghiệp, cơ sở lớn như ngân hàng, kinh doanh thương mại điện tử, tổ chức chính phủ cần độ an toàn cao, việc sử dụng chứng chỉ SSL miễn phí không đảm bảo vì nó không thực hiện xác thực chủ thể doanh nghiệp, cơ sở, tổ chức sẽ dễ bị lợi dụng kiểu tân công giả mạo.
- **SSL miễn phí:** Cung cấp giấy chứng nhận giúp chưng minh bạn là người có quyền sở hưu tên miền đó. Nó không bao gồm bất kỳ các vấn đề bảo hành, bảo đảm, các vấn đề về lạm dụng hoặc gia hạn dịch vụ.
- **SSL mất phí:** Cung cấp chỉ cho tên miền đã xác thực bao gồm các vấn đề về bảo vệ bảo hành, bảo đảm về các vấn đề bảo mật hệ thống. Ngoài ra các thông tin cá nhân, doanh nghiệp, tên miền được thực hiện xác thực qua mail file hoặc DNS. Điều này làm cho việc sử dụng chứng chỉ SSL trên các hệ thống như email, tường lửa và cân bằng tải được cấu hình một cách dễ dàng.

![q](https://f5-zpcloud.zdn.vn/5044744018303327572/e5a31d3b3626fb78a237.jpg)

### 3. Cách thức sử dụng
- **SSL miễn phí**: Được cấp tự động, người dùng phải hiểu biết về lệnh trên máy chủ để thực hiện thao tác cài đặt.
- **SSL mất phí**: Đối với SSL có phí việc cấp pháp Certificate sẽ do CA cấp qua email đăng ký dịch vụ. Thời gian cấp phát có thể ngày lập tức cho đến 15 ngày làm việc tùy vào mức độ xác thực. Việc cài đặt SSL cũng sẽ được các nhà cung cấp , đại lý hỗ trợ miễn phí.
### 4. Tính liên kết
- **SSL miễn phí**: Với SSL miễn phí mỗi máy chủ khác nhau, người dùng phải tao tác lệnh tạo và cài đặt riêng.
- **SSL mất phí**: Với SSL mất phí bạn thể sử dụng chức năng sao chép Certicate cho các server khác nhau.

![q](https://f4-zpcloud.zdn.vn/4091564044413901181/54832f1f0402c95c9013.jpg)

### 5. Tính tập trung
- **SSL miễn phí**: Với chứng chỉ miễn phí người dùng phải tự quản lý với những SLL riêng biệt trên từng máy chủ. Điều này sẽ gây ra nhiều khó khăn hơn.
- **SSL mất phí**: Với SSL mất phí người dùng sẽ có giao diện tập trung cho việc quản lý các chứng chỉ.
### 6. Tính tương thích
- Mặc dù về hiện tại SSL miễn phí hầu hết các trình duyệt phổ biến như Chrome ,FireFox, Safari... Tuy nhiên đối với nhiều trường hợp đặt thù riêng thì SSL trả phí vẫn có cho mình những lợi thế hơn.
### 7. Hỗ trợ con dấu trang động

![q](https://f4-zpcloud.zdn.vn/3758139000331827644/2606d187fa9a37c46e8b.jpg)

- SSL miễn phí không cung cấp con dấu trang động.
- Các SSL mất phí đều cung cấp, con dấu này giúp khách hàng truy cập website có thể yên tâm và tin cậy hơn.
### 8. Chế độ bảo hiểm
- Vì được cung cấp miễn phí nên SSL miễn phí cũng không có được chế độ bảo hiểm, khi gặp sự cố bạn sẽ không được bồi thường như các hình thức SSL mất phí.
### 9. Độ tương thích với các ứng dụng khác

![q](https://f5-zpcloud.zdn.vn/7087411002118456273/3444b0de9bc3569d0fd2.jpg)

- **SSL miễn phí:** Hiện tại SSL miễn phí chỉ hỗ trợ cho Web service.
- **SSL mất phí:** Trong khi SSL mất phí có thể hỗ trợ cho các ứng dụng khác như: Email. Firewall, DNS, Loading Balancing,... rất dễ dàng.
### 10. Thời gian hiệu lực
- **SSL miễn phí:** Chỉ cung cấp tối đa 90 ngày, sau đó bạn cần phải gia hạn định kỳ.
- **SSL mất phí:**  Hỗ trợ thời hạn đăng ký lên đến 3 năm.
### 11. Hỗ trợ Wildcard SSL(chứng chỉ cho tên miền con)

![q](https://f5-zpcloud.zdn.vn/259769436576506660/540f889aa3876ed93796.jpg)

- SSL miễn phí không có Wildcard SSL cho sub-domain, bạn phải đăng ký chứng chỉ cho mỗi tên miền.
### 12. Khả năng hỗ trợ các định dạng tên miền quốc tế
- SSL miễn phí không hỗ trợ các tên miền với nhiều định dạng khác nhau như SSL có phí, ví dụ như trường hợp tên miền chẳng hạn.