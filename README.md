# AAMS Decor — Website Source Files

This is the complete source for the AAMS Decor landing page: elegant home,
event, party, and balloon decoration in Zaria, Kaduna State.

## Folder structure

```
aams-decor-site/
├── index.html          → the page itself
├── css/
│   └── styles.css      → all styling (colors, fonts, layout)
├── images/              → all 9 portfolio photos used in the gallery
└── README.md            → this file
```

Everything is plain HTML/CSS with a small inline script for the contact
form — no build step, no frameworks, no dependencies to install.

## Running it locally in VS Code with Live Server

1. Open the `aams-decor-site` folder in VS Code (`File → Open Folder…`).
2. If you don't already have it, install the **Live Server** extension
   (by Ritwick Dey) from the Extensions panel (`Ctrl+Shift+X` / `Cmd+Shift+X`,
   search "Live Server").
3. Right-click `index.html` in the file explorer and choose
   **"Open with Live Server"** (or click "Go Live" in the bottom-right
   status bar).
4. Your browser will open the site at something like
   `http://127.0.0.1:5500/index.html`, and it will auto-refresh whenever
   you save a change.

## Editing

- **Text and layout** — edit `index.html` directly. Each section is
  commented (`<!-- ---------- HERO ---------- -->` etc.) so you can find
  things quickly.
- **Colors, fonts, spacing** — edit `css/styles.css`. The color palette is
  defined once at the top under `:root` (e.g. `--rose`, `--gold`,
  `--plum`) — change those and the whole site updates.
- **Photos** — swap any file in `images/` (keep the same filename, or
  update the `src="images/..."` reference in `index.html` if you rename
  it).
- **Contact details** — the WhatsApp number, Instagram, and TikTok links
  are in the "Get in touch" section and the footer near the bottom of
  `index.html`.

## Fonts

The page loads two Google Fonts via a `<link>` in the `<head>`:
Cormorant Garamond (headings) and Jost (body text). This requires an
internet connection when viewing the page; if you need it to work fully
offline, the fonts can be downloaded and self-hosted instead.

## Deploying it for real

This is a static site, so it can be hosted almost anywhere for free:
**Netlify**, **Vercel**, **GitHub Pages**, or **Cloudflare Pages** all
work by simply dragging this folder in or connecting a Git repo — no
server setup required.
