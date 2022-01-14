# I. Xác minh tên miền (DV)
> Xác minh tên miền là phương pháp phát hành nhanh nhất trong các phương pháp xác nhận SSL và có sẵn cho khách hàng doanh nghiệp và các khách hàng cá nhân. Không có giấy tờ - vì nó không đòi hỏi tài liệu công ty hoặc doanh nghiệp cho một quá trình xác nhận, thậm chí không có gọi lại để xác nhận qua điện thoại. Quá trình xác nhận là rất đơn giản và dễ dàng, tất cả những gì bạn cần là trả lời tin nhắn tự động qua DCV(Domain Control Validation) sẽ được gửi đến mail của bạn.

![q](https://f5-zpcloud.zdn.vn/182556820872387385/0a72f98bf3973ec96786.jpg)

### 1. Phương pháp truyền thống
- Phương pháp thông qua DCV-Email: bạn sẽ nhận được một email xác nhận cho một tên miền của bạn. Các email sẽ chứa một mã xác nhận duy nhất và một liên kết.
- Địa chỉ email hợp lệ là: bất kỳ địa chỉ email mà hệ thống của chúng ta có thể tọa ra từ việc truy cập thông tin Whois của tên miền, các địa chỉ quản trị chung sau @tenmien đang được áp dụng là: admin@, administrator@, postmaster@, hostmaster@, webmaster@.
### 2. Phương thức thay thế DCV(Comodo)
- Http-based DCV: Các CSR bạn gửi đến comodo sẽ được phân tích. Các giá trị Hash được cung cấp cho bạn và bạn phải tạo một tập tin văn bản đơn giản và đặt trong thư mục gốc của website với giao thức http.
- DNS CName-based: Các CSR bản gửi đến comodo sẽ được phân tích. Các giá trị Hash được cung cấp cho bạn và bạn phải được nhập như một bản ghi DNS CName cho tên miền của bạn.
### 3. Phương pháp thay thế DCV khác
- HTTPS-based DCV: Các CSR bạn gửi đến comodo sẽ được phân tích. Các giá trị Hash được cung cấp cho bạn và bạn phải tạo một tập tin văn bản đơn giản và đặt trong các thư mục gốc của website và giao thức HTTPS.
# II. Xác minh doanh nghiệp
- Xác minh doanh nghiệp(Business Validation) yêu cầu xác nhận Email qua tên miền.