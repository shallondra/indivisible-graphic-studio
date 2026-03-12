# Indivisible Graphic Studio

A browser-based, offline-first graphic design tool built for [Indivisible Auburn WA](https://indivisible.org) and the [No Kings Campaign](https://nokings.org). Create branded social media graphics, event banners, and campaign materials — no internet connection or software installation required.

> 🤖 Built with [Claude Code](https://claude.ai/code) by [Anthropic](https://anthropic.com)

---

## Features

- **5 canvas templates** — Instagram Post, Facebook Post, Bluesky Post, Bluesky Header, Event Banner
- **Brand presets** — one-click Indivisible Auburn WA and No Kings Campaign styling
- **Text tools** — Headlines (Barlow Condensed Black) and body text (Public Sans)
- **Image upload** — upload photos and composite them on the canvas
- **Pre-built brand assets** — No Kings logos, crowns, and Indivisible icons
- **Pixel rulers** — canvas rulers showing design-resolution coordinates
- **Smart background palette** — swatches update automatically from uploaded images or applied brand preset
- **Fit / Fill** — scale any object to contain or fill the canvas in one click
- **Position grid** — snap objects to 9 preset positions with 20px padding
- **Alt text drafting** — short (≤125 chars) + full accessible description fields
- **Full-resolution PNG export** — downloads at the template's native resolution
- **Save / Load project** — JSON format preserves all layers and settings
- **Fully offline** — no CDN, no network calls, no accounts required

---

## Quick Start

1. **Clone this repo**
   ```
   git clone https://github.com/shallondra/indivisible-graphic-studio.git
   cd indivisible-graphic-studio
   ```

2. **Open `index.html`** in your browser:
   ```
   open index.html
   ```
   Or double-click `index.html` in Finder.

3. **If logos/icons don't load** (browser file security on some systems):
   Launch Chrome with file access enabled:
   ```
   /Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome \
     --allow-file-access-from-files \
     /path/to/graphic-studio/index.html
   ```

> **Note:** Brand fonts and assets are not included in this repository. Place the `Indivisible assets/` folder one level above `graphic-studio/` to enable brand assets and logos.

---

## Workflow

1. **Pick a template** in the left panel
2. **Set background color** — click a swatch or use the color picker
3. **Apply brand preset** — "Indivisible Auburn WA" or "No Kings Campaign"
4. **Add content:**
   - `+ Headline` — large Barlow Condensed Black text
   - `+ Text Box` — body copy in Public Sans
   - `📷 Upload Image` — import a photo; background swatches update to image colors automatically
   - **NK Logo / Icons** — pre-built brand asset buttons
5. **Edit selected objects** in the right panel (font, color, size, position)
6. **Write alt text** — short ≤125 chars + full accessible description
7. **Download PNG** — saves at full resolution to your Downloads folder

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Delete` / `Backspace` | Delete selected object |
| `Escape` | Deselect |
| Click + drag | Move objects |
| Handles | Resize / rotate |

---

## Templates

| Template | Size | Use for |
|----------|------|---------|
| Instagram Post | 1080 × 1080 px | Instagram, square social |
| Facebook Post | 1200 × 630 px | Facebook feed posts |
| Bluesky Post | 1080 × 1080 px | Bluesky posts |
| Bluesky Header | 3000 × 1000 px | Bluesky profile banner |
| Event Banner | 1920 × 1080 px | Event promotions, website |

---

## Brand Specs

### Indivisible Auburn WA
| Color | Hex |
|-------|-----|
| Primary Blue | `#00417b` |
| Yellow | `#ffba08` |
| Red | `#ff0c0c` |
| Light Blue | `#21dee8` |

- **Headline font:** Barlow Condensed Black (900)
- **Body font:** Public Sans

### No Kings Campaign
| Color | Hex |
|-------|-----|
| Background Black | `#000000` |
| Accent Yellow | `#ffba08` |

- **Headline font:** Barlow Condensed Black (900)

---

## Folder Structure

```
graphic-studio/         ← This repo
  index.html            ← The entire app (single HTML file)
  fabric.min.js         ← Fabric.js 5.3.1 (bundled for offline use)
  README.md

../Indivisible assets/  ← Brand assets (not included, place alongside this folder)
  Indivisible Project-selected-assets/
    Barlow/             ← Headline fonts
    Barlow Condensed/   ← Condensed fonts
    Barlow Semi Condensed/
    Public_Sans/        ← Body font
    colors/colors.css   ← Official brand colors
    Indivisible Icons_*.png
  No Kings-selected-assets (1)/
    NK Full Logo.png
    NK Crown400px.png
    No Kings Logo_Horizontal_*.png
    No Kings Logo_Horizontal_*.svg
```

---

## Saving Your Work

- **Download PNG** — full-resolution image, saves to your Downloads folder
- **Save Project (.json)** — saves all layers, text, and settings for later editing
- **Load Project (.json)** — reopen a saved project

---

## Tips

- Font sizes in the properties panel are real pixels at full export resolution (not display pixels)
- The canvas shows at reduced zoom to fit your screen — exports are always full resolution
- Use `Auto-suggest from canvas` to generate a draft alt text from your text layers
- The position grid (↖ ↑ ↗ etc.) snaps objects to 9 preset positions with 20px padding
- After exporting, move the PNG from Downloads to Dropbox using Finder

---

## Attribution

- **App design and development:** [Claude Code](https://claude.ai/code) by [Anthropic](https://anthropic.com)
- **Canvas library:** [Fabric.js](http://fabricjs.com/) v5.3.1 — BSD License
- **Fonts:** Barlow family (Jeremy Tribby) and Public Sans (USWDS) — SIL Open Font License
- **Brand assets:** © Indivisible Project and No Kings Campaign — not covered by this repo's license

---

## License

The application code in this repository is released under the [MIT License](LICENSE).

Brand assets, logos, and fonts are property of their respective owners and are **not** covered by this license.
