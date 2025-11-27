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

# Hướng dẫn quy trình làm việc Git/GitHub

**Quan trọng:** Mỗi khi thực hiện bất kỳ thay đổi nào trong dự án, việc đầu tiên cần làm là chạy lệnh `git pull` để cập nhật mã nguồn mới nhất từ kho chứa chung.

---

## Các bước làm việc với dự án

### Bước 1: Kéo dự án về máy lần đầu

1.  Tạo một thư mục rỗng trên máy tính của bạn.
2.  Mở thư mục đó trong VS Code.
3.  Kéo dự án về máy bằng lệnh sau trong Terminal của VS Code:
    ```bash
    git clone https://github.com/Nhanthichcode/QLDAPM-Demo-on-Github.git
    ```
4.  Sau khi clone xong, điều hướng vào thư mục dự án vừa kéo về (thay `"tên-thư-mục-vừa-clone"` bằng tên thư mục thực tế):
    ```bash
    cd "tên-thư-mục-vừa-clone"
    ```

### Bước 2: Kiểm tra nhánh làm việc

1.  Chạy lệnh sau để xem các nhánh hiện có trong dự án:
    ```bash
    git branch
    ```
2.  Đảm bảo rằng bạn thấy có hai nhánh chính: `main` và `None_Branch`.

### Bước 3: Chuyển sang nhánh làm việc của nhóm

1.  Chuyển sang nhánh `None_Branch` để làm việc:
    ```bash
    git checkout None_Branch
    ```

### Bước 4: Tích hợp mã nguồn cá nhân (Quan trọng)

1.  Mở file `WebMoHinhXe_MongoDB_new.zip`.
2.  Kéo và thả các tệp tin thuộc phần công việc của bạn từ file zip vào các thư mục tương ứng trong dự án bạn đã clone trên VS Code.
    - **Ví dụ:** Kéo file `camon.ejs` từ thư mục `views` trong `WebMoHinhXe_MongoDB_new.zip` sang thư mục `views` trong dự án hiện tại của bạn.

### Bước 5: Commit các thay đổi

1.  Vào mục **Source Control** (biểu tượng ba hình tròn nối với nhau) ở thanh bên trái của VS Code.
2.  Commit từng file đã thay đổi hoặc thêm mới.
3.  Đặt thông điệp commit theo định dạng: `'tên file - lệnh commit'`
    - **Ví dụ:** `views - trang cảm ơn`

### Bước 6: Đẩy mã nguồn lên GitHub

1.  Sau khi commit xong tất cả các thay đổi của bạn, chọn **Push** để đẩy toàn bộ mã nguồn đã commit lên nhánh `None_Branch` trên GitHub.

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

### 3. Hữu Khang: Module Product Management

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
