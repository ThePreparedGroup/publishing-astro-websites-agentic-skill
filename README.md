# Publishing Astro Websites - Claude Code Agentic Skill

A comprehensive Claude Code skill for building and deploying static websites with the Astro framework.

## Overview

This skill provides guidance for Astro static site generation (SSG), covering:

- **Content Collections** - Legacy patterns, Content Layer API (Astro 5.0), Custom Loaders
- **Syntax Highlighting** - Shiki configuration, Transformers, Expressive Code (copy buttons, filenames, diff highlighting)
- **Diagram Integration** - Mermaid (client-side, no build dependencies), PlantUML, dark mode theming strategies
- **Client-Side Search** - Pagefind (build-time indexing, scales to 10,000+ pages), Fuse.js for smaller sites
- **Versioned Documentation** - Starlight (purpose-built docs framework, built-in search and i18n), multi-version patterns
- **Internationalization** - i18n routing, fallback logic for missing translations
- **Common Patterns** - Pagination, tag archives, RSS feeds, forms, JSON-LD, dark mode
- **Environment Variables** - PUBLIC_* vs build-time scoping, platform secrets management
- **Performance** - Prefetching, Critical CSS (astro-critters), partial hydration
- **Testing** - Vitest component testing, Playwright E2E, link checking
- **Deployment** - Firebase, Netlify, Vercel, Cloudflare Pages, GitHub Pages, AWS S3+CloudFront, GCS + Cloud CDN

## Installation

Clone this repository into your Claude Code skills directory:

```bash
cd ~/.claude/skills
git clone https://github.com/ThePreparedGroup/publishing-astro-websites-agentic-skill.git
```

Or add as a Git submodule to your existing skills:

```bash
git submodule add https://github.com/ThePreparedGroup/publishing-astro-websites-agentic-skill.git
```

## Usage

Once installed, Claude Code will automatically use this skill when you ask about:

- "Create an Astro site"
- "Deploy Astro to Firebase"
- "Set up content collections"
- "Add Mermaid diagrams to Astro"
- "Configure Astro i18n"
- "Build a static blog"
- "Astro markdown setup"

## Structure

```
publishing-astro-websites-agentic-skill/
├── .claude-plugin/
│   └── marketplace.json
├── publishing-astro-websites/
│   ├── SKILL.md                          # Main skill (quick start, all core topics)
│   └── references/
│       ├── deployment-platforms.md       # Step-by-step platform deployment guides
│       └── markdown-deep-dive.md         # Advanced Markdown/MDX patterns
├── .gitignore
└── README.md
```

## What's Covered

### SKILL.md

The main skill file covers the full Astro SSG workflow:

| Section | Topics |
|---------|--------|
| Quick Start | Project init, dev/build/preview, `astro check` |
| When Not to Use | SSG boundaries — real-time, auth, SPAs, WebSockets |
| Project Structure | File layout, routing conventions |
| SSG / SSR / Hybrid | Mode comparison and trade-offs |
| Content Collections | Legacy (4.x), Content Layer API (5.0+), custom loaders |
| Syntax Highlighting | Shiki themes, transformers, Expressive Code |
| Diagram Integration | Mermaid, PlantUML, dark mode strategies |
| Client-Side Search | Pagefind controls/weighting, Fuse.js |
| Versioned Docs | Starlight setup, multi-version sidebar |
| Internationalization | Routing, locale fallbacks |
| Common Patterns | Pagination, tags, RSS, forms, JSON-LD, dark mode toggle |
| Environment Variables | PUBLIC_* scoping, build-time secrets, platform config |
| Performance | Partial hydration, image optimization, prefetching, critical CSS |
| Deployment | Per-platform numbered steps with verification commands |
| Pre-Deploy Checklist | Build, SEO, 404, trailing slashes, Lighthouse |
| Testing & Quality | Vitest, Playwright, ESLint, linkinator |
| .astro File Anatomy | Frontmatter, template, scoped styles, client scripts |
| File-Based Routing | Route table, dynamic routes, catch-all |
| SEO Essentials | Meta tags, Open Graph, Twitter Cards, canonical URLs |
| Essential Integrations | React, Tailwind, MDX, sitemap, RSS |

### Reference Files

- **[deployment-platforms.md](publishing-astro-websites/references/deployment-platforms.md)** — Full setup guides for Netlify, Vercel, Cloudflare Pages, GitHub Pages, Firebase Hosting, AWS S3+CloudFront, and GCS+Cloud CDN. Includes `netlify.toml`, `vercel.json`, GitHub Actions workflows, firebase.json, and common issue troubleshooting.

- **[markdown-deep-dive.md](publishing-astro-websites/references/markdown-deep-dive.md)** — Advanced schema patterns, collection filtering, MDX component mapping, remark/rehype plugins, reading time, TOC generation, image optimization, and Markdown troubleshooting.

## Requirements

- Claude Code CLI
- Node.js 18+ (for Astro projects)

## License

MIT
