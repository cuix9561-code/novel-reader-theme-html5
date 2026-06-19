# 📖 NovelReaderHTML5 — Responsive Novel Reading Theme

> A professional, **HTML5 responsive novel reader theme** with dark mode, eye-friendly golden-amber text, and full catalog navigation.  
> Perfect for web novel platforms, fan-fiction sites, and digital literature publishers.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.x-06B6D4?style=flat-square&logo=tailwind-css)
![Responsive](https://img.shields.io/badge/Responsive-Yes-22c55e?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

---

## ✨ Features

- 🌙 **Dark reading mode** — Charcoal background reduces eye strain during long reading sessions
- 👁️ **Eye-friendly typography** — Golden-amber `#f0e6c5` text on dark `#0a0a0a` background, optimized for extended reading
- 📱 **Fully responsive** — Seamless experience from mobile to widescreen desktop
- 🔤 **Font size controls** — Three sizes (Small / Medium / Large), persisted in localStorage
- 📊 **Reading progress bar** — Visual scroll progress indicator at the top of the page
- 📋 **Chapter catalog page** — Full table of contents with active chapter highlighting
- 🔒 **Premium chapter indicators** — Lock/unlock visual state for gated content
- ⌨️ **Keyboard navigation** — Arrow key support for chapter flipping
- 🎞️ **Smooth animations** — CSS fade-in and page-flip transitions
- 📖 **Serif-optimized** — Uses `Noto Serif SC` for authentic Chinese/English novel reading experience

## 📸 Page Previews

### reader.html — Reading Page
```
┌─────────────────────────────────────────────┐
│  ← Novel Reader     A A A  [☰]              │
├─────────────────────────────────────────────┤
│                                             │
│          The Last Star                       │
│       Chapter 1: The Silent Observatory      │
│                                             │
│   The observatory had been silent for       │
│   seven years.                              │
│                                             │
│   When Chen Wei stepped through the         │
│   rusted iron gate, the hinges groaned      │
│   like a wounded animal...                  │
│                                             │
│  ─────────── 1 ───────────                  │
│  [← Prev] [Catalog] [Next →]               │
├─────────────────────────────────────────────┤
│  Chapter 1 of 48  •  3,842 words  [☆] [↓]  │
└─────────────────────────────────────────────┘
```

### catalog.html — Table of Contents
```
┌─────────────────────────────────────────────┐
│  ← The Last Star     48 chapters  Updated   │
├─────────────────────────────────────────────┤
│  [Cover Art]  The Last Star                 │
│               by Mark Cui                   │
│  Science Fiction • Mystery • Serial         │
│  [Start Reading] [+ Follow]                 │
├─────────────────────────────────────────────┤
│  Table of Contents         [All] [Unread]   │
│                                             │
│  01  The Silent Observatory     ● Reading   │
│  02  The Signal Returns                     │
│  03  Decoding the Message                   │
│  04  Old Friends, Old Wounds               │
│  ...                                       │
│  ─────── Premium Chapters ───────           │
│  11  Coordinates of Destiny      🔒         │
│  12  The Transmission            🔒         │
└─────────────────────────────────────────────┘
```

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/cuix9561-code/novel-reader-theme-html5.git

# Navigate into the project
cd novel-reader-theme-html5

# No build step required — just open in browser!
open reader.html       # macOS
start reader.html      # Windows
xdg-open reader.html   # Linux
```

## 🌐 Deploy

### Option A: GitHub Pages

```bash
# Push to GitHub, then:
# Settings → Pages → Source: main branch → / (root)
# Your site will be live at:
# https://cuix9561-code.github.io/novel-reader-theme-html5/
```

### Option B: Vercel / Netlify

Just drag and drop the folder to:
- **Vercel**: https://vercel.com/new
- **Netlify**: https://app.netlify.com/drop

Zero configuration required — pure static HTML.

## 🛠️ Features & Customization

### Core Highlights

| Feature | Detail |
|---------|--------|
| 🌙 **Eye-protection backgrounds** | Three built-in themes — Night (dark charcoal), Sepia (warm paper), Green (soft mint) — all designed to reduce eye strain during extended reading sessions |
| 🔤 **Typography adjustment ready** | Three font sizes (Small / Medium / Large) with instant switching and localStorage persistence across sessions |
| ⚡ **Lightweight & Zero-dependency** | Pure HTML5 + Tailwind CDN — no build tools, no npm, no JavaScript frameworks required. Just open and read |
| 📱 **Mobile-first responsive** | Fluid layout adapts seamlessly from 320px mobile screens to ultrawide desktop monitors |
| 💾 **Settings persistence** | Font size and display theme preferences saved to `localStorage` — your settings survive page refreshes and browser restarts |
| 🎛️ **Floating settings panel** | Quick-access control hub pinned to the bottom-right corner — toggle font size, switch themes, and jump to catalog without scrolling to the top |
| ♿ **Accessibility ready** | Semantic HTML structure, ARIA labels, `prefers-reduced-motion` support, and keyboard-navigable controls |

### Customization Guide

### Change Novel Content

Edit `reader.html` — replace the placeholder novel text inside `<article class="reader-content">`:

```html
<article class="reader-content">
  <h1>Your Novel Title</h1>
  <p class="chapter-title">Chapter 1: Your Chapter Name</p>
  <p>Your novel content goes here...</p>
</article>
```

### Update Catalog

Edit `catalog.html` — modify chapter entries in the chapter list:

```html
<a href="reader.html" class="chapter-item">
  <span class="chapter-number">01</span>
  <span class="chapter-title">Your Chapter Title</span>
</a>
```

### Change Color Scheme

The theme uses CSS custom properties. Modify in the `<style>` section:

```css
:root {
  --bg-primary: #0a0a0a;       /* Main background */
  --text-primary: #f0e6c5;     /* Main text color */
  --accent: #d4a853;           /* Accent / highlight color */
}
```

### Add Cover Image

Replace the cover placeholder SVG in `catalog.html`:

```html
<img src="your-cover.jpg" alt="Novel Cover" class="w-28 h-40 rounded-xl object-cover" />
```

## 📁 Project Structure

```
novel-reader-theme-html5/
├── reader.html       # Main novel reading page
├── catalog.html      # Chapter catalog / table of contents
└── README.md         # This file
```

## 🧩 Use Cases

| Use Case | How This Theme Helps |
|----------|---------------------|
| Web novel platform | Ready-made reading UI with catalog navigation |
| Fan-fiction site | Dark theme reduces eye strain for long sessions |
| Premium content | Locked chapter indicators for gated content |
| Self-publishing | Zero-config deployment to GitHub Pages |
| Writing portfolio | Showcase your fiction with a professional reader |

## 📄 License

MIT — Free for personal and commercial use. Attribution appreciated but not required.

---

<div align="center">
  <sub>Built with 💚 by <a href="https://github.com/cuix9561-code">Mark Cui</a></sub>
</div>
