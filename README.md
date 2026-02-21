# Levin Mwange — Developer Portfolio

A modern, single-page personal portfolio website for **Levin Mwange**, a Software Developer based in Nairobi, Kenya. Built with pure HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, just clean code.

---

## Preview

> Dark theme · Cyan accent · Scroll-reveal animations · Fully responsive

---

## Sections

| Section | Description |
|---|---|
| **Hero** | Full-screen intro with animated availability badge and floating stat cards |
| **About** | Personal background, overlapping image layout, and key stats |
| **Skills** | Technology cards for HTML5, CSS3, JavaScript, React, Network Security, and Git |
| **Experience** | Work history with animated left-border cards |
| **Education** | Academic and certification timeline |
| **Portfolio** | Project showcase with cinematic hover overlays |
| **Services** | Offered services with numbered card layout |
| **Contact** | Contact form with details and social links |

---

## Tech Stack

- **HTML5** — Semantic, accessible markup
- **CSS3** — Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript** — IntersectionObserver scroll reveal, navbar scroll effect, active nav tracking
- **Boxicons 2.1.4** — Icon library (CDN)
- **Google Fonts** — Bebas Neue · Outfit · Space Mono

No dependencies to install. No build step required.

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/portfolio.git
cd portfolio
```

### 2. Add your images

Place your images in the `images/` folder. The site expects:

```
images/
├── 2.jpg               # Hero section photo
├── 3.jpg               # About section photo
├── work 1 levin book.png
├── work 2 hotel.png
├── work 3 golden gates hotel.png
└── work 5 levin arts.png
```

### 3. Open in browser

```bash
# Option A: just open the file
open index.html

# Option B: use a local dev server (recommended)
npx serve .
# or
python3 -m http.server 3000
```

---

## Customization

All content is in `index.html`. Here's where to find each piece:

### Personal Info
Search for and update:
- `Levin Mwange` — your name
- `Software Developer` — your role
- `levin@email.com` — your email
- `+254 700 000 000` — your phone
- `Nairobi, Kenya` — your location

### Colors
Edit the CSS variables at the top of the `<style>` block:

```css
:root {
  --bg: #080c10;         /* Main background */
  --accent: #00e5ff;     /* Cyan highlight color */
  --text: #e2eaf2;       /* Body text */
  --muted2: #7a8fa0;     /* Secondary text */
}
```

### Social Links
Update the `href=""` attributes on all `<a>` tags wrapping social icons (GitHub, LinkedIn, Twitter, Facebook, Instagram).

### Projects
Each project card follows this structure:

```html
<div class="project-card reveal">
  <img src="images/your-image.png" alt="Project Name"/>
  <div class="project-overlay">
    <span class="project-tag">Tech · Stack · Used</span>
    <div class="project-name">Project Name</div>
    <p class="project-desc">Short description of the project.</p>
    <div class="project-links">
      <a href="LIVE_URL"><i class='bx bx-link-external'></i> Preview</a>
      <a href="GITHUB_URL"><i class='bx bxl-github'></i> GitHub</a>
    </div>
  </div>
</div>
```

---

## Project Structure

```
portfolio/
├── index.html      # Single file — all HTML, CSS, and JS
├── images/         # Your photos and project screenshots
└── README.md
```

---

## Responsive Breakpoints

| Breakpoint | Behavior |
|---|---|
| `> 1100px` | Full two-column layouts, hero image visible |
| `≤ 1100px` | Single column, hero image hidden |
| `≤ 768px` | Mobile nav (hamburger), condensed spacing |
| `≤ 480px` | Extra-small adjustments for stat grids |

---

## Features

- **Scroll reveal animations** — elements animate in as you scroll using `IntersectionObserver`
- **Sticky navbar** with active section highlighting
- **Navbar shrink** on scroll (padding reduces)
- **Cinematic project overlays** — hover to reveal project info
- **Grain texture overlay** — subtle noise for depth
- **Background grid pattern** on the hero section
- **Floating stat cards** on the hero image
- **CSS-only hover effects** — no JavaScript required for interactions

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

## Author

**Levin Mwange**  
Software Developer · Nairobi, Kenya  
[GitHub](#) · [LinkedIn](#) · [Twitter](#)