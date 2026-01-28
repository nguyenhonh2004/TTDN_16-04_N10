<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>
<h2 align="center">
    XÂY DỰNG HỆ THỐNG CHẤM LƯƠNG VÀ TÍNH CÔNG TỰ ĐỘNG
</h2>
<div align="center">
    <p align="center">
        <img alt="AIoTLab Logo" width="170" src="https://github.com/user-attachments/assets/711a2cd8-7eb4-4dae-9d90-12c0a0a208a2" />
        <img alt="AIoTLab Logo" width="180" src="https://github.com/user-attachments/assets/dc2ef2b8-9a70-4cfa-9b4b-f6c2f25f1660" />
        <img alt="DaiNam University Logo" width="200" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" />
    </p>

[![AIoTLab](https://img.shields.io/badge/AIoTLab-green?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Faculty of Information Technology](https://img.shields.io/badge/Faculty%20of%20Information%20Technology-blue?style=for-the-badge)](https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-orange?style=for-the-badge)](https://dainam.edu.vn)

</div>

---


## 1. Giới thiệu hệ thống


Đây là **hệ thống quản lý tiền lương và bảo hiểm y tế (BHYT)** được xây dựng trên nền tảng **Odoo 19**, theo hướng **module hóa và tùy biến**, phục vụ mục tiêu **nghiên cứu học thuật và đồ án tốt nghiệp**.



Hệ thống **không sử dụng module payroll mặc định của Odoo**, mà triển khai một giải pháp tính lương riêng (BJ Payroll), cho phép chủ động trong thiết kế nghiệp vụ và mở rộng trong tương lai.

---

### 🎯 Mục tiêu chính

- Xây dựng hệ thống **tính lương tùy biến** dựa trên dữ liệu chấm công  
- Tích hợp **bảo hiểm y tế (BHYT)** cho người lao động và doanh nghiệp  
- Đảm bảo **tính chính xác – minh bạch – nhất quán dữ liệu**  
- Phù hợp cho **đào tạo, nghiên cứu và mô phỏng nghiệp vụ doanh nghiệp**

---

### 🧩 Các chức năng chính

- 👤 **Quản lý nhân viên**
- ⏱ **Chấm công và tổng hợp theo tháng**
- 💰 **Quản lý bảng lương (Payslip)**
- 🏥 **Tích hợp bảo hiểm y tế (BHYT)**

---


## ⚙️ 2. Công nghệ sử dụng


### 💻 Nền tảng chính
- **Odoo 19**
- **Python (Odoo ORM)**
- **PostgreSQL**

### 🧩 Kiến trúc hệ thống
- Module lõi: `bj_payroll_core`
- Module mở rộng: `bj_health_insurance`
- Custom model: `bj.hr.payslip`

---

## 3. Một số hình ảnh hệ thống

<p align="center">
    <em>Danh sách bảng lương (Payslip List View)</em><br/>
    <img width="624" height="351" alt="image" src="https://github.com/user-attachments/assets/c4665aec-88d2-44d1-af7a-92bec7af7a75" />

</p>


<p align="center">
    <em>Chi tiết bảng lương và bảo hiểm y tế (BHYT)</em><br/>
    <img width="212" height="150" alt="image" src="https://github.com/user-attachments/assets/da6a5a65-60a2-4840-b201-26c3a606b7ef" />

</p>

<p align="center">
    <em>Chức năng chấm công và tổng hợp theo tháng</em><br/>
    <img width="624" height="293" alt="image" src="https://github.com/user-attachments/assets/ff820bd0-de04-4a31-947c-76cb6c9a48c7" />

</p>

---

## 🛠️ 4. Hướng dẫn cài đặt & triển khai

### 4.1. Yêu cầu hệ thống
- 🐍 Python >= 3.10  
- 🐘 PostgreSQL  
- 🐳 Docker (khuyến nghị)  
- 🌐 Trình duyệt web hiện đại





---

### 📦 4.2. Clone dự án

```bash
git clone https://github.com/<username>/bj-payroll-odoo19.git
cd bj-payroll-odoo19
```












---

### 🔧 4.3. Cài đặt module

1. Sao chép các module sau vào thư mục `addons` của Odoo:
   - `bj_payroll_core`
   - `bj_health_insurance`

2. Cập nhật module trong cơ sở dữ liệu:

```bash
./odoo-bin -d your_database -u bj_payroll_core,bj_health_insurance
```




---

### ▶️ 4.4. Chạy hệ thống

```bash
./odoo-bin -c odoo.conf
```

Truy cập hệ thống tại:

```
http://localhost:8069
```

---

### ✅ 4.5. Kiểm tra hoạt động

1. Tạo nhân viên  
2. Chấm công cho nhân viên  
3. Tạo payslip theo tháng  
4. Nạp dữ liệu chấm công  
5. Compute lương  
6. Kiểm tra kết quả BHYT  

---

## 5. 📰 Poster
<div align="center">
    <p align="center">
        <img src="docs/1.jpg" alt="" width="800"/><br/>
@@ -134,7 +149,7 @@ pip install -r requirements.txt

---

## 6. 🤝Đóng góp & Thông tin nhóm
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

