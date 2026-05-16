# พรรคประชาชน — Visual Identity & Style Guide

> เอกสารแนวทางการออกแบบ (Corporate Identity / CI) สำหรับทีมออกแบบภายใน
> เวอร์ชัน 0.2 — เพิ่ม official logo (SVG) + ฟอนต์ Anakotmai / Pracharath
> สถานะ: **WORKING DRAFT** — ใช้ภายในทีม ตรวจสอบกับทีม Brand ก่อนใช้ external

---

## 1. Brand Essence

| | |
|---|---|
| **ชื่อ** | พรรคประชาชน (People's Party) |
| **แคมเปญที่อ้างอิง** | กรุงเทพง่ายๆ / *Bangkok Made Easy* |
| **Mood** | สด ชัด ตรงไปตรงมา — มองโลกในแง่ดี เข้าถึงง่าย เป็นกันเอง |
| **Personality** | กล้า • โปร่งใส • คนรุ่นใหม่ • ใช้ชีวิตจริง |
| **คำที่ควรนึกถึงตอนออกแบบ** | "ง่าย", "ชัดเจน", "เคลื่อนไหว", "เป็นของทุกคน" |
| **คำที่ควรหลีกเลี่ยง** | "หรูหรา", "ฟอร์มอล", "ลึกลับ", "การ์ตูนเด็ก" |

**หลักคิดเดียวที่ต้องจำ:** สีส้มของพรรค **คือ** brand ไม่ใช่ตัวประดับ — ทุกชิ้นงานควรให้สีส้มเป็นพระเอก ตัวอักษร/ภาพประกอบเป็นตัวรอง

---

## 2. Logo

### 2.1 ตัวโลโก้
โลโก้พรรคประกอบด้วย 2 ส่วน:

1. **Mark** — สามเหลี่ยมชี้ขึ้นแบบเปิดยอด (open-top triangle) ที่เกิดจากการประกบสามเหลี่ยมย่อย 3 ชิ้น — สื่อความหมาย **การก้าวขึ้น** และเอกลักษณ์ตัว **ป.** (ประชาชน)
2. **Wordmark** — "พรรคประชาชน" หรือ "PEOPLE'S PARTY" ในฟอนต์ Anakotmai Bold

**ไฟล์ master:** `assets/brand/logo-source.svg` (vector) — ดึงจาก official asset ของพรรค (Wikimedia, 2024)

### 2.2 Variants ที่มีให้ใช้

| ไฟล์ | คำอธิบาย | ใช้กับ |
|---|---|---|
| `assets/brand/logo-color.svg` | Mark ส้ม + wordmark นาวี | พื้นขาว / สว่าง |
| `assets/brand/logo-on-orange.svg` | ทั้งหมดเป็นสีขาว | พื้นส้มของแบรนด์ |
| `assets/brand/logo-on-navy.svg` | Mark ส้ม + wordmark ขาว | พื้นนาวี |
| `assets/brand/logo-mono-black.svg` | ทั้งหมดเป็นสีดำ | งานพิมพ์ขาว-ดำ |
| `assets/brand/logo-mono-white.svg` | ทั้งหมดเป็นสีขาว | พื้นเข้มอื่น ๆ |
| `assets/brand/mark-only.svg` | เฉพาะ mark (ไม่มีตัวอักษร) | favicon, avatar, pattern |

### 2.2 Clear space
รักษาพื้นที่ว่างรอบโลโก้อย่างน้อย = ครึ่งหนึ่งของความสูง mark (เรียกค่านี้ว่า **`x`**)

```
┌─────────────────────────────┐
│   x                         │
│   ┌───────────────────┐     │
│ x │  ▲  พรรคประชาชน  │ x   │
│   └───────────────────┘     │
│   x                         │
└─────────────────────────────┘
```

ห้ามวาง element อื่น (ข้อความ ปุ่ม รูป) ภายในกรอบ clear space นี้

### 2.3 Minimum size
- **Digital:** mark สูงไม่ต่ำกว่า **24 px** (ถ้าใช้คู่ wordmark) / **16 px** (ถ้าใช้ mark เดี่ยว)
- **Print:** mark สูงไม่ต่ำกว่า **8 mm**

### 2.4 Color variants (สรุป)

| Variant | ใช้เมื่อ | mark | wordmark |
|---|---|---|---|
| **Primary** | พื้นขาวหรือสว่าง | Orange `#E65416` | Navy `#1E1464` |
| **Reverse on Orange** | พื้นสีส้มของแบรนด์ | White | White |
| **Reverse on Navy** | พื้นสีนาวี | Orange | White |
| **Mono Black** | งานพิมพ์ขาว-ดำ, fax | Black | Black |
| **Mono White** | พื้นเข้มที่ไม่ใช่สีแบรนด์ | White | White |

### 2.5 Do / Don't

✅ **DO**
- ใช้ไฟล์ master ที่ทีมแจกเท่านั้น (SVG เป็นไฟล์หลัก)
- รักษาสัดส่วน mark กับ wordmark ตามต้นฉบับ
- ใช้บน background ที่มี contrast เพียงพอ (WCAG AA ขึ้นไป)

❌ **DON'T**
- ห้ามบีบ/ยืดโลโก้ — สเกลเฉพาะแบบ proportional
- ห้ามเปลี่ยนสีนอกเหนือจากตาราง 2.4
- ห้ามใส่ shadow, gradient, stroke, glow, bevel
- ห้ามวางบน background ที่มีลายรบกวน (เช่น รูปคนเต็มเฟรม)
- ห้ามหมุน mark — มันสื่อทิศทาง "ขึ้น" เสมอ
- ห้ามแยก mark ออกจาก wordmark โดยพลการ (ใช้ mark เดี่ยวได้เฉพาะ favicon / avatar / pattern)

---

## 3. Color Palette

### 3.1 Primary colors

| Token | Hex | RGB | Use |
|---|---|---|---|
| `--orange-500` | `#E65416` | 230 / 84 / 22 | **สีหลัก** — background, fills, key surfaces |
| `--navy-900` | `#1E1464` | 30 / 20 / 100 | สีรอง — typography เน้น, ปุ่ม CTA, ภาพประกอบ |
| `--white` | `#FFFFFF` | 255 / 255 / 255 | typography บนพื้นส้ม/นาวี, พื้น header |

> **อัตราส่วนแนะนำในงานชิ้นเดียว:** Orange 60% · Navy 25% · White (ลบ) 15%
> Orange ควรครองพื้นที่ใหญ่ที่สุดเสมอ ไม่ใช่ accent

### 3.2 Supporting / Accent

| Token | Hex | RGB | Use |
|---|---|---|---|
| `--sand-300` | `#F6C885` | 246 / 200 / 133 | accent อบอุ่น (ถนน, เส้นทาง, ภาพประกอบ) |
| `--orange-600` | `#C4430E` | 196 / 67 / 14 | hover state / shadow ของสีส้ม |
| `--navy-700` | `#28135D` | 40 / 19 / 93 | typography handwritten, sub-headline |

### 3.3 Neutrals

| Token | Hex | Use |
|---|---|---|
| `--ink-900` | `#101010` | body text on white |
| `--ink-600` | `#4A4A52` | secondary text |
| `--ink-400` | `#9A9AA3` | placeholder, disabled |
| `--ink-200` | `#E5E5EA` | borders, dividers |
| `--ink-50`  | `#F7F7F8` | section background |

### 3.4 Semantic (suggested)

| Token | Hex | Use |
|---|---|---|
| `--success` | `#1F8A5B` | สำเร็จ |
| `--warning` | `#E0A100` | เตือน |
| `--danger`  | `#C8252C` | ข้อผิดพลาด (เลี่ยงเฉดที่ใกล้สีแบรนด์มาก) |
| `--info`    | `#2A6FDB` | ข้อความข้อมูล |

### 3.5 Contrast & accessibility

| Foreground | Background | Ratio | ผ่าน |
|---|---|---|---|
| White | Orange `#E65416` | 3.6 : 1 | AA (large text ≥18pt) |
| Navy `#1E1464` | Orange | 8.7 : 1 | **AAA** |
| Navy | White | 14.2 : 1 | **AAA** |
| White | Navy | 14.2 : 1 | **AAA** |

⚠ **อย่าวาง body text ขาวบนส้ม** — ใช้ขาวบนส้มได้เฉพาะ headline ใหญ่ (≥24px bold) เท่านั้น
สำหรับ body ให้ใช้ Navy บน Orange หรือ White (พื้น)

---

## 4. Typography

### 4.1 Brand fonts

พรรคประชาชนใช้ฟอนต์หลัก 2 ตระกูล ที่ **เปิดให้ใช้ฟรี** สำหรับงานในนามพรรค:

| ฟอนต์ | ออกแบบโดย | บทบาทในงานของพรรค | ไฟล์ |
|---|---|---|---|
| **Anakotmai** (อนาคตใหม่) | Cadson Demak | ฟอนต์หลัก — ใช้ทั้ง display + body | `assets/fonts/Anakotmai-{Light,Medium,Bold}.{woff2,woff}` |
| **Pracharath** (ประชารัฐ) | Cadson Demak | ฟอนต์เสริม / accent | `assets/fonts/Pracharath-{Regular,Bold}.otf` |

> Anakotmai เป็นฟอนต์ที่ใช้ต่อเนื่องตั้งแต่สมัยอนาคตใหม่ → ก้าวไกล → ประชาชน — เป็น **เอกลักษณ์ทาง typographic ของพรรค**
> ห้ามแทนด้วยฟอนต์อื่นในงาน external เว้นแต่ใช้ในสภาพแวดล้อมที่โหลด custom font ไม่ได้ (เช่น Slack, email plain-text)

### 4.2 Type stack (CSS)

```css
@import url(https://db.onlinewebfonts.com/c/d0124989c5c4ca18457b79471decc1e7?family=Anakotmai);

:root {
  --font-display: 'Anakotmai', 'IBM Plex Sans Thai', system-ui, sans-serif;
  --font-body:    'Anakotmai', 'IBM Plex Sans Thai', system-ui, sans-serif;
  --font-accent:  'Pracharath', 'Anakotmai', serif;
  --font-mono:    'IBM Plex Mono', ui-monospace, monospace;
}
```

Fallback ฟอนต์ไทย: **IBM Plex Sans Thai** (Google Fonts) — รูปร่างใกล้เคียง Anakotmai มากที่สุดในกลุ่ม open-source

### 4.3 Weights ที่มี

| Family | Weight | CSS value | Use |
|---|---|---|---|
| Anakotmai | Light | `300` | body ขนาดใหญ่, intro paragraph |
| Anakotmai | Medium | `500` | body ปกติ, nav item, button |
| Anakotmai | Bold | `700` | headline, label, emphasis |
| Pracharath | Regular | `400` | quote, sub-headline (เสริม) |
| Pracharath | Bold | `700` | display accent (เสริม) |

> Anakotmai **ไม่มี Italic / Black / Thin** — ใช้ weight ที่มีเท่านั้น ห้าม fake italic ด้วย `font-style: italic` หรือ skew

### 4.4 ตัวอย่างการใช้

```css
h1, .display { font-family: var(--font-display); font-weight: 700; }
h2          { font-family: var(--font-display); font-weight: 700; }
h3, .label  { font-family: var(--font-body);    font-weight: 500; }
body, p     { font-family: var(--font-body);    font-weight: 300; }
.lead       { font-family: var(--font-body);    font-weight: 500; }
.quote      { font-family: var(--font-accent);  font-weight: 400; font-style: normal; }
```

### 4.5 Type scale (web, 16px base)

| Step | Size | Line | Weight | Use |
|---|---|---|---|---|
| `display-1` | 96 px / 6 rem | 1.0 | 800 | hero headline (1 บรรทัด) |
| `display-2` | 72 px / 4.5 rem | 1.05 | 800 | hero headline (multi-line) |
| `h1` | 48 px / 3 rem | 1.1 | 700 | page title |
| `h2` | 36 px / 2.25 rem | 1.15 | 700 | section title |
| `h3` | 24 px / 1.5 rem | 1.25 | 600 | sub-section |
| `body-lg` | 20 px / 1.25 rem | 1.5 | 400 | intro paragraph |
| `body` | 16 px / 1 rem | 1.6 | 400 | default |
| `body-sm` | 14 px / 0.875 rem | 1.5 | 400 | caption |
| `label` | 12 px / 0.75 rem | 1.4 | 500 / uppercase | tag, label |

### 4.6 หลักการใช้ฟอนต์ไทย

- ✅ Anakotmai เป็น **ฟอนต์หัวตัด (loopless)** สมัยใหม่ — ใช้ได้ทั้ง display + body ในงานของพรรค
- ✅ ขนาด body ต่ำสุดที่อ่านสบาย: **16 px** (เว็บ) / **11 pt** (พิมพ์)
- ✅ ระยะ word-spacing: ปล่อย default — อย่าใช้ `letter-spacing` มากกว่า 0.02em
- ❌ ห้ามผสม Anakotmai กับฟอนต์ไทยอื่นในชิ้นเดียวกัน (ยกเว้น Pracharath เป็น accent)
- ❌ ห้ามใช้ Thai italic / faux italic — ใช้ weight หนาขึ้นแทนการเน้น
- ❌ ห้ามใช้ Anakotmai Light ขนาดต่ำกว่า 18 px — เส้นบางเกินไป อ่านยาก

### 4.7 Script / Handwritten accent

ในแคมเปญที่เห็นใน hero ("Bangkok Made Easy") มีฟอนต์ **handwritten script** สีนาวี — เป็น **campaign-specific** ไม่ใช่ฟอนต์หลักของแบรนด์

- ใช้ได้เฉพาะ **tagline / sub-headline** ของแคมเปญที่กำหนดเท่านั้น
- ห้ามใช้กับ body, button, navigation, หรือข้อความ functional
- ขนาดต่ำสุด 28 px / 21 pt — ไม่งั้นอ่านไม่ออก
- สีหลัก: Navy `#1E1464`
- หากต้องการ script font ที่ใกล้เคียงสำหรับงาน mockup: **Caveat Brush** หรือ **Allura** (Google Fonts)

---

## 5. Photography & Imagery

### 5.1 Illustration style (อ้างจาก hero: มอเตอร์ไซค์ + เส้นทาง)

| | |
|---|---|
| **Style** | semi-realistic illustration, สี flat + shading นุ่ม ๆ, outline บางหรือไม่มี |
| **Subject** | ของในชีวิตประจำวันคนกรุงเทพ — มอไซค์, รถเมล์, ป้ายรถเมล์, ตึกแถว, ทางเท้า |
| **Color** | ใช้เฉพาะ palette ของแบรนด์ + เฉดอุ่น (ไม่ใช้ฟ้าสด, เขียวสด) |
| **Composition** | subject ลอยบนพื้นสีเรียบ + เส้นนำสายตา (เส้นทาง, ถนน, ลูกศร) |

### 5.2 Photography

- **People-first:** ภาพคนต้องเป็นพระเอก ไม่ใช่ฉาก
- **Real, not staged:** ภาพควรรู้สึกเหมือนถ่ายในชีวิตจริง ไม่ใช่ stock studio
- **Diversity:** หลากหลายเพศ อายุ อาชีพ พื้นที่ — สื่อ "ของทุกคน"
- **Color grading:** เพิ่ม warmth เล็กน้อย, contrast กลาง, ไม่ใช้ filter ทันสมัยจัด ๆ (no teal-orange Hollywood look)
- **Crop:** กล้าเข้าใกล้, ใช้ negative space เพื่อให้สีแบรนด์เข้าไปแทนได้

### 5.3 Treatment patterns

1. **Full-bleed orange + cutout illustration** — แบบใน hero
2. **Photo with orange tint overlay 10–15%** — สำหรับ campaign banner
3. **Duotone Navy × Orange** — สำหรับ portrait ผู้สมัคร / ผู้แทน
4. **White card + ภาพ subject กลาง** — สำหรับ profile / content card

### 5.4 ❌ Don't
- ห้ามใช้ stock photo แบบ corporate / handshake / "team in office"
- ห้ามใส่ filter Instagram แรง ๆ
- ห้ามใส่ภาพคนแบบ AI-generated ที่ดูไม่เป็นธรรมชาติ
- ห้ามใช้ภาพ landscape ไม่มีคน เป็น hero

---

## 6. Layout & Spacing

### 6.1 Grid
- **Desktop:** 12-column, max-width 1280 px, gutter 24 px
- **Tablet:** 8-column, gutter 20 px
- **Mobile:** 4-column, gutter 16 px

### 6.2 Spacing scale (4 px base)
`4 · 8 · 12 · 16 · 24 · 32 · 48 · 64 · 96 · 128`

### 6.3 Corner radius
| Token | Value | Use |
|---|---|---|
| `--r-sm` | 6 px | input, tag, small element |
| `--r-md` | 12 px | card, button |
| `--r-lg` | 24 px | large card, hero block |
| `--r-pill` | 9999 px | chip, pill button |

> ปุ่ม CTA หลักใน hero เป็น `--r-md` (radius กลาง) — ให้ความรู้สึกแน่น มั่นคง ไม่กลมมนเกินไป

---

## 7. Components

### 7.1 Buttons

| Variant | bg | text | border | use |
|---|---|---|---|---|
| **Primary** | `#1E1464` (Navy) | White | none | CTA หลักบนพื้นส้ม |
| **Primary-on-white** | `#E65416` (Orange) | White | none | CTA หลักบนพื้นขาว |
| **Secondary** | transparent | Navy | 2px Navy | action รอง |
| **Ghost** | transparent | current | none | tertiary |

**Specs**
- Padding: `12px 24px` (md) / `16px 32px` (lg)
- Font: 16 px / 600 weight
- Radius: `--r-md` (12 px)
- Hover: lighten 10% (orange) / lighten 15% (navy)
- Active: scale 0.98

### 7.2 Navigation
- พื้น **ขาว** เสมอ (แม้ hero จะเป็นส้ม)
- Logo ซ้าย, menu ขวา
- Item ปกติ: Navy `#1E1464`, weight 500
- Item active: Orange `#E65416`, weight 600, underline 2 px ด้านล่าง
- ระยะระหว่าง item: 32 px

### 7.3 Cards
- พื้นขาว, border `--ink-200`, radius `--r-lg`, shadow `0 2px 12px rgba(30,20,100,.06)`
- Heading ใน card: Navy
- Padding 24 px (md) / 32 px (lg)

---

## 8. Voice & Tone (สั้น)

- **เรียกคน:** "คุณ" / "เรา" / "ทุกคน" — ห้ามใช้ "ท่าน", "ประชาชนผู้มีสิทธิเลือกตั้ง"
- **ประโยค:** สั้น ตรง อ่านครั้งเดียวเข้าใจ
- **คำที่ชอบ:** ง่าย, ชัด, ทำได้, เริ่มเลย, ของทุกคน
- **คำที่เลี่ยง:** ศัพท์เทคนิครัฐ, ภาษากฎหมาย, คำซ้ำซ้อน
- **Headline style:** ขึ้นด้วยสรรพนาม/กริยา ไม่ใช่นามวลีหรู ๆ

---

## 9. Usage Examples (ตัวอย่างการใช้งาน)

### 9.1 Hero (อ้างอิงจาก screenshot ต้นทาง)
```
┌──────────────────────────────────────────────────┐
│ [LOGO]  หน้าแรก  สส.พรรค  เกี่ยวกับ ...   บริจาค │  ← navbar (ขาว)
├══════════════════════════════════════════════════┤
│                                                  │
│   กรุงเทพง่ายๆ              [illustration]      │
│   Bangkok Made Easy           มอไซค์ + ถนน      │
│   เพื่อชีวิตที่ง่ายขึ้น...                       │
│                                                  │
│   ┌─────────────────┐                            │
│   │ คลิกเข้าเว็บไซต์│   ← navy button             │
│   └─────────────────┘                            │
│                                  ●○○○○ slide dots │
└──────────────────────────────────────────────────┘
   background: #E65416 (orange-500)
```

### 9.2 Social media post (1:1, IG)
- พื้นส้ม
- Headline ขาว 2 บรรทัด ขนาดใหญ่
- Sub-headline script navy
- Logo ขาว มุมบนซ้าย
- ไม่มีกรอบ — full bleed

### 9.3 Document cover (A4)
- พื้นขาว
- แถบส้มเต็มซ้ายกว้าง 1/3 หน้ากระดาษ
- Logo สีเต็มมุมล่างขวา
- Title ใหญ่กลางหน้า — Navy

### 9.4 Profile card สส.
- พื้นขาว, radius `--r-lg`
- รูปคน duotone Navy × Orange ครอบ 1:1 บน
- ชื่อ Navy 24/700 + ตำแหน่ง 16/500 (ink-600)
- ไอคอน social ขนาด 20 px Navy

---

## 10. File / Asset checklist

**ที่มีแล้วในโปรเจกต์** ✅

```
assets/
├── reference-hero.png              ← screenshot อ้างอิงต้นทาง
├── brand/
│   ├── logo-source.svg             ← master (Wikimedia 2024)
│   ├── logo-color.svg              ← Primary: orange mark + navy wordmark
│   ├── logo-on-orange.svg          ← Reverse บนพื้นส้ม
│   ├── logo-on-navy.svg            ← บนพื้นนาวี
│   ├── logo-mono-black.svg         ← ขาว-ดำ
│   ├── logo-mono-white.svg         ← พื้นเข้ม
│   └── mark-only.svg               ← เฉพาะ mark (favicon, avatar)
└── fonts/
    ├── fonts.css                   ← @font-face declarations
    ├── Anakotmai-Light.{woff2,woff}
    ├── Anakotmai-Medium.{woff2,woff}
    ├── Anakotmai-Bold.{woff2,woff}
    ├── Pracharath-Regular.otf
    └── Pracharath-Bold.otf
```

**ที่ทีมยังต้องเพิ่ม** 📌

```
brand/
├── color/
│   ├── palette.ase                 (Adobe swatch)
│   └── palette.json                (design tokens)
├── illustration/
│   ├── motorbike.svg
│   ├── road.svg
│   └── …                           (library ภาพประกอบ)
└── templates/
    ├── social-1x1.fig
    ├── document-a4.fig
    └── slide-16x9.fig
```

---

## 11. Open questions / Next steps

- [x] ~~ขอไฟล์ logo master~~ — มีแล้ว (`assets/brand/logo-source.svg`)
- [x] ~~ระบุชื่อฟอนต์ official~~ — Anakotmai + Pracharath (Cadson Demak)
- [ ] ตรวจสีกับงาน print ที่ใช้งานจริง — แปลง Pantone / CMYK
- [ ] ระบุชื่อฟอนต์ script ที่ใช้ใน "Bangkok Made Easy" tagline
- [ ] เพิ่ม section "Motion" (transitions, micro-interactions)
- [ ] เพิ่ม section "Accessibility" แบบเต็ม (focus state, reduced motion, screen reader)
- [ ] ทำ companion HTML brand-guide สำหรับทีม dev/design ดูแบบ interactive
- [ ] ตรวจสอบ license การใช้ฟอนต์ Anakotmai / Pracharath กับงานนอกนามพรรค

---

*เอกสารนี้รวบรวมจากการวิเคราะห์ visual ของหน้า hero + ไฟล์ official ที่ทีมแบ่งปัน (logo SVG + ฟอนต์ Anakotmai/Pracharath) — ค่าสีและสัดส่วนเฉพาะอ้างอิงจากการวัดภาพ ควรเทียบกับ source ทางการก่อนใช้ external*
