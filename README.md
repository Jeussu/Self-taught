# Self-taught
Day1:
Kiểu dữ liệu trong SQL: 
•	BIT trả về true hoặc false
•	Approximate_Data: khai báo biến kiểu float và gán giá trị theo biến, tiếp theo thực hiện tính toán để lấy ra giá trị của biến
Ví dụ float  
•	DateTime: Hàm getdate để trả về ngày tháng năm h, phút,s
 
-	Datetimeofset kiểu dữ liệu real time, sử dụng kèm theo hàm CAST:
SELECT  CAST(GETDATE() AS DATETIMEOFFSET)
•	Kiểu dữ liệu binary: thường thực hiện theo giá trị hecxa và dạng số nguyên(int)
-	Hàm cast để chuyển đổi
 
•	Dữ liệu rowversion: có độ rộng là 8bytes 
•	Kiểu dữ liệu SQL_variant: là kiểu dữ liệu xác định theo kiểu dữ liệu khác
 
•	Basic SQL - Lecture 03: SQL Data Types & Operations - Demo Operations

•	Toán tử Exists: kiểm tra sự tồn tại của một đối tượng

•	Toán tử so sánh và toán tử logic(SQL Comparison operators) : lọc ra các bản ghi thoả mãn điều kiện

 
Ví dụ trên dùng toán tử logic AND, OR và LIKE
-	Toán tử IS NOT NULL là lọc ra bản ghi có giá trị và ko null
-	Toán tử LIKE để lọc ra phần tử có chuỗi cần tìm
 
-	Toán tử IN để lọc ra bản ghi trong cột có giá trị cần tìm
 
-	Toán tử BETWEEN lọc ra bản ghi trong bảng có giá trị trong khoảng cần tìm
 
-	Toán tử EXISTS lọc ra bản ghi có sẵn và kết hợp với điều kiện WHERE + điều kiện và in ra màn hình
 
-	Toán tử ALL đảm bảo rằng bản ghi đã được lọc trong phần tử dựa trên điều kiện
 
-	Toán tử ANY
 
Basic SQL - Lecture 04: DDL Statements
-	DDL - Data Definition Language là ngôn ngữ cho phép chúng ta định nghĩa cấu trúc
-	dữ liệu trong SQL Server bao gồm: tạo, thay đổi, xoá các bảng và thiết lập các rang buộc…
-	Các câu lệnh DDL gồm: CREATE , ALTER , DROP , TRUNCATEMột cơ sở SQL service gồm nhiều đối tượng như: 

 
-	Một SQL là tập hợp các dữ liệu liên quan đến nhau
Create 
Rename
Drop
-	Namespace: chứa một tập hợp bên trong nó bao gồm table stored procedure và view
-	Schema object: các đối tượng có mục đích liên quan đến nhau được gọi là schema
 
Ví dụ mặc định của schema là dbo, schema là danh giới đặt tên và danh giới bảo mật
-	ràng buộc trên bảng(Constraints)
•	khi tạo ràng buộc cần quan tâm đến: kiểu dữ liệu(Data type), chỉ mục(index)
ràng buộc SQL duy trì tính nhất quán dữ liệu, giúp ngăn chặn dữ liệu không hợp lệ, duy trì tính hợp lệ của dữ liệu
 
Default: ràng buộc mặc định nhằm chỉ định giá trị ban đầu khởi tạo cho cột khi insert dữ liệu giá trị mà bạn không chỉ định giá trị cho cột thì giá trị default sẽ đc dùng
-	Struncate statement: dùng để xoá hoàn toàn dữ liệu trong bảng, dùng truncate sẽ tăng performent nhanh hơn delete( nhược điểm truncate không thể dùng where hay from như delete)
Basic SQL - Lecture 05: Table Indexes, Sequences, View
1.	Index trong SQL: tương tự chỉ mục để tìm kiếm dữ liệu trên các cột trong bảng
-	Đầu tiên SQL sẽ tìm dữ liệu trong index, sau đó index sẽ xác định dòng dữ liệu cần tìm
-	Index có thể tạo trong hàng cột của bảng ngoại trừ các cột có kiểu dữ liệu lớn như IMG, varchar.v.v
 
Non-clustered index
 
Creating an Index:
 

2.	Sequences
- giống với Identity là tạo dãy tăng tự động cho các cột
- khác: giá trị đc khởi tạo trong bộ nhớ thay vì đc khởi tạo từ ổ cứng như identity do đó hiệu xuất cao hơn
- Creating sequences
 
Ví dụ: 
 
3.	Bảng ảo trong SQL(View)
-	View là bảng ảo mà dữ liệu trong đó đc mô tả bằng câu truy vấn và view ko chứa dữ liệu.
-	Lý do cho phép sử dụng view là: cho phép giới hạn người truy cập dữ liệu, view giúp giảm độ phức tạp cho người dùng cuối
 
Basci SQL - Lecture 06: DML Statements
DML - Data Manipulation Language là ngôn ngữ thao tác dữ liệu.
Các câu lệnh DML gồm: SELECT, INSERT, UPDATE, DELETE…
Insert statement: được sử dụng để thêm 1 hoặc nhiều bản ghi vào các cột trong bảng
 

-	Ví dụ về insert: 
 

Update statement: được sử dụng để thay đổi dữ liệu đã tồn tại của một bảng hoặc bảng ảo
 

Delete Statement: được sử dụng để xoá dữ liệu ở một bảng hoặc bảng ảo, khi delete bạn nên dùng truncate
 
Ví dụ về delete:
 

Select statement: Giúp lấy về các dòng SQL và cho phép một hay nhiều dòng hoặc cột trong bảng
Ví dụ Select:

 
-	Select into: giúp lấy dữ liệu từ 1 bảng và insert chúng vào 1 bảng khác
Ví dụ Select into:
 
-	SQL Alias: SQL bí danh được sử dụng để cung cấp cho 1 bảng dữ liệu hoặc 1 cột trong 1 bảng tên tạm thời, về cơ bản bí danh(Alias) được tạo ra để tên bảng dễ đọc hơn
Ví dụ về Alias:
 
Từ khoá DISTINCT: loại bỏ các bản ghi trùng lặp
Basic SQL - Lecture 07: SELECT Options
1.	SQL function: Hàm là một đối tượng trong CSDL bao gồm một tập hợp nhiều câu lệnh SQL đc nhóm lại với nhau thành 1 nhóm
•	Điểm khác biệt giữa hàm và thủ tục là:
-	Hàm trả về một giá trị thông qua tên hàm, điều này cho phép ta sử dụng hàm như một biểu thức. Ví dụ câu lệnh truy vấn, update
1.2	Aggregate function: nhóm hàm tập hợp có tác dụng với nhiều giá trị nhưng chỉ trả về 1 giá trị
-	Hàm tập hợp có thể sử dụng trong câu lệnh select và trong mệnh đề having
 
-	Một số hàm trong nhóm hàm tập hợp
 	1.4 Scalar function: Hàm định hướng
 
2.	SQL Clauses
2.1 GROUP BY
Trong câu lệnh SELECT có chức năng tổng hợp dữ liệu
 
2.2	Mệnh đề HAVING giúp kiểm tra điều kiện với các hàm tập hợp
Ví dụ mệnh đề:  
•	Mệnh đề WHERE tham chiếu tới các bản ghi trong bảng và không sử dụng được với các hàm tập hợp
•	Mệnh đề HAVING tham chiếu tới các bản ghi trong bảng và có thể sử dụng với các hàm tập hợp(HAVING luôn đi kèm GROUP BY)
 
2.3	ORDER BY
Mệnh đề sắp xếp(ORDER BY) theo thứ tự tăng dần hoặc giảm dần các bản ghi
 
3.1	UNION Operator:
Được dùng để kết hợp các dòng nhiều bảng khác nhau, Union sẽ kết hợp kết quả của 2 hay nhiều câu lệnh select lại thành 1 kết quả
•	Lưu ý: mỗi câu lệnh select phải có cấu trúc 
Và để sử dụng đc toán tử Union bạn phải chú ý đến 2 điều kiện: dữ liệu các cột phải tương ứng (kiểu  dữ liệu trong câu select bảng này phải giống kiểu kiểu dữ liệu trong câu select bảng kia)
-	Số lượng cột trong mỗi câu truy vấn phải bằng nhau tuy nhiên tên cột có thể khác nhau
-	Về cú pháp toán tử UNION sẽ lọc các bản ghi có giá trị trùng nhau, nếu sử dụng từ khoá ALL
 
 
 
ROUND để làm tròn số thập phân
Basic SQL - Lecture 08: Built-in Functions
Các built-in function được sử dụng trong các biểu thức SELECT để tính toán các giá trị và
thao tác dữ liệu.
Built-in function gồm các loại chính sau:
Các hàm chuyển đổi ( Conversion Functions )
Các hàm ngày giờ ( Date and Time Functions )
Các hàm xử lý chuỗi ( String Functions )
1.1.	CAST function: chuyển đổi một biểu thức từ kiểu dữ liệu này sang kiểu dữ liệu khác có thể sử dụng hàm CAST
-	Hàm CAST dùng để chuyển đổi dữ liệu kiểu variable
-	Hàm CAST cung cấp kiểu dữ liệu đến tham  số động hoặc một giá trị null
1.2 CONVERT Function
-	Hàm Convert dùng để chuyển đổi dữ liệu
 
 
2.1 GETDATE()&DATEPART() Function
- GETDATE(): hàm trả về ngày giờ hiện tại của hệ thống
- DATEPART(): được sử dụng lấy về ngày giờ có thể là ngày tháng năm, giờ phút giây(giá trị trả về phụ thuộc vào đối số đầu tiên của hàm này)
 
 
 
Lấy về ngày tháng, năm của tháng ngày hiện tại
2.4	DATEADD Function
-	Giúp cộng thêm hoặc trừ đi giá trị ngày tháng phụ thuộc vào đối số thứ 2(number)
-	 
-	 
-	3. String FUNCTION
-	3.1 RTRIM, LTRIM FUNCTION
-	- giúp cắt bỏ kí tự trắng trong một chuỗi kí tự
-	- LTRIM giúp cắt bỏ kí tự trắng bên trái chuỗi
-	- RTRIM giúp cắt bỏ kí tự trắng bên phải chuỗi
-	 
SUBSTRING Function: chả về chuỗi con trong chuỗi ban đầu
 





