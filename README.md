# TranAnhDuc_22661261_GK_LTHSK

Repository chứa bài tập/đồ án môn LTHSK của Trần Anh Đức (MSSV: 22661261).

## Mô tả
Project Node.js sử dụng Express, Mongoose và có test bằng Mocha/Chai. Có thể dùng RabbitMQ (amqplib) tuỳ module.

## Yêu cầu
- Node.js >= 16
- npm
- MongoDB (nếu project dùng mongoose)
- RabbitMQ (nếu dùng amqplib)

## Cài đặt
1. Mở PowerShell tại thư mục project:
   ```powershell
   cd C:\TranAnhDuc_22661261_GK_LTHSK
   ```
2. Cài dependencies:
   ```bash
   npm install
   ```

## Biến môi trường
Tạo file `.env` ở gốc (không commit). Ví dụ:
```env
PORT=3000
MONGO_URI=mongodb://localhost:27017/mydb
JWT_SECRET=your_jwt_secret
RABBITMQ_URL=amqp://localhost
```

## Chạy ứng dụng
- Nếu entry là `index.js`:
```bash
node index.js
```
- Hoặc thêm script `start` vào `package.json` và chạy:
```bash
npm start
```

## Chạy test
```bash
npm test
```
(Test sử dụng Mocha; tham số timeout được cấu hình trong `package.json`.)

## Cấu trúc thư mục (ví dụ)
- /auth - dịch vụ xác thực
- /product - dịch vụ product
- /order - dịch vụ order
- index.js - điểm khởi động chính
- package.json
- .env (local)

(Giá trị thực tế có thể khác; tham khảo mã nguồn cụ thể trong repo.)

## Git / Push lên GitHub
Nếu chưa có repo remote:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/DavidBeckD23/TranAnhDuc_22661261_GK_LTHSK.git
git push -u origin main
```
Lưu ý: với HTTPS, sử dụng Personal Access Token (PAT) khi GitHub yêu cầu mật khẩu.

## Ghi chú
- Đảm bảo thêm `.env` vào `.gitignore` (đã có).
- Cập nhật README nếu thêm hướng dẫn khởi động từng service hoặc cấu hình chi tiết.

## License
ISC
