# Tải xuống và cài đặt PHP theo cách thủ công
- Mở trình duyệt và truy cập vào link sau để tải PHP: ```https://windows.php.net/download/```
> ![q](https://f5-zpcloud.zdn.vn/2755884506661723700/56fc9ea3f0b73de964a6.jpg)
 
- Sau đó tải xuống tiện ích mở rộng WinCache link: ```https://sourceforge.net/projects/wincache/```
> ![q](https://f4-zpcloud.zdn.vn/4188159310354472618/94767c29183dd5638c2c.jpg)

- Giải nén tệp PHP.zip vừa tải ví dụ vào thư mục ```C:\PHP\```
> ![q](https://f4-zpcloud.zdn.vn/4248894603975742146/c86297760862c53c9c73.jpg)

- Giải nén tệp WinCache.zip vào thư mục mở rộng ```C:\PHP\ext``` 
> ![q](https://f5-zpcloud.zdn.vn/7752610474365047732/b7524c2bfd3f3061692e.jpg)

- Tiếp theo ta mở Control Panel, click System and Security, click System, and then click Advanced system settings.
> ![q](https://f5-zpcloud.zdn.vn/3772100693893656233/2299465eed4a2014795b.jpg)

> ![q](https://f4-zpcloud.zdn.vn/3774296682656471596/94637ba3d0b71de944a6.jpg)

> ![q](https://f4-zpcloud.zdn.vn/524351987158022862/27d8d0197b0db653ef1c.jpg)

> ![q](https://f4-zpcloud.zdn.vn/6677058020801880738/b4520b90a0846dda3495.jpg)

- Tiếp chọn Advanced, click Environment Variables.
> ![q](https://f4-zpcloud.zdn.vn/4938295424147535702/d8f3079ea08a6dd4349b.jpg)

> ![q](https://f5-zpcloud.zdn.vn/6105224187859466218/7127bf4f185bd5058c4a.jpg)

- Tiếp tục ở System variables chọn Path, click Edit
> ![q](https://f5-zpcloud.zdn.vn/8410490118313025019/2776d9ed10f9dda784e8.jpg)

> ![q](https://f5-zpcloud.zdn.vn/8627315462099876905/58a79b3c52289f76c639.jpg)

- Thêm đường dẫn đến thư mục cài đặt PHP vào phần Variable value ví dụ ```C:\PHP``` và click OK
> ![q](https://f5-zpcloud.zdn.vn/6925098220643465531/b1cce3602474e92ab065.jpg)

- Tiếp theo ta vào IIS Manage chọn vào localhost click Handler Mappings
> ![q](https://f5-zpcloud.zdn.vn/1726579662957914269/a1a41139fa2d37736e3c.jpg)

> ![q](https://f5-zpcloud.zdn.vn/4698820593346776864/891c2181ca9507cb5e84.jpg)

- Trong phần Handler Mappings ta chọn Add Module Mapping
 > ![q](https://f4-zpcloud.zdn.vn/5750795159410653175/741381ae64baa9e4f0ab.jpg)

- Trong mục Executable nhập đường dẫn đầy đủ đến Php-cgi.exe ví dụ ```C:\PHP\Php-cgi.exe```, điền tên vào và OK
> ![q](https://f5-zpcloud.zdn.vn/5338798830539822330/90a99e4ca75b6a05334a.jpg)

- Trở về phần Connections panel click Default Document
> ![q](https://f4-zpcloud.zdn.vn/1335356171751704954/73405f091b1ed6408f0f.jpg)

- Click Add, tạo 1 index.php trong, 1 Default.php ở mục Name
> ![q](https://f5-zpcloud.zdn.vn/8290561127053619685/9047262b5d3c9062c92d.jpg)

> ![q](https://f5-zpcloud.zdn.vn/2446382476065151468/ccd931b24aa587fbdeb4.jpg)
