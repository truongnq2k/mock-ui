# Kolia Mock UI

Bộ prototype HTML/CSS tiếng Việt cho giao diện Kolia AI. Thư mục này là nguồn tham chiếu trực quan cho Flutter app và định nghĩa design system glassmorphism của sản phẩm.

## Nội Dung

- `DESIGN.md`: Design system, color tokens, typography, spacing, shape và component guideline
- `index.html`: Trang tổng hợp/liên kết prototype
- `trang-chu.html`: Trang chủ theo dõi sức khỏe
- `nhan-dinh-suc-khoe.html`: Nhận định sức khỏe
- `danh-gia-tong-quan.html`, `danh-gia-tong-quan-ca-ngay.html`: Màn hình đánh giá
- `phieu-theo-doi.html`, `phieu-theo-doi-chi-tiet.html`: Phiếu theo dõi sức khỏe
- `chat-bot-cho-ly.html`: Chat trợ lý AI
- `thong-bao.html`: Thông báo
- `thanh-toan.html`: Thanh toán
- `thong-tin-ca-nhan.html`: Thông tin cá nhân
- `modal-bat-thuong.html`, `modal-canh-bao.html`: Modal cảnh báo
- `cai-dat/`: Prototype cài đặt
- `qua-tang/`: Prototype quà tặng
- `thong-so-chi-tiet/`: Prototype chi tiết chỉ số
- `assets/`: Tài nguyên tĩnh

## Xem Prototype

Có thể mở trực tiếp các file `.html` trong trình duyệt, hoặc chạy một static server tại thư mục này.

Ví dụ:

```bash
npx serve .
```

Sau đó mở URL do `serve` hiển thị và bắt đầu từ `index.html`.

## Design System

Tóm tắt từ `DESIGN.md`:

- Phong cách: Clinical Clarity, glassmorphism, mềm và rõ ràng
- Primary: `#00BFA5`
- Secondary: `#2196F3`
- Background: gradient sáng, thiên về neutral/soft blue
- Typography: Manrope cho nội dung và số liệu, Plus Jakarta Sans cho label nhỏ
- Card: nền trắng trong suốt, blur, viền nhẹ, bo góc lớn
- Button: pill-shaped, tối thiểu 48px chiều cao
- Spacing: base unit 4px, stack gap 16px, container padding 24px

## Vai Trò Trong Repo

- Là tài liệu thị giác cho `../kolia-app`.
- Dùng để đối chiếu khi triển khai màn hình Flutter mới.
- Không chứa build pipeline bắt buộc; đây là prototype tĩnh.

## Ghi Chú Phát Triển

- Khi thay đổi visual language, cập nhật `DESIGN.md` trước rồi mới chỉnh các màn hình prototype.
- Giữ nội dung tiếng Việt để đồng bộ với trải nghiệm người dùng cuối.
- Nếu Flutter app đã triển khai khác mockup, ưu tiên thống nhất lại bằng cách so sánh với design token trong `DESIGN.md`.
