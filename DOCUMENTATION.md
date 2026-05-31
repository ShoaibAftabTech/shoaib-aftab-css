<div align="center">
  <br>
  <strong>🌍 Official Live Documentation:</strong> <a href="https://shoaibaftab.com/shoaib-aftab-css-docs">https://shoaibaftab.com/shoaib-aftab-css-docs</a>
  <br><br>
</div>

# Shoaib Aftab CSS Framework - Complete Documentation

Welcome to the comprehensive, offline reference manual for the **Shoaib Aftab CSS Framework (V2)**. This framework is an enterprise-grade, zero-dependency, and GDPR-compliant utility and component library designed for the modern web. 

This document serves as an exhaustive guide to utilizing the framework's architecture, including CSS Level 4 and Level 5 features.

---

## Table of Contents
1. [Core Philosophy](#core-philosophy)
2. [GDPR & Typography Fallbacks](#gdpr--typography-fallbacks)
3. [The OKLCH Color System](#the-oklch-color-system)
4. [Advanced Grid & Subgrid](#advanced-grid--subgrid)
5. [Container Queries](#container-queries)
6. [Dynamic Viewport Units](#dynamic-viewport-units)
7. [Scroll-Driven Animations](#scroll-driven-animations)
8. [Utility Classes Reference](#utility-classes-reference)

---

## 1. Core Philosophy

### The "Zero Dependency" Rule
The defining feature of this framework is its absolute independence. It requires **0 NPM packages** to run in production. There is no Webpack, no PostCSS, and no Tailwind compiler required. The compiled `shoaib-aftab.min.css` file works natively in any modern browser.

**Why?**
- **Security:** Zero risk of supply-chain attacks.
- **Compatibility:** Works flawlessly on high-end AWS clusters and budget shared hosting alike.
- **Longevity:** Pure CSS doesn't deprecate like JavaScript build tools do.

---

## 2. GDPR & Typography Fallbacks

We have strictly removed Google Fonts and third-party CDNs from the core framework to ensure **100% GDPR, ePrivacy, and CCPA compliance**.

### Native System Font Stack
By default, the framework utilizes the operating system's native fonts. This makes rendering lightning-fast and preserves battery life on mobile devices.

- **Apple Devices:** San Francisco
- **Windows Devices:** Segoe UI
- **Android Devices:** Roboto

### Custom Fonts (Strict Fallback)
If you apply a custom font class (e.g., `sa-font-inter`), and the font fails to load or the client blocks it, the framework will gracefully and invisibly fall back to the `sa-font-sans` stack.

```html
<!-- Automatically uses OS native font if Inter is not self-hosted -->
<h1 class="sa-font-inter sa-font-bold">Enterprise Headline</h1>
```

---

## 3. The OKLCH Color System

We have transitioned from RGB/HSL to the next-generation **OKLCH** color space. OKLCH represents colors exactly how the human eye perceives them, resulting in smoother gradients and perfectly uniform lightness across different hues.

### Usage
Colors are applied via utility classes:
- Backgrounds: `sa-bg-primary-500`
- Text: `sa-text-danger-400`
- Borders: `sa-border-success-300`

### Example
```html
<div class="sa-bg-primary-600 sa-text-white sa-border sa-border-primary-400">
  This uses vivid OKLCH colors!
</div>
```

---

## 4. Advanced Grid & Subgrid

The framework provides full support for CSS Grid Level 2, specifically **Subgrid**.

### Basic Grid
Use standard column configurations.
```html
<div class="sa-grid sa-grid-cols-4 sa-gap-4">
  <div class="sa-col-span-2">Spans 2 columns</div>
</div>
```

### Grid Subgrid (Enterprise Layouts)
Subgrid allows nested elements to participate in the sizing of their parent grid.
```html
<div class="sa-grid sa-grid-cols-3 sa-gap-6">
  <!-- Parent Card -->
  <div class="sa-grid sa-grid-cols-subgrid sa-col-span-3">
    <!-- These children align perfectly to the top-level 3-column grid -->
    <div class="sa-p-4">Header</div>
    <div class="sa-col-span-2 sa-p-4">Content Area</div>
  </div>
</div>
```

### Masonry Layout
A true masonry layout without JavaScript.
```html
<div class="sa-masonry sa-masonry-cols-3 sa-gap-4">
  <div class="sa-break-inside-avoid">Card 1</div>
  <div class="sa-break-inside-avoid">Card 2</div>
</div>
```

---

## 5. Container Queries

Container Queries (`@container`) are the future of responsive design. Instead of styling elements based on the width of the browser window (`@media`), you style them based on the width of their parent container.

### How to Use
1. Define the container using `sa-container-type-inline-size`.
2. Apply specific query prefixes to the children (e.g., `sa-cq-md:`).

```html
<div class="sa-container-type-inline-size">
  <!-- If the parent is wider than 768px, use 2 columns. 
       Regardless of what the browser window size is. -->
  <div class="sa-grid sa-gap-4 sa-cq-md:sa-grid-cols-2">
    <div>Widget A</div>
    <div>Widget B</div>
  </div>
</div>
```

---

## 6. Dynamic Viewport Units

Mobile browsers have dynamic toolbars (URL bar showing/hiding on scroll). Traditional `100vh` causes content to be hidden behind these bars. We solve this natively using `dvh`.

```html
<!-- This element will always be exactly the height of the visible screen -->
<header class="sa-h-dvh sa-flex sa-items-center">
  Hero Content
</header>
```

---

## 7. Scroll-Driven Animations

You no longer need heavy JavaScript libraries (like GSAP or AOS) for simple scroll animations. We utilize the native CSS `animation-timeline`.

```html
<!-- This element will fade in exactly as it enters the viewport -->
<div class="sa-animate-scroll-fade">
  I animate natively on scroll!
</div>
```

---

## 8. Utility Classes Reference

### Spacing (Padding / Margin)
Uses a standard `0.25rem` multiplier.
- `sa-p-4` (Padding: 1rem)
- `sa-px-6` (Padding Left/Right: 1.5rem)
- `sa-mb-8` (Margin Bottom: 2rem)

### Typography
- `sa-text-xs` through `sa-text-9xl`
- `sa-font-light`, `sa-font-normal`, `sa-font-bold`, `sa-font-black`
- `sa-text-center`, `sa-text-right`, `sa-text-justify`

### Display & Flexbox
- `sa-flex`, `sa-inline-flex`, `sa-hidden`, `sa-block`
- `sa-items-center`, `sa-justify-between`, `sa-flex-col`

### Visual Effects (Glassmorphism)
- `sa-glass` (Applies backdrop-filter blur and semi-transparent background)
- `sa-shadow-sm` through `sa-shadow-2xl`
- `sa-rounded-sm` through `sa-rounded-full`

---
*For interactive demos and more details, please visit [shoaibaftab.com](https://shoaibaftab.com).*
