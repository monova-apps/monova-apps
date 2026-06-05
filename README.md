# Monova Apps — Website

Minimal site for **Monova Apps**, the independent mobile app studio affiliated with [Monova Tech](https://monovatech.com). Monova designs, builds, and ships apps to the **App Store** and **Google Play**.

Static — plain HTML, CSS, and vanilla JS. No build step, no dependencies. Deploy to any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages, S3…).

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Landing page — a single hero section |
| `contact.html` | Contact page — just the email |
| `styles.css` | All styling (design tokens are CSS variables at the top) |
| `script.js` | Sticky nav, scroll reveals |
| `favicon.svg` | Brand mark |

## Run locally

```bash
python3 -m http.server 8000   # or: npx serve .
```

Then open http://localhost:8000.

## Design

- **Theme:** deep-ink (near-black) canvas, luminous acid-lime accent, violet/teal ambient aurora glows.
- **Type:** Clash Display (display) + General Sans (body), from Fontshare.
- **Motion:** floating CSS phone mockup, staggered/scroll-triggered reveals — all respect `prefers-reduced-motion`.

## Customizing

- **Brand colors / spacing:** edit the CSS variables in `:root` at the top of `styles.css` (`--lime`, `--ink`, `--violet`, `--teal`…).
- **Store links:** the hero "App Store" / "Google Play" buttons (`.store`) currently link to `#`. Swap in your real store URLs.
- **Contact / emails:** replace `hello@monovatech.com` and `support@monovatech.com` throughout (`contact.html`, footer links).
- **Hero metrics:** the "4.8 avg rating / 4M+ downloads / 12 apps" line in `index.html` is placeholder copy — update it.
