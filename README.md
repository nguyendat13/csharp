# Employee Management System (WPF)

Ứng dụng desktop được xây dựng bằng **WPF (Windows Presentation Foundation)** với ngôn ngữ **C#**, hỗ trợ các doanh nghiệp quản lý nhân viên, vai trò và phòng ban một cách hiệu quả.  
Ứng dụng áp dụng mô hình **MVVM (Model-View-ViewModel)** kết hợp với **Entity Framework Core** để thao tác với cơ sở dữ liệu.

---

## Chức năng chính

### Nhân viên
- Thêm, sửa, xóa thông tin nhân viên.  
- Tìm kiếm, lọc nhân viên theo nhiều tiêu chí.  

### Phòng ban và vai trò
- Quản lý phòng ban.  
- Quản lý vai trò nhân viên.  

### Hệ thống
- Lưu trữ dữ liệu vào cơ sở dữ liệu cục bộ (**SQL Server hoặc SQLite**).  
- Giao diện WPF trực quan, thân thiện với người dùng, thiết kế theo mô hình **MVVM**.  

---

## Công nghệ sử dụng

### Ngôn ngữ và nền tảng
- .NET (C#)  
- WPF (XAML)  
- MVVM Architecture  

### Cơ sở dữ liệu
- SQL Server / SQLite  
- Entity Framework Core (ORM)  

---

## Hướng dẫn cài đặt

### Yêu cầu
- Visual Studio 2022 trở lên  
- Đã cài workload **.NET Desktop Development**  
- SQL Server hoặc SQLite  

### Clone repository
```bash
git clone https://github.com/nguyendat13/employee-management-wpf.git
Mở dự án

Mở file .sln trong Visual Studio.

Cấu hình cơ sở dữ liệu

Chỉnh sửa chuỗi kết nối trong appsettings.json hoặc DbContext.

Chạy migration và khởi tạo database
dotnet ef database update

Chạy ứng dụng

Nhấn Start trong Visual Studio để khởi động ứng dụng.

Cấu trúc dự án
├── Models/           # Các lớp dữ liệu (Entity)
├── ViewModels/       # Business logic theo mô hình MVVM
├── Views/            # Giao diện XAML
├── Data/             # DbContext và cấu hình database
├── App.xaml          # File cấu hình ứng dụng
└── Program.cs        # Điểm khởi đầu của ứng dụng
