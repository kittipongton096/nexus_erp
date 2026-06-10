# ⬡ Nexus ERP

> ระบบ ERP สำหรับองค์กรยุคใหม่ — ครบทั้งคลังสินค้า การเงิน HR และรายงาน ในไฟล์ HTML เดียว

![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue?style=flat-square&logo=github)
![HTML](https://img.shields.io/badge/HTML-Single%20File-orange?style=flat-square&logo=html5)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## 🌐 Live Demo

👉 [kittipongton096.github.io/nexus_erp](https://kittipongton096.github.io/nexus_erp/)

---

## 📋 หน้าที่มีในระบบ

| หน้า | คำอธิบาย |
|------|-----------|
| 🔐 Login | หน้าเข้าสู่ระบบ รองรับ SSO |
| 📊 Dashboard | ภาพรวม KPI, กราฟรายได้, Donut chart |
| 📦 คลังสินค้า | จัดการ SKU, Stock bar, สถานะสินค้า |
| 🧾 คำสั่งซื้อ | ติดตามออเดอร์, สถานะการจัดส่ง |
| 💰 การเงิน | งบกำไร-ขาดทุน, ธุรกรรม, ใบแจ้งหนี้ |
| 👥 HR | ข้อมูลพนักงาน, คำขอลา, สัดส่วนแผนก |
| 📈 รายงาน | สรุปยอดขาย, รายงานอัตโนมัติ |
| ⚙️ ตั้งค่า | ข้อมูลบริษัท, การแจ้งเตือน, Toggle settings |

---

## ✨ Features

- **Single File** — ทั้งระบบอยู่ในไฟล์ `index.html` เดียว ไม่ต้อง build หรือติดตั้ง
- **Responsive Layout** — Sidebar + Main content ปรับตามหน้าจอ
- **Interactive Charts** — กราฟเส้นและ Donut chart ด้วย Chart.js สลับ Period ได้ (7D / 1M / 1Y)
- **Modern UI** — Font: Sora + DM Sans, สีหลัก Navy Blue + White, rounded corners, smooth animation
- **SVG Icons** — ใช้ icon จาก Font Awesome ทั้งระบบ ไม่มี emoji
- **Navigation** — สลับหน้าผ่าน Sidebar โดยไม่ต้อง reload
- **Mock Data** — มีข้อมูลตัวอย่างครบทุกหน้า พร้อม present

---

## 🚀 วิธีใช้งาน

### เปิดใช้งานทันที (ไม่ต้องติดตั้ง)

```bash
# ดาวน์โหลดหรือ clone repo
git clone https://github.com/kittipongton096/nexus_erp.git

# เปิดไฟล์ในเบราว์เซอร์ได้เลย
open index.html
```

> ⚠️ ต้องต่ออินเทอร์เน็ตเพื่อโหลด Google Fonts และ Chart.js จาก CDN

### Deploy บน GitHub Pages

```bash
git add .
git commit -m "update"
git push
```

เว็บจะ update อัตโนมัติภายใน 1–2 นาที

---

## 🛠️ Tech Stack

| ส่วน | เทคโนโลยี |
|------|------------|
| Structure | HTML5 |
| Styling | CSS3 (Custom Properties, Flexbox, Grid) |
| Charts | [Chart.js 4.4.1](https://www.chartjs.org/) |
| Icons | [Font Awesome 6](https://fontawesome.com/) |
| Fonts | [Google Fonts](https://fonts.google.com/) — Sora, DM Sans |
| Deploy | GitHub Pages |

---

## 🎨 Design System

```
Colors
  --blue-deep:  #1a2f5e   (Sidebar, Headings)
  --blue-mid:   #2d4f9e   (Buttons, Links)
  --blue-soft:  #4a72d4   (Accents, Charts)
  --blue-light: #6b93e8   (Hover states)
  --gray-100:   #f8f9fc   (Page background)

Border Radius
  --radius-sm: 12px
  --radius-md: 18px
  --radius-lg: 24px
  --radius-xl: 32px (Login card)
```

---

## 📁 โครงสร้างไฟล์

```
nexus_erp/
└── index.html        # ทั้งระบบอยู่ในไฟล์นี้
    ├── <style>       # CSS ทั้งหมด
    ├── Login Page
    ├── Dashboard Page
    │   ├── Sidebar (navigation)
    │   └── Main Content
    │       ├── #page-dashboard
    │       ├── #page-inventory
    │       ├── #page-orders
    │       ├── #page-finance
    │       ├── #page-hr
    │       ├── #page-reports
    │       └── #page-settings
    └── <script>      # Navigation + Chart.js logic
```

---

## 📌 หมายเหตุ

- ระบบนี้เป็น **UI Prototype** เท่านั้น ยังไม่มี backend หรือฐานข้อมูลจริง
- ข้อมูลทั้งหมดเป็น Mock Data สำหรับ demo
- สามารถนำ design system และ component ไปต่อยอดกับ framework อื่นได้

---

## 📄 License

MIT License — ใช้งานได้เสรี ทั้งส่วนตัวและเชิงพาณิชย์
