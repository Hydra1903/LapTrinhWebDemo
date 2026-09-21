# Ẩm Thực Miền Tây — Website Du Lịch Ẩm Thực

Website giới thiệu các món ăn đặc sản khu vực miền Tây Nam Bộ Việt Nam, phục vụ mục đích quảng bá du lịch.

## Cấu trúc dự án

```
project/
├── index.html        # Trang chủ
├── about.html        # Đồng Bằng Ẩm Thực (giới thiệu vùng)
├── products.html     # 20 Món Đặc Sản + Các loại bánh
├── contact.html      # Liên hệ & form gửi tin nhắn
├── css/
│   └── style.css     # Toàn bộ stylesheet (responsive)
├── images/           # Thư mục chứa ảnh cục bộ (xem ghi chú)
└── README.md
```

## Trang web gồm

| Trang | File | Nội dung |
|-------|------|----------|
| Trang Chủ | `index.html` | Hero, giới thiệu, 3 món nổi bật, trải nghiệm |
| Đồng Bằng Ẩm Thực | `about.html` | Lịch sử, 13 tỉnh thành, đặc trưng ẩm thực |
| 20 Món Đặc Sản | `products.html` | Grid 20 món chính + 6 loại bánh miền Tây |
| Liên Hệ | `contact.html` | Form liên hệ, thông tin, FAQ |

## Công nghệ sử dụng

- **HTML5** — cấu trúc ngữ nghĩa (semantic HTML)
- **CSS3** — định dạng giao diện, không dùng framework
  - CSS Custom Properties (biến màu, font)
  - CSS Grid & Flexbox (bố cục)
  - Media Queries (responsive)
  - CSS-only hamburger menu (không cần JavaScript)
- **Google Fonts** — Playfair Display (tiêu đề) + Nunito (nội dung)

## Responsive

| Màn hình | Breakpoint | Bố cục |
|----------|------------|--------|
| Desktop  | > 900px    | 4 cột |
| Tablet   | 640–900px  | 3 cột |
| Mobile   | 480–640px  | 2 cột |
| Mobile S | < 480px    | 1–2 cột |

## Ghi chú về hình ảnh

Hiện tại hình ảnh đang dùng URL từ **Unsplash** (CDN online) để làm placeholder.

Để dùng ảnh cục bộ (đường dẫn tương đối), thực hiện:
1. Tải ảnh về và đặt vào thư mục `images/`
2. Thay thế các URL Unsplash bằng đường dẫn tương đối, ví dụ:
   ```html
   <!-- Trước -->
   <img src="https://images.unsplash.com/photo-xxx?..." />

   <!-- Sau -->
   <img src="images/lau-mam.jpg" alt="Lẩu mắm" />
   ```

## Màu sắc chủ đạo

| Biến | Mã màu | Mục đích |
|------|--------|----------|
| `--red` | `#C0272C` | Màu chính (đỏ đặc trưng) |
| `--cream` | `#FAF7F2` | Nền kem |
| `--dark` | `#1A1A1A` | Văn bản |
| `--muted` | `#6B5B4E` | Văn bản phụ |
| `--sand` | `#F2EAE0` | Nền section phụ |

## Cách mở

Mở trực tiếp file `index.html` trong trình duyệt, hoặc dùng Live Server (VS Code):
```
project/index.html
```
