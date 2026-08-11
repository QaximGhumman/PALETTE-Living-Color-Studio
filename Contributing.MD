# Contributing to PALETTE · Living Color Studio

Thanks for your interest in improving PALETTE! This is a small, single-file, dependency-free project — contributions of any size are welcome, from typo fixes to new features.

## 🧭 Ground Rules

- Be respectful and constructive in issues and PRs.
- Keep the project **dependency-free** (no build step, no npm packages) unless there's a strong reason to add one — open an issue to discuss first.
- Keep `index.html` as the single source file unless a change genuinely requires splitting it up.

## 🐛 Reporting Bugs

Open an [issue](../../issues) and include:

- What you did (steps to reproduce)
- What you expected to happen
- What actually happened
- Browser + OS (some features like `navigator.clipboard` and `backdrop-filter` behave differently across browsers)
- Screenshots or a screen recording, if relevant

## 💡 Suggesting Features

Open an issue describing:

- The problem you're trying to solve
- Your proposed solution
- Any alternatives you considered

Good candidates: new palette generation modes, export formats, accessibility improvements, or UI polish.

## 🔧 Making Changes

1. **Fork** the repository
2. **Clone** your fork:
   ```bash
   git clone https://github.com/<your-username>/palette-living-color-studio.git
   cd palette-living-color-studio
   ```
3. **Create a branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Make your changes** in `index.html`. Since there's no build step, just open the file in a browser to test:
   ```bash
   open index.html
   ```
5. **Test thoroughly** before submitting:
   - Upload an image and confirm colors extract correctly
   - Try a few mood keywords, including ones not in the mood map (fallback generator)
   - Let the time-based palette run, or press `T` to force a refresh
   - Shuffle a few times (`R`) and check different harmony types look reasonable
   - Lock a color, regenerate, and confirm it stays fixed
   - Drag the palette size slider to both extremes (3 and 8)
   - Save a palette, reload the page, confirm it persists
   - Export as CSS and JSON and check the output
   - Resize the window / test on mobile widths (768px, 480px breakpoints)
6. **Commit** with a clear message:
   ```bash
   git commit -m "Add: short description of your change"
   ```
7. **Push** and open a **Pull Request** against `main`, describing what changed and why.

## 🎨 Code Style

- Vanilla JS, no frameworks — match the existing style (small focused functions, `const`/`let`, arrow functions where used elsewhere in the file)
- CSS uses custom properties and BEM-ish class naming (`.color-card .hex`, `.preview-item.card`) — follow the existing pattern
- Keep functions pure where possible (e.g. color conversion utilities take input, return output, no side effects)
- Comment non-obvious color math (HSL conversions, contrast calculations) briefly

## ✅ Pull Request Checklist

- [ ] Changes are contained to `index.html` (or justified if not)
- [ ] Tested manually across the scenarios above
- [ ] No console errors
- [ ] Works at both desktop and mobile widths
- [ ] README updated if you added/changed a user-facing feature

## 📄 License

By contributing, you agree your contributions will be licensed under the project's MIT License.
