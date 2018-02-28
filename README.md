
# Pacman
## I. Mô tả mini game Pacman.
Pacman là mini game mà người chơi phải điều khiển nhân vật của mình ăn những chấm trắng trên mọi đường đi và tránh sự truy đuổi của bọn quái vật. Game như một cuộc chạy đua với quái thú, người chơi phải né chúng và ăn hết những chấm tròn. Nếu vượt qua thử thách các gamer sẽ được nâng cấp (level) với mức độ khó tăng dần cho đến khi tất cả các vòng đều vượt qua bạn đã trở thành người chiến thắng rồi đấy!
## II. Cách chơi.
Người chơi dùng các phím di chuyển cơ bản trên bàn phím: >, <, ^, v để di chuyển nhân vật của mình. Nhiệm vụ của bạn là tránh sự truy đuổi của quái thú khi chúng có màu: xanh, hồng, cam, đỏ,... Nếu chúng chuyển thành màu xám thì bạn có thể đi xuyên/ăn chúng. Cứ như thế cho đến khi không còn hạt gạo nào. Nếu vượt qua hết các level bạn sẽ là người chiến thắng.
## III. Công cụ cần sử dụng.
XAMPP Control Panel v3.2.2 - phần mềm hỗ trợ sử dụng game này vì source code của game được viết bằng ngôn ngữ php. 
Trong trường hợp bạn muốn đổi localhost theo ý muốn thì nên sử dụng XAMPP kết hợp Sublime Text để có thể tùy chỉnh code dễ dàng.
## IV. Hướng dẫn cài đặt.
### 1. Lấy bằng GitHub.
- Dùng “Git bash here” để tải xuống file source trên thùng chứa trên gitHub. 
- Tạo một forlder với tên tùy đặt để clone dữ liệu về đây.
- Thực hiện lệnh " $ git clone https://github.com/NhanPhanKyanon/Pacman.git " để lấy file game xuống máy tính của bạn. 
- Sau khi clone thành công file game sẽ nằm thư mục bạn đã tạo trước đó.
- Người dùng mở XAMPP Control Panel, nhấn "Start" - cột Action ứng với Apache-cột Module.
- Tiếp thep người dùng vào trình duyệt web gõ  http://localhost:6040/  để vào game.
### 2. Lấy bằng giao diện.
 Nếu không cài đặt git về máy bạn có cũng có thể tải chúng theo cách nhấn “Clone or download” và chờ tải.
## V. Lưu ý.
Khi clone file về người sử dụng cần phải thay đổi đường dẫn cho nó.
- Vào đường dẫn: "C:\xampp\apache\conf\extra" mở file "httpd-vhosts.conf" và thay đổi các đường dẫn cho nó.
### Trong CONF file "httpd-vhosts.conf":
 Code:
>`<VirtualHost *:6040>`
`ServerAdmin webmaster@dummy-host2.example.com`
>`DocumentRoot "D:/GamePacman/Pacman/pacman-canvas"`
`ServerName dummy-host2.example.com`
>`ErrorLog "logs/dummy-host2.example.com-error.log"`
`CustomLog "logs/dummy-host2.example.com-access.log" common`
>`<Directory "D:/GamePacman/Pacman/pacman-canvas">`
`Options Indexes FollowSymLinks MultiViews`
>`AllowOverride all`
`Order Deny,Allow`
>`Allow from all`
`Require all granted`
>`</Directory>`
`</VirtualHost>`
         
- Thực hiện sửa ở 'DocumentRoot' & 'DocumentRoot'.
  + DocumentRoot "D:/GamePacman/Pacman/pacman-canvas" -> Thay đường dẫn của bạn vào đây.
  + DocumentRoot "D:/GamePacman/Pacman/pacman-canvas" -> Thay đường dẫn của bạn vào đây. 
- Bạn có thể đổi port theo mong muốn nếu không muốn sử dụng: 6040. 
Để đổi port trong XAMPP bạn hãy lần lượt thay đổi các 'Listen 6040' trong các file của "Config".
•Ngoài ra:
- Người dùng có thể nhấn vào README để đọc hướng dẫn sử dụng.
- Muốn thực hiện cài chi tiết về code game trên vào file word " Hướng dẫn cài đặt Pacman". 


                                   === Chúc Bạn Cài Đặt Thành Công ===
