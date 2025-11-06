<!-- # 📌 Quản Lý Dự Án Phần Mềm

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

--- -->

- Mỗi khi thực hiện bất kì thay đổi nào trong dự án việc đầy tiên cần làm là chạy lệnh " git pull ".

```
  B1: Kéo dự án về máy.
  B2: chạy lệnh " git branch " xem có đủ 2 nhánh main/None_Branch.
  B3: chạy lệnh " git checkout None_Branch " để chuyển sang bộ nhớ của nhóm.
  B4 Quan trọng: Mở file "WebMoHinhXe_MongoDB_new.zip" và kéo thả tệp thuộc phân công của
      mình vào các thư mục tương ứng trong dự án trên VsCode ( ví dụ: kéo file camon.ejs
      từ Folder views trong "WebMoHinhXe_MongoDB_new.zip" sang Folder views trong dự án hiện
      tại ).
  B5: vào Source Control ở thanh bên trái và commit từng file theo dạng 'tên file - lệnh commit'
     ( ví dụ: views - trang cảm ơn ).
  B6: sau khi commit xong thì chọn Push để đẩy tất cả code lên None_Branch.
```

## 🛠️ Phân Công Công Việc (5 Thành Viên)

### 1. Trí Nhàn: Project Setup & Core

_Phụ trách: Thiết lập dự án, cấu hình server, middleware, và layout/trang chủ._

- `index.js`
- `package.json`
- `package-lock.json`
- `middleware/auth.js`
- `routers/index.js`
- `views/index.ejs`
- `views/header.ejs`
- `views/footer.ejs`
- `views/navbar.ejs`
- `views/error.ejs`
- `views/huongdan.ejs`

### 2. Khôi Nguyên: Module Authentication & User

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

### 3. Hữu Khang iu Knguyen: Module Product Management

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

### 4. Thanh Phong: Module Cart & Order

_Phụ trách: Quy trình nghiệp vụ (giỏ hàng, thanh toán, hóa đơn)._

- `views/hangsanxuat.ejs`
- `views/phanloai.ejs`
- `models/giohang.js`
- `models/hoadon.js`
- `routers/giohang.js`
- `routers/hoadon.js`
- `routers/thanhtoan.js`
- `views/giohang.ejs`
- `views/thanhtoan.ejs`

### 5. Ngọc Phượng: Static Assets

_Phụ trách: Quản lý tài nguyên tĩnh (hình ảnh upload)._
- nguyên file `node_modules`
- `views/camon.ejs`
- `views/hoadon.ejs`
- `views/hoadon_chitiet.ejs`
- `views/hoadon_cuatoi.ejs`
- `public/uploads/1751675935050.webp`
- `public/uploads/1751677063990.jpg`
- `public/uploads/1751763220662.jpg`
- `public/uploads/1751763220728.webp`
- `public/uploads/1751763254143.jpg`
- `public/uploads/1751763254151.webp`
- `public/uploads/1751763311535.jpg`
- `public/uploads/1751763311543.webp`
