Câu 1.
a) Ý nghĩa của tính đóng gói: Đóng gói giúp ẩn giấu chi tiết cài đặt bên trong đối tượng và chỉ cung cấp các phương thức/thuộc tính công khai ra ngoài. Điều này ngăn chặn dữ liệu bị chỉnh sửa trái phép, đảm bảo tính toàn vẹn của dữ liệu và giảm sự phụ thuộc lẫn nhau giữa các thành phần.

b) Phân biệt các Access Modifiers:
private: Chỉ có thể truy cập nội bộ bên trong cùng một lớp.
protected: Có thể truy cập nội bộ trong lớp đó và các lớp con kế thừa.  
internal: Có thể truy cập từ bất kỳ lớp nào trong cùng một file Assembly (project/chương trình).
public: Có thể truy cập tự do từ bất kỳ đâu.

c) Từ khóa init trong C# 9+: Dùng để khai báo thuộc tính Read-Only chỉ khởi tạo một lần duy nhất tại thời điểm tạo đối tượng (qua Constructor hoặc Object Initializer).
Khác biệt so với set: Mệnh đề set cho phép ghi lại giá trị của thuộc tính bất kỳ lúc nào trong suốt vòng đời của đối tượng, còn init chỉ cho phép gán giá trị tại thời điểm khởi tạo và chặn việc sửa đổi sau đó.

Câu 2.
C# không hỗ trợ đa kế thừa đối với Lớp (một lớp con chỉ kế thừa duy nhất 1 lớp cha). Sử dụng dấu hai chấm : để khai báo sự kế thừa (vd: class Con : Cha). 
Sử dụng từ khóa base trong Constructor lớp con: Từ khóa base(...) được gọi tại khai báo Constructor lớp con để thực thi Constructor của lớp cha trước, giúp truyền các tham số dùng chung lên cho lớp cha khởi tạo.
Tác dụng của từ khóa sealed trước Class: Từ khóa sealed niêm phong lớp, ngăn chặn các lớp khác tiếp tục kế thừa từ lớp đó.
Câu 3.
sự khác biệt : 
Compile-time Polymorphism (Method Overloading): Xảy ra khi các phương thức cùng tên nằm trong một lớp nhưng khác tham số/kiểu dữ liệu. Trình biên dịch xác định hàm cần gọi ngay trong quá trình biên dịch.
Runtime Polymorphism (Method Overriding): Xảy ra khi lớp con định nghĩa lại hành vi phương thức của lớp cha. Trình biên dịch xác định hàm thực thi tại thời điểm chương trình chạy dựa vào kiểu của đối tượng thực sự.
Để phương thức ở lớp cha có thể bị ghi đè: dùng từ khóa virtual (hoặc abstract) ở lớp cha.  
Phương thức ở lớp con muốn ghi đè: dùng từ khóa override. 
