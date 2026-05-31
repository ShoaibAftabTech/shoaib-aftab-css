# Typography

Shoaib Aftab CSS makes it easy to handle fonts, sizes, weights, and alignment.

## Font Sizes

Use `.sa-text-{size}` classes to control the font size.

### Example
```html
<h1 class="sa-text-4xl sa-font-bold">Heading 4XL</h1>
<p class="sa-text-base sa-text-gray-600">This is base level paragraph text.</p>
```

**Visual Representation:**
<h1 style="font-size: 2.25rem; font-weight: 700; margin:0;">Heading 4XL</h1>
<p style="font-size: 1rem; color: #4b5563; margin:0;">This is base level paragraph text.</p>

## Text Alignment

Classes: `.sa-text-left`, `.sa-text-center`, `.sa-text-right`, `.sa-text-justify`

```html
<div class="sa-text-center sa-bg-gray-100 sa-p-4">
  Centered Text
</div>

## Font Families & Premium Google Fonts

Shoaib Aftab CSS has pre-integrated 12 curated, industry-standard Google Fonts that satisfy 100% of all future development or client typography needs.

### 1. Default Role Assigners (Global Customizability)
The framework maps fonts to active roles inside `:root`. You can override these variables globally to change font families across your entire application instantly:
- `--sa-font-primary`: The primary body/interface font (Default: `Inter`)
- `--sa-font-heading`: The primary heading font (Default: `Plus Jakarta Sans`)
- `--sa-font-display`: The heavy marketing display font (Default: `Bebas Neue`)
- `--sa-font-code`: The coding/monospace font (Default: `JetBrains Mono`)

### 2. Available Font Family Utility Classes
Apply specific fonts instantly to any element:

| Class | Font Family | Ideal Use Case |
| :--- | :--- | :--- |
| `.sa-font-inter` | **Inter** | SAAS dashboards, general UI text, clean body |
| `.sa-font-jakarta` | **Plus Jakarta Sans** | Punchy headings, modern tech startups UI |
| `.sa-font-outfit` | **Outfit** | Soft, elegant rounded-geometric design |
| `.sa-font-montserrat` | **Montserrat** | Professional landing pages, clean marketing titles |
| `.sa-font-playfair` | **Playfair Display** | Traditional, luxury editorial or serif headings |
| `.sa-font-lora` | **Lora** | High-readability editorial articles, blogs |
| `.sa-font-fira` | **Fira Code** | Coding examples, technical terminals with ligatures |
| `.sa-font-jetbrains` | **JetBrains Mono** | Ultra-readable system metrics, logs, monospace charts |
| `.sa-font-grotesk` | **Space Grotesk** | Futuristic, tech-oriented landing pages |
| `.sa-font-bebas` | **Bebas Neue** | Bold, condensed attention-grabbing poster headers |
| `.sa-font-syne` | **Syne** | Ultra-modern, artistic, offbeat creative designs |
| `.sa-font-cinzel` | **Cinzel** | High-end luxury brands, book titles, roman-serif headings |

### 3. Font Role Utility Classes
Apply dynamically assigned roles:
- `.sa-font-primary`: Maps to `--sa-font-primary` (Default: `Inter`)
- `.sa-font-heading`: Maps to `--sa-font-heading` (Default: `Plus Jakarta Sans`)
- `.sa-font-display`: Maps to `--sa-font-display` (Default: `Bebas Neue`)
- `.sa-font-code`: Maps to `--sa-font-code` (Default: `JetBrains Mono`)
