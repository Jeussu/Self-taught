# Self-taught SQL:
![UC-945b25b2-08b4-47d8-a9e7-012017766a5d](https://user-images.githubusercontent.com/94780400/181032828-beb00a65-4178-44c6-8f42-e55ef49ac75a.jpg)
https://github.com/Jeussu/Self-taught-SQL/blob/main/UC-945b25b2-08b4-47d8-a9e7-012017766a5d.pdf <br>
Note report: https://github.com/Jeussu/Self-taught-SQL/blob/main/Note%20SQL%20Udemy.pdf
![CodeLearn_certification](https://user-images.githubusercontent.com/94780400/179392286-50504ee9-e64f-4a42-a0da-642f2f7b009c.png)
Link to certificate: https://codelearn.io/certification/yzq3nwnh
![CodeLearn_certification (1)](https://user-images.githubusercontent.com/94780400/179392296-ea062e80-0f8c-44ad-bc64-d85bbec50284.png)
Link to certificate: https://codelearn.io/certification/nzk0ntrk
<h2>if you want see details my report about SQL, Please click to link here: [Note SQL.pdf](https://github.com/Jeussu/Self-taught-SQL/files/9127362/Note.SQL.pdf) or flow this link https://github.com/Jeussu/Self-taught-SQL/blob/main/Note%20SQL.pdf</h2>

Day1:
Kiểu dữ liệu trong SQL: 
•	BIT trả về true hoặc false
•	Approximate_Data: khai báo biến kiểu float và gán giá trị theo biến, tiếp theo thực hiện tính toán để lấy ra giá trị của biến
Ví dụ float 
![image](https://user-images.githubusercontent.com/94780400/179392340-38f680ac-79ac-4a34-885f-02c929551070.png)
•	DateTime: Hàm getdate để trả về ngày tháng năm h, phút,s
![image](https://user-images.githubusercontent.com/94780400/179392348-a30fe6e5-2b26-471a-bac6-9d58d69ece98.png)
-	Datetimeofset kiểu dữ liệu real time, sử dụng kèm theo hàm CAST:
SELECT  CAST(GETDATE() AS DATETIMEOFFSET)
•	Kiểu dữ liệu binary: thường thực hiện theo giá trị hecxa và dạng số nguyên(int)
-	Hàm cast để chuyển đổi
![image](https://user-images.githubusercontent.com/94780400/179392358-857d06d7-8372-4e21-9d4c-70b9de8b7b86.png)
•	Dữ liệu rowversion: có độ rộng là 8bytes 
•	Kiểu dữ liệu SQL_variant: là kiểu dữ liệu xác định theo kiểu dữ liệu khác
![image](https://user-images.githubusercontent.com/94780400/179392366-867c86f5-3eb7-4f59-8da4-f49bcb36c61d.png)
•	Basic SQL - Lecture 03: SQL Data Types & Operations - Demo Operations
•	Toán tử Exists: kiểm tra sự tồn tại của một đối tượng
•	Toán tử so sánh và toán tử logic(SQL Comparison operators) : lọc ra các bản ghi thoả mãn điều kiện
![image](https://user-images.githubusercontent.com/94780400/179392379-ba57341e-b1a6-4911-aaa1-984acbbd28b2.png)
Ví dụ trên dùng toán tử logic AND, OR và LIKE
-	Toán tử IS NOT NULL là lọc ra bản ghi có giá trị và ko null
-	Toán tử LIKE để lọc ra phần tử có chuỗi cần tìm
![image](https://user-images.githubusercontent.com/94780400/179392389-d424e83b-110a-41cd-929d-d9fad3371bf5.png)
-	Toán tử IN để lọc ra bản ghi trong cột có giá trị cần tìm
![image](https://user-images.githubusercontent.com/94780400/179392392-588282ad-90a8-46ec-b141-45d70c179124.png)
-	Toán tử BETWEEN lọc ra bản ghi trong bảng có giá trị trong khoảng cần tìm
![image](https://user-images.githubusercontent.com/94780400/179392405-eee8c72f-bd14-4cd5-ac47-784c400fc947.png)
-	Toán tử EXISTS lọc ra bản ghi có sẵn và kết hợp với điều kiện WHERE + điều kiện và in ra màn hình
![image](https://user-images.githubusercontent.com/94780400/179392410-0decb3e5-8b8d-4c22-87fe-f2bb42ae4030.png)
-	Toán tử ALL đảm bảo rằng bản ghi đã được lọc trong phần tử dựa trên điều kiện
![image](https://user-images.githubusercontent.com/94780400/179392414-f24c54d0-ae41-4bf0-a955-ffbaf43f965a.png)
-	Toán tử ANY
![image](https://user-images.githubusercontent.com/94780400/179392418-e11b56f2-a654-4849-a66d-e3b1aa443905.png)
Basic SQL - Lecture 04: DDL Statements
-	DDL - Data Definition Language là ngôn ngữ cho phép chúng ta định nghĩa cấu trúc
-	dữ liệu trong SQL Server bao gồm: tạo, thay đổi, xoá các bảng và thiết lập các rang buộc…
-	Các câu lệnh DDL gồm: CREATE , ALTER , DROP , TRUNCATEMột cơ sở SQL service gồm nhiều đối tượng như: 
![image](https://user-images.githubusercontent.com/94780400/179392429-df1fd545-5ab8-4bcf-b9ae-79c1c779365c.png)
-	Một SQL là tập hợp các dữ liệu liên quan đến nhau
Create 
Rename
Drop
-	Namespace: chứa một tập hợp bên trong nó bao gồm table stored procedure và view
-	Schema object: các đối tượng có mục đích liên quan đến nhau được gọi là schema
![image](https://user-images.githubusercontent.com/94780400/179392451-8b853e95-9697-4bce-a85a-d1a64b35d49c.png)
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
 



Advanced SQL - Lecture 01: JOINs in SQL Server

JOIN: cho phép kết nối dữ liệu từ nhiều bảng lại với nhau
Join được dùng để lấy dữ liệu từ hai hay nhiều bảng và trả về dữ liệu trong cùng một tập
kết quả.
Join có các loại sau:
Inner Join
Outer Join
Cross Join
Self Join
Excluding Join
 
-	Khi bạn cần truy vấn các cột dữ liệu từ nhiều bảng khác nhau để trả về cùng 1 kết quả thì bạn dùng join
2.1 INNER JOIN: lấy phần trung và trả về tất cả bản ghi trong cả 2 bảng
 
3.	Outer join: lấy về các bản ghi có mặt trong cả 2 bảng và các bản ghi chỉ xuất hiện ở 1 trong 2 bảng được chỉ ra trong mệnh đề from miễn là các dòng đó thoả mãn điều kiện WHERE hoặc HAVING
-	Có 3 loại outer join:
 
•	LEFT JOIN: trả về tất cả bản ghi ở bên trái 
 
 
•	Right JOIN: trả về tất cả các bản ghi ở bản bên phải và ko quan tâm nó có đối sánh với bản bên trái hay không
 
 
•	FULL JOIN: Trả về tất cả bản ghi ở cả 2 bản và là sự kết hợp của left join và right join
 
 
Advanced SQL - Lecture 02: Subqueries
1.	What is a SUBQUERY?
Truy vấn con(Subqueries) là một truy vấn được lồng vào bên trong 1 truy vấn lớn hơn
-	1 subqueries có thể lồng bên trong câu lệnh select,insert,update,delete hay bên trong 1 truy vấn con khác 
-	Bạn có thể sử dụng các toán tử so sánh như >,< or =. Toán tử so sánh cũng có thể là 1 toán tử nhiều dòng IN,ANY hoặc ALL
-	1 truy vấn con được đặt như 1 phần của truy vấn ngoài còn gọi là outer query
 
•	Subquery hoạt động như thế nào?
-	Inner query độc lập với outer query
-	Inner query thực thi trước và lưu lại kết quả sau
-	Outer query được chạy sau đó và sử dụng kết quả đã lưu trước đó của inner query 
2.	Các loại truy vấn con (subquery type)
-	Single row subquery: truy vấn con 1 dòng đơn sẽ trả về kết quả tối đa 1 bản ghi cho truy vấn bên ngoài. Có thể đặt truy vấn con loại này trong mệnh đề WHERE, HAVING hoặc FROM của truy vấn ngoài
 
-	Multiple row subquery: loại này trả về ít nhất 1 bản ghi trong tập truy vấn con, có thể sử dụng các toán tử IN, ANY, ALL trong truy vấn ngoài để điều khiển kết quả trả về của toàn bộ truy vấn 
 
-	Multiple column subquery: truy vấn con trả về tập kết quả chứa nhiều cột 
 
-	Correlated subquery:là loại truy vấn đặc biệt trong đó truy vấn con có tham chiếu tới một hoặc vài cột của truy vấn ngoài, nói cách khác truy vấn con có quan hệ với truy vấn ngoài
 
-	Nested subquery: truy vấn lồng là truy vấn con lồng bên trong các truy vấn con khác
 
3.	COMMON case use subquery
Các trường hợp điển hình dùng subquery
-	Subquery với bí danh(ALIAS): nhiều câu lệnh trong đó subquery và outer query tham chiếu tới cùng 1 bảng 
-	Subquery với IN/NOT IN: kết quả của subquery khi dùng với IN hoặc NOT IN là một danh sách 0 hoặc nhiều giá trị sau khi subquery trả về kết quả, outer query sẽ sử dụng chúng để kiểm tra phần tử so sánh có nằm trong hay không nằm trong tập kết quả trả về subquery
-	Subquery với EXISTS/NOT EXISTS: trường hợp này toán tử kết hợp với subquery tạo thành một chức năng kiểm tra sự tồn tại.
-	Subquery in update, delete, insert, select
4.	Các quy tắc sử dụng subquery
-	Truy vấn con phải được đặt trong ngoặc
-	Các truy vấn con trả về một hay nhiều dòng thì chỉ sử dụng được với toán tử đa trị chẳng hạn như toán tử IN
-	Truy vấn con có thể bao gồm mệnh đề WHERE, GROUP BY, HAVING
-	Truy vấn con không bao gồm mệnh đề COMPUTE hoặc FOR BROWSE 
-	Bạn chỉ được phép chứa 1 mệnh đề ORDER BY khi có mệnh đề TOP
-	Bạn có thể lồng truy vấn con lên đến 32 cấp
Advanced SQL - Lecture 03: CTE & Ranking Functions, SQL Code Practice
Biểu thức bảng và các hàm ranking trong SQL
•	Biểu thức bảng(Common table expression): là cách tạo ra bộ dữ liệu trung gian từ các phép truy vấn và được sử dụng lại trong phép truy vấn ngay sau đó
•	Biểu thức bảng(CTE) tương tự như 1 bảng dẫn xuất ở chỗ nó không được lưu trữ một số đối tượng và chỉ kéo dài trong suốt thời gian của câu truy vấn, nhưng lại khác bảng dẫn xuất ở chỗ biểu thức bảng(CTE) có thể tự tham chiếu tới bản thân nó và có thể tham chiều nhiều lần trong 1 câu truy vấn
•	Mục đích của biểu thức bảng(CTE): nó giúp tạo truy vấn đệ quy, thay thế view cho một số trường hợp, cho phép nhóm 1 cột từ truy vấn con, tham chiếu tới bảng kết quả nhiều lần trong cùng 1 lệnh 
 

 
 
•	Trong biểu thức bảng có thể tạo truy vấn đệ quy()
 
2.	Ranking function
Các hàm xếp hạng ranking cho phép bạn đánh số liên tục hay xếp loại cho tập hợp kết quả, các hàm này có thể được sử dụng để cung cấp số thứ tự trong hệ thống đánh số tuần tự khác nhau
-	Có 4 hàm ranking:
 
•	Rank: trả về thứ tự bên trong dòng của tập kết quả, thứ hạng này phụ thuộc vào tiêu chí đưa ra để xếp hạng. Hàm Rank cho phép chọn vùng xếp hạng, có nghĩa là thứ hạng chỉ có nghĩa trong vùng đó mà thôi.
 
•	Rank_DENSE:Tương tự như rank nhưng hàm này không cung cấp khoảng cách giữa các số xếp loại, nghĩa là nếu có 2 số cùng thứ hạng 1 thì thứ hạng tiếp theo vẫn là 2
 
•	NTILE: được sử dụng để phân tán các bản ghi hoặc các dòng thành các nhóm theo số nhóm được chỉ định. Số nhóm tuỳ thuộc vào đối số N(Nếu N=3 thì chia bản ghi thành 3 nhóm và hệ quản trị sẽ tự xác định bản ghi rồi chia ra cho 3 để ra được số nhóm)
 
•	ROW_NUMBER: Trả về số thứ tự của mỗi dòng trong một phân vùng của tập kết quả, phân vùng tuỳ thuộc vào lựa chọn của người viết
 
3.	SQL code practice
Lưu ý trong code SQL
•	Khai báo tường minh danh sách cột trả về trong lệnh select
•	Thay vì dùng select * thì điều này sẽ cải thiện hiệu năng truy vấn
•	Ngăn ngừa những lỗi tiềm ẩn liên quan đến việc thay đổi CSDL trong tương lai
 
•	Đối với lệnh insert thì tương tự như lệnh select: thì việc khai báo tương minh danh sách cột giúp code rõ ràng và sáng hơn tránh những nhầm lẫn đáng tiếc về thứ tự cột. Việc khai báo này sẽ giúp chúng ta không phải quan tâm đến thứ tự cột trong DB mà chỉ cần quan tâm có những cột nào để truyền dữ liệu tương ứng 
 
•	Luôn chỉ định schema cho các truy vấn , việc này giúp ngăn ngừa lỗi tiềm ẩn liên quan đến thay đổi schema hoặc thay đổi quyền trong các schema trong tương lai
 
•	Nên cung cấp bí danh cho các bảng, điều này giúp cho truy vấn trở nên gọn gàng và dễ đọc hơn.
 
•	Hạn chế sử dụng hàm trong mệnh đề WHERE, vì sử dụng hàm sẽ làm giảm hiệu xuất truy vấn
 
•	Chỉ sử dụng từ khoá DISTINCT và UNION ALL khi thực sự cần thiết hay khi không biết dữ liệu có trùng lặp hay không vì với các từ khoá này SQL ENGINE sẽ phải xử lý thêm các thao tác sắp xếp và loại bỏ bản ghi trùng lặp dẫn đến hiệu năng giả đáng kể 

Advanced SQL - Lecture 04: SQL Language Elements
Phần tử trong SQL
•	Comment : --ghi chú trong sql
1.	Định danh(Identifiers) : tên các đối tượng, đối tượng ở đây là CSDL, bảng, bảng ảo, chỉ mục, hàm thủ tục.v.v.
•	Một định danh được tạo khi đối tượng được tạo ra hoặc được định nghĩa ra
•	Định danh được dùng để tham chiếu đến đối tượng
•	Có 2 loại định danh:
-	Regular identifiers: tên các bảng
-	Delimited Identifiers: loại này sử dụng dấu “” hoặc dấu[] để bao quanh định danh, loại này dùng cho các định danh bị trùng trong sql hoặc các định danh có chứa khoảng trắng giữa các từ
 
2.	Variables
-	Biến trong SQL: biến cần phải khai báo trước câu lệnh tham chiếu đến nó, khi khai báo biến trong SQL ta sử dụng @. Còn đối với các biến toàn cục globle variable thì sẽ sử dụng 2 biến @@, khi khai báo biến chúng ta dùng DECLARE
-	Để thực hiện gán giá trị ban đầu cho biến chúng ta dùng từ khoá set @tênbien = giá trị
 
3.	Control-of-flow
Khi chúng ta thực hiện 1 chương trình theo chế độ mặc định thì các câu lệnh được thực hiện tuần tự, chúng ta có thể thực hiện điều khiển luồng của chương trình bằng cách dùng các câu lệnh điều khiển như sau:
 
•	IF…ELSE: chúng ta có thể thực hiện một tập hợp các câu lệnh khác của SQL dựa trên điều khiển được chỉ ra câu lệnh SQL sau từ khoá IF chỉ được thực hiện nếu điều kiện đúng, trong trường hợp mệnh đề IF sai thì tập hợp các câu lệnh sau từ khoá else sẽ được thực hiện.
 
•	GOTO: lệnh goto sẽ chuyển luồng xử lý tới vị trí khác được chỉ định bởi nhãn
 
•	CASE…WHEN: hàm CASE kiểm định giá trị trên danh sách các điều kiện đưa ra sau đó trả về 1 hoặc nhiều kết quả 
 
•	TRY…CATCH: thay vì luôn phải check biến error của SQL lúc thực hiện transaction thì bây giờ ta thực hiện các chuỗi lệnh đó trong try catch nếu lỗi thì roolback lại
 
•	While : với cấu trúc lặp thì người lập trình có thể chỉ định 1 hoặc nhiều câu lệnh sẽ được lặp lại nhiều lần trong khi giá trị của biểu thức điều kiện có thể đúng 
-	Thực tế cấu trúc lặp WHILE bị giới hạn trong nhiều trường hợp, bởi vì bản thân các lệnh truy vấn cập nhật dữ liệu như select,update,delete trong transaction SQL đã tự động thực hiện việc lặp từ dòng dữ liệu đầu tiên đến dòng dữ liệu cuối cùng trong bảng, vì vậy cấu trúc lặp while thông thường được dùng với các biến kiểu dữ liệu con trỏ
 
•	Return : câu lệnh này giúp trả về giá trị của một hàm, thủ tục lưu trữ hoặc lệnh này sẽ giúp thoát khỏi thủ tục lưu trữ hay các truy vấn
 
 
Advanced SQL - Lecture 05: Stored Procedure
Thủ tục lưu trữ là tập hợp các câu lệnh SQL được mô tả như 1 khối các câu lệnh đơn lẻ dùng để thực thi 1 nhiệm vụ cụ thể nó giúp ích khi 1 nhiệm vụ được thực hiện nhiều lần. Khi đó thay vì viết lại các đoạn code thì ta chỉ việc gọi thủ tục 
1.	Stored procedure: thủ tục lưu trữ là tập hợp các câu lệnh SQL được biên dịch trước, gọi là pre compiles
•	Thủ tục lưu trữ được đặt tên và được xử lý như một khối lệnh thống nhất chứ không phải thực hiện rời rạc. SQL server cũng cấp sẵn các thủ tục được lưu trong hệ thống giúp thực hiện một số công việc thường xuyên. Nó được gọi là thủ tục hệ thống(System stored procedure)
•	Thủ tục lưu trữ trong SQL cũng tương tự như khái niệm thủ tục trong các ngôn ngữ lập trình khác bởi vì nó chấp nhận biến đầu vào và trả lại kết quả khi thực hiện. chứa những câu lệnh dùng trong lập trình, có thể thao tác với CSDL và có thể gọi đến các thủ tục khác và trả lại giá trị trạng thái khi thủ tục được gọi
 
•	Thủ tục lưu trữ có thể trả về dữ liệu 1 trong 4 cách
-	Trả về theo đối số đầu ra(output parameter): trả về dữ liệu kiểu số nguyên hoặc kiểu kí tự hay biến con trỏ
 
 
•	Trả về kết quả sử dụng từ khoá return
 
•	Trả về một tập kết quả với mỗi lệnh select chứa trong thủ tục lưu trữ hoặc trong một thủ tục lưu trữ khác được gọi bởi thủ tục lưu trữ hiện hành
•	Trả về kết quả thông qua một con trỏ toàn cục mà có thể tham chiếu tới bên ngoài con trỏ lưu trữ
•	Lợi ích của thủ tục lưu trữ:
-	Giảm dung lượng chuyển đổi qua lại giữa client và server
-	Bảo mật hơn
 
-	Có thể tái sử dụng code, có thể viết 1 lần và gọi nhiều lần
-	Cải thiện hiệu năng
 
Cú pháp cơ của SP:
 
 
Hạn chế khi dùng SP:
 
Advanced SQL - Lecture 06: Trigger
Tương tự như thủ tục lưu trữ đó là trigger, trigger bao gồm tập các lệnh SQL kết hợp với nhau nhưng trigger phải được gắn liền với một bảng nào đó và được tự động thực thi xảy ra một trong các thao tác như insert, update,delete làm thay đổi dữ liệu của bảng
•	Một số điểm khác biệt của trigger và SP được nói đến như:
-	Trigger được viết bên trong 1 bảng, được chỉ định và thực thi khi có sự thay đổi dữ liệu
-	Không thể thực thi trong các thủ tục khác
-	Trigger không thể phân quyền đến từng user trong SQL, nó được phân quyền với quyền của bảng. Với SP thì bạn có thể phân quyền đến từng user
1.	What is trigger?
Trigger là một thủ tục lưu trữ đặc biệt và nó sẽ được tự động thực thi khi có sự kiện tương ứng tác động. Trigger còn được gọi là bẫy lỗi, một bẫy lỗi được gắn liền với 1 bảng và được thực thi khi xuất hiện một sự kiện đặc biệt trong bảng khi insert,update,delete
 
•	Các bẫy lỗi sẽ được kích hoạt tự động khi một hành động xảy ra
•	Các bẫy lỗi được xử dụng phổ biến để ép các thao tác tuân theo một quy tắc nhất định, chúng giám sát sự thay đổi để chắc chắn rằng sự thay đổi đó là phù hợp với các quy tắc nghiệp vụ, vì vậy các bẫy lỗi thường được sử dụng để đảm bảo tính toàn vẹn dữ liệu
•	Một số mục đích thông thường của bẫy lỗi như sau:
-	Duy trì bản sao và dẫn xuất của dữ liệu
-	Sử dụng trong trường hợp cột phải có ràng buộc phức tạp mà không biểu diễn được bằng constraints
-	Làm thay đổi theo tầng hoặc xoá dữ liệu liên quan đến bảng khác trong 1 CSDL
-	Thiết lập giá trị ban đầu cho cột: giá trị này thường phức tạp và không thể sử dụng default
-	Huỷ bỏ những thay đổi không đúng để đảm bảo toàn vẹn dữ liệu
•	Có 3 loại trigger:
-	DML trigger: là các trigger cho phép biến cố thao tác dữ liệu, nó sẽ được kích hoạt khi có thay đổi dữ liệu trên bảng hoặc bảng ảo. Loại này cũng thường được dùng để đảm bảo quy tắc nghiệp vụ hoặc toàn vẹn dữ liệu
-	DLL trigger: loại này được kích hoạt khi có sự thay đổi cấu trúc bảng, bảng ảo hay thủ tục lưu trữ qua các lệnh create, alter, drop với ý nghĩa đảm bảo an toàn CSDL mỗi khi có sự thay đổi về định nghĩa dữ liệu thì người thực hiện có nhu cầu xử lý tự động để ngăn chặn hoặc ghi nhận thông tin như ai thực hiện, thời gian, nội dung.v.v. thì người thực hiện có thể làm được điều này bằng DDL trigger
•	DML trigger chia làm 2 loại:
-	After trigger: trigger loại này sẽ được tự động gọi ngay sau khi các câu lệnh DML vừa kết thúc. Khi trigger được tạo nếu không có thiết lập gì thì mặc định là after và không sử dụng cho bảng ảo
-	Instead of trigger: trigger loại này hoạt động khác một chút: B1:các lệnh DML vẫn được gọi để thực thi. B2: dữ liệu chưa bị thay đổi. B3: các lệnh instead of trigger sẽ được thực thi. Như vậy dựa trên cách thức hoạt động của nó thì ta có thể thấy thực chất các lệnh DML tác động trên bảng có gắn trigger instead of thì nó chỉ mang tính chất phát sinh sự kiện kích hoạt bên trong trigger thực thi. 
•	Cú pháp trigger
 
Ví dụ:
 
Bật tắt trigger:
 
Delete and inserted table:
-	Đoạn mã chứa trong 1 trigger có thể truy cập đến 2 bảng logic các bảng này là bộ phận của bẫy lỗi và được gọi là inserted và deleted
-	Bảng inserted và deleted chứa ảnh của dữ liệu trước và sau quá trình cập nhật dữ liệu trong bảng không bị tác động bơi thao tác cập nhật thì sẽ không nằm trong bảng inserted và deleted. Chúng được lưu trữ trong bộ nhớ mà không phải lưu trữ trên đĩa
-	Bảng inserted chứa dữ liệu được thêm mới trong hành động insert hoặc update. Bảng này có ở cả 2 loại trigger
-	Bảng delete chứa dữ liệu bị xoá trong hành động delete hoặc update, bảng này có ở cả 2 loại trigger
 

Advanced SQL - Lecture 07: UDF & SQL Code Practice
User define function: Hàm do người dùng định nghĩa
•	Hàm là đối tượng CSDL tương tự như thủ tục lưu trữ, điểm khác biệt giữa hàm và thủ tục là: Hàm trả về giá trị thông qua tên hàm, còn thủ tục thì không. Điều này cho phép ta sử dụng hàm như một biểu thức chẳng hạn bạn có thể gọi hàm trong danh sách chọn của lệnh select. Ngoài những hàm do CSDL cũng cấp sẵn người sử dụng có thể định nghĩa thêm các hàm có thể phục vụ mục đích riêng của mình
•	Hàm do người dùng định nghĩa thông thường sẽ nhận một tham số đầu vào
•	Thực hiện một công việc và trả về kết quả, giá trị trả về có thể là giá trị đơn hoặc tập kết quả
•	Phân loại hàm người dùng(UDF type) :Về phân loại tuỳ thuộc kết quả trả về của hàm mà chia loại như sau
-	Hàm vô hướng: tức là trả về giá trị đơn, giá trị trả về thuộc một trong các giá trị kiểu (in,char,varchar.v.v.v). Nhưng không hỗ trợ trả về kiểu Text, ntext, image, timestamp
-	Hàm trả về một bảng: loại này chia thành: 
	Hàm trả về bảng từ truy vấn đơn
	Hàm trả về bảng từ truy vấn nhiều câu lệnh
•	Cú pháp UDF scalar function
 
Cú pháp trả về inline table-valued function
 
Hàm multi-statement table-valued function
 
•	Code practice
-	Lời khuyên liên quan đến việc transaction: nên dùng các transaction cho thao tác thay đổi dữ liệu delete,insert, update. Điều đó giúp ta đảm bảo đặc tính “ACID” quan trọng của CSDL
	Atomicity,Consystence, Isolation, Durability: tính nguyên tố, nhất quán, tách biệt và bền vững
	Transaction được dùng để đảm bảo tính toàn vẹn dữ liệu khi xảy ra cập nhật, cập nhật sẽ được hiểu theo nghĩa rộng là các hành động sửa đổi dữ liệu như insert,update,delete. Khi một transaction bao gồm nhiều lệnh cập nhật nó đảm bảo các lệnh cập nhật đều thành công hoặc trong trường hợp 1 lệnh gặp sự cố thì toàn bộ transaction bị huỷ bỏ, khi đó dữ liệu trở về trạng thái ban đầu. Nói cách khác transaction ngăn chặn tình huống dữ liệu cập nhật nửa chừng(trong đó 1 phần đc cập nhật, một phần bị bỏ qua)
	Transaction properties(ACID): Automicity là tính nguyên tố, thuộc tính này đảm bảo mỗi transaction là một khối duy nhất được thực hiện trọn vẹn hoặc hoàn toàn không được thực hiện trọn vẹn hoặc hoàn toàn không được thực hiện, nếu có một lỗi nào đó xảy ra trong transaction nó sẽ đc rollback về trạng thái ban đầu
	Consistency: tính nhất quán SQL server ở mọi thời điểm dữ liệu đều phải nhất quán, tuân theo các ràng buộc được định nghĩa. Ví dụ: trường kiểu ngày phải có dữ liệu kiểu ngày giờ, bản ghi bán hàng phải có mã sản phẩm hợp lệ. Khi transaction được thực hiện dữ liệu sau khi được cập nhật phải ở trạng thái nhất quán, nếu transaction gây ra những vi phạm về ràng buộc dữ liệu thì hệ thống sẽ không cho phép thực hiện tiếp và huỷ bỏ toàn bộ transaction
	Isolation: tính tách biệt cũng như các server khác thì SQL có thể đáp ứng nhiều yêu cầu xảy ra cùng lúc nhưng mỗi transaction được đảm bảo theo một ngữ cảnh riêng biệt của nó và không bị ảnh hưởng bởi các transaction khác, khi 2 transaction cùng cập nhật 1 dữ liệu thi SQL đảm bảo chúng thực hiện tuần tự không dẫm lên chan của nhau
	Durability: tính bền vững khi transaction thực hiện xong đã commit những cập nhật đã trở nên cố định và dữ liệu sẽ luôn cố định, khi hệ thống gặp sự cố thì trong quá trình khôi phục nó sẽ đảm bảo dữ liệu cho những transaction đã commit
-	Lời khuyên liên quan đến câu lệnh dùng Stored proceduce
-	Lời khuyên khi dùng truy vấn con(subquery)
-	Lời khuyên dùng cho biểu thức câu lệnh truy vấn
 




