# 🎨 PALETTE · Living Color Studio

> A living, breathing color palette generator — extract palettes from photos, moods, or the current time of day.

## ✨ Overview

**PALETTE** is a single-file, dependency-free web app for generating and exploring color palettes. Instead of a static color picker, it pulls palettes from three living sources:

- 🖼️ **From Photo** — drag & drop or upload an image to extract its dominant colors
- 💭 **From Mood** — type a feeling or word (e.g. *serenity*, *autumn*, *midnight*) and get a matching palette
- 🕐 **From Time** — palettes shift automatically with the time of day (sunrise, morning, afternoon, sunset, evening, night)

Every palette comes with a live UI preview (cards, buttons, accents) so you can see how the colors actually look in context, one-click hex copying, and the ability to save favorite palettes locally.

## 🚀 Features

- Dominant color extraction from uploaded images via canvas pixel sampling
- Mood-to-color mapping with a fallback generative algorithm for unmapped moods
- Real-time, time-of-day-based palette generation (auto-refreshes every minute)
- Click-to-copy hex codes with visual feedback
- Live component preview (cards, buttons, outlines) using the generated palette
- Save/delete named palettes (persisted via `localStorage`)
- Keyboard shortcuts: `Ctrl/Cmd + S` to save, `T` for a time-based refresh
- Fully responsive layout (desktop, tablet, mobile)
- Zero build step — pure HTML, CSS, and vanilla JavaScript

## 🛠️ Tech Stack

- HTML5 / CSS3 (custom properties, backdrop-filter, CSS grid)
- Vanilla JavaScript (Canvas API, Clipboard API, LocalStorage API)
- [Google Fonts](https://fonts.google.com/) — Inter & Space Grotesk

## 📦 Getting Started

No build tools or dependencies required.

```bash
git clone https://github.com/<your-username>/palette-living-color-studio.git
cd palette-living-color-studio
open index.html   # or just double-click the file / use a local server
```

## 🖱️ Usage

1. **Upload a photo** — drop an image into the sidebar to extract its dominant palette
2. **Type a mood** — enter a word like "ocean" or "lavender" and hit Generate
3. **Let time do it** — the app auto-generates a palette based on the current time of day
4. Click any swatch to **copy its hex code**
5. Click the ❤️ icon (or `Ctrl/Cmd + S`) to **save** the current palette for later


## 📄 License

MIT License — feel free to use, modify, and distribute.

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.
