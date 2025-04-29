# BeautySkyShop - E-commerce Cosmetics Platform 🌿

<div align="center">
  <picture>
    <img alt="BeautySky Logo" src="/BeautySky-FE/src/assets/screenshot/SkyBeauty-removebg-preview.png" width="200">
  </picture>
</div>

<div align="center">
  <h1>BeautySkyShop - Nền tảng Thương mại điện tử Mỹ phẩm</h1>
  <p>Nền tảng thương mại điện tử hiện đại cho công ty mỹ phẩm, cho phép người dùng khám phá sản phẩm, đọc blog, xác định loại da, tìm phác đồ chăm sóc da phù hợp và mua sắm thông minh.</p>
</div>

## 📸 Preview

<div align="center">
  <h3>Home Page</h3>
  <img src="/BeautySky-FE/src/assets/screenshot/HomePage.png" alt="Home Page" />
  <p><em></em></p>

  <h3>Product Interface</h3>
  <img src="/BeautySky-FE/src/assets/screenshot/Product.png"/>
  <p><em></em></p>

  <h3>Dashboard</h3>
  <img src="/BeautySky-FE/src/assets/screenshot/DashBoard.png" alt="Dashboard" />
  <p><em></em></p>
</div>

## 🌐 Live Demo & API Documentation

- Website: `<YOUR_FRONTEND_DEPLOYMENT_URL>`
- API Documentation: `<API_DOCS_URL>`
- API Base URL: `http://localhost:7112`

## ✨ Tính năng nổi bật

### Giao diện người dùng
- Trang chủ tương tác giới thiệu công ty và sản phẩm
- Blog và nền tảng chia sẻ tin tức
- Đánh giá loại da thông qua bài kiểm tra
- Đề xuất routine chăm sóc da cá nhân hóa
- Gợi ý sản phẩm thông minh dựa trên loại da
- Tính năng so sánh sản phẩm
- Quản lý đơn hàng và lịch sử mua sắm
- Đánh giá và phản hồi sản phẩm

### Quản lý và Bảo mật
- Xác thực JWT và phân quyền người dùng
- Tích hợp thanh toán an toàn qua VNPAY
- Lưu trữ hình ảnh trên Amazon S3
- Quản lý khuyến mãi và chương trình tích điểm
- Dashboard quản trị và báo cáo
- Bảo mật đa lớp (rate limiting, SQL injection, XSS protection)

## 🛠 Tech Stack

### Frontend
- **Framework:** React.js (Vite)
- **Styling:** Tailwind CSS
- **State Management:** Context API
- **Routing:** React Router
- **API Calls:** Axios
- **Authentication:** JWT-based authentication

### Backend
- **Framework:** ASP.NET Web API
- **Database:** Microsoft SQL Server
- **Authentication:** JWT (JSON Web Tokens)
- **Cloud Storage:** Amazon S3
- **Payment Processing:** VNPAY
- **Documentation:** Swagger/OpenAPI

## 🚀 Hướng dẫn cài đặt

### Yêu cầu hệ thống
- Node.js (v16+)
- .NET SDK 8.0+
- Microsoft SQL Server
- Tài khoản Amazon S3 & VNPAY

### Cài đặt Frontend

1. Clone repository:
   ```bash
   git clone https://github.com/huynhtoan3152004/BeautySky-FE.git
   ```

2. Di chuyển vào thư mục dự án:
   ```bash
   cd beautyskyshop-frontend
   ```

3. Cài đặt dependencies:
   ```bash
   npm install
   ```

4. Cấu hình môi trường:
   ```bash
   cp .env.example .env
   ```
   ```bash
   VITE_API_KEY = <Your localhost BE>
   ```

5. Khởi chạy development server:
   ```bash
   npm run dev
   ```
   Frontend sẽ chạy tại `http://localhost:5173`

### Cài đặt Backend

1. Clone repository:
   ```bash
   git clone https://github.com/huynhtoan3152004/BeautySky-BE.git
   ```

2. Di chuyển vào thư mục dự án:
   ```bash
   cd beautyskyshop-backend
   ```

3. Chạy migration database:
   ```bash
   dotnet ef database update
   ```

4. Khởi chạy server:
   ```bash
   dotnet run
   ```
   API sẽ chạy tại `http://localhost:7112`

### Cấu hình Backend (appsettings.json)

```json
{
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  },
  "AllowedHosts": "*",
  "ConnectionStrings": {
    "MyDBConnection": ""
  },
  "JWT": {
    "ValidAudience": "User",
    "ValidIssuer": "https://localhost:7112",
    "Secret": ""
  },
  "Authentication": {
    "Google": {
      "ClientId": "",
      "ClientSecret": "_"
    }
  },
  "AWS": {
    "BucketName": "beautysky",
    "AccessKey": "",
    "SecretKey": "",
    "Region": "ap-southeast-2"
  },
  "Vnpay": {
    "TmnCode": "",
    "HashSecret": "",
    "BaseUrl": "",
    "Command": "pay",
    "CurrCode": "VND",
    "Version": "2.1.0",
    "Locale": "vn",
    "PaymentBackReturnUrl": "",
    "UsdToVndRate": 24500
  },
  "TimeZoneId": "SE Asia Standard Time"
}
```

## 🧪 Kiểm thử

- Xác thực và phân quyền người dùng
- Quy trình đặt hàng và quản lý
- Xử lý thanh toán (thành công/thất bại)
- Đánh giá loại da và đề xuất
- Kiểm tra bảo mật

## 👥 Đóng góp

1. Fork repository
2. Tạo nhánh tính năng: `git checkout -b feature/amazing-feature`
3. Commit thay đổi: `git commit -m 'Add some amazing feature'`
4. Push lên nhánh: `git push origin feature/amazing-feature`
5. Tạo Pull Request

## 📄 Giấy phép

Dự án được phát hành dưới giấy phép MIT - xem chi tiết tại [LICENSE.md](LICENSE.md)

## 🤝 Hỗ trợ & Liên hệ

### Frontend Team
- Email: `haile170504@gmail.com`
- Email: `huynhhuutoanwork@gmail.com`
- Email: `danhthanh18102004@gmail.com`
- Email: `uyennhi01022004@gmail.com`

### Backend Support
- API Issues: Tạo issue trên GitHub
- Email: `haile170504@gmail.com`
- Email: `huynhhuutoanwork@gmail.com`
- Email: `danhthanh18102004@gmail.com`

## 🙏 Lời cảm ơn

- Cảm ơn tất cả thành viên đã đóng góp cho dự án
- Đặc biệt cảm ơn thầy [Nguyen The Hoang](https://github.com/doit-now) đã hướng dẫn
- Trân trọng cộng đồng mã nguồn mở vì những công cụ tuyệt vời

<div align="center">
  Made with ❤️ by the BeautySky Team
</div>
