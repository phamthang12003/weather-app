# 🌤️ React Weather App

Một ứng dụng tra cứu thời tiết giao diện hiện đại, trực quan được phát triển bằng ReactJS và Vite. Ứng dụng gọi dữ liệu từ OpenWeatherMap API để cung cấp thông tin thời tiết theo thời gian thực cho bất kỳ thành phố nào trên thế giới.

## ✨ Tính năng nổi bật
* **Tra cứu nhanh chóng:** Nhập tên thành phố và nhận kết quả tức thì.
* **Thông tin chi tiết:** Hiển thị nhiệt độ chuẩn xác (°C), phần trăm độ ẩm và tốc độ gió.
* **Giao diện động:** Tự động thay đổi biểu tượng thời tiết (trời quang, nhiều mây, mưa, mưa phùn, tuyết rơi) khớp với mã dữ liệu trả về từ API.

## 🛠️ Công nghệ sử dụng
* **Môi trường & Framework:** Vite, ReactJS.
* **Giao diện (UI/UX):** HTML5, CSS3 (`Weather.css`, `index.css`).
* **Lấy dữ liệu (Fetching):** `fetch` API, sử dụng `async/await`.
* **Quản lý state:** React Hooks (`useState`, `useEffect`, `useRef`).

## 📁 Cấu trúc dự án
Dự án được tổ chức gọn gàng theo chuẩn kiến trúc Component của React:

```text
weather/
├── public/
│   └── vite.svg              
├── src/
│   ├── assets/                # Chứa các icon (clear.png, cloud.png, rain.png...)
│   ├── components/            # Chứa component chính: Weather.jsx và Weather.css
│   ├── App.jsx               
│   ├── index.css             
│   └── main.jsx              
├── .env                       # Chứa khóa API bảo mật (VITE_APP_ID)
├── .gitignore                
├── package.json              
└── vite.config.js

🚀 Hướng dẫn Cài đặt & Khởi chạy
Để chạy dự án này trên máy tính cá nhân, hãy thực hiện theo các bước sau:

1. Clone repository
Mở Terminal/Command Prompt và chạy lệnh:

Bash
git clone [https://github.com/phamthang12003/weather-app.git](https://github.com/phamthang12003/weather-app.git)
cd weather
2. Cài đặt thư viện (Dependencies)
Bash
npm install
3. Cấu hình biến môi trường API
Dự án này sử dụng OpenWeatherMap API. Bạn cần khai báo khóa API của mình để ứng dụng hoạt động:

Tạo một file có tên .env ngay tại thư mục gốc của dự án.

Thêm dòng sau vào file .env (thay thế bằng API Key thật của bạn):

Đoạn mã
VITE_APP_ID="your_openweathermap_api_key_here"

4. Khởi chạy môi trường phát triển (Dev Server)
Bash
npm run dev
Mở trình duyệt và truy cập vào đường dẫn cục bộ (thường là http://localhost:5173) để trải nghiệm ứng dụng.