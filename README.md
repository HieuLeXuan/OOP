ôn tập kiến thức cơ bản java core.
OOP,  sql server.
cấu trúc dữ liệu và giải thuật.

English:
to day by work.
free time, reading books, playing soccer…
family.



# (OOP-Object-Oriented Programming)
+ kế thừa:
1 thông qua từ khóa: extends
2 có thể tạo một class mới được xây dựng thông qua các lớp đã tồn tại, có thể sử dụng các phương thức, thuộc tính của lớp cha đồng thời có thể triển khai các phương thức, thuộc tính khác.
+ tại sao phải sử dụng?
1 tăng tính tái sử dụng code

+ đa hình 
1 thông qua hai phương thức overriding và overloading
+ overloading:	
1 được thể hiện trong cùng một lớp 
2 định nghĩa cùng tên với class cha nhưng khác số lượng với method của class cha.
## overriding:	
+ thể hiện ở lớp con 
+ tồn tại method cùng tên, cùng số lượng tham số với method của class cha
+ tại sao phải sử dụng?
+ cho phép một đối tượng xử lý công việc theo nhiều cách	

## trừu tượng 
+ cho phép loại bỏ các tính chất phức tạp của đối tượng bằng cách đưa ra các thuộc tính và phương thức cần thiết của các đối tượng lập trình.
+ giúp tập trung vào cốt lõi cần thiết thay vì quan tâm tới đến cách nó thực hiện.
+ sử dụng abstract class và abstract interface.	

+ abstract class:
- là một class.
- chứa phương thức trừu tượng.
- khi các class kế thừa abstract class phải định nghĩa lại các phương thức.
- không thể khai báo nội dung phương thức
- mức truy cập các hàm của abstract phải ở public hoặc protected để lớp kế thừa.
+ có hai loại abstract: 
- abstract thường có thực thi.
- abstract method không có thực thi.
* ưu điểm:
- có thể linh động các method.
- các class extend có thể override hoặc không override các method thường.
* nhược điểm:
- không thể extend nhiều abstract class.

+ interface:
- như một cái khung có sẵn, các class khác implement và thực hiện các khung có sẵn đó.
- không phải là class.
- chứa các method/properties trống không có thực thi.
- các lớp implement phải triển khai các method mà interface đã định nghĩa.
* ưu điểm:
- kế thừa nhiều interface.
- xây dựng bộ khung mẫu mà các lớp follow theo.
- quản lí tốt, nắm bắt được các chức năng phải có cho một đối tượng nào đó.
* nhược điểm:
- mỗi khi định nghĩa thêm tính năng, các class implement nó đồn loạt phải thêm tính năng đó, khả năng cao sẽ không có xử lý gì.

VÍ DỤ:
* interface:
+ Khi bạn muốn tạo dựng một bộ khung chuẩn gồm các chức năng mà module hay project phải có. 
Giống như sau khi nhận requirement của khách hàng về team ngồi với nhau và phân tích các đầu mục các tính năng của từng module, 
sau đó triển khai vào code viết các interface như đã phân tích,
để các bạn dev có thể nhìn vào đó để thực hiện đủ các tính năng.

* abstract:
+ Có các chức năng A, B, C trong đó A, B chắc chắn được thực hiện theo cách nào đó
còn chức năng C phải phụ thuộc vào một đối tượng cụ thể.
+ Đối tượng Dog, Cat tuy chúng đều có thể phát ra âm thanh nhưng âm thanh là khác nhau. 
Vì vậy method Speak() là abstract method để chỉ ra rằng tính năng này còn dang dở chưa rõ thực thi, 
các lớp extend phải hoàn thành nốt tính năng này, 
còn những tính năng đã hoàn thành vẫn sử dụng như bình thường đây là những tính năng chung.




** đóng gói
* trạng thái được bảo vệ không cho các truy cập bên ngoài như thay đổi trạng thái nhìn trực tiếp
* toàn vẹn và bảo mật đối tượng 
* thể hiện qua các access modifier 	
* tại sao sử dụng?
* các thuộc tính private của đối tượng được sử dụng để ẩn dấu thông tin về đối tượng đó
* nếu không sử dụng đóng gói, trạng thái và hành vi của đối tượng có thể dễ dàng bị truy cập và thay đổi trạng thái

** Cấu trúc dữ liệu và giải thuật

** stack:
	
