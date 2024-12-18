# 📋 Dự án Đặt Lịch Hẹn Khám Sức Khỏe

## 💡 Thông tin nhóm
- **Tên nhóm:** Mixture-Tech
- **Thành viên nhóm:**  
  - Nguyễn Văn Hoàng
  - Dương Hoàng Châu

---

## 🔧 Công nghệ sử dụng

### Backend:
- **Ngôn ngữ:** Java (Spring Boot)
- **Cơ sở dữ liệu:** MySQL
- **Bảo mật:** Spring Security, JWT
- **Mapping:** MapStruct

### Frontend:
- **Ngôn ngữ:** ReactJS
- **Thư viện hỗ trợ:** Axios, React Router

### Khác:
- **Triển khai:** Docker
- **API Documentation:** Swagger
- **Quản lý mã nguồn:** GitHub

---

## 🌟 Chức năng chính

1. **Người dùng:**
   - Đăng ký tài khoản (vai trò: Bệnh nhân, Bác sĩ, Quản trị viên)
   - Đăng nhập/Đăng xuất
   - Đặt lịch hẹn khám (cho bản thân hoặc người thân)
   - Quản lý lịch hẹn (xem, cập nhật, hủy lịch hẹn)

2. **Bác sĩ:**
   - Quản lý hồ sơ cá nhân
   - Xác nhận và quản lý lịch hẹn khám của bệnh nhân

3. **Quản trị viên:**
   - Quản lý tài khoản người dùng
   - Quản lý danh sách bác sĩ và chuyên khoa

4. **Hệ thống:**
   - Gửi thông báo qua email khi đặt lịch hoặc thay đổi trạng thái lịch hẹn

---

## 📡 Danh sách các API chính

### Người dùng (User):
- **POST** `/api/v1/auth/register` - Đăng ký tài khoản
- **POST** `/api/v1/auth/login` - Đăng nhập
- **GET** `/api/v1/users/{id}` - Xem thông tin cá nhân

### Lịch hẹn (Appointment):
- **POST** `/api/v1/appointments` - Đặt lịch hẹn mới
- **GET** `/api/v1/appointments` - Danh sách lịch hẹn của người dùng
- **PUT** `/api/v1/appointments/{id}` - Cập nhật lịch hẹn
- **DELETE** `/api/v1/appointments/{id}` - Hủy lịch hẹn

### Bác sĩ (Doctor):
- **GET** `/api/v1/doctors` - Danh sách bác sĩ
- **GET** `/api/v1/doctors/{id}` - Thông tin bác sĩ

### Chuyên khoa (Specialization):
- **GET** `/api/v1/specializations` - Danh sách chuyên khoa

---

## 🚀 Hướng dẫn cài đặt và chạy dự án

### Yêu cầu hệ thống:
- **Java:** JDK 17 trở lên
- **Node.js:** 16.x trở lên
- **MySQL:** 8.0

### Các bước cài đặt:
1. **Clone dự án:**
   ```bash
   git clone https://github.com/Mixture-Tech/healthcare-appointment.git
   ```

2. **Cài đặt backend:**
   - Di chuyển vào thư mục `back-end`
   - Cấu hình file `application.properties` theo thông tin MySQL
   - Chạy lệnh:
     ```bash
     ./mvnw spring-boot:run
     ```

3. **Cài đặt frontend:**
   - Di chuyển vào thư mục `front-end`
   - Chạy lệnh:
     ```bash
     npm install
     npm start
     ```

4. **Truy cập ứng dụng:**
   - Backend API: [http://localhost:4000](http://localhost:4000)
   - Frontend: [http://localhost:3000](http://localhost:3000)

---

## 📚 Tài liệu và liên hệ
- **Swagger API Documentation:** [http://localhost:4000/swagger-ui.html](http://localhost:4000/swagger-ui.html)
- **Email liên hệ:** mixture-tech@gmail.com

---

> **Lưu ý:** Đây là dự án mẫu được phát triển bởi nhóm Mixture-Tech nhằm mục đích học tập và nghiên cứu.
