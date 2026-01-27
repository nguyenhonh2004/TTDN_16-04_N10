- **Cơ sở dữ liệu**: PostgreSQL
- **Hệ điều hành**: Linux / WSL / macOS (khuyến nghị)

### 📦 Cài đặt thư viện cần thiết
Sau khi clone source code, chạy lệnh:

```bash
pip install -r requirements.txt
```
2. Cấu hình quy định Tăng ca (OT)
Dữ liệu tăng ca (Overtime – OT) được hệ thống tự động xác định dựa trên thời điểm làm việc thực tế:

Ngày thường: Hệ số 200%

Cuối tuần: Hệ số 200%

Ngày Lễ / Tết: Hệ số 400%

3. Chạy hệ thống
Khởi động Odoo Server và cài đặt module tùy chỉnh của nhóm:

./odoo-bin -c odoo.conf -i hr_payroll_custom
📘 Hướng dẫn sử dụng hệ thống
1. Thiết lập ban đầu
Nhập hồ sơ nhân viên

Thiết lập phòng ban

Cấu hình mức lương cơ bản trong module Nhân sự (HR)

2. Phân ca làm việc
Tạo các loại ca:

Ca sáng

Ca chiều

Ca đêm

Gán ca cho từng nhân viên

3. Chấm công
Nhân viên Check-in / Check-out qua:

Giao diện Web

Thiết bị chấm công

Hệ thống tự động:

Đối chiếu ca làm việc

Phát hiện đi muộn / về sớm

4. Kết xuất bảng lương
Cuối kỳ, bộ phận kế toán:

Kiểm tra bảng tổng hợp công

Nhấn “Sinh phiếu lương” (Payslip)

⚙️ Công thức tính toán cốt lõi
1. Lương thực tế
Lương thực tế = (Lương cơ bản / Công chuẩn) × Công thực tế
Công chuẩn: 26 ngày/tháng

2. Khấu trừ bảo hiểm
Tổng mức khấu trừ: 10.5% lương đóng bảo hiểm, bao gồm:

BHXH: 8%

BHYT: 1.5%

BHTN: 1%

3. Lương Net
Lương Net = Lương Gross - Bảo hiểm - Thuế TNCN
📰 Báo cáo & Phân tích dữ liệu
Hệ thống hỗ trợ:

Phát hiện bất thường (Anomaly Detection) bằng AI

Gắn cờ các trường hợp:

Quên chấm công

Quỹ lương dự báo vượt mức cho phép

🤝 Đóng góp & Thông tin nhóm
Dự án được thực hiện bởi:

Nhóm 10 – CNTT 16-04

Trường Đại học Đại Nam

Thành viên:
Nguyễn Văn Bắc – 1671020038

Nguyễn Văn Giang – 1671020094

Nguyễn Thu Hồng – 1671020131

Giảng viên hướng dẫn:
TS. Trần Đăng Công
