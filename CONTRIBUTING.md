# Contributing

Contributions are welcome — bug fixes, new patterns, and expanded platform coverage all improve the skill for everyone.

## What Belongs in This Skill

This skill covers **Astro static site generation (SSG)**. Contributions should stay within that scope:

- Astro SSG patterns, configuration, and best practices
- Content Collections (Astro 4.x and 5.0+ Content Layer API)
- Markdown/MDX authoring patterns
- Deployment to supported platforms (Netlify, Vercel, Cloudflare Pages, GitHub Pages, Firebase, AWS, GCS)
- Testing and quality tooling for Astro projects

Out of scope: Astro SSR-only patterns, non-Astro frameworks, general web development topics.

## File Structure

```
publishing-astro-websites/
├── SKILL.md                    # Main skill — keep lean and scannable
└── references/
    ├── deployment-platforms.md # Platform-specific depth
    └── markdown-deep-dive.md   # Advanced Markdown/MDX patterns
```

**SKILL.md** is the first file Claude reads. Keep it concise — essential patterns only, with one-line comments instead of paragraph explanations. Move verbose conceptual material to a reference file.

**Reference files** can be more thorough. Each exceeds 350 lines and includes a TOC — maintain the TOC when adding sections.

## Code Examples

- Trim to the essential pattern — aim for the minimum lines that demonstrate the concept
- Use one-line `// comments` instead of inline prose explanations
- Prefer imperative voice throughout (`run`, `configure`, `set`) — avoid `you can`, `you should`
- No subjective labels (`Recommended`, `Easiest`) — use objective technical criteria in parentheses instead

## How to Contribute

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-topic`
3. Make changes following the style guide above
4. Open a pull request with a clear description of what was added or fixed and why

## Reporting Issues

Open a GitHub issue with:
- The trigger phrase or context where the skill gave incorrect or incomplete guidance
- What you expected vs what you got
- The Astro version you were targeting (4.x or 5.0+)

## Versioning

This project follows [Semantic Versioning](https://semver.org/):

- **Patch** (1.1.x) — corrections, typo fixes, small clarifications
- **Minor** (1.x.0) — new sections, new platform coverage, significant content additions
- **Major** (x.0.0) — breaking restructure of skill layout or scope change

Update `SKILL.md` frontmatter `version` and `marketplace.json` `metadata.version` together, and add an entry to `CHANGELOG.md`.
