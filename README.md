# 🌐 Md. Ibrahim Zihad — Developer Portfolio

A personal portfolio website for **Md. Ibrahim Zihad**, a beginner-level full stack developer and BSc CSE student (Software Engineering) at United International University. Built entirely with **HTML, CSS, and vanilla JavaScript** — no frameworks, no build tools, just one clean file.

---

## 📸 Preview

> Open `portfolio.html` directly in any modern browser to preview.

---

## 📁 Project Structure

```
portfolio/
└── portfolio.html      # Single-file portfolio (HTML + CSS + JS)
```

No dependencies. No `npm install`. Just open and go.

---

## ✨ Features

- **Single-file** — everything lives in one `portfolio.html`
- **Fully responsive** — works on mobile, tablet, and desktop
- **Smooth scroll** — native CSS scroll behavior with JS anchor handling
- **Scroll-reveal animations** — sections animate in using IntersectionObserver
- **Sticky navbar** — shrinks on scroll, active on all viewports
- **Mobile hamburger menu** — full-screen overlay nav for small screens
- **Dark theme** — deep dark background with indigo/purple accent palette
- **Noise texture overlay** — subtle SVG noise for depth
- **Grid hero background** — decorative CSS grid pattern in the hero section
- **No external dependencies** — only Google Fonts loaded via CDN

---

## 🗂️ Sections

| Section | Description |
|---|---|
| **Hero** | Name, role, short tagline, CTA buttons, and key stats |
| **About** | Personal bio and quick-stat cards |
| **Education** | BSc CSE (UIU), HSC (2022), SSC (2018) timeline |
| **Skills** | Tech stack categorized into Frontend, Backend, Tools, Domains |
| **Projects** | POTHIK, Subscription Seller, AI E-Learning — with stack tags and links |
| **Achievements** | Frontend Mastery Certificate and academic distinctions |
| **Activities** | Extracurricular clubs and social/volunteer work |
| **Contact** | Social links, email, phone, location |

---

## 🎨 Design Tokens

| Token | Value | Usage |
|---|---|---|
| `--bg` | `#0a0a0f` | Page background |
| `--surface` | `#111118` | Section/card background |
| `--surface2` | `#1a1a24` | Nested card background |
| `--primary` | `#a78bfa` | Indigo/violet accent |
| `--accent` | `#38bdf8` | Sky blue secondary accent |
| `--gold` | `#fbbf24` | Achievement badges |
| `--text` | `#e8e8f0` | Primary text |
| `--muted` | `#6b6b8a` | Secondary/muted text |

**Fonts (Google Fonts):**
- Display / Headings: `Syne` (400, 600, 700, 800)
- Body: `DM Sans` (300, 400, 500)

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Interactivity | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts CDN |

---

## 🚀 Getting Started

### View Locally

Just open the file in your browser:

```bash
# Clone or download the repo, then:
open portfolio.html          # macOS
start portfolio.html         # Windows
xdg-open portfolio.html      # Linux
```

Or drag and drop `portfolio.html` into any browser tab.

### Deploy

Since it's a single HTML file, it can be deployed anywhere static files are served:

| Platform | How |
|---|---|
| **GitHub Pages** | Push to a repo → Settings → Pages → Deploy from branch |
| **Netlify** | Drag and drop the file on netlify.com/drop |
| **Vercel** | `vercel --prod` in the project folder |
| **Any web host** | Upload `portfolio.html` to the root directory |

---

## ✏️ Customization Guide

All editable content is in the HTML body. No config files, no JS data objects — just find and update the text directly.

### Update personal info
Search for placeholder values and replace:

```
your.email@example.com      → your real email
+880 1X XXX XXXXX           → your phone number
https://github.com          → your GitHub profile URL
https://linkedin.com        → your LinkedIn profile URL
https://facebook.com        → your Facebook profile URL
https://twitter.com         → your Twitter/X profile URL
```

### Update project links
Each project card has two anchor tags:

```html
<a href="#" class="project-link">↗ Live Demo</a>
<a href="#" class="project-link">↗ GitHub</a>
```

Replace `#` with the actual URLs.

### Change the color theme
Edit the CSS variables in `:root` at the top of the `<style>` block:

```css
:root {
  --primary: #a78bfa;   /* change to any color */
  --accent:  #38bdf8;   /* change secondary accent */
}
```

### Add a new section
1. Add a `<section id="new-section">` block in the HTML body
2. Add a nav link: `<li><a href="#new-section">New</a></li>`
3. Add the same link to the mobile menu

---

## 📱 Responsive Breakpoints

| Breakpoint | Behaviour |
|---|---|
| `> 900px` | Full desktop layout, horizontal nav |
| `≤ 900px` | Nav hidden, hamburger shown; single-column grids |
| `≤ 600px` | Reduced padding, all grids collapse to 1 column |

---

## ⚡ JavaScript Features

All JS is at the bottom of the file in a single `<script>` block:

- **Nav shrink on scroll** — toggles `.scrolled` class after 40px
- **Hamburger toggle** — opens/closes full-screen mobile menu, locks body scroll
- **Scroll-reveal** — `IntersectionObserver` watches `.reveal` elements, adds `.visible` class with staggered delay
- **Smooth scroll** — intercepts `<a href="#...">` clicks for smooth in-page navigation

---

## 👤 Author

**Md. Ibrahim Zihad**
BSc CSE (Software Engineering) — United International University, Dhaka
Full Stack Developer

---

## 📄 License

This project is open for personal use. Feel free to use it as a template for your own portfolio.
