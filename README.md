# ASPNguyenThanhDanh
![image](https://github.com/user-attachments/assets/eed1648a-d289-4944-80f8-8601a4fce527)

cách thức hoạt động của chức năng và giao diện trong ứng dụng mã hóa và giải mã file AES:

1. Chức năng
a. Mã hóa file
Nhập khóa: Người dùng nhập khóa AES (16 ký tự).
Chọn file: Người dùng chọn file cần mã hóa.
Mã hóa:
Ứng dụng tạo một vector khởi tạo (IV) ngẫu nhiên.
Dữ liệu file được đọc và được thêm padding để phù hợp với kích thước khối của AES.
Dữ liệu được mã hóa bằng thuật toán AES trong chế độ CBC.
Kết quả mã hóa (bao gồm IV) được lưu vào file mới với đuôi .enc.

b. Giải mã file
Nhập khóa: Người dùng nhập khóa AES (phải giống với khóa đã dùng để mã hóa).
Chọn file đã mã hóa: Người dùng chọn file có đuôi .enc.
Giải mã:
Ứng dụng đọc IV từ đầu file đã mã hóa.
Dữ liệu được giải mã và loại bỏ padding.
Kết quả giải mã được lưu vào file mới, không có đuôi .enc.


2. Quy trình hoạt động
Mở ứng dụng: Người dùng truy cập vào địa chỉ ứng dụng.
Nhập thông tin: Nhập khóa và chọn file.
Thực hiện thao tác: Nhấn nút mã hóa hoặc giải mã.
Nhận kết quả: Ứng dụng hiển thị thông báo và lưu file kết quả.
