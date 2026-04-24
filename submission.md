# CometChat Marketing Website - Submission Notes

## SEO Assumptions & Implementation
- **Semantic HTML**: Utilized `<header>`, `<main>`, `<section>`, and `<footer>` tags to ensure screen readers and search engines correctly parse the page structure.
- **Metadata**: Implemented dynamic title tags and meta descriptions within SvelteKit's `<svelte:head>`.
- **Structured Data**: Injected JSON-LD (Schema.org) for `SoftwareApplication` to help search engines understand the product context.
- **Typography**: Integrated the custom 'Satoshi' variable font as the primary display face for high-end readability.

## Technical Tradeoffs
- **Asset Integration**: For the "Integration Options" and "Footer" sections, I prioritized pixel-perfect fidelity by utilizing high-resolution image exports (`Group` and `Content.png`). While this reduces DOM complexity, it requires careful management of `alt` tags for accessibility.
- **Vanilla CSS**: Chose Vanilla CSS over Tailwind to ensure total control over the custom design tokens (gradients, glassmorphism) without fighting framework defaults.
- **Single Page Architecture**: Built as a high-fidelity landing page rather than a multi-page site to focus on the modular engineering of the feature sections.

## Production Improvements
- **Component System**: In a production environment, I would replace the static image exports with a fully-featured component library (like shadcn/svelte) for better internationalization and dynamic content updates.
- **Image Optimization**: Implement automated WebP/AVIF conversion pipelines to reduce LCP (Largest Contentful Paint) times.
- **Testing**: Add Playwright end-to-end tests to verify interactive states (like the hover animations in the Integration section) across all browser engines.
- **Analytics**: Integrate a privacy-focused analytics tool (like Plausible) to track user engagement with the CTA buttons.
