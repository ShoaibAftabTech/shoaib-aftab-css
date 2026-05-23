# 📋 shoaib-aftab-css | Documentation

Welcome to the official documentation for **shoaib-aftab-css**—a powerful, lightweight, utility-first, and component-driven CSS framework designed to build scalable UI architectures rapidly.

---

## 🗺️ Documentation Map (Pattern: shoaibaftab.com/shoaib-aftab-css-docs)

### 1. Getting Started
* [Introduction](#introduction)
* [Installation](#installation)
* [Core Concepts](#core-concepts)

### 2. Layout & Grid
* [Containers](#containers)
* [Grid System](#grid)
* [Flexbox Utilities](#flexbox)
* [Breakpoints](#breakpoints)
* [Z-Index](#z-index)

### 3. Components
* [Buttons & Groups](#buttons)
* [Cards & Panels](#cards)
* [Forms & Inputs](#forms)
* [Modals & Popups](#modals)

### 4. Utilities
* [Colors & Backgrounds](#colors)
* [Margin & Padding](#spacing)
* [Typography](#typography)
* [Shadows & Borders](#shadows)
* [Interactive Pseudo-States (New!)](#interactive-states)

---

## 🚀 1. Getting Started

### Introduction
`shoaib-aftab-css` is a modern CSS framework built strictly on W3C CSS Specifications with absolutely **zero dependencies**. It features a robust layout engine, built-in dark mode support, and native RTL mirroring for Urdu and Arabic web platforms.

### Installation
Include the minified stylesheet inside the `<head>` of your HTML document:
```html
<link href="https://cdn.jsdelivr.net/gh/ShoaibAftabTech/shoaib-aftab-css@main/dist/shoaib-aftab.min.css" rel="stylesheet">
```

### Core Concepts
The framework combines the agility of **Utility CSS** (like Tailwind) with pre-designed **Components** (like Bootstrap) to eliminate custom CSS write-ups:
* **Utilities:** Fast spacing, alignments, and typography adjustments.
* **Prefix `sa-`:** Prevents naming collisions with other global stylesheets.

---

## 📐 2. Layout & Grid

### Grid System
Create modern responsive grid systems up to 12 columns:
```html
<div class="sa-grid sa-grid-cols-1 sa-md:grid-cols-2 sa-lg:grid-cols-4 sa-gap-4">
  <div class="sa-bg-gray-100 sa-p-4">Box 1</div>
  <div class="sa-bg-gray-100 sa-p-4">Box 2</div>
  <div class="sa-bg-gray-100 sa-p-4">Box 3</div>
  <div class="sa-bg-gray-100 sa-p-4">Box 4</div>
</div>
```

### Breakpoints
The framework defines 6 highly responsive screen breakpoints:
* `sa-sm:` (Mobile Landscape - `640px`)
* `sa-md:` (Tablets - `768px`)
* `sa-lg:` (Laptops - `1024px`)
* `sa-xl:` (Desktops - `1280px`)
* `sa-2xl:` (Large Desktops - `1536px`)
* `sa-3xl:` (Ultra-Wide Monitors - `1920px`)

---

## 🎨 3. Components

### Buttons & Groups
Buttons support hover effects, click scaling transitions, and sizes:
```html
<button class="sa-btn sa-btn-primary sa-hover:bg-primary-hover sa-active:scale-95">Submit</button>
<button class="sa-btn sa-btn-outline">Cancel</button>
```

### Cards & Panels
```html
<div class="sa-card sa-hover:shadow-lg sa-transition-all">
  <div class="sa-card-header">Profile Card</div>
  <div class="sa-card-body">Name: Shoaib Aftab</div>
</div>
```

---

## 🛠️ 4. Utilities

### Colors & Backgrounds
* Background colors: `.sa-bg-primary`, `.sa-bg-success`, `.sa-bg-danger`, `.sa-bg-gray-50` to `.sa-bg-gray-900`.
* Opacity modifiers (New!): Use `\/20` to `\/80` to apply HSL opacity adjustments.

### Margin & Padding
Spacings (paddings, margins, gaps) range from `0` to `24` (`6rem`) for ultimate visual control:
* Gaps: `.sa-gap-4`, `.sa-gap-x-2`, `.sa-gap-y-6`.
* Spacing: `.sa-p-4`, `.sa-m-6`, `.sa-px-12`, `.sa-my-24`.

### Typography
Text sizes range from `.sa-text-xs` (0.75rem) to `.sa-text-9xl` (8rem) for elegant headings:
* Weight: `.sa-font-thin` (100) to `.sa-font-black` (900).

### Shadows & Borders
Premium drop shadows for depth:
* Shadows: `.sa-shadow-sm`, `.sa-shadow-md`, `.sa-shadow-lg`, `.sa-shadow-xl`, `.sa-shadow-2xl` (New!), `.sa-shadow-inner` (New!).

---

## ⚡ 5. Interactive Pseudo-States (New!)
Equip any HTML element with 30+ responsive pseudo-states for hovering, focus outline, active scaling, and group-hover:
```html
<!-- 3D Lift card on hover with active click scale -->
<div class="sa-card sa-hover:translate-y-neg2 sa-hover:shadow-xl sa-active:scale-95 sa-transition-all">
  <h3>Interactive Component</h3>
</div>

<!-- Focus outlines for smart inputs -->
<input class="sa-input sa-focus:ring-2 sa-focus:border-primary sa-transition">
```
