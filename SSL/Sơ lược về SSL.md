# Tìm hiểu sơ lược về SSL
### 1. Khái niệm
- **SSL(Secure Sockets Layer)** là một tiêu chuẩn an ninh công nghệ toàn cầu tạo ra một liên kết giữa máy chủ web và trình duyệt. Liên kết này đảm bảo tất cả dữ liệu trao đổi giữa máy chủ web và trình duyệt luôn được bảo mật và an toàn.
- **SSL** đảm bảo rằng tất cả các dữ liệu được truyền giữa các máy chủ web và các trình duyệt được mang tính riêng tư, tách rời. SSL là một chuẩn công nghệ được sử dụng bởi hàng triệu trang web trong việc bảo vệ các giao dịch trực tuyến với khách hàng của họ.

![q](https://f5-zpcloud.zdn.vn/5256175433796277230/e0c3ef476650ab0ef241.jpg)

### 2. Các loại chứng chỉ SSL
- **Domain Validation (DV SSL)** : Chứng thư số SSL chứng thực cho Domain Name – Website. Khi 1 Website sử dụng DV SSL thì sẽ được xác thực tên domain, website đã được mã hoá an toàn khi trao đổi dữ liệu.
- **Organization Validation (OV SSL)**: Chứng thư số SSL chứng thực cho Website và xác thực doanh nghiệp đang sở hữu website đó .
- **Extended Validation (EV SSL)**: Cho khách hàng của bạn thấy Website đang sử dụng chứng thư SSL có độ bảo mật cao nhất và được rà soát pháp lý kỹ càng.
- **Subject Alternative Names (SANs SSL)**: Nhiều tên miền hợp nhất trong 1 chứng thư số:
    + Một chứng thư số SSL tiêu chuẩn chỉ bảo mật cho duy nhất một tên miền đã được kiểm định. Lựa chọn thêm SANs chỉ với chứng thư duy nhất bảo đảm cho nhiều tên miền con. SANs mang lại sự linh hoạt cho người sử dụng, dễ dàng hơn trong việc cài đặt, sử dụng và quản lý chứng thư số SSL. Ngoài ra, SANs có tính bảo mật cao hơn Wildcard SSL, đáp ứng chính xác yêu cầu an toàn đối với máy chủ và làm giảm tổng chi phí triển khai SSL tới tất cả các tên miền và máy chủ cần thiết.
    + Chứng thư số SSL SANs có thể tích hợp với tất cả các loại chứng thư số SSL của GlobalSign bao gồm: Chứng thực tên miền (DV SSL), Chứng thực tổ chức doanh nghiệp (OV SSL) và Chứng thực mở rộng cao cấp (EV SSL).
- **Wildcard SSL Certificate (Wildcard SSL)**: Sản phẩm lý tưởng dành cho các cổng thương mại điện tử. Mỗi e-store là một sub-domain và được chia sẻ trên một hoặc nhiều địa chỉ IP. Khi đó, để triển khai giải pháp bảo bảo mật giao dịch trực tuyến (đặt hàng, thanh toán, đăng ký & đăng nhập tài khoản,…) bằng SSL, chúng ta có thể dùng duy nhất một chứng chỉ số Wildcard cho tên miền chính của website và tất cả sub-domain.

![q](https://f4-zpcloud.zdn.vn/778643876543425640/99145b969d8150df0990.jpg)
### 3. Lợi ích khi sử dụng SSL
- Bảo mật và mã hóa các thông điệp trao đổi giữa trình duyệt và server.
- Bảo mật các giao dịch giữa khách hàng và doanh nghiệp, các dịch vụ truy nhập hệ thống.
- Bảo mật webmail và các ứng dụng như Outlook Web Acess, Exchange, và Office Communication Server.
- Bảo mật các ứng dụng ảo hóa như Citrix Delivery Platform hoặc các ứng dụng điện toán mây.
- Bảo mật dịch vụ FTP.
- Bảo mật truy cập Control panel
- Bảo mật các dịch vụ truyền dữ liệu trong mạng nội bộ, file sharing, extranet.
- Bảo mật VPN Access Servers, Citrix Access Gateway.
- Nâng cao hình ảnh, thương hiệu và uy tín doanh nghiệp
- Nâng cao thứ hạng website trên kết quả tìm kiếm Google (SEO)
- Tạo lợi thế cạnh tranh, tăng niềm tin của khách hàng đối với website, tăng số lượng giao dịch, giá trị giao dịch trực tuyến của khách hàng. Website không được xác thực và bảo mật sẽ luôn ẩn chứa nguy cơ bị xâm nhập dữ liệu, dẫn đến hậu quả khách hàng không tin tưởng sử dụng dịch vụ.

![q](https://f5-zpcloud.zdn.vn/8705296879558327101/028dbf164401895fd010.jpg)

### 4. Quy trình làm việc của SSL
- Công nghệ SSL bảo vệ những giao dịch trực tuyến và nâng cao mức độ tin cậy của website đối với khách hàng chỉ trong 3 bước cơ bản:
![q](https://f4-zpcloud.zdn.vn/6625921873769988653/4a512b31c2260f785637.jpg)

- Những gì xảy ra khi một máy tính kết nối với một Website đã được chứng thực ?
![q](https://f4-zpcloud.zdn.vn/1024486186225030773/c27d6d9f86884bd61299.jpg)

- Trình duyệt làm thế nào để kiểm tra một SSL là có thực hay không ?
    + Khi Website gửi cho trình duyệt một chứng chỉ SSL, trình duyệt sẽ gửi chứng chỉ này đến một máy chủ lưu trữ các chứng chỉ số đã được phê duyệt.
    + Về mặt kỹ thuật, SSL sử dụng mã hóa công khai. Kỹ thuật này giúp cho Website và trình duyệt tự thỏa thuận (bước 4 ở hình trên) một bộ khóa sẽ dùng trong suốt quá trình trao đổi thông tin sau đó. Bộ khóa sẽ thay đổi theo mỗi trong lần giao dịch kế tiếp, một người khác sẽ không thể giải mã ngay cả khi có được dữ liệu của máy chủ lưu trữ chứng chỉ số nói trên.
