# CometChat Marketing Page Build

## Live Links
- **GitHub Repository**: [Your Repo Link Here]
- **Live Hosted Link**: [Your Vercel/Netlify Link Here]

## Implementation Notes

### SEO Assumptions
* **Target Audience Focus**: Assumed the target audience consists of Developers, Product Managers, and CTOs searching for terms like "In-app chat API", "Chat SDK", or "Chat Infrastructure".
* **Meta & Canonical Data**: Implemented explicit `<title>`, `<meta name="description">`, OpenGraph tags, and a unified Canonical URL assuming the target domain is mapped to standard canonical paths.
* **Structured Data**: Included a `SoftwareApplication` JSON-LD schema payload directly on the homepage to inform search engines of exactly what the software product does.
* **Semantic Code structure**: Prioritized structured semantic DOM tags (`<header>`, `<main>`, `<footer>`, `<section>`) and strict heading hierarchy (single `<h1>`) for absolute clarity in search indexing.

### Tradeoffs Made
* **Static Interactions vs Full State**: Because this is a layout and static site exercise, I implemented the "Dashboard Visual" using pure CSS layouts (Glassmorphism + skeletons) rather than building a heavy interactive state component. This creates the "wow" factor with zero JavaScript overhead.
* **Vanilla CSS over Tailwind**: For absolute visual fidelity and extreme control over the gradient/glassmorphism aesthetics, I curated global CSS custom properties mapped strictly to perceived design tokens instead of locking into utility classes.
* **Zero External Dependencies**: Avoided heavy icon libraries or animation libraries (like Framer Motion). Used native CSS keyframes (`@keyframes`) for micro-animations to prioritize a microscopic bundle size and perfect Lighthouse scores.

### Future Production Improvements
* **Advanced Asset Pipeline**: Integrate `vite-imagetools` or a CDN (Cloudinary) for automatic `avif`/`webp` multi-resolution `srcset` generation.
* **Internationalization (i18n)**: Prepare the static site generator to emit multi-locale paths (e.g., `/en/`, `/es/`) mapped to `hreflang` tags.
* **Strict A11y Verification**: Enhance keyboard routing, Focus-Visible rings, and ARIA live regions for complex components. 

## Local Development

```bash
npm install
npm run dev -- --open
```

Built with **SvelteKit** + **Adapter Static** + **Vanilla CSS**.
