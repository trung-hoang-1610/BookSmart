# BookSmart - Ứng dụng hỗ trợ đặt phòng khách sạn 🏨

**BookSmart** là nền tảng giúp người dùng tìm kiếm và đặt phòng khách sạn nhanh chóng, gồm:  

- Mobile App (Flutter): Ứng dụng di động cho khách hàng đặt phòng.
- API Backend (ASP.NET Core MVC): Hệ thống API quản lý logic nghiệp vụ và kết nối cơ sở dữ liệu.
- Admin Website (ASP.NET Core MVC): Giao diện quản trị cho quản lý khách sạn, phòng và đơn đặt phòng.

## Source Code  
- Mobile App (Flutter): https://github.com/trung-hoang-1610/BookSmart-Flutter-UI.git 
- API Backend (ASP.NET Core): https://github.com/trung-hoang-1610/BookSmart-API.git  
- Admin Website (ASP.NET Core MVC): https://github.com/trung-hoang-1610/BookSmart-Admin-Dashboard.git

---

## Chức Năng Chính
### Ứng dụng Mobile (Client)
- Tìm kiếm theo địa điểm, tên khách sạn, và các tiêu chí khác.
- Hiển thị hình ảnh, mô tả, tiện nghi của các phòng, đánh giá.
- Gửi yêu cầu đặt phòng trực tuyến và chờ xác nhận.
- Xem lịch sử đặt phòng, chi tiết đặt phòng và trạng thái giao dịch.
  
### API Backend
- Xử lý các nghiệp vụ liên quan đến khách sạn, phòng, người dùng và đơn đặt phòng.
- Sử dụng JWT Authentication để bảo mật API.

### Trang Web Admin
**Quản lý hệ thống:**  
  - Admin: Quản lý toàn bộ hệ thống, duyệt đơn đặt phòng, quản lý người dùng, và giám sát hoạt động của ứng dụng.
  - Chủ Khách Sạn: Quản lý thông tin khách sạn và phòng của mình, theo dõi đơn đặt phòng liên quan đến khách sạn mà mình sở hữu.
**Các chức năng chính:**
  - Tạo, chỉnh sửa và xóa thông tin khách sạn và phòng.
  - Xác nhận hoặc hủy đơn đặt phòng.
  - Quản lý tài khoản người dùng.

---

## Hướng dẫn chạy dự án  
**Yêu cầu:** Flutter SDK, .NET Core SDK, SQL Server  
1. **Clone các repository:**
   - Mobile App: `git clone https://github.com/trung-hoang-1610/BookSmart-Flutter-UI.git`
   - API Backend: `git clone https://github.com/trung-hoang-1610/BookSmart-API.git`
   - Admin Website: `git clone https://github.com/trung-hoang-1610/BookSmart-Admin-Dashboard.git`
   - File backup CSDL (.bak): https://drive.google.com/file/d/1NjUuBkg6PdqPxcpL5RdYx0hV1QGCb1wL/view

2. **Chạy API Backend:**
   - Mở terminal, chuyển đến thư mục chứa mã nguồn của API.
   - Cài đặt các gói cần thiết: `dotnet restore`
   - Áp dụng migration: `dotnet ef database update`
   - Chạy API
   - API mặc định chạy trên `http://localhost:5000` (có thể thay đổi cấu hình cho phù hợp).

3. **Chạy Ứng Dụng Mobile:**
   - Mở project Flutter trong IDE (VS Code/Android Studio).
   - Cài đặt các package: `flutter pub get`
   - Chạy ứng dụng: `flutter run`  
     (Đảm bảo cấu hình API endpoint trong code trỏ đến `http://localhost:5000` hoặc endpoint đã triển khai)

4. **Chạy Web Admin:**
   - Mở terminal, chuyển đến thư mục Web Admin.
   - Cài đặt các gói: `dotnet restore`
   - Chạy ứng dụng: `dotnet run`
   - Truy cập trang
   
---

## Công Nghệ Sử Dụng

- **Front-end:** Flutter, Dart, Bloc 
- **Backend:** ASP.NET Core MVC, Entity Framework Core, SQL Server
- **Admin Dashboard:** ASP.NET Core MVC, Bootstrap/CSS
- **Bảo mật:** JWT Authentication

---

**Liên hệ:** 161002trung@gmail.com

