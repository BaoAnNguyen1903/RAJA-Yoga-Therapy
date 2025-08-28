# RAJA Yoga & Therapy Website

Website chính thức của RAJA Yoga & Therapy - Trung tâm chăm sóc sức khỏe và yoga tại Đà Nẵng.

## 🚀 Tính năng

- ✅ **Responsive Design** - Tương thích mọi thiết bị
- ✅ **Đa ngôn ngữ** - Tiếng Anh và Tiếng Việt
- ✅ **Form liên hệ hoạt động** - Gửi tin nhắn thực tế
- ✅ **Lịch học responsive** - Hiển thị tốt trên mọi màn hình
- ✅ **Map Google Maps** - Responsive và tương tác
- ✅ **Giao diện hiện đại** - Thiết kế đẹp mắt với Tailwind CSS

## 📋 Cài đặt Form Liên Hệ

### 🔴 Phương án 1: Formspree (KHUYẾN NGHỊ - MIỄN PHÍ)

1. **Đăng ký tài khoản**
   - Truy cập [https://formspree.io/](https://formspree.io/)
   - Đăng ký tài khoản miễn phí

2. **Tạo form mới**
   - Click "New Form"
   - Đặt tên form (ví dụ: "RAJA Contact Form")
   - Chọn email nhận tin nhắn

3. **Lấy Form ID**
   - Copy Form ID từ dashboard
   - Ví dụ: `xrgjqkzw`

4. **Cập nhật config**
   - Mở file `config.js`
   - Thay thế `your_actual_form_id_here` bằng Form ID thực tế:
   ```javascript
   window.FORMSPREE_FORM_ID = 'xrgjqkzw';
   ```

5. **Kiểm tra**
   - Form sẽ hoạt động ngay lập tức!
   - Tin nhắn sẽ được gửi đến email của bạn

### 🔵 Phương án 2: EmailJS (Nhiều tính năng hơn)

1. **Đăng ký EmailJS**
   - Truy cập [https://www.emailjs.com/](https://www.emailjs.com/)
   - Tạo tài khoản

2. **Thiết lập Email Service**
   - Kết nối Gmail, Outlook hoặc email khác
   - Lấy Service ID

3. **Tạo Email Template**
   - Tạo template email
   - Lấy Template ID

4. **Cập nhật config**
   ```javascript
   // Trong config.js
   window.EMAILJS_PUBLIC_KEY = 'your_public_key';
   window.EMAILJS_SERVICE_ID = 'your_service_id';
   window.EMAILJS_TEMPLATE_ID = 'your_template_id';
   ```

## 🛠️ Cấu trúc dự án

```
RAJA/
├── index.html          # Trang chính
├── config.js           # Cấu hình (KHÔNG commit lên git)
├── .gitignore          # Danh sách file bỏ qua
├── README.md           # Hướng dẫn này
├── images/             # Thư mục hình ảnh
│   └── logo.png       # Logo RAJA
└── .env.example        # File mẫu biến môi trường
```

## 🔐 Bảo mật

- **KHÔNG BAO GIỜ** commit file `config.js` lên git
- File `.gitignore` đã được cấu hình để bảo vệ thông tin nhạy cảm
- Sử dụng biến môi trường hoặc file config riêng

## 📱 Responsive Breakpoints

- **Mobile**: < 768px (md:hidden)
- **Tablet**: 768px - 1023px (md:block lg:hidden)  
- **Desktop**: ≥ 1024px (lg:block)

## 🎨 Customization

### Màu sắc chính
- **Primary**: #B94C6F (Hồng đậm)
- **Secondary**: #F4A6B8 (Hồng nhạt)
- **Accent**: #F7D7DD (Hồng rất nhạt)

### Fonts
- **Heading**: Playfair Display
- **Body**: Inter

## 🚀 Triển khai

1. **Local Development**
   ```bash
   # Mở file index.html trong trình duyệt
   # Hoặc sử dụng Live Server extension trong VS Code
   ```

2. **Production**
   - Upload tất cả file lên hosting
   - Đảm bảo `config.js` được cập nhật với Form ID thực tế
   - Kiểm tra form hoạt động

## 📞 Hỗ trợ

Nếu gặp vấn đề với form liên hệ:
1. Kiểm tra Form ID trong `config.js`
2. Xem console browser để debug
3. Kiểm tra kết nối internet
4. Đảm bảo Formspree form đang hoạt động

## 📄 License

© 2025 RAJA Yoga & Therapy. All rights reserved.

---

**Lưu ý**: Đây là website demo với form liên hệ hoạt động thực tế. Hãy cập nhật thông tin liên hệ và nội dung phù hợp với doanh nghiệp của bạn.
