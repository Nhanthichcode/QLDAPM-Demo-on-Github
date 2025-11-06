# 📌 Quản Lý Dự Án Phần Mềm

Đây là dự án nhằm giúp sinh viên hoặc người mới học **làm quen với Git và GitHub** để dễ dàng quản lý, phát triển và cộng tác trong các dự án phần mềm — đặc biệt là các dự án website trong tương lai.

---

## 🎯 Mục Tiêu

- Làm quen với Git (lệnh cơ bản, quản lý phiên bản).
- Sử dụng GitHub để cộng tác nhóm.
- Tổ chức dự án theo mô hình thực tế.
- Chuẩn bị nền tảng để phát triển các website chuyên nghiệp.

---

## 🚀 Tính Năng Dự Án

- Quản lý phiên bản mã nguồn.
- Làm việc nhóm hiệu quả qua GitHub.
- Phân chia nhánh, hợp nhất code (branching & merging).
- Thực hành các thao tác Git cơ bản:
  - `git init`, `git clone`
  - `git add`, `git commit`, `git push`, `git pull`
  - `git branch`, `git checkout`, `git merge`
- Hiểu cách làm việc với **README**, **.gitignore**, **branch**, **pull request**, v.v.

---

## 🛠️ Phân Công Công Việc (5 Thành Viên)

### 1. Thành viên 1: Project Setup & Core (12 tệp)

_Phụ trách: Thiết lập dự án, cấu hình server, middleware, và layout/trang chủ._

- `index.js`
- `package.json`
- `package-lock.json`
- `README.md`
- `middleware/auth.js`
- `routers/index.js`
- `views/index.ejs`
- `views/header.ejs`
- `views/footer.ejs`
- `views/navbar.ejs`
- `views/error.ejs`
- `views/huongdan.ejs`

### 2. Thành viên 2: Module Authentication & User (9 tệp)

_Phụ trách: Logic và giao diện liên quan đến người dùng (đăng ký, đăng nhập, quản lý)._

- `models/taikhoan.js`
- `routers/auth.js`
- `routers/taikhoan.js`
- `views/dangky.ejs`
- `views/dangnhap.ejs`
- `views/taikhoan.ejs`
- `views/taikhoan_them.ejs`
- `views/taikhoan_sua.ejs`
- `views/taikhoan_cuatoi.ejs`

### 3. Thành viên 3: Module Product Management (13 tệp)

_Phụ trách: Logic và giao diện quản lý sản phẩm, hãng, và phân loại._

- `models/sanpham.js`
- `models/hangsanxuat.js`
- `models/phanloai.js`
- `routers/sanpham.js`
- `routers/hangsanxuat.js`
- `routers/phanloai.js`
- `views/sanpham.ejs`
- `views/sanpham_danhsach.ejs`
- `views/sanpham_them.ejs`
- `views/sanpham_sua.ejs`
- `views/sanpham_chitiet.ejs`
- `views/hangsanxuat.ejs`
- `views/phanloai.ejs`

### 4. Thành viên 4: Module Cart & Order (11 tệp)

_Phụ trách: Quy trình nghiệp vụ (giỏ hàng, thanh toán, hóa đơn)._

- `models/giohang.js`
- `models/hoadon.js`
- `routers/giohang.js`
- `routers/hoadon.js`
- `routers/thanhtoan.js`
- `views/giohang.ejs`
- `views/thanhtoan.ejs`
- `views/camon.ejs`
- `views/hoadon.ejs`
- `views/hoadon_chitiet.ejs`
- `views/hoadon_cuatoi.ejs`

### 5. Thành viên 5: Static Assets (8 tệp)

_Phụ trách: Quản lý tài nguyên tĩnh (hình ảnh upload)._

- `public/uploads/1751675935050.webp`
- `public/uploads/1751677063990.jpg`
- `public/uploads/1751763220662.jpg`
- `public/uploads/1751763220728.webp`
- `public/uploads/1751763254143.jpg`
- `public/uploads/1751763254151.webp`
- `public/uploads/1751763311535.jpg`
- `public/uploads/1751763311543.webp`
