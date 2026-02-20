# XcogniVis — Next.js Web Application

**Founded by Wilfred Aquila | xcognivis.com**

A production-ready, SEO-optimised Next.js 14 website built with TypeScript, Tailwind CSS, and custom CSS.

---

## Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS + Custom CSS Variables
- **Fonts**: Google Fonts (Orbitron, Rajdhani)
- **SEO**: Full metadata API, JSON-LD structured data, Open Graph, Twitter Cards, robots.txt, web manifest

---

## Project Structure

```
xcognivis/
├── app/
│   ├── layout.tsx          ← Root layout + ALL SEO metadata
│   ├── page.tsx            ← Home page (assembles all sections)
│   ├── globals.css         ← CSS variables + Tailwind + custom styles
│   ├── hooks/
│   │   └── useScrollReveal.ts   ← Scroll animation hook
│   └── components/
│       ├── Nav.tsx         ← Fixed nav with mobile menu
│       ├── Hero.tsx        ← Landing / Hero section
│       ├── About.tsx       ← About Us section
│       ├── Services.tsx    ← Services section
│       ├── Shared.tsx      ← CTABanner + Footer
│       └── RevealProvider.tsx  ← Client wrapper for scroll reveal
├── public/
│   ├── robots.txt          ← Search engine crawl rules
│   └── site.webmanifest    ← PWA manifest
├── package.json
├── tsconfig.json
├── tailwind.config.ts
├── next.config.ts
└── postcss.config.js
```

---

## Quick Start

### 1. Install dependencies
```bash
npm install
```

### 2. Run development server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000)

### 3. Build for production
```bash
npm run build
npm start
```

---

## Deploy to Vercel (Free — Recommended)

1. Push this project to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Click **Deploy** — done!

Vercel auto-detects Next.js and handles everything.

---

## SEO Checklist — Before Go Live

- [ ] Replace `https://xcognivis.com` in `layout.tsx` with your actual domain
- [ ] Add `public/og-image.png` (1200×630px) — used for social media previews
- [ ] Add `public/favicon.ico`, `favicon-16x16.png`, `apple-touch-icon.png`
- [ ] Update email in `Shared.tsx` CTABanner
- [ ] Add your social media handles in `layout.tsx` Twitter metadata
- [ ] Add your social media URLs in `layout.tsx` JSON-LD `sameAs`
- [ ] Submit sitemap to Google Search Console after launch

---

## Brand Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Blue | `#1e7de0` | X logo letter, primary CTA |
| Purple Light | `#b44de8` | "Vis" logo text, accents |
| Cyan | `#00d4ff` | Circuit lines, highlights |
| Black | `#040810` | Background |
| Dark | `#080f1c` | Services section |

---

## Agile Sprint Roadmap (Next Steps)

- **Sprint 2**: Add Contact Us page with form (EmailJS — no backend needed)
- **Sprint 3**: Add Portfolio / Projects section
- **Sprint 4**: Add Blog powered by MDX
- **Sprint 5**: Add Careers page
- **Sprint 6**: Client portal / dashboard (requires backend)
