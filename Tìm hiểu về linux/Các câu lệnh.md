# CÁC CÂU LỆNH CƠ BẢN TRONG LINUX
### 1. pwd
- Dùng để tìm đường dẫn của thư mục hiện tại (folder) mà bạn đang ở trong đó.
![m](https://f4-zpcloud.zdn.vn/8100952652820938003/063c12f611abdbf582ba.jpg)
### 2. cd
- Dùng để chuyển hướng trong hệ thống tập tin Linux, nó sẽ cần nhập đường dẫn đầy đủ hoặc tên thư mục bạn muốn chuyển tới.
- ![m](https://f4-zpcloud.zdn.vn/4605086188260149051/fbc00f050c58c6069f49.jpg)
    + **cd ..** (với 2 chấm) để chuyển lên 1 cấp thư mục trên.
    + **cd** để tới thẳng thư mục home.
    + **cd-** (với dấu gạch ngang) để chuyển tới thư mục bạn đã ở trước đó.
### 3. ls
- Được dùng để xem nội dung thư mục.
![m](https://f4-zpcloud.zdn.vn/2208872976231106966/43b26776642bae75f73a.jpg)
    + **ls -R** liệt kê các file bao gồm cả các thư mục phụ bên trong.
    + **ls -a** liệt kê những file ẩn.
    + **ls -al** liệt kê tất cả file và thư mục với thông tin chi tiết như phân quyền, kích thước, chủ sở hữu,..
### 4. cat
- Dùng để xem nội dung file trên output tiêu chuẩn (sdout).
    + **cat > filename** tạo ra file mới.
    + **cat > filename1 filename2>filename3** nhập file (1 và 2) để lưu kết quả vào file (3)
    + **cat filename | tr a-z A-Z >output.txt** để chuyển một file từ in thường tới in hoa hoặc ngược lại.
### 5. cp
- Dùng để sao chép files từ thư mục hiện tại.
![m](https://f5-zpcloud.zdn.vn/5722061442954138873/bebb597d5a20907ec931.jpg)
### 6. mv
- Dùng để di chuyển files, nó cũng có thể được dùng để đổi tên files.
![m](https://f4-zpcloud.zdn.vn/7612573747768433713/a0cb860b85564f081647.jpg)
### 7. mkdir
- Được dùng để tạo thư mục mới.
![m](https://f5-zpcloud.zdn.vn/4194693871794072623/d5ce220d2150eb0eb241.jpg)
    + Để tạo một thư mục mới trong thư mục khác sử dụng lệnh: **mkdir Music/Newfile**
    + Sử dụng **p** (parents) option để tạo thư mục giữa 2 thư mục đã tồn tại. Ví dụ: **mkdir -p Music/2020/Newfile** sẽ tạo thư mục **2020**
### 8. rmdir
- Dùng để xóa các thư mục trống.
![m](https://f5-zpcloud.zdn.vn/2027699989675590933/0d6490b893e559bb00f4.jpg)
### 9. rm
- Được sử dụng để xóa thư mục cùng nội dung bên trong.
![m](https://f5-zpcloud.zdn.vn/7590369046740161095/396bccb4cfe905b75cf8.jpg)
> Khi dùng lệnh này bạn nên chú  ý xem mình đang ở thư mục nào vì nó sẽ xóa mọi thứ và không khôi phục được.
### 10. touch
- Cho phép bạn tạo files mới trống thông qua dòng lệnh.
![m](https://f4-zpcloud.zdn.vn/1555418389606324867/d33cfbe4f8b932e76ba8.jpg)
### 11. locate
- Dùng để định vị - tìm kiếm file.
![m](https://f5-zpcloud.zdn.vn/42686488538562839/1e78f9acfaf130af69e0.jpg)
### 12. find
- Tương tự như **locate**, **find** cũng dùng để tìm file. Sự khác biệt là bạn sử dụng **find** để xác định vị trí files trong thư mục nhất định.
![m](https://f5-zpcloud.zdn.vn/6599963598545749244/8c5e1f8f1cd2d68c8fc3.jpg)
### 13. grep
- Cho phép bạn tìm kiếm tất cả text thông qua tập tin nhất định.
![m](https://f5-zpcloud.zdn.vn/1905867260115152914/282a5bc5589892c6cb89.jpg)
### 14. sudo
- **sudo(SuperUser Do)** cho phép bạn thực hiện các tác vụ yêu cầu quyền quản trị hoặc quyền root.
### 15. df
- dùng để nhận báo cáo về dung lượng lưu trữ được sử dụng trên hệ thống, hiển thị theo tỷ lệ phần trăm và KBs.
![m](https://f5-zpcloud.zdn.vn/8540824310813962814/82bfd951da0c1052491d.jpg)
### 16. du
- **du(Disk Usage – Dung lượng lưu trữ)** dùng để kiểm tra dung lượng của file hoặc của thư mục.
![m](https://f5-zpcloud.zdn.vn/7436272170613914639/203721df2282e8dcb193.jpg)
### 17. head
- được sử dụng để xem dòng đầu tiên của bất kỳ file văn bản nào. Theo mặc định, nó sẽ hiển thị 10 dòng đầu tiên, nhưng bạn có thể thay đổi số này theo ý mình.
![m](https://f5-zpcloud.zdn.vn/4004448589519904147/e4da513e5263983dc172.jpg)
### 18. tail
- có chức năng tương tự như lệnh head, nhưng thay vì hiển thị dòng đầu tiên, tail sẽ hiển thị 10 dòng cuối cùng của file văn bản.
![m](https://f4-zpcloud.zdn.vn/9075454013033382939/b052a4b1a7ec6db234fd.jpg)
### 19. diff
- diff(difference) sẽ so sánh nội dung của 2 files từng dòng một. Sau khi phân tích files này, nó sẽ xuất ra các dòng không khớp nhau. Lập trình viên thường dùng lệnh này khi cần thực hiện một số thay đổi chương trình thay vì viết lại toàn bộ mã nguồn.
![m](https://f4-zpcloud.zdn.vn/2601118084299147728/a3e56f196c44a61aff55.jpg)
### 20. tar
- là lệnh được sử dụng rộng rãi nhất để lưu trữ nhiều file vào tarball – một định dạng file Linux phổ biến tương tự định dạng zip, nhưng nén file thì tùy.
![m](https://f5-zpcloud.zdn.vn/281202391252565444/4fa2165c1501df5f8610.jpg)
### 21. chmod
- là một lệnh thiết yếu khác, dùng để thay đổi quyền đọc, ghi và quyền thực thi files và thư mục.
![m](https://f4-zpcloud.zdn.vn/5720224590774286714/86b63e483d15f74bae04.jpg)
### 22. chown
- Trong Linux, tất cả files được sở hữu bởi một người dùng cụ thể. chown cho phép bạn thay đổi hoặc chuyển quyền sở hữu file sang tên người dùng được chỉ định.
![m](https://f5-zpcloud.zdn.vn/3466524365326914057/7b1fb8e7bbba71e428ab.jpg)
### 23. jobs
- sẽ hiển thị tất cả jobs hiện tại và trạng thái jobs. Job cơ bản là một tiến trình được tạo bởi shell.
![m](https://f4-zpcloud.zdn.vn/7989956294821978348/c66308940bc9c19798d8.jpg)
### 24. kill
- Nếu có chương trình nào đó không phản hồi, bạn có thể chấm dứt chương trình thủ công bằng cách sử dụng lệnh kill. Nó sẽ gửi tín hiệu nhất định đến những ứng dụng đang hoạt động sai và hướng ứng dụng tự chấm dứt.
![m](https://f5-zpcloud.zdn.vn/4203354673847805332/32fbc0f6c4ab0ef557ba.jpg)
### 25. ping
- dùng để kiểm tra trạng thái kết nối của bạn với server.
![m](https://f4-zpcloud.zdn.vn/3928512180848430933/587d5d7459299377ca38.jpg)
### 26. wget
- Với lệnh **wget** bạn có thể tải file từ internet xuống, chỉ cần gõ wget đằng trước link muốn tải.
![m](https://f4-zpcloud.zdn.vn/7416246627106827296/03656062643fae61f72e.jpg)
### 27. uname
- **uname(Unix Name)** sẽ in thông tin chi tiết về hệ thống Linux của bạn như tên máy, hệ điều hành, kernel, v.v.
![m](https://f5-zpcloud.zdn.vn/3858880686383864177/51e16fe76bbaa1e4f8ab.jpg)
### 28. top
-  **top** sẽ hiển thị danh sách tiến trình đang chạy và lượng CPU mà tiến trình đó sử dụng. Rất có ích khi bạn giám sát dung lượng lưu trữ tài nguyên trên hệ thống, đặc biệt là biết được quá trình nào cần chấm dứt vì tiêu thụ quá nhiều tài nguyên.
![m](https://f5-zpcloud.zdn.vn/1243612273444684129/3b3e773d7360b93ee071.jpg)
### 29. history
- **history** giúp bạn xem những lệnh đã nhập trước đó.
- ![m](https://f4-zpcloud.zdn.vn/15303271308373703/393ed422d07f1a21436e.jpg)
### 30. man
- **man** giúp bạn học cách sử dụng các lệnh. Ví dụ: nhập man tail sẽ hiển thị hướng dẫn thủ công của lệnh **tail**.
- ![m](https://f5-zpcloud.zdn.vn/2601708202899068061/a71ef500f15d3b03624c.jpg)
### 31. echo
- được dùng để chuyển dữ liệu vào một file.
![m](https://f5-zpcloud.zdn.vn/3000395079118480649/07d45bcf5f9295cccc83.jpg)
### 32. zip,unzip
- Sử dụng lệnh zip để nén file thành zip archive và lệnh unzip để giải nén file zipped trong zip archive.
### 33. hostname
- **hostname** giúp bạn biết tên của một máy / mạng máy tính. Thêm option -i vào cuối file để hiển thị địa chỉ IP address của network bạn.
- ![m](https://f5-zpcloud.zdn.vn/6717605746667759119/d6d19cc4989952c70b88.jpg)
### 34. useradd, userdel, passwd
- **useradd** được dùng để tạo user mới, còn **passwd** đặt mật khẩu cho một tài khoản user. Để thêm user có tên Quynh, **useradd Quynh** rồi thiết lập password bằng lệnh **passwd 123456789**.
![m](https://f4-zpcloud.zdn.vn/5174858334742276214/8f0e0e1a0a47c0199956.jpg)
- Để xóa user account, nhập lệnh **userdel UserName**.