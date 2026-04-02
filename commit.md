Commit 1.0.0: feat(1.0.2): add initial landing page structure and assets


Commit 1.1.0: feat(): optimize core web vitals and revamp UI animations

- Resolved render-blocking fonts and duplicate CSS (-750ms FCP).
- Fixed LCP broken srcsets and resized heavy images.
- Replaced CPU-bound animations with GPU-safe transforms (CLS to ~0).
- Handled mobile tap delays & increased accessibility (WCAG AA).
- Added flowing dynamics & floating illustrations to Bento Grid S4.
- Implemented infinite marquee scroll for Trust Signals.
- Fixed i18n routing bug on Navbar Logo.

Commit 1.1.1: feat(performance): improve Core Web Vitals and asset delivery strategy
Addresses PageSpeed Insights audit findings on staging.parkin.my.id:

Image optimization:
- Add responsive variants (800w, 1200w) for Hero LCP image (Macbook-Air.webp)
- Add 500w variant for iPhone-14 feature mockup
- Update srcset/sizes on all affected <img> elements to serve correct sizes
- Fix Layout.astro preload link to reference existing 800w variant

Caching strategy:
- Add long-term Cache-Control headers for /images/* and /_astro/* routes
- Restructure vercel.json headers array to comply with schema validation

Anticipated improvements: ~700ms render-blocking savings (FCP/LCP),
~63 KB reduction in image transfer size, improved repeat visit performance.