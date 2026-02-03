# Landing Page Prompt Template

## Design System: Titanium Command

### Core Design Principles
- **NO rounded corners** - Chamfered corners ONLY (clip-path polygon)
- **Industrial/Tactical aesthetic** - Precision-engineered, professional look
- **High contrast** - Dark borders, bold typography
- **Touch-first** - Large click targets for kiosk/mobile

---

## Prompt Template

```
Tạo landing page HTML/CSS/JS với design system "Titanium Command":

### DESIGN RULES (BẮT BUỘC):
1. KHÔNG dùng border-radius - chỉ dùng clip-path chamfered corners:
   - Small (8px): polygon(8px 0, 100% 0, 100% calc(100% - 8px), calc(100% - 8px) 100%, 0 100%, 0 8px)
   - Medium (12px): polygon(12px 0, 100% 0, 100% calc(100% - 12px), calc(100% - 12px) 100%, 0 100%, 0 12px)
   - Large (20px): polygon(20px 0, 100% 0, 100% calc(100% - 20px), calc(100% - 20px) 100%, 0 100%, 0 20px)

2. COLOR PALETTE:
   - Primary: #0055FF (blue)
   - Secondary: #FF4800 (orange)
   - Dark: #111111
   - Light: #F0F2F5
   - Success: #00CC66
   - Error: #FF3333
   - Grays: #F8FAFC → #0F172A

3. TYPOGRAPHY:
   - UI/Headings: Inter (400-900 weight)
   - Technical/Prices: JetBrains Mono (500-800 weight)
   - Headings: UPPERCASE, bold (700-900)
   - Body: 16px minimum

4. BUTTONS:
   - Box-shadow offset (e.g., 6px 6px 0 var(--color-dark))
   - Hover: translate + reduce shadow
   - Chamfered corners
   - Border: 2px solid dark

5. CARDS:
   - White/light background
   - 2-3px dark border
   - Chamfered corners
   - Hover: translateY(-4px) + box-shadow

6. ICONS:
   - Lucide Icons library (https://unpkg.com/lucide@latest)
   - Initialize: lucide.createIcons()

7. GRID BACKGROUNDS:
   - Tech grid pattern với linear-gradient
   - 40px grid size
   - Subtle opacity (0.02-0.04)

### STRUCTURE SECTIONS:
1. Navigation (fixed, blur backdrop)
2. Hero Section (full viewport, centered/split layout)
3. Pain Points (problem cards với red accent)
4. Solution (2-column: visual + content)
5. Integration Models (grid cards)
6. Features (dark section, feature cards)
7. Target Audience (audience cards)
8. Dashboard Preview (mock UI)
9. Video Demo
10. CTA Form (dark section)
11. Footer (dark, multi-column)
12. Floating CTA (fixed bottom-right)

### RESPONSIVE:
- Desktop: 1400px max-width
- Tablet: 1024px breakpoint
- Mobile: 768px breakpoint

### ANIMATIONS:
- Smooth scroll
- Hover transitions (0.15-0.2s)
- Navbar shadow on scroll

### BRANDING ELEMENTS:
- Logo + 4-line brand text:
  - Line 1: Company name (bold, large)
  - Line 2: Tagline (primary color)
  - Line 3: System name (mono, uppercase)
  - Line 4: Powered by (small, gray)
```

---

## Example Usage

```
/cook Tạo landing page cho [SẢN PHẨM/DỊCH VỤ] sử dụng Titanium Command design system.

Thông tin công ty:
- Tên: [TÊN CÔNG TY]
- Hotline: [SỐ ĐIỆN THOẠI]
- Email: [EMAIL]
- Website: [WEBSITE]

Nội dung chính:
- Hero: [TIÊU ĐỀ CHÍNH]
- Vấn đề: [3 VẤN ĐỀ KHÁCH HÀNG GẶP]
- Giải pháp: [MÔ TẢ GIẢI PHÁP]
- Tính năng: [6 TÍNH NĂNG NỔI BẬT]
- Đối tượng: [4 NHÓM KHÁCH HÀNG MỤC TIÊU]

Hình ảnh:
- Logo: [ĐƯỜNG DẪN]
- Hero background: [ĐƯỜNG DẪN]
- Product images: [ĐƯỜNG DẪN]
```

---

## CSS Variables Reference

```css
:root {
    /* Brand Colors */
    --color-primary: #0055ff;
    --color-primary-hover: #0044cc;
    --color-secondary: #ff4800;
    --color-dark: #111111;
    --color-light: #f0f2f5;
    --color-white: #ffffff;
    --color-success: #00cc66;
    --color-warning: #ffaa00;
    --color-error: #ff3333;

    /* Grays */
    --gray-50: #f8fafc;
    --gray-100: #f1f5f9;
    --gray-200: #e2e8f0;
    --gray-300: #cbd5e1;
    --gray-400: #94a3b8;
    --gray-500: #64748b;
    --gray-600: #475569;
    --gray-700: #334155;
    --gray-800: #1e293b;
    --gray-900: #0f172a;

    /* Chamfered Shapes */
    --chamfer-sm: polygon(8px 0, 100% 0, 100% calc(100% - 8px), calc(100% - 8px) 100%, 0 100%, 0 8px);
    --chamfer-md: polygon(12px 0, 100% 0, 100% calc(100% - 12px), calc(100% - 12px) 100%, 0 100%, 0 12px);
    --chamfer-lg: polygon(20px 0, 100% 0, 100% calc(100% - 20px), calc(100% - 20px) 100%, 0 100%, 0 20px);
    --chamfer-xl: polygon(30px 0, 100% 0, 100% calc(100% - 30px), calc(100% - 30px) 100%, 0 100%, 0 30px);

    /* Typography */
    --font-display: 'Inter', sans-serif;
    --font-mono: 'JetBrains Mono', monospace;
}
```

---

## Component Patterns

### Button Primary
```css
.btn-primary {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    padding: 16px 32px;
    background: var(--color-primary);
    color: white;
    font-weight: 700;
    font-size: 16px;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    border: 2px solid var(--color-dark);
    clip-path: var(--chamfer-md);
    box-shadow: 6px 6px 0 var(--color-dark);
    transition: all 0.15s;
}

.btn-primary:hover {
    transform: translate(3px, 3px);
    box-shadow: 3px 3px 0 var(--color-dark);
}
```

### Card
```css
.card {
    background: white;
    border: 2px solid var(--color-dark);
    clip-path: var(--chamfer-lg);
    padding: 32px;
    transition: all 0.2s;
}

.card:hover {
    transform: translateY(-8px);
    box-shadow: 8px 8px 0 var(--color-dark);
}
```

### Section Badge
```css
.section-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 8px 16px;
    background: var(--color-primary);
    color: white;
    font-family: var(--font-mono);
    font-size: 12px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    clip-path: var(--chamfer-sm);
}
```

---

## Slideshow Pattern

```html
<div class="slideshow">
    <div class="slides">
        <div class="slide"><img src="image1.jpg" alt=""></div>
        <div class="slide"><img src="image2.jpg" alt=""></div>
    </div>
    <div class="slideshow-nav">
        <button id="prev"><i data-lucide="chevron-left"></i></button>
        <button id="next"><i data-lucide="chevron-right"></i></button>
    </div>
</div>
```

```javascript
const slides = document.querySelector('.slides');
let current = 0;
const total = 6;

function goToSlide(index) {
    current = index;
    if (current < 0) current = total - 1;
    if (current >= total) current = 0;
    slides.style.transform = `translateX(${-(current * 100)}%)`;
}

setInterval(() => goToSlide(current + 1), 3000);
```

---

## File Structure

```
project/
├── src/
│   └── templates/
│       └── landing-page.html
├── pictures/
│   ├── logo.png
│   └── [product-images].png
└── docs/
    └── landing-page-prompt-template.md
```
