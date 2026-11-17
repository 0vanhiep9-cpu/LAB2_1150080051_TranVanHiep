# LAB 2 - Mã hóa đối xứng hiện đại

**Họ và tên:** Trần Văn Hiệp
**MSSV:** 1150080051
**Lớp:** 11_ĐH_THMT
## Hướng dẫn chạy chương trình

1.  **Yêu cầu phần mềm:**
    *   JDK 17 hoặc 21 (có thể dùng OpenJDK).
    *   Apache NetBeans (bản 20 trở lên).
    *   SQL Server Express (cổng 14333) + SQL Server Management Studio (SSMS).
    *   Python 3.10+ (cho bài nâng cao 02).
    *   Kết nối Internet (để Maven tải thư viện lần đầu).

2.  **Chuẩn bị cơ sở dữ liệu:**
    *   Mở SSMS, kết nối vào `localhost\SQLEXPRESS`.
    *   Chạy script `01_Tao_CSDL.sql` để tạo database `LAB2_MaHoaHienDai` và các bảng `app_users`, `crypto_history`.
    *   Chạy script `02_Tao_Tai_Khoan_SQL.sql` để tạo user `lab2_user` với mật khẩu `LabUser@2026`.

3.  **Chạy dự án Java (NetBeans):**
    *   Mở project `LAB2_MaHoaHienDai` trong NetBeans.
    *   Nhấp chuột phải vào project, chọn **Clean and Build** (Shift+F11) để Maven tải các thư viện cần thiết (`mssql-jdbc` và `bcprov-jdk18on`).
    *   Nhấp chuột phải vào project, chọn **Run** (F6) hoặc nhấn F6 để chạy menu chính.
    *   Trên menu chính, chọn form tương ứng với từng bài tập (2.1 - 2.6).

4.  **Chạy bài nâng cao 02 (Python - AES-CBC):**
    *   Cài đặt thư viện: Mở Command Prompt, chạy lệnh `py -m pip install cryptography`.
    *   Chạy giao diện: Di chuyển đến thư mục chứa tệp `aes_cbc_gui.py` (`cd /d C:\BaoMat\LAB2_Python`) và chạy lệnh `py aes_cbc_gui.py`.
    *   Chạy self-test: `py aes_cbc_gui.py --self-test`.
