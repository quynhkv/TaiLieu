# Cài đặt IIS cho windows
> Có 3 cách để cài đặt và thiết lập trang web trong IIS trên Windows 10; sử dụng giao diện người dùng đồ họa (GUI), PowerShell hoặc Windows CMD.
### 1. Cài đặt IIS bằng GUI
- **Bước 1**: Tìm kiếm Turn Windows features on or off trên thanh search và click vào.
- Cửa sổ Windows Features sẽ mở. Có thể mất một chút thời gian để các tính năng khác load. Khi đã xong, nhấp vào hộp kiểm bên cạnh Internet Information Services, sau đó click vào nút OK.
![q](https://f4-zpcloud.zdn.vn/6788347401038102374/8319d90d1f73d22d8b62.jpg)
- Việc cài đặt sẽ bắt đầu và có thể mất vài phút. Sau khi hoàn thành, hãy nhấp vào nút Close.
- Để đảm bảo IIS được cài đặt và hoạt động, hãy nhập IIS vào thanh Search gần nút Start. Kết quả là bạn sẽ thấy Internet Information Services Manager. Nhấn vào đó để mở.
- Khi IIS Manager mở, hãy nhìn vào bên trái cửa sổ trong phần Connections. Mở rộng menu dạng cây cho đến khi bạn thấy Default Web Site. Đó là một trang web giữ chỗ được cài đặt với IIS. Nhấn vào nó để chọn.
> ![q](https://f4-zpcloud.zdn.vn/4569966086237369809/cf322927ef5922077b48.jpg)
- Ở bên phải của IIS Manager, hãy xem phần Browse Website. Nhấp vào Browse *:80 (http). Trang web mặc định sẽ mở trong trình duyệt web mặc định.
> ![q](https://f5-zpcloud.zdn.vn/8300147375980414706/13fca3ef6591a8cff180.jpg)
- Bạn sẽ thấy một trang web như sau. Lưu ý thanh địa chỉ có nội dung localhost. Đó là địa chỉ để nhập vào trang web mới.
> ![q](https://f5-zpcloud.zdn.vn/8515950069616078062/465dfe4d3833f56dac22.jpg)
 