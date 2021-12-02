# Chương 2: TẦNG ỨNG DỤNG
2.1 *GIAO THỨC TẦNG ỨNG DỤNG*
    Tầng ứng dụng là nơi đơn giản nhất để bắt đầu nghiên cứu về giao thức. Chúng ta sẽ làm quen với một vài ứng dụng cũng như giao thức giữa chúng . Điều này giúp ta hiểu rõ hơn về giao thức.
2.1.1 *Giao thức tầng ứng dụng*
- Giao thức tầng ứng dụng chỉ là một phần của ứng dụng mạng.
- Giao thức tầng ứng dụng đĩnh nghĩa cách thức truyền thông điệp giữa các tiến trình ứng dụng chạy trên các thiết bị khác nhau. Nó xác định:
    + Kiểu thông điệp trao đổi, ví dụ như thông điệp yêu cầu hay thông điệp trả lời.
    + Cú pháp thông điệp, ví dụ các trường trong thông điệp cũng như cách xác định chúng.
    + Ý nghĩa của các trường
    + Quy tắc xác định khi nào và như thế nào tiến trình gửi và trả lời thông điệp.
- Nhiều giao thức tầng ứng dụng được đặc tả trong các RFC.
* Mô hình Khách hàng/Người phục vụ(Client/Server)
    - Giao thức ứng dụng mạng thường chia ra hai phần hay hai phía, phía Client và phía Server.
    - Trong nhiều ứng dụng, máy tính sẽ thực hiện cả phần client và phần server của ứng dụng.
* Truyền thông giữa các tiến trình
    - Ứng dụng bao gồm hai tiến trình trên hai thiết bị khác nhau và liên lạc với nhau qua mạng. Hai tiến trình liên lạc với nhau bằng cách gửi và nhận thông điệp qua socket của chúng. Socket có thể xem như "cửa" của tiến trình vì tiến trình nhận và gửi thông điệp qua "cửa". Khi muốn gửi thông điệp tới tiến trình khác, tiền trình đẩy thông điệp cần gửi qua "cửa" với giả định rằng thực thể giao vận nằm bên kia "cửa" sẽ chuyển thông điệp đến "cửa" của tiến trình nhận.
* Địa chỉ tiến trình
    Để gửi thông điệp cho tiến trình trên máy tính khác thì tiến trình gửi phải xác định được tiến trình nhận. Tiến trình được xác định qua 2 phần: (1) tên hay địa chỉ của máy tính và (2) định danh xác định tiến trình trên máy tính nhận.
* Trương trình giao tiếp người dùng (user agent)
    - User agent là giao diện giữa người dùng và ứng dụng mạng.
2.1.2 *Các yêu cầu của ứng dụng*
- Ứng dụng đòi hỏi gì của giao thức giao vận? Về đại thể chúng ta có thể phân loại theo 3 nhóm: mất mát dữ diệu, băng thông, và thời gian.
    + Mất mát dữ liệu (Data loss): Một số ứng dụng như thư điện tử, truyền file, truy cập từ xa, truyền các đối tượng Web, và ứng dụng tài chính đòi hỏi dữ liệu phỉa được truyền chính xác và đầy đủ, tức là không được mất dữ liệu. Đặc biệt, mất mát file dữ liệu hoặc dữ liệu trong cấc giao dịch tài chính có thể gây nên hậu quả nghiêm trọng.
    + Băng thông (Bandwith): Để hoạt động hiệu quả, một só ứng dụng truyền tải dữ liệu với một tốc độ nhất định. Những ứng dụng đa phương tiện hiện nay là ứng dụng phụ thuộc vào băng thông (bandwith sensitive), nhưng trong tương lai ứng dụng đa phương tiện sẽ sử dụng các kỹ thuật mã hóa thích nghi để mã hóa tốc độ cho phù hợp với dải tần số hiện có.
    + Thời gian (timing): Những ứng dụng thời gian thực (real-time) mang tính chất tương tác, như Internet telephone, hội thảo qua điện thoại, hay các trò chơi nhiều người tham gia cùng một lúc(multiplayer game) yêu cầu những ràng buộc chặt chẽ về thời gian trong việc trao đổi giữ liệu.
2.1.3 *Dịch vụ của các giao thức giao vận Internet*
    Internet (và nói chung TCP/IP) cung cấp hai giao thức giao vận cho tầng ứng dụng: UDP và TCP. Khi xậy dựng ứng dọng cho Internet, một trong những quyết định đầu tiên mà nhà thiết kế phải đưa ra là sử dụng UDP hay TCP. Mỗi gioa thức cung cấp một kiểu phục vụ khác nhau cho ứng dụng.
- TCP
    Đặc trưng của giao thức TCP là hướng kết nối và cung cấp dịch vụ truyền dữ liệu tin cậy. Khi sử dụng giao thức giao vận TCP, ứng dụng sữ nhận được cả hai loại dịch vụ này.
- Dịch vụ hướng nối (conection oriented)
- Dịch vụ giao vận tin cậy
- Dịch vụ UDP
2.1.4 *Một số ứng dụng phổ biến*
    Các kiểu ứng dụng mạng ngày càng đa dạng và phong phú. Một số ứng dụng phổ biến mà ta thường gặp như:
- Web: là ứng dụng đầu tiên là vì Web cực kỳ phổ biến và giao thức tầng ứng dụng của nó - HTTP, tương đối đơn giản và minh họa nhiều đặc trưng cơ bản của giao thức.
- Truyền file: ứng dụng này có nhiều đặc điểm trái ngược với HTTP
- Thư điện tử: một trong những ứng dụng xuất hiện đầu tiên và thông dụng nhất của Internet
- Dịch vụ tên miền (DNS): cung cấp dịch vụ chỉ dẫn. Người dùng không tương tác trực tiếp với DNS mà yêu cầu dịch vụ DNS gián tiếp thông qua ứng dụng khác. DNS minh họa cách thức triển khai một cơ sở dữ liệu phân tán trên mạng.
2.2 *WORLD WIDE WEB: HTTP*
    Vào đầu thập niên 90, ứng dụng quan trọng nhất của Internet - World Wide Web xuất hiện, và nhanh chóng được gọi mọi người chấp nhận. Nó thay đổi cách thức tương tác giữa con người và môi trường làm việc . Chính điều này đã giúp đưa Internet từ một trong rất nhiều mạng thông tin thành một mạng thống nhất duy nhất.
2.2.1 *Tổng quan về HTTP*
    Hyper Text Transfer Protocol (HTTP) - giao thức tầng ứng dụng của Web - là trái tim của Web. HTTP được triển khai trên cả hai phí client và server. Các tiến trình clietn và server trên các hệ thống đầu cuối khác nhau gioa tiếp với nhau thông qua việc trao đổi các thông điệp giữa client và server.
- Trang Web (Webpage - hay còn gọi là một tâp tin) chưa các đối tượng (Object). Đơn giản đối tượng chỉ là một file như file HTML, file ảnh JPEG, file ảnh GIF,... Đối tượng xách định qua địa chỉ URL. Trang Web chứa một file HTML cơ sở và tham chiếu đến các đối tượng khác.
- Trình duyệt (Browser) - trương trình giao tiếp người dùng của ứng dụng Web cho phép hiển thị trang Web. Browser là phía client của giao thức HTTP. Hiện nay có rất nhiều phần mềm trình duyệt nhưng phổ biến nhất là Nestcape Communication và Microsoft Internet Explorer. Web server lưu giữ các đối tượng Web và được xác định qua đại chỉ URL. Phần mềm Web server là phía server của giao thức HTTP. Một số phần mềm Web server phổ biến là Apache, Microsoft Internet Information Server và Nestcape Enterorise Server.
HTTP xác định cách thức trình duyệt yêu cầu trang Web từ Web server cũng như cách thức server gửi trang Web được yêu cầu tới trình duyệt.
2.2.2 *Kết nối liên tục và không liên tục (persistent/nonpersistnt)*
    HTTP hôc trợ cả hai cách kết nối liên tục và không liên tục . HTTP 1.0 sử dụng kết nối không liên tục. Chế độ mặc định của HTTP 1.1 là kết nối liên tục.
2.2.3 *Khuôn dạng thông điệp HTTP*
    Các đặc tả HTTP 1.0 (RFC 1945) và HTTP 1.1 (RFC 2016) đặc tả khuôn dạng thông điệp HTTP. Có hai kiểu khuôn dạng HTTP: thông điệp yêu cầu (HTTP request mesage) và thông điệp trả lời (HTTP reponse mesage)
2.2.4 *Tương tác giữa người dùng và Hrver-server*
    HTTP server không lưu giữ trạng thái. Điều này đơn giản hóa kiến trúc và làm tăng hiệu suất hoạt động của server. Tuy nhiên server muốn phân biệt người dùng không chỉ vì muốn hạn chế sự truy cập mà còn vì muốn phục vụ theo định danh người dùng. HTTP có 2 cơ chế để server phân biệt người dùng: Authentication(kiểm chứng) và cookies.
- Authentication: nhiều server yêu cầu người dùng phải cung cấp tên (username) và mật khẩu (password) để có thể try cập được vào tài nguyên trên máy chủ. Yêu cầu này gọi là kiểm chứng.
- Cookies: là kỹ thuật khác được sử dụng để ghi lại dấu vết của người truy cập. Nó được đặc tả trong RFC 2109.
2.2.5 *GET có điều kiện (Conditional GET)*
    Lưu giữ lại các đối tượng đã từng được lấy, Web cache có thể làm giảm thời gian chờ từ khi gửi yêu cầu đến khi nhận đối tượng và làm giảm lưu lượng thông tin truyền trên Internet. Web cache được triển khai trên trình duyệt hay các cache server.
2.2.6 *Web cache*
- Web cache (proxy server) là thực thể đáp ứng yêu cầu từ client. Máy tính làm nhiệm vụ Web cache có ổ đĩa riêng lưu trữ bản sao các đối tượng đã từng được yêu cầu.
- Web cache vừa là client vừa là server. Web cache đóng vai trò server khi nhận yêu cầu và trả lời, đóng vai trò client khi gửi yêu cầu nhận thông điệp trả lời.
- Web cache được sử dụng rộng rãi vì 3 nguyên nhân sau: 
    + Làm giảm thời gian client phải đợi
    + Làm giảm tải mạng
    + Mạng Internet với nhiều Web cache giúp cho việc nhanh chóng phát tán thông tin - thậm chí ngay cho những nhà cung cấp thông tin có tốc độ server chậm hay tốc độ kết nôi chậm. Nếu một nhà cung cấp có một nội dung cần phổ biến thì nội dung này ngay lập tức được chuyển đến các Web cache và yêu cầu của người dùng từ mọi nơi được đáp ứng nhanh chóng.
- Cache liên hợp (Cooperative caching)
    Có thể kết hợp nhiều Webcache đặt ở các vị trí khác nhau trên mạng nhằm nâng cao hiệu suất tổng thể.
2.2.7 *Web động*
   * Một trang Web động không tồn tại dưới dạng một file cố định trên Web server. Trang Web động chỉ được tạo ra khi nhận được một yêu cầu cụ thể từ trình duyệt Web. Khi nhận được một yêu cầu, Web server sẽ chạy một chương tình ứng dụng nào đó để tạo ra nội dung một văn bản. Sau đó văn bản này được trả về cho trình duyệt.
    * Web tích cực(active Web) là loại văn bản có chứa chương trình. Chương trình này có khả năng tính toán và hiển thị thông tin. Khi trình duyệt yêu cầu, server sẽ gửi cho trình duyệt một văn bản có đính kèm chương trình. Trình duyệt sẽ chạy lại chương trình này tại máy tính cục bộ của mình, chương trình có thể tương tác với người sử dụng, tự động cập nhật thông tin theo nhu cầu người sử dụng. Do vậy nội dung trang Web tích cực không bất biến mà thay đổi khi chương trình tương ứng thực thi. Cơ chế Web động có ưu nhược điểm riêng so với Web tĩnh truyền thống.
* Chuẩn CGI (Common Gateway Interface)
    CGI là một trong những công nghệ đã từng được sử dụng rất rộng rãi khi xây dựng Web động. Chuẩn CGI quy định cách thức Web server tương tác với chương trình ứng dụng (chương trình CGI).
* Các kỹ thuật phía Server
    Một phương pháp giúp Web server tạo nội dung động là các công nghệ phía server (server side technology). Ngày nay có khá nhiều công nghệ như vậy:
    + ASP (Active Server Pages): Là công nghệ của Microsoft, có phần mở rộng là .asp.
    + PHP (Personal Home Pages): Công nghệ mã nguồn mở, phần mở rộng là .jsp.
    Với những công nghệ trên, dễ dàng cài đặt và bảo trì cho một Website lớn.