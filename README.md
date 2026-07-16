# Đề tài 35 - Quản lý rủi ro bảo mật cho hệ thống IoT quy mô nhỏ

> **Học phần:** Bảo mật trong IoT (INT4410)  
> **Giảng viên hướng dẫn:** Hồ Nhựt Minh Sĩ  
> **Sinh viên thực hiện:** Võ Nguyễn Duyên  
> **Mã số sinh viên:** 231A010722  
> **Năm học:** 2025–2026

---

# Giới thiệu

Đề tài **"Quản lý rủi ro bảo mật cho hệ thống IoT quy mô nhỏ"** được thực hiện nhằm xây dựng một quy trình đánh giá và quản lý rủi ro bảo mật cho hệ thống Internet of Things (IoT) trong môi trường phòng Lab thực hành.

Nội dung nghiên cứu tập trung vào việc xác định tài sản, phân tích mối đe dọa và lỗ hổng, đánh giá mức độ rủi ro, xây dựng Risk Register, thiết kế Ma trận rủi ro (Risk Matrix) và đề xuất các biện pháp xử lý phù hợp.

Đề tài được xây dựng dựa trên các tiêu chuẩn và hướng dẫn của:

- OWASP IoT Security Verification Standard (ISVS)
- OWASP IoT Security Testing Guide (ISTG)
- OWASP Internet of Things Project
- NIST SP800-30
- ISO/IEC 27005

---

# Mục tiêu

- Xác định các tài sản cần bảo vệ trong hệ thống IoT.
- Phân tích các mối đe dọa và lỗ hổng bảo mật.
- Đánh giá mức độ rủi ro theo phương pháp Likelihood × Impact.
- Xây dựng Risk Register.
- Thiết kế Ma trận rủi ro 5×5.
- Đề xuất kế hoạch xử lý các rủi ro ưu tiên.
- Xây dựng Checklist kiểm tra định kỳ.

---

# Mô hình hệ thống

Hệ thống IoT khảo sát bao gồm:

- Camera IP
- Cảm biến nhiệt độ và độ ẩm
- Cảm biến khói và PIR
- Khóa cửa điện tử
- Gateway Node-RED
- Router Wi-Fi
- Cloud Dashboard
- Ứng dụng Mobile

```text
Camera IP
      │
Cảm biến
      │
Gateway Node-RED
      │
Router Wi-Fi
      │
Cloud Dashboard
      │
Ứng dụng Mobile
```

---

# Cấu trúc Repository

```text
detai35-quanlyruiro-iot
│
├── README.md
│
├── report
│   └── Bao_cao_tieu_luan.docx
│
├── results
│   ├── 01_danh_muc_tai_san.csv
│   ├── 02_risk_register.csv
│   ├── 03_ma_tran_rui_ro_5x5.csv
│   ├── 04_ke_hoach_xu_ly_top5.csv
│   └── 05_checklist_dinh_ky.csv
│
└── references
    └── link_nguon.md
```

---

# Nội dung Repository

## 📁 report

Thư mục chứa báo cáo chính của đề tài.

Bao gồm:

- Báo cáo Word (.docx)
- (Có thể bổ sung PDF nếu cần)

Nội dung báo cáo:

- Mở đầu
- Mục tiêu
- Cơ sở lý thuyết
- Phương pháp nghiên cứu
- Danh mục tài sản
- Risk Register
- Ma trận rủi ro
- Kế hoạch xử lý
- Checklist
- Đánh giá bảo mật
- Kết luận
- Tài liệu tham khảo

---

## 📁 results

Thư mục chứa toàn bộ sản phẩm phân tích của đề tài.

### 01_danh_muc_tai_san.csv

Danh mục các tài sản cần bảo vệ trong hệ thống IoT.

### 02_risk_register.csv

Sổ đăng ký rủi ro gồm:

- Tài sản
- Mối đe dọa
- Lỗ hổng
- Khả năng xảy ra
- Mức độ ảnh hưởng
- Điểm rủi ro
- Biện pháp xử lý

### 03_ma_tran_rui_ro_5x5.csv

Ma trận đánh giá rủi ro theo 5 mức Khả năng xảy ra và 5 mức Ảnh hưởng.

### 04_ke_hoach_xu_ly_top5.csv

Kế hoạch xử lý 5 rủi ro có mức ưu tiên cao nhất.

### 05_checklist_dinh_ky.csv

Checklist kiểm tra định kỳ nhằm duy trì mức độ an toàn của hệ thống.

---

## 📁 references

Thư mục lưu danh sách các nguồn tài liệu được sử dụng trong quá trình thực hiện đề tài.

---

# Kết quả đạt được

Đề tài đã hoàn thành các nội dung sau:

- Xây dựng danh mục tài sản của hệ thống IoT.
- Phân tích 17 rủi ro bảo mật.
- Xây dựng Risk Register.
- Thiết kế Ma trận rủi ro 5×5.
- Đề xuất kế hoạch xử lý 5 rủi ro ưu tiên.
- Xây dựng Checklist kiểm tra định kỳ.
- Đánh giá mức độ rủi ro và đề xuất giải pháp giảm thiểu.

---

# Tài liệu tham khảo

Các tiêu chuẩn và tài liệu được sử dụng:

- OWASP IoT Security Verification Standard (ISVS)
- OWASP IoT Security Testing Guide (ISTG)
- OWASP Internet of Things Project
- NIST SP800-30 – Guide for Conducting Risk Assessments
- ISO/IEC 27005 – Information Security Risk Management

Chi tiết xem trong:

```text
references/link_nguon.md
```

---

# Giới hạn của đề tài

- Hệ thống được xây dựng dưới dạng mô hình phục vụ học tập.
- Không thực hiện kiểm thử trên hệ thống thực tế.
- Không sử dụng dữ liệu cá nhân hoặc dữ liệu nhạy cảm.
- Các đánh giá rủi ro được xây dựng dựa trên tài liệu tham khảo và mô hình giả định.

---

# Cam kết

Đề tài được thực hiện phục vụ mục đích học tập và nghiên cứu.

Không sử dụng cho mục đích tấn công, khai thác hoặc gây ảnh hưởng đến bất kỳ hệ thống thực tế nào.

---

# Tác giả

**Võ Nguyễn Duyên**

**Mã số sinh viên:** 231A010722

**Trường:** Đại học Văn Hiến

**Học phần:** Bảo mật trong IoT (INT4410)

**Giảng viên hướng dẫn:** Hồ Nhựt Minh Sĩ

**Năm học:** 2025–2026

---

# Giấy phép

Repository này được tạo nhằm phục vụ mục đích học tập và nghiên cứu tại Trường Đại học Văn Hiến.

© 2026 Võ Nguyễn Duyên. All Rights Reserved.
