# OOP, sql server, cấu trúc dữ liệu và giải thuật.

# English, to day by work. Free time, reading books, playing socce. Family.



# (OOP-Object-Oriented Programming)
+ kế thừa:
	1. thông qua từ khóa: extends
	2. có thể tạo một class mới được xây dựng thông qua các lớp đã tồn tại, có thể sử dụng các phương thức, thuộc tính của lớp cha đồng thời có thể triển khai các phương thức, thuộc tính khác.
+ tại sao phải sử dụng?
	1. tăng khả năng tái sử dụng code
	2. tăng mối liên hệ thực tế 
+ đa hình: thông qua hai hai ví dụ củ thể overriding và overloading
	+ overloading:	
		1. được thể hiện trong cùng một lớp hoặc lớp khác nhau nhưng phải kế thừa
		2. định nghĩa cùng tên với class cha nhưng khác số lượng với method của class cha.
	+ overriding:	
		1. thể hiện ở lớp con 
		2. tồn tại method cùng tên, cùng số lượng tham số với method của class cha
		3. tại sao phải sử dụng?
		4. cho phép một đối tượng xử lý công việc theo nhiều cách	
+ trừu tượng 
	1. cho phép loại bỏ các tính chất phức tạp của đối tượng bằng cách đưa ra các thuộc tính và phương thức cần thiết của các đối tượng lập trình.
	2. giúp tập trung vào cốt lõi cần thiết thay vì quan tâm tới đến cách nó thực hiện.
	3. sử dụng abstract class và abstract interface.	
+ abstract class:
	1. là một class trừu tượng.
	2. chứa phương thức trừu tượng.
	3. khi các class kế thừa abstract class phải định nghĩa lại các phương thức.
	4. không thể khai báo nội dung phương thức
	5. mức truy cập các hàm của abstract phải ở public hoặc protected để lớp kế thừa.
	+ có hai loại abstract: 
		1. abstract thường có thực thi.
		2. abstract method không có thực thi.
	+ ưu điểm:
		1. có thể linh động các method.
		2. các class extend có thể override hoặc không override các method thường.
	+ nhược điểm:
		1. không thể extend nhiều abstract class.

+ interface:
	1. như một cái khung có sẵn, các class khác implement và thực hiện các khung có sẵn đó.
	2. không phải là class.
	3. chứa các method/properties trống không có thực thi.
	4. các lớp implement phải triển khai các method mà interface đã định nghĩa.
	+ ưu điểm:
		1. kế thừa nhiều interface.
		2. xây dựng bộ khung mẫu mà các lớp follow theo.
		3. quản lí tốt, nắm bắt được các chức năng phải có cho một đối tượng nào đó.
	+ nhược điểm:
		1. mỗi khi định nghĩa thêm tính năng, các class implement nó đồn loạt phải thêm tính năng đó, khả năng cao sẽ không có xử lý gì.

# VÍ DỤ:
1. interface:
	1. Khi bạn muốn tạo dựng một bộ khung chuẩn gồm các chức năng mà module hay project phải có. 
	Giống như sau khi nhận requirement của khách hàng về team ngồi với nhau và phân tích các đầu mục các tính năng của từng module, 
	sau đó triển khai vào code viết các interface như đã phân tích,
	để các bạn dev có thể nhìn vào đó để thực hiện đủ các tính năng.
2. abstract:
	1. Có các chức năng A, B, C trong đó A, B chắc chắn được thực hiện theo cách nào đó
	còn chức năng C phải phụ thuộc vào một đối tượng cụ thể.
	2. Đối tượng Dog, Cat tuy chúng đều có thể phát ra âm thanh nhưng âm thanh là khác nhau. 
	Vì vậy method Speak() là abstract method để chỉ ra rằng tính năng này còn dang dở chưa rõ thực thi, 
	các lớp extend phải hoàn thành nốt tính năng này, 
	còn những tính năng đã hoàn thành vẫn sử dụng như bình thường đây là những tính năng chung.
+ đóng gói
	1. trạng thái được bảo vệ không cho các truy cập bên ngoài như thay đổi trạng thái nhìn trực tiếp
	2. toàn vẹn và bảo mật đối tượng 
	3. thể hiện qua các access modifier 	
	4. tại sao sử dụng?
	5. các thuộc tính private của đối tượng được sử dụng để ẩn dấu thông tin về đối tượng đó
	6. nếu không sử dụng đóng gói, trạng thái và hành vi của đối tượng có thể dễ dàng bị truy cập và thay đổi trạng thái
# Cấu trúc dữ liệu và giải thuật
+ stack (first in last out)
	1. Hoạt động push(): lưu giữ một phần tử trên ngăn xếp.
	2. Hoạt động pop(): xóa một phần tử từ ngăn xếp.
	3. Phương thức peek(): lấy phần tử ở đầu hàng đợi, mà không xóa phần tử này.
	4. Phương thức isFull(): kiểm tra xem hàng đợi là đầy hay không.
	5. Phương thức isEmpty(): kiểm tra xem hàng đợi là trống hay hay không.
+ queue (first in first out)
	1. Hoạt động enqueue(): thêm (hay lưu trữ) một phần tử vào trong hàng đợi.
	2. Hoạt động dequeue(): xóa một phần tử từ hàng đợi.
	3. Phương thức peek(): lấy phần tử ở đầu hàng đợi, mà không xóa phần tử này.
	4. Phương thức isFull(): kiểm tra xem hàng đợi là đầy hay không.
	5. Phương thức isEmpty(): kiểm tra xem hàng đợi là trống hay hay không.
+ search:
	1. nhị phân (Binary Search)
	2. tuyến tính (Linear Search)	
+ sort:
	1. bubble sort
	2. selection sort
	3. insertion sort
	4. quick sort
	5. merge sort
	6. heap sort
	7. radix sort
	8. ...
+ graph:
	1. Dijkstra
	2. Bellman-Ford
	3. Ford-Fulkerson
	
# SQL
+ 
***
+ inner joint
	1. This query will return all of the records in the left table (table A) that have a matching record in the right table (table B)
+ left joint
	1. This query will return all of the records in the left table (table A) regardless if any of those records have a match in the right table (table B)
+ right joint
	1. This query will return all of the records in the left table (table B) regardless if any of those records have a match in the right table (table A)
+ full joint (outer joint)
	1. This query will return the joined result of all records in both tables
