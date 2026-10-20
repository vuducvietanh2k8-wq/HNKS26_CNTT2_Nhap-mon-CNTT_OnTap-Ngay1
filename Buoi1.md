# BÀI THỰC HÀNH 01: QUẢN LÝ THƯ MỤC VÀ FILE

## Phần A – Tổ chức thư mục bằng GUI

### A1. Hiển thị đuôi file và file ẩn

* Đã bật hiển thị phần mở rộng tên file.
* Đã bật hiển thị file ẩn trong File Explorer.

### A2. Đổi tên thư mục gốc

* Tên cũ: `Trung Tam Tieng Anh FINAL`
* Tên mới: `trung-tam-tieng-anh`

### A3. Tạo thư mục

* `docs`
* `media`
* `data`
* `logs`
* `archive`

### A4. Đổi tên file theo snake_case

* `Logo Trung Tam.PNG` → `logo_trung_tam.png`
* `Anh Lop Hoc.JPG` → `anh_lop_hoc.jpg`
* `Lich Hoc.txt` → `lich_hoc.txt`
* `Hoc Vien Khoa 3.xlsx` → `hoc_vien_khoa_3.xlsx`
* `Access.log` → `access.log`

### A5. Di chuyển file bằng GUI

* `hoc_vien_khoa_3.xlsx` → `data`
* `access.log` → `logs`
* Giữ các file còn lại theo yêu cầu tại thư mục gốc.

### A6. Sao chép file mẫu

* Đã sao chép `bai_lam_ngay1.md` vào thư mục gốc.
* Giữ file `.env` tại thư mục gốc.

## Phần B – Thao tác bằng CLI

### B1. Hiển thị đường dẫn tuyệt đối

```powershell
pwd
```

Kết quả thực tế:

```text
DÁN KẾT QUẢ LỆNH pwd TẠI ĐÂY
```

### B2. Liệt kê nội dung, gồm file ẩn

```powershell
ls -Force
```

### B3. Di chuyển file

```powershell
mv .\lich_hoc.txt .\docs\
mv .\logo_trung_tam.png .\media\
mv .\anh_lop_hoc.jpg .\media\
```

### B4. Sao chép logo vào archive

```powershell
cp .\media\logo_trung_tam.png .\archive\
```

### B5. Xóa hai file tạm

```powershell
rm .\temp_201.tmp
rm .\temp_202.tmp
```

### B6. Kiểm tra thư mục logs và quay lại

```powershell
cd .\logs
ls
cd ..
```

### B7. Sao chép ảnh bằng đường dẫn tương đối

```powershell
cd .\docs
cp ..\media\anh_lop_hoc.jpg ..\archive\
cd ..
```

### B8. Liệt kê toàn bộ dự án, gồm file ẩn

```powershell
Get-ChildItem -Force -Recurse
```

Kết quả thực tế:

```text
DÁN KẾT QUẢ LỆNH B8 TẠI ĐÂY
```

## Kết luận

Đã thực hành tổ chức thư mục bằng GUI, đổi tên file theo snake_case, sử dụng các lệnh PowerShell để xem đường dẫn, liệt kê, di chuyển, sao chép, xóa file và thao tác với đường dẫn tương đối.
