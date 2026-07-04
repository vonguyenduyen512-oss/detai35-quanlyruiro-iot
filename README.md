# Đề tài 35 — Quản lý rủi ro bảo mật cho hệ thống IoT quy mô nhỏ

**Học phần:** Bảo mật IoT (INT570 / INT4410)
**Lớp:** INT4410 — Bảo mật trong IoT, HK03, năm học 2025–2026
**Giảng viên hướng dẫn:** Hồ Nhựt Minh Sĩ
**Sinh viên thực hiện:** Võ Nguyễn Duyên
**Mã số sinh viên:** 231A010722

---

## 1. Mô tả đề tài

Đề tài xây dựng một quy trình quản lý rủi ro bảo mật đơn giản, dễ áp dụng cho hệ thống
IoT quy mô nhỏ, cụ thể là mô hình **phòng Lab thực hành Công nghệ thông tin** gồm: camera IP
giám sát, cảm biến nhiệt độ/độ ẩm, cảm biến khói/PIR, khóa cửa điện tử, gateway chạy Node-RED,
router Wi-Fi, dashboard giám sát trên cloud và ứng dụng di động điều khiển.

Đề tài không yêu cầu code/demo kỹ thuật; sản phẩm phân tích chính gồm: **danh mục tài sản**,
**sổ đăng ký rủi ro (risk register)**, **ma trận rủi ro 5x5**, **kế hoạch xử lý 5 rủi ro cao nhất**
và **checklist kiểm tra định kỳ**.

## 2. Nguồn đã sử dụng

| Nguồn | Link | Ngày truy cập | Phần đã sử dụng |
|---|---|---|---|
| OWASP IoT Security Verification Standard (ISVS) | https://github.com/OWASP/IoT-Security-Verification-Standard-ISVS | 04/07/2026 | Khung yêu cầu bảo mật để xây dựng risk register và checklist |
| OWASP IoT Security Testing Guide (ISTG) | https://github.com/OWASP/owasp-istg | 04/07/2026 | Tham khảo phương pháp kiểm tra từng hạng mục |
| OWASP Internet of Things Project | https://github.com/OWASP/www-project-internet-of-things | 04/07/2026 | Tổng hợp các nhóm rủi ro phổ biến (OWASP IoT Top 10) |

Xem chi tiết tại [`references/link_nguon.md`](references/link_nguon.md).

## 3. Cách xem/sử dụng sản phẩm

Vì đây là đề tài phân tích (không có code chạy được), không cần cài đặt môi trường. Người chấm/người
đọc có thể mở trực tiếp:

1. `report/Bao_cao_tieu_luan.docx` — báo cáo đầy đủ (mở đầu → mục tiêu → cơ sở lý thuyết →
   phương pháp → kết quả → đánh giá bảo mật → kết luận → tài liệu tham khảo).
2. `results/01_danh_muc_tai_san.csv` — danh mục 10 tài sản của hệ thống.
3. `results/02_risk_register.csv` — sổ đăng ký 17 rủi ro với điểm khả năng, ảnh hưởng, mức ưu tiên.
4. `results/03_ma_tran_rui_ro_5x5.csv` — ma trận rủi ro 5x5.
5. `results/04_ke_hoach_xu_ly_top5.csv` — kế hoạch xử lý 5 rủi ro cao nhất.
6. `results/05_checklist_dinh_ky.csv` — checklist kiểm tra định kỳ.
7. `slides/Slide_trinh_bay.pptx` — slide thuyết trình 8–12 trang (đang cập nhật).

Các file `.csv` trong `results/` có thể mở trực tiếp bằng Excel/Google Sheets để xem dạng bảng.

## 4. Kết quả chính

- Xác định **17 rủi ro cụ thể**, trong đó 2 rủi ro ở mức **Nghiêm trọng** (truy cập trái phép
  camera IP do mật khẩu mặc định; bẻ mật khẩu tài khoản admin do thiếu MFA).
- Đề xuất **5 biện pháp xử lý ưu tiên**, đều là biện pháp cấu hình chi phí thấp, không cần
  đầu tư phần cứng mới (đổi mật khẩu, bật MFA, đóng cổng router, xác thực dữ liệu cảm biến,
  chống replay lệnh khóa cửa).
- Xây dựng **checklist kiểm tra định kỳ** theo tuần/tháng/quý để duy trì mức an toàn lâu dài.

## 5. Giới hạn an toàn (cam kết)

- Toàn bộ phân tích thực hiện trên **mô hình giả định**, không khảo sát, quét hay truy cập
  bất kỳ hệ thống/thiết bị thật nào.
- Không sử dụng dữ liệu cá nhân thật, không đưa mật khẩu/token/secret thật vào repo.
- Điểm số khả năng xảy ra và mức độ ảnh hưởng trong risk register mang tính ước lượng dựa trên
  tài liệu tham khảo và kinh nghiệm triển khai phổ biến, chưa được kiểm chứng bằng dữ liệu sự cố
  thực tế — đây cũng là hạn chế đã nêu rõ trong báo cáo.

## 6. Cấu trúc repo

```
vonguyenduyen-detai35-quanlyruiro-iot/
├── README.md
├── report/
│   └── Bao_cao_tieu_luan.docx
├── slides/
│   └── Slide_trinh_bay.pptx        (đang cập nhật)
├── results/
│   ├── 01_danh_muc_tai_san.csv
│   ├── 02_risk_register.csv
│   ├── 03_ma_tran_rui_ro_5x5.csv
│   ├── 04_ke_hoach_xu_ly_top5.csv
│   └── 05_checklist_dinh_ky.csv
└── references/
    └── link_nguon.md
```

> Ghi chú: đề tài không có code/config/dataset mô phỏng nên các thư mục `src/`, `configs/`,
> `data/` theo mẫu chung của lớp không được tạo; các sản phẩm phân tích được đặt trong `results/`.
