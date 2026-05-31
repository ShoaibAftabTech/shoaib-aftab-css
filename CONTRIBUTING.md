# Contributing to Shoaib Aftab CSS

First off, thank you for considering contributing to the Shoaib Aftab CSS Framework! It's people like you that make this ecosystem enterprise-ready and globally adopted.

## 🛑 The Golden Rule: Absolute Zero Dependency
Before you submit a Pull Request, you MUST understand our core architecture:
**We do not use NPM packages for the final build. We do not use PostCSS. We do not use external CDNs.**

If your PR requires adding a dependency to `package.json` (other than standard dev tools if absolutely negotiated), it will be **rejected**.

## How to Contribute

### 1. Local Development
1. Clone the repository.
2. Make your CSS changes in the `src/modules/` directory.
3. Run the custom native build script to minify the CSS:
   ```bash
   npm run build
   ```
4. Verify that `dist/shoaib-aftab.min.css` was generated successfully and no errors were thrown.

### 2. Style Guidelines
- **Variables:** Always use the `--sa-` prefix.
- **Classes:** Always use the `sa-` prefix to prevent collisions with other libraries.
- **Modern CSS:** You are encouraged to use CSS Level 4/5 features (Grid Subgrid, `oklch`, `:has()`, Container Queries), but ensure they degrade gracefully if possible.

### 3. Submitting a Pull Request
- Create a feature branch (`git checkout -b feature/amazing-feature`).
- Commit your changes.
- Ensure the build passes.
- Open a PR with a clear description of the problem solved or feature added.
