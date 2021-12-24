# DNS VÀ CÁC BẢN GHI THƯỜNG ĐƯỢC SỬ DỤNG
> ![q](https://f5-zpcloud.zdn.vn/8288592350514319659/f97feea2d5941fca4685.jpg)
### 1. Khái niệm
- **DNS** là viết tắt của cụm từ Domain Name System, mang ý nghĩa đầy đủ là hệ thống phân giải tên miền. Hiểu một cách ngắn gọn nhất, DNS cơ bản là một hệ thống chuyển đổi các tên miền website mà chúng ta đang sử dụng, ở dạng www.tenmien.com sang một địa chỉ IP dạng số tương ứng với tên miền đó và ngược lại.
> ![q](https://f5-zpcloud.zdn.vn/4342288213932945007/648d3f570461ce3f9770.jpg)
### 2. Chức năng của DNS
- **DNS** có thể được hiểu như một “người phiên dịch” và “truyền đạt thông tin”. DNS sẽ làm công việc dịch tên miền thành một địa chỉ IP gồm 4 nhóm số khác nhau. Ví dụ như www.tenmien.com thành 421.64.874.899 hoặc ngược lại dịch một địa chỉ IP thành tên miền.
> ![q](https://f5-zpcloud.zdn.vn/6521124928288416144/3161bbba808c4ad2139d.jpg)
### 3. Các loại bản ghi DNS
- **CNAME Record(Bản ghi CNAME)**: Cho phép bạn tạo một tên mới, điều chỉnh trỏ tới tên gốc và đặt TTL. Tóm lại, tên miền chính muốn đặt một hoặc nhiều tên khác thì cần có bản ghi này.
- **A Record**: Bản ghi này được sử dụng phổ biến để trỏ tên Website tới một địa chỉ IP cụ thể. Đây là bản ghi DNS đơn giản nhất, cho phép bạn thêm Time to Live (thời gian tự động tái lại bản ghi), một tên mới và Points To ( Trỏ tới IP nào).
- **MX Record**: Với bản ghi này, bạn có thể trỏ Domain đến Mail Server, đặt TTL, mức độ ưu tiên (Priority). MX Record chỉ định Server nào quản lý các dịch vụ Email của tên miền đó.
- **AAAA Record**: Để trỏ tên miền đến một địa chỉ IPV6 Address, bạn sẽ cần sử dụng AAA Record. Nod cho phép bạn thêm Host mới, TTL,IPv6.
- **TXT Record**: Bạn cũng có thể thêm giá trị TXT, Host mới, Points To, TTL. Để chứa các thông tin định dạng văn bản của Domain, bạn sẽ cần đến bản ghi này.
- **SRV Record**: Là bản ghi dùng để xác định chính xác dịch vụ nào chạy Port nào. Đay là Record đặc biệt trong DNS. Thông qua nó, bạn có thể thêm Name, Priority, Port, Weight, Points to, TTL.
- **NS Record**: Với bản ghi này, bạn có thể chỉ định Name Server cho từng Domain phụ. Bạn có thể tạo tên Name Server, Host mới, TTL.
### 4. Các loại DNS Server
- **Root Name Server**:
    + Là máy chủ tên miền chứa các thông tin, để tìm kiếm các máy chủ tên miền lưu trữ (authority) cho các tên miền thuộc mức cao nhất (top-level-domain).
    + Máy chủ ROOT có thể đưa ra các truy vấn (query) để tìm kiếm tối thiểu các thông tin về địa chỉ của các máy chủ tên miền authority thuộc lớp top-level-domain chứa tên miền muốn tìm.
    + Quá trình tìm kiếm tên miền luôn được bắt đầu bằng các truy vấn gửi cho máy chủ ROOT. Nếu như các máy chủ tên miền ở mức ROOT không hoạt động, quá trình tìm kiếm này sẽ không được thực hiện.
> ![q](https://f5-zpcloud.zdn.vn/8371436728242721181/e10ec8d7f3e139bf60f0.jpg)
- **Local Name Server**:
    + Server này chứa thông tin, để tìm kiếm máy chủ tên miền lưu trữ cho các tên miền thấp hơn. Nó thường được duy trì bởi các doanh nghiệp, các nhà cung cấp dịch vụ Internet (ISPs).
> ![q](https://f5-zpcloud.zdn.vn/2566830044143235308/20bdb31b882d42731b3c.jpg)
### 5. Cơ chế hoạt động của DNS
- Giả sử bạn muốn truy cập vào trang có địa chỉ quynhkv.vn
- Trước hết chương trình trên máy người sử dụng gửi yêu cầu tìm kiếm địa chỉ IP ứng với tên miền quynhkv.vn tới máy chủ quản lý tên miền (name server) cục bộ thuộc mạng của nó.
- Máy chủ tên miền cục bộ này kiểm tra trong cơ sở dữ liệu của nó có chứa cơ sở dữ liệu chuyển đổi từ tên miền sang địa chỉ IP của tên miền mà người sử dụng yêu cầu không. Trong trường hợp máy chủ tên miền cục bộ có cơ sở dữ liệu này, nó sẽ gửi trả lại địa chỉ IP của máy có tên miền nói trên.
- Trong trường hợp máy chủ tên miền cục bộ không có cơ sở dữ liệu về tên miền này nó sẽ hỏi lên các máy chủ tên miền ở mức cao nhất (máy chủ tên miền làm việc ở mức ROOT). Máy chủ tên miền ở mức ROOT này sẽ chỉ cho máy chủ tên miền cục bộ địa chỉ của máy chủ tên miền quản lý các tên miền có đuôi .vn.
- Tiếp đó, máy chủ tên miền cục bộ gửi yêu cầu đến máy chủ quản lý tên miền Việt Nam (.VN) tìm tên miền quynhkv.vn.
- Máy chủ tên miền cục bộ sẽ hỏi máy chủ quản lý tên miền vnn.vn địa chỉ IP của tên miền quynhkv.vn. Do máy chủ quản lý tên miền vnn.vn có cơ sở dữ liệu về tên miền quynhkv.vn nên địa chỉ IP của tên miền này sẽ được gửi trả lại cho máy chủ tên miền cục bộ.
- Cuối cùng, máy chủ tên miền cục bộ chuyển thông tin tìm được đến máy của người sử dụng. Người sử dụng dùng địa chỉ IP này để kết nối đến server chứa trang web có địa chỉ quynhkv.vn.
> ![q](https://f5-zpcloud.zdn.vn/6259437679394187575/37b8741f4f298577dc38.jpg)
### 6. Nguyên tắc làm việc của DNS
- Mỗi nhà cung cấp dịch vụ vận hành và duy trì DNS server riêng của mình, gồm các máy bên trong phần riêng của mỗi nhà cung cấp dịch vụ đó trong Internet.
- Tức là, nếu một trình duyệt tìm kiếm địa chỉ của một website bất kỳ thì DNS server phân giải tên website này phải là DNS server của chính tổ chức quản lý website đó chứ không phải là của một tổ chức (nhà cung cấp dịch vụ) nào khác.
- INTERNIC (Internet Network Information Center) chịu trách nhiệm theo dõi các tên miền và các DNS server tương ứng. INTERNIC là một tổ chức được thành lập bởi NFS (National Science Foundation), AT&T và Network Solution, chịu trách nhiệm đăng ký các tên miền của Internet. INTERNIC chỉ có nhiệm vụ quản lý tất cả các DNS server trên Internet chứ không có nhiệm vụ phân giải tên cho từng địa chỉ.
- DNS có khả năng tra vấn các DNS server khác để có được một cái tên đã được phân giải. DNS server của mỗi tên miền thường có hai việc khác biệt.
    + Chịu trách nhiệm phân giải tên từ các máy bên trong miền về các địa chỉ Internet, cả bên trong lẫn bên ngoài miền nó quản lý.
    + Chúng trả lời các DNS server bên ngoài đang cố gắng phân giải những cái tên bên trong miền nó quản lý. DNS server có khả năng ghi nhớ lại những tên vừa phân giải. Để dùng cho những yêu cầu phân giải lần sau. Số lượng những tên phân giải được lưu lại tùy thuộc vào quy mô của từng DNS.
### 7. Một số DNS phổ biến nhất hiện nay
- **DNS Google**
- **DNS OpenDNS**
- **DNS Cloudflare**
- **DNS VNPT**
- **DNS Viettel**
- **DNS FPT**
