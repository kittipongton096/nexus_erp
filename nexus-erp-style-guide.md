# Nexus ERP — Style Guide

> ระบบ Enterprise Resource Platform สำหรับองค์กรยุคใหม่

---

## 1. Brand Identity

**Product Name:** Nexus ERP  
**Tagline:** Enterprise Resource Platform  
**Logo Icon:** Cube (`fa-solid fa-cube`) บน background gradient สี blue

---

## 2. Color Palette

### Primary Blues

| Token | Hex | ใช้งาน |
|---|---|---|
| `--blue-deep` | `#1a2f5e` | Page title, KPI value, headings หลัก |
| `--blue-mid` | `#2d4f9e` | Primary button gradient, link hover, order ID |
| `--blue-soft` | `#4a72d4` | Button gradient, focus ring, accent, chart line |
| `--blue-light` | `#6b93e8` | Logo icon gradient, sidebar active indicator |
| `--blue-pale` | `#e8eef8` | Mini bar background |
| `--blue-ghost` | `#f0f4fc` | — |
| `--accent` | `#5b8af0` | Accent สำรอง |

### Neutrals

| Token | Hex | ใช้งาน |
|---|---|---|
| `--gray-100` | `#f8f9fc` | Body background, input background |
| `--gray-200` | `#eef1f8` | Border, divider, table separator |
| `--gray-400` | `#9aa5c0` | Placeholder, label, subtitle, legend text |
| `--gray-600` | `#5a6882` | Body text, nav item, table cell |
| `--gray-800` | `#2c3a55` | Primary text color |
| `--white` | `#ffffff` | Card background, form background |

### Semantic / Accent Colors

| สี | Hex | ใช้งาน |
|---|---|---|
| Teal | `#0ea5e9` | KPI card variant |
| Violet | `#8b5cf6` | KPI card variant, activity dot |
| Emerald | `#10b981` | KPI card variant, trend up, status success |
| Amber | `#f59e0b` | Activity dot warning |
| Red / Danger | `#ef4444` | Notification dot, trend down |
| Red cancel | `#dc2626` | Status pill cancel |

### Status Pills

| สถานะ | Background | Text |
|---|---|---|
| สำเร็จ (success) | `#d1fae5` | `#059669` |
| รอชำระ (pending) | `#fef3c7` | `#d97706` |
| กำลังดำเนิน (process) | `#dbeafe` | `#2563eb` |
| ยกเลิก (cancel) | `#fee2e2` | `#dc2626` |

---

## 3. Typography

### Font Families

| Font | Weight | ใช้งาน |
|---|---|---|
| **Sora** | 300, 400, 600, 700 | Heading, brand name, KPI value, card title, chart tooltip title |
| **DM Sans** | 300, 400, 500, 600 | Body text, input, button, table, nav item |

> นำเข้าจาก Google Fonts: `https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500;600&family=Sora:wght@300;400;600;700`

### Type Scale

| Role | Font | Size | Weight | Color |
|---|---|---|---|---|
| Brand name | Sora | 24px (sidebar: 20px) | 700 | White |
| Brand tagline | DM Sans | 13px | 400 | `rgba(255,255,255,0.5)`, uppercase, letter-spacing 2px |
| Brand headline | Sora | 32px | 600 | White, line-height 1.3 |
| Page title | Sora | 22px | 700 | `--blue-deep` |
| Page subtitle | DM Sans | 13px | 400 | `--gray-400` |
| Form title | Sora | 26px | 700 | `--blue-deep` |
| Card title | Sora | 15px | 600 | `--blue-deep` |
| Card subtitle | DM Sans | 12px | 400 | `--gray-400` |
| KPI label | DM Sans | 12px | 500 | `--gray-400`, uppercase, letter-spacing 0.8px |
| KPI value | Sora | 28px | 700 | `--blue-deep` |
| Stat number | Sora | 24px | 700 | White |
| Table header | DM Sans | 11px | 600 | `--gray-400`, uppercase, letter-spacing 0.8px |
| Table cell | DM Sans | 13px | 400 | `--gray-600` |
| Input label | DM Sans | 13px | 500 | `--gray-600` |
| Input text | DM Sans | 15px | 400 | `--gray-800` |
| Button | DM Sans | 15px | 600 | White |
| Nav item | DM Sans | 14px | 400 / 500 (active) | `rgba(255,255,255,0.55)` |
| Nav section label | DM Sans | 10px | 600 | `rgba(255,255,255,0.3)`, uppercase, letter-spacing 2px |
| Activity text | DM Sans | 13px | 400 | `--gray-600` |
| Activity time | DM Sans | 11px | 400 | `--gray-400` |
| Status pill | DM Sans | 11px | 600 | ตามสถานะ |

---

## 4. Spacing & Border Radius

### Border Radius

| Token | Value | ใช้งาน |
|---|---|---|
| `--radius-sm` | `12px` | Input, button, nav item, icon button, logo icon |
| `--radius-md` | `18px` | KPI card, chart card, table card |
| `--radius-lg` | `24px` | — |
| `--radius-xl` | `32px` | Login grid wrapper |

### Shadows

| Token | Value | ใช้งาน |
|---|---|---|
| `--shadow-sm` | `0 2px 12px rgba(26,47,94,0.06)` | Card default |
| `--shadow-md` | `0 8px 32px rgba(26,47,94,0.10)` | Card hover |
| `--shadow-lg` | `0 20px 60px rgba(26,47,94,0.15)` | Login grid |

### Spacing หลัก

| บริเวณ | ค่า |
|---|---|
| Main content padding | `32px 36px` |
| Card padding | `24px` |
| KPI card padding | `22px 22px 20px` |
| Login form padding | `56px 48px` |
| Sidebar width | `256px` |
| Sidebar padding | `28px 0` |
| KPI grid gap | `18px` |
| Charts / bottom row gap | `18px` |
| Input margin-bottom | `20px` |

---

## 5. Components

### Login Page

- **Layout:** 2-column grid (`1fr 1fr`), max-width 960px, rounded `--radius-xl`, `box-shadow: --shadow-lg`
- **Left (Brand):** `rgba(255,255,255,0.06)` backdrop-filter blur(20px), border `rgba(255,255,255,0.1)` — glassmorphism บน gradient background
- **Right (Form):** White background สะอาด
- **Background:** Gradient `135deg, #0f1e45 → #1a2f6e → #2d4f9e` พร้อม ambient orbs blur ทั้ง 3 จุด
- **Animation:** `loginFadeIn` — fade + translateY(30px) + scale(0.97) → normal, duration 0.8s, easing cubic-bezier(0.16,1,0.3,1)

### Sidebar

- **Background:** `--blue-deep` (`#1a2f5e`)
- **Width:** 256px, sticky, full height
- **Nav item active:** Background `rgba(107,147,232,0.2)`, text `#a0baf5`, left border indicator 3px `#6b93e8`
- **Nav item hover:** Background `rgba(255,255,255,0.07)`
- **Badge:** `--blue-soft` background, white text, pill shape
- **User card:** Avatar 36×36px gradient blue, border-radius 10px, initials ตัวพิมพ์ใหญ่
- **Animation:** `sidebarIn` — translateX(-30px) → normal, duration 0.6s

### KPI Cards

- **Grid:** 4 คอลัมน์, gap 18px
- **Variants:** `.blue`, `.teal`, `.violet`, `.emerald` — เปลี่ยน icon background และ decorative orb สีตามนั้น
- **Icon:** 40×40px, border-radius 11px, สีพื้นหลัง opacity 10%
- **Decorative orb:** Pseudo-element `::after` วงกลม 80px opacity 6% มุมขวาบน
- **Hover:** `translateY(-3px)` + `--shadow-md`
- **Animation:** `cardIn` — stagger delay 0.1s ต่อ card

### Buttons

**Primary (Login)**
- Background: `linear-gradient(135deg, --blue-mid, --blue-soft)`
- Border-radius: `--radius-sm`
- Padding: 15px
- Shadow: `0 4px 20px rgba(45,79,158,0.35)`
- Hover: `translateY(-2px)` + shadow เข้มขึ้น + overlay shine

**SSO Button**
- Background: `--gray-100`, border `--gray-200`
- Hover: white background, border `--blue-light`, text `--blue-mid`

**Icon Button (Topbar)**
- 40×40px, white background, border `--gray-200`, border-radius `--radius-sm`
- Hover: border `--blue-light`, text `--blue-mid`

### Input Fields

- Padding: `14px 18px` (with icon: `padding-left: 46px`)
- Background: `--gray-100` → white (focus)
- Border: `1.5px solid --gray-200` → `--blue-soft` (focus)
- Focus ring: `0 0 0 4px rgba(74,114,212,0.1)`
- Border-radius: `--radius-sm`

### Charts (Chart.js)

**Revenue Line Chart**
- Revenue line: `#4a72d4`, width 2.5px, fill gradient fade
- Expense line: `#a0baf5`, width 2px, dashed `[5,4]`, fill gradient fade
- Tension: 0.45 (smooth curve)
- Tooltip: White card, Sora title, DM Sans body, border `--gray-200`, border-radius 12px

**Donut Chart**
- Cutout: 72%
- Colors: `#4a72d4` → `#6b93e8` → `#a0baf5` → `#d4e3fc` (gradient-like sequence)
- Center label: Sora 22px bold

### Period Tabs

- Container: `--gray-100` background, border-radius 8px, padding 3px
- Active tab: White background, `--blue-mid` text, `--shadow-sm`
- Inactive: `--gray-400` text

### Status Pills

- Padding: `3px 10px`, border-radius `20px`, font-size 11px, weight 600
- ดูสี → ตาราง Status Pills ในหัวข้อ Colors

### Activity Feed

- Icon dot: 34×34px, border-radius 10px, สี variants: blue / green / amber / red / violet
- Hover: row background `--gray-100`

---

## 6. Animation Principles

| Animation | Effect | Duration | Easing |
|---|---|---|---|
| `loginFadeIn` | opacity + translateY(30) + scale(0.97) | 0.8s | cubic-bezier(0.16,1,0.3,1) |
| `sidebarIn` | translateX(-30) + opacity | 0.6s | cubic-bezier(0.16,1,0.3,1) |
| `contentIn` | opacity + translateY(20), delay 0.15s | 0.6s | cubic-bezier(0.16,1,0.3,1) |
| `cardIn` | opacity + translateY(16), stagger | 0.5s | cubic-bezier(0.16,1,0.3,1) |
| `loadingBar` | gradient sweep top bar | 1s | ease |
| Button hover | translateY(-2px) | 0.3s | ease |
| Card hover | translateY(-3px) | 0.25s | ease |

> ใช้ easing เดียวกัน `cubic-bezier(0.16,1,0.3,1)` (spring-like) สำหรับ entrance animations ทั้งหมด

---

## 7. Layout & Grid

```
┌─────────────────────────────────────────────┐
│ Sidebar (256px fixed)  │  Main Content (flex)│
│                        │  padding: 32px 36px │
│  [Logo]                │  [Topbar]           │
│  [Nav items]           │  [KPI Grid — 4 col] │
│                        │  [Charts — 1.7:1]   │
│  [User Card]           │  [Bottom — 1:1]     │
└─────────────────────────────────────────────┘
```

- **KPI Grid:** `repeat(4, 1fr)`, gap 18px
- **Charts Row:** `1.7fr 1fr`, gap 18px
- **Bottom Row:** `1fr 1fr`, gap 18px

---

## 8. Icons

ใช้ **Font Awesome 6.5.2** (CDN)

| บริเวณ | Icon |
|---|---|
| Logo | `fa-solid fa-cube` |
| Email input | `fa-regular fa-envelope` |
| Password input | `fa-solid fa-lock` |
| SSO | `fa-solid fa-building` |
| Dashboard nav | `fa-solid fa-chart-line` |
| คลังสินค้า | `fa-solid fa-boxes-stacked` |
| คำสั่งซื้อ | `fa-solid fa-file-invoice` |
| การเงิน | `fa-solid fa-wallet` |
| HR | `fa-solid fa-users` |
| CRM | `fa-solid fa-handshake` |
| รายงาน | `fa-solid fa-chart-pie` |
| ตั้งค่า | `fa-solid fa-gear` |
| Logout | `fa-solid fa-right-from-bracket` |
| Notification | `fa-regular fa-bell` |

---

## 9. Scrollbar

```css
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: var(--gray-200); border-radius: 3px; }
```

---

## 10. Design Principles

1. **Monochromatic Blue** — ใช้ blue spectrum เป็น primary palette ทั้งระบบ เพิ่มความน่าเชื่อถือแบบ enterprise
2. **Glassmorphism เฉพาะจุด** — ใช้เฉพาะ login brand panel เพื่อสร้างความโดดเด่นโดยไม่รก
3. **Subtle depth** — shadow เบา (`rgba(26,47,94,0.06–0.15)`) สร้าง hierarchy โดยไม่หนัก
4. **Spring easing** — entrance animations ทุกชิ้นใช้ cubic-bezier เดียวกัน ให้ความรู้สึก smooth และ premium
5. **Staggered cards** — KPI cards โผล่ทีละใบสร้าง rhythm ที่ดี
6. **Functional color** — semantic colors (green/amber/red) ใช้สื่อความหมายชัดเจน ไม่ใช้ตกแต่ง
