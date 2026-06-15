# Changelog

All notable changes to this skill are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Versions follow [Semantic Versioning](https://semver.org/).

---

## [1.2.0] - 2026-06-15

### Added
- **Cloudflare Pages — C3 CLI setup** — `npm create cloudflare@latest` as the primary scaffold-and-deploy path
- **`@astrojs/cloudflare` adapter** — documented SSG (no adapter) vs SSR/hybrid (adapter required), `platformProxy` for local binding emulation
- **Pages Functions and Bindings** — KV, D1, R2, Durable Objects access via `Astro.locals.runtime.env`, `wrangler.toml` binding config, `env.d.ts` typing
- **Local dev with `wrangler pages dev`** — test bindings locally with `--kv`, `--d1` flags
- **Preview deployment details** — branch alias URLs, auto `X-Robots-Tag: noindex`, Cloudflare Access protection, delete command
- **Cloudflare build notes** — exit code behavior, monorepo root directory config
- **CF_ system environment variables** — `CF_PAGES`, `CF_PAGES_BRANCH`, `CF_PAGES_COMMIT_SHA`, `CF_PAGES_URL`, `CI` — added to both SKILL.md env vars table and deployment-platforms.md
- **SSG vs SSR mode table** — Cloudflare-specific comparison in deployment-platforms.md

### Changed
- Cloudflare Pages deploy steps in SKILL.md expanded with C3 CLI option, PR preview URL detail, and pointer to reference file for bindings
- `deployment-platforms.md` TOC entry for Cloudflare Pages updated to list new subsections
- Version bumped to 1.2.0 in SKILL.md frontmatter and marketplace.json

---

## [1.1.0] - 2026-06-14

### Added
- **Environment Variables section** — covers `PUBLIC_*` vs build-time scoping, reference table, and platform secrets management
- **`npx astro check`** added to Quick Start command block for type-checking and Content Collection schema validation
- **WebSockets / Server-Sent Events** added to `When Not to Use` — common SSG trap for developers expecting persistent connections
- **Table of Contents in both reference files** — `deployment-platforms.md` and `markdown-deep-dive.md` now have anchor-linked TOCs
- **Back-links in reference files** — both reference files link back to `SKILL.md` for two-way navigation
- **Per-platform deployment steps** — Netlify, Vercel, Cloudflare Pages, GitHub Pages, and Firebase now have numbered steps with verification commands
- **Missing TOC entries in SKILL.md** — `.astro File Anatomy`, `File-Based Routing`, `SEO Essentials`, `Essential Integrations`, and `Environment Variables` sections now appear in the main TOC
- **New triggers** — `astro netlify`, `astro vercel`, `astro cloudflare`, `astro github pages`, `astro search`, `astro pagefind`, `astro environment variables`, `astro i18n`

### Changed
- **Promotional labels removed** — `Recommended` and `Easiest` replaced with objective technical criteria throughout (Expressive Code, Mermaid, Pagefind, Starlight, Formspree)
- **Fuse.js example trimmed** — reduced from ~40 lines to ~22 lines by removing verbose inline commentary
- **References section** — upgraded from bare filenames to descriptive markdown links with content summaries
- **GCS vs Firebase comparison table** — `Recommendation` column header renamed to `Better Choice`; row labels reworded to objective criteria
- **`marketplace.json`** — owner updated to The Prepared Group; plugin description expanded to cover new topics and platforms
- **SKILL.md frontmatter** — `author` updated to The Prepared Group; version bumped to 1.1.0
- **README** — install URLs corrected; feature list updated; `What's Covered` section added with full SKILL.md section table and reference file descriptions

---

## [1.0.0] - Initial Release

- Initial skill covering Astro SSG fundamentals, Content Collections, Markdown/MDX, syntax highlighting, diagrams, client-side search, Starlight, i18n, common patterns, performance, and deployment
