# Tối ưu WordPress
### 1. Chia tỷ lệ hình ảnh (Tùy chọn).
- Trong WordPress, bạn có thể chèn hình ảnh có kích thước nhỏ hơn dựa theo các kích thước sẵn có.

![q](https://f5-zpcloud.zdn.vn/7082416058608604148/1ccb2ced272dea73b33c.jpg)

### 2. Tối ưu hình ảnh WordPress với Smush.
- Ta có thể cài đặt và kích hoạt WP Smush đẻ tối ưu hóa và nén hình ảnh cho website WordPress.

![q](https://f5-zpcloud.zdn.vn/6013540339477389967/7f09b4bbb07b7d25246a.jpg)

### 3. Cài đặt và kích hoạt wp fastest cache.
- Ta vào mục Plugins chọn add new sau đó tìm và cài đặt wp fastest cache, sau khi cài đặt thì active nó.
- Sau đó ta click vào wp fastest cache vừa cài đặt.

![q](https://f5-zpcloud.zdn.vn/6776890799986982953/c9be1e4b328bffd5a69a.jpg)

- Kích hoạt một số cài đặt sau.

![q](https://f5-zpcloud.zdn.vn/2912797876382796084/e5c202372ef7e3a9bae6.jpg)

### 4. Một số Cache tối ưu phổ biến nhất.
- WP Rocket – Cache WordPress Plugin
- Comet Cache – WordPress Plugin
- Powered Cache
- Fresh Performance Cache 
- Borlabs Cache – WordPress Caching Plugin
- W3 Total Cache
- WP Super Cache
- Cache Enabler

### 5. Một số chú ý quan trọng khi tối ưu website WordPress.
- Giảm thiểu và kết hợp HTML / CSS / JavaScript có thể phá vỡ chức năng trong website.
    + Việc thu nhỏ về cơ bản thông qua các tập lệnh sẽ loại bỏ dữ liệu không liên quan như nhận xét, định dạng, khoảng trắng và những thứ khác mà máy tính không cần đọc. Việc kết hợp sẽ lấy nội dung của từng tập lệnh riêng lẻ và tổng hợp tất cả chúng thành một tập lệnh duy nhất.

    + Bởi vì các quy trình này sửa đổi dữ liệu, đôi khi chúng phá vỡ chức năng do lỗi chính tả, lỗi cú pháp, tên hàm trùng lặp, v.v.

    + Đảm bảo kiểm tra chức năng website của bạn sau khi bật các tính năng thu nhỏ / kết hợp. Nếu bạn thấy mọi thứ bị hỏng, hãy tắt tất cả các tính năng thu nhỏ / kết hợp và bật lại từng cái một để tìm ra tính năng nào gây ra sự cố.

    + Nếu môi trường lưu trữ của bạn hỗ trợ HTTP / 2, thì không cần kết hợp các tập lệnh, vì giao thức HTTP / 2 hỗ trợ ghép kênh – về cơ bản cho phép nhiều lượt tải xuống bằng một kết nối TCP (chỉ có 6 kết nối song song trong HTTP / 1.x.)
- Trang bộ nhớ đệm.
    + Bất cứ khi nào bạn thực hiện các thay đổi lớn cho trang web, như thêm plugin hoặc sửa đổi CSS / theme, bạn nên xóa bộ đệm và tải lại nó một lần nữa để đảm bảo website sẽ hiển thị phiên bản mới nhất. Bạn có thể tìm thấy tùy chọn xóa bộ nhớ cache trong WP Fastest Cache trong tab “Delete Cache”.
    + WP Fastest Cache sẽ tự động tải lại bộ đệm một lần nữa sau khi bạn xóa nó.
