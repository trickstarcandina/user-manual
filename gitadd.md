"git add ."
Câu lệnh trên sẽ add
+ Các thay đổi trên các file đã tồn tại sẵn.
+ Các file mới được tạo ra.

"git add -u ."
Câu lệnh trên sẽ add
+ Các thay đổi trên các file đã tồn tại sẵn.
+ Các file đã bị xóa.

"git add -A"
Câu lệnh trên sẽ add cả 3 loại:
+Các thay đổi trên các file đã tồn tại sẵn.
+Các file mới được tạo ra.
+Các file đã bị xóa.

Lưu ý:
"add *" có nghĩa là thêm tất cả các tệp trong thư mục hiện tại, ngoại trừ các tệp có tên bắt đầu bằng dấu chấm. Đây là chức năng shell của bạn và Git chỉ nhận được một danh sách các tệp.

"add . "không có ý nghĩa đặc biệt trong trình bao của bạn, và do đó Git thêm toàn bộ thư mục một cách đệ quy, gần như giống nhau, nhưng bao gồm các tệp có tên bắt đầu bằng dấu chấm.
