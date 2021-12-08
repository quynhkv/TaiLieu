# Chương 1: GIỚI THIỆU CHUNG
## 1.1 *MẠNG TRUYỀN THÔNG VÀ CÔNG NGHỆ MẠNG*
### 1.1.1 **Giới thiệu chung**
- **Truyền thông máy tính (computer communications)** là quá trình truyền dữ liệu từ thiết bị này sang thiết bị khác.
- **An ninh (security)**: đảm bảo an toàn hoặc bảo vệ tất cả các thành phần của mạng.
- **Chuẩn (standard)**: thiết lập các quy tắc và luật lệ cụ thể cần phải tuân theo.
### 1.1.2 *Mạng máy tính*
- Mạng máy tính bao gồm nhiều thành phần, các thành phần được nối với nhau theo một cách thức nào đó và cùng sủa dụng chung một ngôn ngữ:
    + **Các thiết bị đầu cuối (en system)**: kết nối với nhau tạo thành mạng có thể là các máy tính (computer) hoặc các thiết bị khác.
    + **Môi trường truyền thông(media)**: thực hiện việc dẫn các tín hiệu vật lý, môi trường truyền thông mạng được chia thành 2 loại: cáp(cable) và không dây(wireless).
    + **Giao thức(protocol)**: là quy tắc quy định cách thức trao đổi dữ liệu giữa các thực thể.
### 1.1.3 *Phân loại mạng máy tính*
* **Phân loại mạng theo diện hoạt động:**
    - **Mạng cục bộ(Local Area Network - LAN)**: liên kết các tài nguyên máy tính trong một khu vực địa lý có kích thước hạn chế.
    - **Mạng diện rộng(Wide Area Network - WAN)**: kết hợp giữa nhiều mạng LAN qua các router trong một vùng đại lý rộng như thị xã, thành phố , tỉnh/bang, quốc gia.
    - **Mạng toàn cầu(Global Area Network - GAN)**: là mạng của các mạng WAN, trải rộng trên phạm vi toàn cầu.
    - **Mạng dô thị(Metropolitan Area Network - MAN)**: kết hợp nhiều mạng LAN trong 1 khu vực địa lý.
    - **Mạng cá nhân(Personal Area Network - PAN)**: chỉ mạng máy tính nhỏ sư dụng trong gia đình.
    - **Mạng lưu trữ(Storage Area Network - SAN)**
* **Phân loại theo mô hình ghép nối:**
    - Một cách khác để phân loại mạng là theo topo - mô hình ghép nối mạng hay còn gọi là hình trạng mạng.
* **Mô hình điêm-điểm(point-to-point)**
    - **ạng point-to-point**: gồm nhiều nút , mỗi nút chỉ có thể liên lạc với nút liền kề qua đường liên kết trực tiếp .
    - **Mạng hình sao(Star)**: đặc điểm chính của mạng hình sao là có 1 hub xử lý trung tâm -hub này là trung tâm truyền tin cho tất cả các nút.
    - **Mô hình cây(Tree)**: mô hình cây là mô hình phân cấp , gồm một nút gốc hoặc hub nối đến các nút mức 2 hoặc hub mức 2 rồi mức 3 mức 4....
    - **Mô hình điểm- nhiều điểm(Broadcast)**: mô hình này gồm các nút dung chung một kênh truyền thông.
    - **Bus**
    - **Ring**
    - **Vệ tinh**
* **Phân loại theo kiểu chuyển**
   > Ngoài việc phân loại theo diện hoạt động và topo, mạng còn được phân loại theo kiểu truyền thông mà chúng sử dụng , cùng với cách dữ liệu  được truyền đi. Hai phân loại điển hình là mạng chuyển mạch ảo(virtual circuit-switched) và mạng chuyển gói (packet-switched).
    - Trong mạch chuyển ảo(circuit-switched), phải thiết lập mạch vật lý giữa nút nguồn và đích trước khi di chuyển dữ liệu thực sự.
    - Trong mạng chuyển goi(packet-switched network), thông điệp đầu tiền được chia thành những đơn vị nhỏ gọn hơn gọ là gói (packet), sau những packet lần lượt được gửi tới nút nhận qua mạng lưới các thiết bị chuyển mạch trung gian (switch).
### 1.1.4 *Địa chỉ mạng , định tuyến, tính tin cậy, tính liên tác và an ninh mạng*
 > Khái niệm mạng máy tính liên quan đến nhiều yếu tố , trong đó có đại chỉ, định tuyến, tính tin cậy, tính liên tác và an ninh mạng. 
 - **Địa chỉ (Address)**
     + Khái niệm địa chỉ liên quan đến việc gán cho mỗi nút mạng một địa chỉ duy nhất - cho phép các thiết bị khác định vị được nó.
 - **Routing - Định tuyến**
     + Định tuyến xác định tuyến đường mà dữ liệu sẽ đi qua trong quá trình chuyển từ nút nhận đến nút gửi.
 - **Tính tin cậy**
     + Tính tin cậy chỉ tính toàn vẹn dữ liệu - đảm bảo dữ liệu nhận được giống hệt dữ liệu gửi đi.
 - **Tính liên tác(interoperability)**
     + Chỉ khả năng các sản phẩm (phần cứng và phần mềm) của các hãng sản xuất khác nhau có thể giao tiếp được với nhau trong mạng.
 - **An ninh**
     + Chỉ việc bảo vệ mọi thứ trong mạng, bao gồm dữ liệu, phương tiện truyền thông và các thiết bị.
### 1.1.5 *Chuẩn mạng*
> Chuẩn mạng định nghĩa các giao tiếp phần cứng, giao tiếp truyền thông, kiến trúc mạng... Chuẩn mạng thiết lập những quy tắc hay các quy ước cụ thể mà các bên tham gia truyên thông cần tuân thủ.
- **Chuẩn chính thức(De jure standard)**
   + Chuẩn chính thực được công nhận bởi tổ chức chuẩn hóa chuyên nghiệp.
- **Chuẩn thực tế(De facto standard)**
   + Chuẩn thực tế là chuẩn tồn tại trong thực tế chứ không phải do các tổ chức chuẩn hóa xậy dụng nên. Chúng được phát triển thông qua sự chấp nhận của toàn ngành đối với chuẩn nào đó của một hãng nhà snar xuất cụ thể.
- **Chuẩn riêng của hãng**
   + Chuẩn của hãng quy định những yêu cầu cụ thể của một nhà sản xuất nào đó.
- **Chuẩn hiệp hội**
   + Chuẩn hiệp hội tương tự như chuẩn chính thức theo nghĩa chúng là sản phẩm của quá trình chuẩn hóa.
## 1.2 *MÔ HÌNH OSI*
    Tổ chức ISO (International Standards Organization) được thành lập năm 1971 với mục đích xậy dựng các tiêu chuẩn quốc tế.
### 1.2.1 *Mô hình*
> Mô hình OSI được phân tầng với mục đích thiết kế các hệ thống mạng cho phép tất cả các kiểu hệ thống máy tính khác nhau có thể truyền thông với nhau. Mô hình có 7 tầng riêng biệt nhưng có liên quan đến nhau, mỗi tầng định nghĩa một phần của quá trình truyền thông tin trên mạng.
* **Kiến trúc phân tầng**
    - ***Mô hình OSI gồm 7 tầng***
        + *Tầng vật lý (Physical layer)*
        + *Tầng liên kết dữ liệu (Datalink layer)*
        + *Tầng mạng (Network layer)*
        + *Tầng giao vận (Transport layer)*
        + *Tầng phiên (Session layer)*
        + *Tầng trình diễn (Presentation layer)*
        + *Tầng ứng dụng (Application layer)*
* **Các tiến trình ngang hàng(peer-to-peer)**
    - Tại thiết bị đầu cuối, mỗi tầng sử dụng các dịch vụ do tầng bên dưới cung cấp.
* **Giao diện giữa các tầng**
    - Trên cùng một máy tính, hai tầng kề nhau trao đổi dữ liệu với nhau qua các giao diện (interface). Giao diện định nghĩa cách thức và khuôn dạng dữ liệu trao đổi giữa hai tầng kề nhau trên cùng một thiết bị. Định nghĩa giao diện giữa các tầng một cách rõ ràng cho phép thay đổi cách thức triển khai tại một tầng mà không ảnh hưởng đến các tầng khác.
* **Chức năng các tầng**
    - *Tầng vật lý (Physical layer)*: Tầng vật lí thực hiện các chức năng cần thiết để truyền luồng bit dữ liệu đi qua môi trường vật lý. Nó giải quyết những vấn đề liên quan đến đặc điểm kỹ thuật về cơ và điện giữa card ghép nối (interface) với môi trường truyền dẫn. Nó cũng xác định các thủ tục, chức năng mà thiết bị vật lý và thiết bị giao tiếp cần phải tuân thủ.
    - *Tầng vật lý liên quan đến*:
        + Đặc điểm vật lý của môi trường(thiết bị) giao tiếp và truyền thông.
        + Biểu diễn bit.
        + Tốc độ dữ liệu.
        + Đồng bộ hóa cá bit.
        + Cấu hình đường truyền.
        + Topo(Mô hình ghép nối)vật lý.
        + Chế độ truyền dẫn.
    - *Tầng liên kết dữ liệu (Datalink layer)*: Nhiệm vụ cảu tầng liên kết dữ liệu là truyền thông giữa 2 nút nối trực tiếp với nhau. Nó biến tầng vật lý không tin cậy thành đường truyền tin cậy cho tầng mạng bên trên.
    - *Tầng liên kết chịu trách nhiệm*:
        + Framing - Đóng gói dữ liệu
        + Định địa chỉ vật lý
        + Kiểm soát lưu lượng
        + Kiểm soát lỗi
        + Kiểm soát truy cập
    - *Tầng mạng (Network layer)*: Tầng mạng chịu trách nhiệm chuyển gói dữ liệu từ nơi nhận, gói dữ liệu có thể phải đi qua nhiều mạng (các chặng trung gian). Tầng liên kết giữ liệu thực hiện truyền gói dữ liệu giữa hai thiết bị trong cùng một mạng, còn tầng mạng đảm bảo gói dữ liệu sẽ được chuyển từ nơi gửi đến đúng nơi nhận. Nếu 2 thiết bị nằm trên cùng một môi trường truyền thì rõ ràng không cần mạng. Tuy nhiên, nếu 2 thiết bị ở trên 2 mạng khác nhau, và giữa chúng có nhiều thiết bị kết nối trung gian thì cần phải có tầng mạng để thực hiện việc chuyển giữ liệu từ nguồn đến đích.
    - *Tầng mạng có nhiệm vụ*:
        + Định địa chỉ logic
        + Định tuyến
    - *Tầng giao vận (Transport layer)*: Tầng giao vận chịu trách nhiệm chuyển toàn bộ thông điệp từ nơi gửi đến nơi nhận. Tầng mạng chuyển từng gói dữ liệu riêng lẻ từ nơi gửi đến nơi nhận mà không quan tâm đến quan hệ giữa các gói dữ liệu. Tầng mạng xử lý mỗi gói dữ liệu một cách độc lập mà không quan tâm các gói có thuộc vào cùng một thông điệp hay không. Nói cách khác, tầng giao vận đảm bảo gửi thông điệp đến nơi nhận 1 cách toàn vẹn.
    - *Tầng giao vận chịu trách nhiệm*:
        + Địa chỉ cổng(port number)
        + Phân mảnh và tái hợp nhất
        + Kiểm soát kết nối
        + Kiểm soát lưu lượng
        + Kiểm soát lỗi
    - *Tầng phiên (Session layer)*: Các dịch vụ của 3 tầng đầu chưa đủ để 2 tiến trình trên 2 thiết bị có thể truyền thông. Tầng phiên đóng vai trò "kiểm soát viên" họi thoại(dialog) của mạng với nhiệm vụ thiết lập, duy trì và đồng bộ hóa tính liên lạc giữa 2 bên.
    - Tầng phiên chịu trách nhiệm về:
        + Kiểm soát hội thoại
        + Đồng bộ hóa
    - *Tầng trình diễn (Presentation layer)*: Tầng trình diễn biểu diễn cú pháp và nghĩa các thông tin được trao đổi giữa hai hệ thống.
    - Tầng trình diễn có nhiệm vụ:
        + Phiên dịch(Translation)
        + Mã hóa
        + Nén
    - *Tầng ứng dụng (Application)*: Tầng ứng dụng cho phép người dùng truy cập vào mạng bằng cách cung cấp gaio diện người sử dụng, hỗ trợ các dịch vụ như gửi thư điện tử, truy cập và chuyển file từ xa, quản lý CSDL dùng chung và một số dịch vụ khác về thông tin.
    - *Tầng ứng dụng cung cấp các dịch vụ*:
        + Thiết bị đầu cuối ảo mạng
        + Quản lý, truy cập và chuyển file
        + Các dịch vụ khác
### 1.2.3 *Bộ giao thức TCP/IP - Mô hình Internet*
- Bộ giao thức TCP/IP được ra đời khi có mô hình OSI. Các tầng trong bộ giao thức TCP/IP không giống hệt các tầng trong mô hình OSI. Bộ giao thức TCP/IP có 5 tầng: vật lý, liên kết dữ liệu, mạng, giao vận và ứng dụng.
- TCP/IP là giao thức phân cấp, được tạo thành bởi các module độc lập, mỗi module cung cấp một chức năng nhất dịnh, tuy nhiên các module này không nhất thiết phải độc lập với nhau. Mô hình OSI xác định rõ chức năng nào thuộc về tầng nào; trong khi đó các tầng của giao thức TCP/IP chứa các giao thức tương đối đọc lập với nhau, nhưng các giao thức này vẫn có thể kết hợp với nhau tùy thuộc nhu cầu hệ thống. Thuật ngữ "phân cấp" mang nghĩa mỗi giao thức ở tầng trên được hỗ trợ bởi 1 hoặc nhiều giao thức ở tầng dưới.
- Tại tầng giao vận, mô hình Internet có 2 giao thức: Transmission Control Protocol(TCP) và User Datagram Protocol(UDP). Tại tầng mạng là gioa thức Internetworking Protocol(IP), thường được gọi là IP.
