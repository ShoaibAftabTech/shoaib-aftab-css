<div align="center">
  <br>
  <strong>🎯 Official Live Examples:</strong> <a href="https://shoaibaftab.com/shoaib-aftab-css#examples">https://shoaibaftab.com/shoaib-aftab-css#examples</a>
  <br><br>
</div>

# Shoaib Aftab CSS Framework - Practical Examples

This document provides ready-to-use, copy-pasteable HTML snippets that demonstrate the power and beauty of the **Shoaib Aftab CSS Framework**. All examples are fully responsive and rely on 0 external dependencies.

---

## 1. The Glassmorphism Hero Section
A modern, vibrant hero section using OKLCH gradients, `dvh` (Dynamic Viewport Height), and the `sa-glass` utility.

```html
<header class="sa-h-dvh sa-flex sa-items-center sa-justify-center sa-relative sa-overflow-hidden sa-bg-neutral-900">
    
    <!-- Animated OKLCH Background Blob -->
    <div class="sa-absolute sa-inset-0 sa-opacity-50" style="background: radial-gradient(circle at top right, oklch(0.65 0.3 260) 0%, transparent 60%);"></div>

    <div class="sa-container sa-text-center sa-relative sa-z-10">
        <h1 class="sa-font-heading sa-text-6xl md:sa-text-8xl sa-font-bold sa-mb-6 sa-text-transparent sa-bg-clip-text sa-bg-gradient-to-r sa-from-white sa-to-gray-400">
            Design the Future.
        </h1>
        <p class="sa-text-xl sa-text-gray-300 sa-mb-10 sa-max-w-2xl sa-mx-auto">
            Zero dependencies. Infinite possibilities.
        </p>
        
        <div class="sa-flex sa-gap-4 sa-justify-center">
            <!-- Glass Button -->
            <button class="sa-glass sa-text-white sa-px-8 sa-py-4 sa-rounded-full sa-font-semibold hover:sa-bg-white/10 sa-transition-all">
                Get Started
            </button>
            <!-- Solid Button -->
            <button class="sa-bg-white sa-text-black sa-px-8 sa-py-4 sa-rounded-full sa-font-semibold sa-shadow-xl hover:sa-scale-105 sa-transition-transform">
                Read Docs
            </button>
        </div>
    </div>
</header>
```

---

## 2. Next-Gen Dashboard Layout (Grid Subgrid)
This layout uses CSS Grid Level 2. The inner widgets align perfectly to the main dashboard's 12-column grid.

```html
<div class="sa-min-h-dvh sa-bg-neutral-100 sa-p-8">
    <div class="sa-grid sa-grid-cols-12 sa-gap-6 sa-max-w-7xl sa-mx-auto">
        
        <!-- Sidebar (Spans 3 cols) -->
        <aside class="sa-col-span-12 lg:sa-col-span-3 sa-bg-white sa-p-6 sa-rounded-2xl sa-shadow-sm">
            <h2 class="sa-font-bold sa-text-xl sa-mb-4">Menu</h2>
            <nav class="sa-flex sa-flex-col sa-gap-2">
                <a href="#" class="sa-text-primary-600 sa-bg-primary-50 sa-p-3 sa-rounded-lg sa-font-medium">Dashboard</a>
                <a href="#" class="sa-text-neutral-600 hover:sa-bg-neutral-50 sa-p-3 sa-rounded-lg">Analytics</a>
                <a href="#" class="sa-text-neutral-600 hover:sa-bg-neutral-50 sa-p-3 sa-rounded-lg">Settings</a>
            </nav>
        </aside>

        <!-- Main Content (Spans 9 cols) -->
        <main class="sa-col-span-12 lg:sa-col-span-9 sa-grid sa-grid-cols-subgrid">
            
            <!-- Widget 1 (Spans 6 out of 9 parent cols) -->
            <div class="sa-col-span-12 lg:sa-col-span-6 sa-bg-white sa-p-8 sa-rounded-2xl sa-shadow-sm sa-flex sa-items-center sa-justify-center sa-h-64">
                <h3 class="sa-text-neutral-400 sa-font-medium">Revenue Chart</h3>
            </div>

            <!-- Widget 2 (Spans 3 out of 9 parent cols) -->
            <div class="sa-col-span-12 lg:sa-col-span-3 sa-bg-primary-600 sa-text-white sa-p-8 sa-rounded-2xl sa-shadow-sm sa-flex sa-flex-col sa-justify-center">
                <h3 class="sa-text-primary-100 sa-font-medium sa-mb-2">Total Users</h3>
                <p class="sa-text-4xl sa-font-bold">24,500</p>
            </div>

        </main>
    </div>
</div>
```

---

## 3. Responsive Product Cards (Container Queries)
Unlike media queries that look at the screen size, this component changes its layout based on where you place it. Put it in a narrow sidebar, it becomes a stack. Put it in a wide main area, it becomes a row.

```html
<!-- Define the Container -->
<div class="sa-container-type-inline-size">
    
    <!-- Apply Query-based classes -->
    <article class="sa-flex sa-flex-col sa-cq-md:sa-flex-row sa-bg-white sa-rounded-2xl sa-shadow-lg sa-overflow-hidden">
        
        <!-- Image Area -->
        <div class="sa-w-full sa-cq-md:sa-w-1/3 sa-bg-neutral-200 sa-h-48 sa-cq-md:sa-h-auto sa-flex sa-items-center sa-justify-center">
            <span class="sa-text-neutral-500">Product Image</span>
        </div>
        
        <!-- Content Area -->
        <div class="sa-p-6 sa-cq-md:sa-p-8 sa-flex sa-flex-col sa-justify-center">
            <span class="sa-text-xs sa-font-bold sa-text-primary-600 sa-uppercase sa-tracking-wider sa-mb-2">New Arrival</span>
            <h2 class="sa-text-2xl sa-font-bold sa-text-neutral-900 sa-mb-2">Enterprise Server</h2>
            <p class="sa-text-neutral-600 sa-mb-4">Zero dependency architecture for maximum security and compliance.</p>
            <button class="sa-bg-black sa-text-white sa-px-6 sa-py-3 sa-rounded-lg sa-font-medium sa-w-full sa-cq-md:sa-w-auto">Buy Now</button>
        </div>

    </article>

</div>
```

---

## 4. Scroll-Driven Animations Layout
A simple layout where elements natively fade in as you scroll down the page.

```html
<div class="sa-container sa-py-24">
    <div class="sa-max-w-3xl sa-mx-auto sa-space-y-12">
        
        <div class="sa-bg-neutral-100 sa-p-12 sa-rounded-3xl sa-animate-scroll-fade">
            <h2 class="sa-text-3xl sa-font-bold sa-mb-4">Section 1</h2>
            <p class="sa-text-neutral-600">Scroll down to see the next section fade in.</p>
        </div>

        <div class="sa-bg-neutral-100 sa-p-12 sa-rounded-3xl sa-animate-scroll-fade">
            <h2 class="sa-text-3xl sa-font-bold sa-mb-4">Section 2</h2>
            <p class="sa-text-neutral-600">This faded in natively using CSS animation-timeline!</p>
        </div>

    </div>
</div>
```
