# Responsive changes

- Navbar: right-hand controls no longer push the page wider than the screen on phones; brand text wraps instead of overflowing; avatar has an offline fallback.
- Demand Forecast: chart legend wraps on narrow screens.
- Full-height layouts use `dvh` instead of `vh`/`screen`, so mobile browser toolbars don't cut content off.
- package.json: esbuild bumped to ^0.27.0 to fix the `npm install` peer-dependency error with Vite 8.

Checked at 360px (phone), 768px (tablet) and 1280px (laptop) across all 17 screens: no horizontal overflow; `tsc` and `vite build` pass.

Run: `npm install`, then `npm run dev`. Build for hosting: `npm run build` (output in `dist/`).
