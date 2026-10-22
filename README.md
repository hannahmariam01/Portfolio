# ✦ Hannah Mariam — AI Developer & Web Builder Portfolio

[![Vite](https://img.shields.io/badge/Vite-8.3.5-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-v22.x%20LTS-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2023-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-Custom%20Design%20System-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

> A modern, ultra-smooth, product-driven personal portfolio web application built for **Hannah Mariam** — AI Developer & Web Builder based in Würzburg, Germany. Features tactile micro-interactions, hardware-accelerated animations, bespoke case study modals, and interactive canvas visualizers.

---

## ⚡ Quick Links & Live Preview

| Environment | URL |
| :--- | :--- |
| **Local Dev Server** | [http://localhost:5173](http://localhost:5173) |
| **Network Address** | Accessible on your local network via `http://<LAN-IP>:5173` |

---

## ✨ Features & Visual Highlights

- **🌸 Interactive Scroll Intro & Sakura Canvas**: Dynamic multi-stage 3D intro viewport zoom with falling cherry blossom petals rendered on HTML5 canvas.
- **⏳ Dynamic Preloader**: Letter-by-letter kinetic typographic reveal (`HANNAH`), live percentage counter, and animated progress indicator.
- **🎯 Custom Dual Cursor**: Fluid trailing micro-dot and magnetic halo (`#cdot`, `#cring`) with smooth acceleration curves and dynamic hover states on interactive links.
- **🌌 Hero Particle System**: Interactive 60fps canvas particle physics simulation reacting to cursor position and viewport dimensions.
- **🔤 Kinetic Typographic Scramble**: Algorithmic text scramble effect animating hero headlines upon entrance.
- **🃏 3D Perspective Tilt Cards**: 3D interactive physics on project cards with `rotateX` and `rotateY` responding dynamically to pointer coordinates.
- **↔️ Horizontal Drag-to-Scroll Showcase**: Smooth mouse-drag and wheel-based gallery slider with a real-time responsive progress bar.
- **📚 Rich Case Study Slide-over Modals**: Detailed deep-dive overlays for all flagship projects with full problem/solution breakdowns, workflow flowcharts, tech badges, and keyboard shortcuts (`ESC` to exit, backdrop click handling).
- **📑 Sticky Stacking Panels**: 3D sticky stacking depth architecture with calculated RAF-throttled scroll scaling.
- **💡 Philosophy Interactive Accordion**: Clean engineering values showcase with expandable visual previews.
- **📱 Fully Responsive Design**: Flawless presentation across ultra-wide monitors, laptops, tablets, and mobile devices.

---

## 🛠️ Featured Case Studies

### 1. 📊 Presentation Designer
* **Category**: AI Tool / Web App
* **Tech Stack**: React, TypeScript, OpenAI API, pptxgenjs, Gravity Design System
* **Highlights**: Automates tedious slide formatting. Uploads any raw document or unstructured deck, extracts key content, applies brand tokens, and generates pixel-perfect PowerPoint (`.pptx`) presentations in under 60 seconds (~95% time saved).

### 2. 🌐 RDG (Rapid Design Generator)
* **Category**: Web-to-Design Automation
* **Tech Stack**: React, TypeScript, Figma REST API, Vite
* **Highlights**: Ingests live URLs, scrapes typography, layout geometry, colors, and components in real time, and reconstructs editable multi-layer screens directly inside Figma workspaces.

### 3. ✦ Fig Pilot
* **Category**: Figma Plugin & AI Co-pilot
* **Tech Stack**: React, TypeScript, Google Gemini API, Figma Plugin API
* **Highlights**: An integrated AI assistant for designers inside Figma. Supports one-click smart dark mode remapping, Auto Layout refactoring, presentation deck export, and visual inconsistency auditing.

### 4. 🇦🇺 Department of Health (DOH) Australia
* **Category**: Interactive Policy Landscape & Gov App
* **Tech Stack**: React 19, TypeScript, Tailwind CSS, Vite
* **Highlights**: Transforms dense government healthcare policies into an exploratory digital visual landscape with demographic population mapping and embedded interactive prototype walkthroughs.

---

## 💻 Tech Stack

* **Core Structure**: Semantic HTML5 with accessible ARIA modals and viewport meta tags.
* **Styling**: Modern Vanilla CSS3 design system using CSS custom properties (`--ink`, `--cream`, `--blue`, `--purple`), smooth cubic-bezier transitions, glassmorphic overlays, and grid/flexbox layouts.
* **Logic & Animations**: Modern ES Modules JavaScript, HTML5 2D Canvas API, IntersectionObserver for scroll triggers, and requestAnimationFrame loops.
* **Bundler & Tooling**: [Vite 8](https://vitejs.dev/) with hot module replacement (HMR) and optimized Rolldown/Rollup production builds.
* **Typography**: Modern Google Fonts pairing — [Outfit](https://fonts.google.com/specimen/Outfit) (geometric display headlines) and [Inter](https://fonts.google.com/specimen/Inter) (readable body copy).

---

## 🚀 Getting Started

### Prerequisites

Ensure you have **Node.js** (v20.19.0+ or v22.12.0+ recommended) and **npm** installed:

```bash
node -v   # Should be v20.19+ or v22+
npm -v
```

> **Note**: If Node.js is installed in `~/.local/node/bin`, ensure your `PATH` contains it:
> ```bash
> export PATH="$HOME/.local/node/bin:$PATH"
> ```

### 1. Clone or Open the Repository

```bash
cd /path/to/portfolio
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Start the Development Server

```bash
npm run dev
```

By default, the Vite dev server starts at:
```
  ➜  Local:   http://localhost:5173/
  ➜  Network: http://<your-ip>:5173/
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

---

## 📦 Build for Production

To create an optimized production bundle:

```bash
npm run build
```

This compiles minified static assets into the `dist/` directory:
```
dist/
├── assets/
│   ├── index-[hash].css
│   └── index-[hash].js
├── doh-preview.jpg
├── pres-designer-preview.png
├── rdg-preview.png
├── figma-copilot-preview.png
└── index.html
```

### Preview the Production Build Locally

```bash
npm run preview
```

---

## 📂 Project Structure

```
portfolio/
├── index.html              # Main HTML entry point & font preconnects
├── main.js                 # Primary UI markup, canvas logic, and interaction controllers
├── style.css               # Core CSS design system, typography, animations, and modals
├── package.json            # Scripts & Vite dev dependencies
├── public/                 # Static assets, project thumbnails, icons, and illustrations
│   ├── doh-preview.jpg
│   ├── figma-copilot-preview.png
│   ├── pres-designer-preview.png
│   ├── rdg-preview.png
│   ├── phil_design.png
│   ├── phil_scale.png
│   ├── phil_polish.png
│   └── favicon.svg
└── dist/                   # Production build output (generated on build)
```

---

## 🎨 Customization Guide

### Updating Information
- **Name & Roles**: Edit the hero text, ticker tags, and title in [index.html](file:///home/dylan-abraham-k/Downloads/portfolio-20261022T172113Z-1-001/portfolio/index.html) and [main.js](file:///home/dylan-abraham-k/Downloads/portfolio-20261022T172113Z-1-001/portfolio/main.js).
- **Projects**: Project cards are defined in `#work` and their deep-dive modals in the `cs-overlay` containers inside [main.js](file:///home/dylan-abraham-k/Downloads/portfolio-20261022T172113Z-1-001/portfolio/main.js).
- **Contact Details**: Update email, phone, and LinkedIn links in the `#contact` panel section in [main.js](file:///home/dylan-abraham-k/Downloads/portfolio-20261022T172113Z-1-001/portfolio/main.js).

### Theme & Colors
Custom CSS variables are defined at the top of [style.css](file:///home/dylan-abraham-k/Downloads/portfolio-20261022T172113Z-1-001/portfolio/style.css):
```css
:root {
  --ink: #110e1b;
  --cream: #fbf9f5;
  --cream2: #f2eee5;
  --coral: #ff5757;
  --yellow: #ffc947;
  --teal: #00c9a7;
  --blue: #4361ee;
  --pink: #f72585;
  --purple: #7c3aed;
}
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
