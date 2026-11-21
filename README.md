# Hướng dẫn Xuất bản Landing Page cho Tổ chức QZCore (qzcore.github.io)

Tài liệu này hướng dẫn cách xuất bản trang landing page của tổ chức **QZCore** lên **`https://qzcore.github.io`**.

---

## 1. Nguyên tắc Độc lập & Bảo toàn

- Thư mục cũ `frontend/landing_page/` (phục vụ `tmtuongsv.github.io`) **được giữ nguyên 100% không chỉnh sửa**.
- Thư mục `frontend/qzcore_landing/` là phiên bản nâng cấp nhận diện thương hiệu dành riêng cho tổ chức **`qzcore`**.

---

## 2. Quy trình Xuất bản lên GitHub Pages (3 Bước)

### Bước 1: Tạo Repository `qzcore.github.io` trên GitHub
1. Truy cập vào trang tạo repo mới của tổ chức `qzcore`:
   👉 [https://github.com/organizations/qzcore/repositories/new](https://github.com/organizations/qzcore/repositories/new)
2. Điền thông tin:
   - **Repository name:** Nhập chính xác `qzcore.github.io`
   - **Visibility:** Chọn **Public** (để dùng GitHub Pages miễn phí)
   - Bấm **Create repository**.

### Bước 2: Đẩy tệp `index.html` lên repository mới

Mở terminal tại thư mục `frontend/qzcore_landing/` và thực thi:

```bash
cd /run/media/tmt/data/Trac_nghiem_TM/frontend/qzcore_landing
git init
git branch -M main
git add index.html README.md
git commit -m "feat: khoi tao landing page chinh thuc cho qzcore"
git remote add origin git@github.com:qzcore/qzcore.github.io.git
git push -u origin main
```

### Bước 3: Kiểm tra Trang chủ

Sau khi đẩy code khoảng 30–60 giây, trang chủ của tổ chức sẽ tự động hoạt động tại:
👉 **https://qzcore.github.io**
