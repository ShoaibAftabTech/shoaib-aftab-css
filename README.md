<div align="center">
  <a href="https://shoaibaftab.com">
    <img src="https://shoaibaftab.com/images/logo.png" alt="Shoaib Aftab Tech Logo" width="300">
  </a>
  <br><br>
  <h1>🚀 Shoaib Aftab CSS Ecosystem (V2)</h1>
  <p><strong>The Ultimate, 0-Dependency, GDPR-Compliant, Enterprise CSS Framework</strong></p>
  
  <p>
    [![Version](https://img.shields.io/npm/v/@shoaibaftabtech/css)](https://www.npmjs.com/package/@shoaibaftabtech/css)
    [![License: MIT](https://img.shields.io/badge/License-MIT-success.svg)](https://opensource.org/licenses/MIT)
    <a href="#"><img src="https://img.shields.io/badge/dependencies-0-success?style=flat-square" alt="Dependencies"></a>
    <a href="#"><img src="https://img.shields.io/badge/GDPR-Compliant-success?style=flat-square" alt="GDPR"></a>
  </p>
</div>

<br>

Shoaib Aftab CSS is a next-generation, utility-first, and component-driven CSS framework designed for enterprise scale. Built completely from scratch with the philosophy of **Absolute Zero Dependency**, it guarantees maximum performance, unparalleled security, and absolute privacy compliance.

## ✨ Why Shoaib Aftab CSS?

Unlike traditional frameworks (Bootstrap, Tailwind) that require heavy Node.js build steps, PostCSS pipelines, or extensive configuration, our framework runs entirely natively in the browser while offering CSS Level 4 & 5 features.

- **0% Dependency:** No Node.js required. No external CDNs. Works flawlessly on shared hosting.
- **100% GDPR Compliant:** No third-party font tracking. Defaults to blazing-fast native system fonts.
- **Future-Proof Standards:** Features CSS Grid Level 2 (Subgrid), Masonry layouts, Container Queries (`@container`), and Scroll-Driven Animations natively.
- **Dynamic Viewports:** Full support for `svh`, `lvh`, and `dvh` units for perfect mobile rendering.
- **Next-Gen Colors:** Built-in support for ultra-vivid `oklch()` color spaces.
- **Enterprise Security:** Hardened against ReDoS. Completely static architecture with zero runtime injection vulnerabilities.

## 📦 Installation

We offer three ways to integrate the framework, ranging from basic script tags to NPM modules.

### Option 1: Direct Download (Maximum Security / Air-gapped)
Download the `dist/shoaib-aftab.min.css` file and include it directly in your HTML.
```html
<link rel="stylesheet" href="./path/to/shoaib-aftab.min.css">
```

### Option 2: NPM / Yarn
```bash
npm install @shoaibaftabtech/css
```
```javascript
import '@shoaibaftabtech/css/dist/shoaib-aftab.min.css';
```

### Option 3: CDN (Development Only)
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@shoaibaftabtech/css/dist/shoaib-aftab.min.css">
```

## 🎨 Modern Features

### 1. Advanced Grid & Layouts
Take advantage of CSS Level 4 Grid capabilities directly through utility classes.
```html
<!-- Grid Level 2 Subgrid -->
<div class="sa-grid sa-grid-cols-3">
  <div class="sa-grid sa-grid-cols-subgrid sa-col-span-3">
    <!-- Items align perfectly to parent grid -->
  </div>
</div>

<!-- Native Masonry Layout -->
<div class="sa-masonry sa-masonry-cols-3 sa-gap-4">
  <div class="sa-break-inside-avoid">...</div>
</div>
```

### 2. Scroll-Driven Animations
No JavaScript required. Bind animations directly to the scroll timeline.
```html
<div class="sa-animate-scroll-fade">Fades in as you scroll!</div>
```

### 3. Container Queries
Responsive design based on the parent's width, not the viewport.
```html
<div class="sa-container">
  <div class="sa-cq-lg:sa-grid-cols-2">
    <!-- Two columns only when the *container* is large -->
  </div>
</div>
```

### 4. Dynamic Viewport Units
Say goodbye to the mobile browser bar issue.
```html
<div class="sa-h-dvh">Perfect 100% height, adapting dynamically to the browser UI</div>
```

## 🔒 Security & Privacy (Enterprise Grade)

We built this framework for banking, healthcare, and high-security sectors:
1. **Zero Google Fonts / CDNs:** The framework defaults to the native system font stack (San Francisco, Segoe UI, Roboto) preventing IP leakage to third parties.
2. **ReDoS Protected:** The internal custom build pipeline uses strictly linear RegEx, protecting against catastrophic backtracking.
3. **Impenetrable CSS:** Static nature prevents CSS Keylogging and Data URI bypasses.

> Note: To use custom fonts (like Inter or Roboto), we strongly recommend self-hosting `.woff2` files to maintain strict GDPR compliance.

## 🛠 Project Architecture

The source files are highly modular, following atomic design principles:
- `modules/variables.css` (OKLCH Tokens, Fonts)
- `modules/layout.css` (Grid, Subgrid, Masonry)
- `modules/sizing.css` (svh, lvh, dvh)
- `modules/utilities.css` (Container Queries, Has() selectors)
- `modules/animations.css` (Scroll-Timelines)

## 🤝 Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](./CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) for guidelines. **Note: All PRs must adhere to the 0-dependency rule.**

## 📄 License

This project is licensed under the [MIT License](./LICENSE) - see the LICENSE file for details.

---

## 🏢 About Shoaib Aftab Tech

💻 **Specializing in Custom Development:** We build future-proof software, intuitive mobile apps, professional websites, scalable e-commerce platforms, and API development (WhatsApp Business API).

🔧 **Your End-to-End Partner:** From initial concept to successful scaling, we provide complete digital solutions for your business.

🤝 **Ready to Build & Grow?** Let's connect to discuss your project and strategic goals.

### 🌐 Connect With Us
- **Visit us at:** [shoaibaftab.com](https://shoaibaftab.com)
- **Email:** [tech@shoaibaftab.com](mailto:tech@shoaibaftab.com)
- **Facebook:** [Shoaib Aftab Tech](https://facebook.com/ShoaibAftabTech)

<div align="center">
  <br>
  <em>Developed with excellence by <a href="https://shoaibaftab.com">Shoaib Aftab Tech</a></em>
</div>
