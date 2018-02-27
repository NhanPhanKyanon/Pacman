
# Pacman
## I. Mô tả mini game Pacman.
Pacman là mini game ăn những chấm trắng và tránh sự truy đuổi của bọn quái vậy săn đuổi. Game như một cuộc chạy đua với quái thú, người chơi phải né chúng và ăn hết những chấm tròn. Nếu vượt qua thử thách các gamer sẽ được nâng cấp (level) với mức độ khó tăng dần. 
## II. Cách chơi.
Người chơi nào cùng các phím ->, <-, ^, v để di chuyển nhân vật của mình. Tránh những quái thú khi chúng có màu: xanh, hồng, cam, đỏ,... Nếu chúng chuyển thành màu xám thì bạn có thể đi xuyên/ăn chúng. Cứ như thế cho đến khi hết hạt gạo, vượt qua hết các level bạn sẽ là người chiến thắng.
## III. Công cụ cần sử dụng.
XAMPP Control Panel v3.2.2 - phần mềm hỗ trợ sử dụng game này vì source code của game được viết bằng ngôn ngữ php. 
## IV. Hướng dẫn cài đặt.
- Dùng “Git bash here” để tải xuống file source trên repos, người cài đặt nên sử dụng Git để lấy dữ liệu. Tuy nhiên nếu không cài đặt git về máy bạn có cũng có thể tải chúng theo cách nhấn “Clone or download” và chờ tải.
- Nếu sử dụng câu lệnh git người dùng bắt buộc tạo một forlder với tên tùy đặt.
- Thực hiện lệnh $ git clone https://github.com/NhanPhanKyanon/Pacman.git
- Sau khi clone thành công dữ liệu của thư mục game sẽ nằm hoàn toàn trong thư mục này (thư mục bạn đã tạo trước đó).
- Người dùng mở XAMPP, thiệt lập các thông số sau vào file tương ứng: 

•Trong CONF file "httpd-vhosts.conf":
       <VirtualHost *:6040>
            ServerAdmin webmaster@dummy-host2.example.com
            DocumentRoot "<đường dẫn đến thư mục pacman-canvas đã clone>"
            ServerName dummy-host2.example.com
            ErrorLog "logs/dummy-host2.example.com-error.log"
            CustomLog "logs/dummy-host2.example.com-access.log" common
            <Directory "<đường dẫn đến thư mục pacman-canvas đã clone>">
                Options Indexes FollowSymLinks MultiViews
                AllowOverride all
                Order Deny,Allow
                Allow from all
                Require all granted
            </Directory>
         </VirtualHost>
- Mở XAMPP, chọn Start ứng với dòng Apache
- Tiếp thep người dùng vào trình duyệt web gõ  http://localhost:6040/  để vào game.

•Ngoài ra:
- Người dùng có thể nhấn vào README để đọc hướng dẫn sử dụng.
- Muốn thực hiện cài chi tiết về code game trên vào file word " Hướng dẫn cài đặt Pacman". 

## V. Lưu ý.
Khi clone file về người sử dụng cần phải thay đổi đường dẫn cho nó.
- Vào đường dẫn: "C:\xampp\apache\conf\extra" mở file "httpd-vhosts.conf" và thay đổi các đường dẫn cho nó khi cần thiết.
- Thực hiện sửa ở 'DocumentRoot' & 'Directory'.
  + DocumentRoot "D:/GamePacman/Pacman/pacman-canvas" -> Thay đường dẫn của bạn vào đây.
  + Directory "D:/GamePacman/Pacman/pacman-canvas" -> Thay đường dẫn của bạn vào đây. 
- Bạn có thể đổi port theo mong muốn nếu không muốn sử dụng: 6040. 
Để đổi port trong XAMPP bạn hãy lần lượt thay đổi các 'Listen 6040' trong các file của "Config".



                                                                             === Chúc Bạn Cài Đặt Thành Công ===
