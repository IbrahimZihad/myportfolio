# 🌐 Md. Ibrahim Zihad — Developer Portfolio

A personal portfolio for **Md. Ibrahim Zihad**, a full-stack web developer and BSc CSE graduate (Software Engineering) from United International University. Built entirely with **HTML, CSS and vanilla JavaScript** — no frameworks, no build tools, just one clean file.

The design follows a **Bento Grid & Architectural Slate** direction: a modular card dashboard with a deep midnight-slate background, subtle steel borders and electric sky-blue accents.

---

## 📸 Preview

> Open `index.html` directly in any modern browser to preview.

---

## 📁 Project Structure

```
portfolio/
├── index.html                  # Single-file portfolio (HTML + CSS + JS)
├── profile.jpg                 # Hero portrait
├── og-image.png                # 1200×630 social share card (Open Graph / Twitter)
├── favicon.svg                 # Gradient monogram favicon
├── apple-touch-icon.png        # 180×180 iOS home-screen icon
├── Ibrahim Zihad Resume.pdf    # CV served by the download buttons
└── README.md
```

No dependencies. No `npm install`. Just open and go.

---

## ✨ Features

- **Single file** — all markup, styles and scripts live in `index.html`
- **Fully responsive** — mobile-first bento grid that reflows at 680px, 720px and 1040px
- **Bento grid layout** — 12-column CSS grid with `span-3` … `span-12` card utilities
- **Scroll progress bar** — gradient indicator at the top of the page
- **Scrollspy navigation** — the active section is underlined as you scroll
- **Scroll-reveal animations** — cards fade and lift in via `IntersectionObserver`
- **Sticky glass navbar** — blurred background, denser on scroll
- **Mobile hamburger menu** — full-screen overlay nav with body-scroll lock
- **Live status indicators** — pulsing emerald dot for "available / live" badges
- **Interactive hover states** — cards lift, glow and shift their border colour
- **Architectural background** — fixed grid pattern plus ambient radial glows
- **Reduced-motion support** — animations collapse when the OS requests it
- **SEO & social metadata** — description, canonical, Open Graph, Twitter card, theme colour and `Person` JSON-LD
- **No external dependencies** — only Google Fonts via CDN

---

## 🗂️ Sections

| Section | Description |
|---|---|
| **Hero** | Name, role, tagline, CTA buttons, portrait card and four metric cards (CGPA, projects, live systems, HSC/SSC GPA) |
| **About** | Personal bio plus compact skill cards (Frontend, Backend, Data & ORMs, Tools) |
| **Education** | BSc CSE (UIU, 3.93/4.00, Software Engineering major), HSC (2020), SSC (2018) |
| **Stack** | Six skill cards: Frontend, Backend, Databases & ORMs, DevOps & Testing, Payments & Integrations, AI & Modern Web |
| **Experience** | Saloon Sweden, Dhaka Hotel and DexxoxxBD freelance engagements |
| **Projects** | CakeFlow, Saloon Sweden, Dhaka Hotel, SubscriptionsBD, LittleLingo AI, Pothik, SmartLibrary, Inventory Management, ShopManager — with stack chips and live/GitHub links |
| **Certifications** | Frontend Mastery (CDIP, UIU) and the Ostad full-stack course in progress |
| **Achievements** | CGPA 3.93/4.00 plus perfect 5.00 HSC and SSC results |
| **Contact** | Social links, email, phone, location, university and CV download |

---

## 🎨 Design Tokens

| Token | Value | Usage |
|---|---|---|
| `--bg` | `#090d16` | Deep midnight slate page background |
| `--surface` | `#111827` | Elevated slate card surface |
| `--surface-2` | `#0e1522` | Card gradient end stop |
| `--border` | `#1f2937` | Subtle steel card border |
| `--accent` | `#38bdf8` | Electric sky-blue primary accent |
| `--accent-2` | `#34d399` | Emerald secondary accent (live status) |
| `--text` | `#f9fafb` | Primary text |
| `--muted` | `#9ca3af` | Secondary / muted text |
| `--radius` | `16px` | Card corner radius (14px on mobile) |
| `--mono` | `JetBrains Mono` | Stack tags, endpoints, metrics |
| `--display` | `Plus Jakarta Sans` | Headings |

**Fonts (Google Fonts):**
- Display / headings: `Plus Jakarta Sans` (500–800)
- Body: `Inter` (300–600)
- Technical labels, chips, metrics: `JetBrains Mono` (400–600)

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, gradients, animations) |
| Interactivity | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts CDN |

---

## 🚀 Getting Started

### View Locally

```bash
# Clone or download the repo, then:
start index.html         # Windows
open index.html          # macOS
xdg-open index.html      # Linux
```

Or drag and drop `index.html` into any browser tab.

### Deploy

Since it's a single HTML file, it can be deployed anywhere static files are served:

| Platform | How |
|---|---|
| **GitHub Pages** | Push to a repo → Settings → Pages → Deploy from branch |
| **Netlify** | Drag and drop the folder on netlify.com/drop |
| **Vercel** | `vercel --prod` in the project folder |
| **Any web host** | Upload `index.html` to the root directory |

---

## ✏️ Customization Guide

All editable content lives in the HTML body. No config files, no JS data objects — just find and update the text directly.

### Update personal info

```
ibrahimzihad5@gmail.com                      → your email
+880 1885434861                              → your phone number
https://github.com/IbrahimZihad               → your GitHub profile
https://linkedin.com/in/ibrahim-zihad-…       → your LinkedIn profile
```

### Update project cards

Each project card has a label, title, description, a chip list and link anchors:

```html
<a href="https://example.com" class="link">↗ Live Demo</a>
<a href="https://github.com/user/repo" class="link">↗ GitHub</a>
```

### Update the site URL (Open Graph / canonical)

The absolute URL appears in the `<head>` and must match your deployment domain. Replace it in one pass:

```html
<link rel="canonical" href="https://myportfolio-nine-blond-83.vercel.app/" />
<meta property="og:url" content="https://myportfolio-nine-blond-83.vercel.app/" />
<meta property="og:image" content="https://myportfolio-nine-blond-83.vercel.app/og-image.png" />
<meta name="twitter:image" content="https://myportfolio-nine-blond-83.vercel.app/og-image.png" />
```

Also update `"url"` and `"image"` inside the `application/ld+json` block.

### Update the social share image

`og-image.png` is a 1200×630 card. To change the text or portrait, edit the source HTML used to render it, or simply replace the file — keep the 1200×630 size and the same filename so the meta tags keep working.

### Change the colour theme

Edit the CSS variables in `:root` at the top of the `<style>` block:

```css
:root {
  --accent:   #38bdf8;  /* primary accent */
  --accent-2: #34d399;  /* secondary accent / live status */
  --surface:  #111827;  /* card background */
}
```

### Change card widths

Cards use 12-column span utilities:

```html
<article class="card span-4">…</article>   <!-- 4 of 12 columns -->
<article class="card span-8">…</article>   <!-- 8 of 12 columns -->
```

Spans collapse to full width on mobile automatically.

### Add a new section

1. Add a `<section id="new-section">` block in the HTML body
2. Add a nav link: `<li><a href="#new-section">New</a></li>`
3. Add the same link to the mobile menu

---

## 📱 Responsive Breakpoints

| Breakpoint | Behaviour |
|---|---|
| `≥ 1040px` | Full desktop bento: 3- and 4-column card rows, horizontal nav |
| `720px – 1039px` | Two-column bento, hero photo becomes a full-width banner, stats line up 4-across |
| `≤ 900px` | Nav collapses into the hamburger menu |
| `≤ 680px` | Single column, tighter padding, full-width buttons |
| `≤ 400px` | Smaller portrait and chip typography |

---

## ⚡ JavaScript Features

All JS is at the bottom of the file in a single `<script>` block:

- **Scroll progress** — computes document scroll percentage into a gradient top bar
- **Nav state** — adds `.scrolled` styling past 24px and highlights the active section link
- **Hamburger toggle** — opens/closes the full-screen mobile menu and locks body scroll
- **Scroll reveal** — `IntersectionObserver` adds `.visible` to `.reveal` cards with a staggered delay
- **Smooth scroll** — intercepts `<a href="#…">` clicks and respects the fixed-nav offset

---

## 👤 Author

**Md. Ibrahim Zihad**
BSc CSE (Software Engineering) — United International University, Dhaka
Full Stack Developer

---

## 📄 License

This project is open for personal use. Feel free to use it as a template for your own portfolio.
