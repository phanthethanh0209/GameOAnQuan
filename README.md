# GameOAnQuan
#### Công nghệ sử dụng:
- Python Pygame, PyQt

#### Thực hiện: Nhóm 3 thành viên

#### Thuật toán sử dụng:
- Giải thuật Minimax
- Giải thuật cắt tỉa Alpha – Beta

#### Chức năng đảm nhận:
- Thiết kế giao diện, chuyển động
- Code thuật toán cho chế độ với máy, đối kháng

#### Hướng dẫn sử dụng:
a.	Giao diện trò chơi
-	Khi vào giao diện main thì chúng ta có ba sự lựa chọn là Chơi, Tùy Chọn,Thoát.
+ Khi chọn vào nút chơi chúng ta sẽ có thể lựa chọn chơi với máy hoặc chơi đối kháng giữa 2 người với nhau 
+ Khi chọn vào nút tùy chọn giúp chúng ta điều chỉnh âm thanh 
+ Thoát khỏi trò chơi nếu không muốn tiếp tục 
-	Khi bấm vào chơi thì hiện ra bàn chơi có 10 ô quân và 2 ô quan, 2 ô tính điểm giữa hai người chơi

b.	Luật chơi
- Khi chơi ta có 10 ô quân mỗi ô có 5 sỏi, 2 ô quan mỗi ô 2 sỏi 
- Khi tới lượt mình đi mình chọn một trong năm ô phía mình để rải, ta có thể di chuyển theo hướng bên phải, hoặc bên trái để di chuyển. 
- Các trường hợp có thể xảy ra trong ô ăn quan khi chúng ta rải quân khi quân cuối cùng được rải xuống
  + TH1: Nếu như ô kế bên có sỏi ta sẽ lấy sỏi ô tiếp theo đó rải và đi tiếp 
  + TH2 : Nếu như ô kế bên không có sỏi mà ô kế tiếp có sỏi ta ăn sỏi ô đó
  + TH3 : Nếu như 2 ô kế tiếp nhau không có sỏi thì ta mất lượt 
  + TH4 : Nếu như các ô xen kẻ nhau 1 ô trống ta sẽ được ăn double
  + TH5 : Nếu như sỏi cuối cùng kế nó là ô quan thì không bốc ô quan để đi
- Khi 2 ô quan không còn quân hay quan thì trò chơi kết thúc tính tổng điểm ai lớn hơn thì thắng nếu bằng nhau thì thông báo hoà
