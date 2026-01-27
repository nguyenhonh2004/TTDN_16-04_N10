<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
        🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>

<h2 align="center">
    XÂY DỰNG HỆ THỐNG CHẤM CÔNG-TÍNH LƯƠNG TỰ ĐỘNG
</h2>

<div align="center">
    <p align="center">
        <img alt="AIoTLab Logo" width="170" src="https://github.com/user-attachments/assets/711a2cd8-7eb4-4dae-9d90-12c0a0a208a2" />
        <img alt="AIoTLab Logo" width="180" src="https://github.com/user-attachments/assets/dc2ef2b8-9a70-4cfa-9b4b-f6c2f25f1660" />
        <img alt="DaiNam University Logo" width="200" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" />
    </p>
</div>

---

## 🧭 Giới thiệu chung

Quản trị nhân sự là **nòng cốt của sự ổn định và phát triển doanh nghiệp**.  
Việc áp dụng hệ thống tự động hóa trong chấm công và tính lương giúp:

- Tối ưu hóa quy trình vận hành  
- Giảm thiểu sai sót thủ công  
- Đảm bảo tính **minh bạch – chính xác – kịp thời** trong chi trả quyền lợi cho người lao động  

Đề tài tập trung xây dựng **giải pháp quản trị nhân sự tập trung** trên nền tảng **ERP Odoo 19**, tích hợp chặt chẽ giữa chấm công, tiền lương và báo cáo phân tích.

---

## 📌 Giới thiệu hệ thống

Hệ thống chấm công – tính lương trên nền tảng **Odoo ERP** là một giải pháp **khép kín**, bao phủ toàn bộ quy trình từ quản lý hồ sơ nhân sự đến xuất phiếu lương.

### Các chức năng chính

- 🗂️ **Quản lý nhân sự**  
  Lưu trữ tập trung hồ sơ nhân viên, phòng ban, chức vụ và vòng đời hợp đồng.

- 🕒 **Ghi nhận chấm công**  
  Hỗ trợ nhiều nguồn dữ liệu: nhập tay, camera, API thiết bị ngoại vi.

- ⚖️ **Tự động tính lương**  
  Tính lương dựa trên công thực tế, hệ số tăng ca và các khoản phụ cấp.

- 🛡️ **Bảo hiểm & Thuế**  
  Khấu trừ tự động BHXH, BHYT, BHTN và thuế TNCN theo quy định pháp luật.

- 📊 **Báo cáo thông minh**  
  Dashboard trực quan theo dõi quỹ lương và hiệu suất làm việc.

---

## 🏗️ Cấu trúc hệ thống

Hệ thống được thiết kế theo **kiến trúc module**, liên kết chặt chẽ thông qua cơ sở dữ liệu tập trung.

1. **Module Nhân sự (Core)**  
   Quản lý thông tin nhân viên, hợp đồng lao động và khung lương cơ bản.

2. **Module Chấm công (Center)**  
   Xử lý dữ liệu hiện diện, đối chiếu ca làm việc, phát hiện đi muộn – về sớm.

3. **Module Tính lương (Payroll)**  
   Tính toán lương Gross/Net, áp dụng biểu thuế lũy tiến và sinh phiếu lương điện tử.

---

## 🛠️ Công cụ và công nghệ sử dụng

- **Ngôn ngữ**: Python (xử lý logic nghiệp vụ, ORM)
- **Nền tảng**: Odoo 19 (ERP mã nguồn mở)
- **Cơ sở dữ liệu**: PostgreSQL
- **Công cụ hỗ trợ**:
  - GitHub (quản lý mã nguồn)
  - PlantUML (thiết kế sơ đồ hệ thống)
- **Tích hợp dữ liệu**:
  - Google Sheets
  - Microsoft Excel

---

## Hình ảnh các MODULE
<div align="center">
    <p align="center">
        <img src="docs/1.jpg" alt="" width="800"/><br/>
        <i>Hình 1: Module nhân sự<i><br/><br/>
        <img src="docs/2.jpg" alt="" width="800"/><br/>
         <i>Hình 2: Module chấm công<i><br/><br/>
        <img src="docs/3.jpg" alt="" width="800"/><br/>
        <i>Hình 3: Module tính lương<i><br/><br/>
         <img src="docs/4.jpg" alt="" width="800"/><br/>
        <i>Hình 4: chức năng chấm công bằng camera  <i><br/><br/>
         <img src="docs/5.jpg" alt="" width="800"/><br/>
         <i>Hình 5:<i><br/><br/>
         <img src="docs/6.jpg" alt="" width="800"/><br/>
         <i>Hình 6:<i><br/><br/>
    </p>
</div>

---

# 🚀 Hướng dẫn cài đặt và vận hành hệ thống

## 1. Cài đặt môi trường Odoo

### 🔧 Yêu cầu hệ thống

- **Hệ điều hành**: Linux / WSL / macOS (khuyến nghị)
- **Python**: Phiên bản 3.8 trở lên
- **PostgreSQL**: Phiên bản 12 trở lên
- **Odoo Server**
- **Bộ nhớ RAM**: Tối thiểu 2 GB
- **Port**: 8069

### 📦 Cài đặt thư viện cần thiết

Sau khi clone source code, chạy lệnh:

```bash
pip install -r requirements.txt
```
---

## Đóng góp & Thông tin nhóm
Dự án được thực hiện bởi:
- Họ và tên: Nguyễn Thu Hồng
- SDT: 0853972752
- Email: nguyenhongnunu@gmail.com
- Họ và tên: Nguyễn Văn Giang
- SDT: 0353397306
- Email:  giangnguyen27112k4@gmail.com
- Họ và tên: Nguyễn Văn Bắc
- SDT: 0876476687
- Email: nguyenbacdz04@gmail.com

- © 2026 AIoTLab, Faculty of Information Technology, DaiNam University. All rights reserved.
---
