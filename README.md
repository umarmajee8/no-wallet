# E Wallet

All your cards. One tidy wallet.

A single-file, production-ready landing page for the **E Wallet** mobile app (a digital pouch for ID, licence, student and bank cards). The whole site lives in one HTML file with inline CSS + vanilla JS and embedded screenshots, so you can drop it on any static host.

## Live preview

Just open `index.html` in a browser, or serve the folder with any static server.

## The app link (one place only)

Every "Download" button reads a single constant at the top of the main script in `index.html`:

```js
const APP_LINK = "[APP_LINK]";   // ← replace with your Play Store / app URL
```

## Swapping screenshots

The four phone screens in the carousel are embedded as data-URIs (search for `SCREENSHOT 1…4` comments in `index.html`). Replace any `<img src="…">` with your own file or URL. Source copies live in `assets/screens/`:

| File | Screen |
| --- | --- |
| `deck.webp` | 3D card deck |
| `open.webp` | Open card with WhatsApp / Save |
| `settings.webp` | Settings sheet |
| `customize.webp` | Pouch customization |

The Open Graph image is `assets/og-cover.jpg`. Use an **absolute URL** for `og:image` when you deploy.

## Deploying

- **GitHub Pages:** Settings → Pages → deploy from the branch root.
- **Netlify / Vercel / Cloudflare Pages:** drag the folder or connect the repo; no build step needed.
- Or copy `index.html` to any web server.

## Features

- Sticky blur navbar, hero with animated 3D card-deck phone mockup (pure CSS/SVG)
- Features grid, screenshots carousel, backup & privacy, how-it-works, final CTA, footer
- Scroll-reveal animations with `prefers-reduced-motion` support
- Accessible: semantic HTML, aria labels, keyboard nav, skip link
- SEO: title, meta description, Open Graph, Twitter cards, JSON-LD
- Font stack led by SF Compact with graceful fallbacks
- No frameworks, no build step, ~190 KB total

## License

All rights reserved.
