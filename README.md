# Glowing — Responsive Skincare E‑Commerce Template

A sleek, **mobile‑first e‑commerce** template for beauty and skincare brands. Built with **vanilla HTML, CSS & JavaScript** — no frameworks, no build step. Optimized for fast loads and clean UX.

![Desktop Demo](./readme-images/desktop.png)

---

## ✨ Highlights

- **Fully responsive** layout powered by CSS Grid & Flexbox (mobile → desktop).
- **Sticky, auto‑hiding header** with **Back‑to‑Top** button.
- **Accessible mobile menu** (open/close, overlay, focusable links).
- **Hero showcase** and **collection banners** with hover shine effect.
- **Shop sections**: *What’s New*, *Bestsellers*, and *Under $25* (≈12 product cards).
- **Offer banners** (e.g., *Buy 1 Get 1*) and seasonal promo sections.
- **Blog preview** grid (3 cards).
- **Newsletter signup UI** in the footer.
- **Scroll‑reveal animation** for sections.
- **Lazy‑loaded images** for better performance.
- Uses **Google Fonts – Urbanist** and **Ionicons** (via CDN).

> Page title: **“Glowing - Reveal The Beauty of Skin”**

---



---

## ⚙️ Tech Stack

- **HTML5** (semantic header/main/footer, sectioning with `data-section`)
- **CSS3** (custom properties, Grid, Flexbox, animations)
- **JavaScript (ES6)** — sticky header, scroll‑reveal, mobile navbar, back‑to‑top
- **CDNs**: Google Fonts (Urbanist), Ionicons

Linked assets (from `index.html`):
```html
<link rel="stylesheet" href="./assets/css/style.css" />
<script type="module" src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"></script>
<script nomodule src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.js"></script>
<script src="./assets/js/script.js"></script>
```

---

## 🚀 Getting Started

**Option 1 — Open file:**  
Just open `index.html` in any modern browser.

**Option 2 — Local server (recommended):**  
Use VS Code **Live Server** or run a quick Python server:
```bash
# from the project root
python -m http.server 5173
# then visit http://localhost:5173
```

---

## 🎨 Customize

### Colors, spacing, typography
Change design tokens in `assets/css/style.css` under `:root`:

```css
:root {
  --hoockers-green: hsl(148, 20%, 38%);
  --pale-spring-bud: hsl(60, 68%, 85%);
  --spanish-gray: hsl(0, 0%, 61%);
  --fs-1: 4.8rem; /* display */
  --fs-4: 2.4rem; /* heading */
  --fs-7: 1.5rem; /* body */
  --section-padding: 35px;
  --shadow-1: 0 8px 16px hsla(0,0%,0%,0.15);
  --transition-1: 0.25s ease;
}
```

### Images & content
Replace images in `assets/images/` (hero, collection, offers, blog).  
Update copy in `index.html` (headings, prices, CTA labels).

### Icons & fonts
- Edit or remove Ionicons usages in the markup.
- Swap the Google Font by changing the `<link>` and `--ff-urbanist` variable.

---

## 🧠 UX Details

- **Sticky header** appears after `150px` scroll and **hides on scroll‑down**, re‑shows on scroll‑up.
- **Back‑to‑top button** toggles with the header.
- **Section reveal**: elements with `data-section` gain `.active` on entering viewport.
- **Mobile menu**: controlled via data‑attributes and JS utilities.

*(See `assets/js/script.js` for event handlers and utilities.)*

---

## 🧪 Browser Support

Modern Chromium, Firefox, Safari, and Edge.  
No IE support (ES6 modules & modern CSS features are used).

---

## 📦 Deployment

- **GitHub Pages:** push to `main` → Settings → Pages → Deploy from branch → `/ (root)`.
- **Netlify / Vercel:** drag‑and‑drop the folder or connect the repo (no build command).

---

## 🗺️ Roadmap (suggested)

- Product details page & routing
- Search, **filters & sorting**
- Cart, wishlist, and checkout flow
- Form validation + toasts
- Dark mode (prefers‑color‑scheme)
- PWA (offline + installable)

---

## 🙌 Credits

- **Design & base template inspiration:** *Glowing* by the front‑end community.  
- **Icons:** [Ionicons](https://ionic.io/ionicons) via unpkg CDN.  
- **Font:** [Urbanist](https://fonts.google.com/specimen/Urbanist) via Google Fonts.  
- **Images:** Placeholder images shipped in `assets/images/` (replace with your licensed assets).

> If this work derives from a public template, **keep attribution** to the original author in your repo/readme.

---

## 📄 License

This repository is intended for **learning and portfolio use**.  
For production/commercial use, ensure you have the rights to all assets and verify upstream template licensing.  
You can add an open‑source license (e.g., **MIT**) to *your* modifications if appropriate.

---

## 💬 Support

Have questions or want enhancements? Open an **Issue** or start a **Discussion**.

---

### 🔧 Dev Notes (for maintainers)
- Lint HTML/CSS/JS before commits.
- Compress images for performance.
- Use descriptive `alt` text for images to improve accessibility & SEO.


