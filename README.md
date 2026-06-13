# RuSource.org — Complete Static Mirror

A 1:1 identical static copy of [rusource.org](https://rusource.org) — 749+ Curated Resources to Learn Russian.

## What's Included

- **56 HTML pages** — all content fully server-side rendered
- **1 CSS stylesheet** — all styling, animations, and responsive design
- **26 JS bundles** — available but not required (content works without JS)
- **Zero broken internal links** — all 1,968 links verified
- **14 CSS animations** — marquee, float, spin, aurora, fade effects all preserved
- **8.3 MB total** — lightweight enough for any free hosting

## Pages

| Section | Count | Examples |
|---------|-------|---------|
| Homepage | 1 | `index.html` |
| Main pages | 9 | `about.html`, `browse.html`, `faq.html`, `roadmap.html` |
| Category pages | 32 | `category/grammar.html`, `category/podcasts-and-audio.html` |
| Learn pages | 6 | `learn/apps.html`, `learn/free.html`, `learn/grammar.html` |
| CEFR level pages | 6 | `levels/A1.html` through `levels/C2.html` |
| Error fallback | 1 | `404.html` |

## Features Preserved

✅ All 749+ Russian learning resources with descriptions
✅ 32 category pages with resource cards
✅ CEFR level filtering (A1-C2)  
✅ Dark/light theme toggle (via vanilla JS)
✅ Search/filter functionality (via vanilla JS)
✅ Favorites system (localStorage, via vanilla JS)
✅ CSS animations (floating elements, marquee, transitions)
✅ Responsive design (mobile, tablet, desktop)
✅ All internal navigation links
✅ All external resource links (YouTube, GitHub, etc.)

## Deploy to Free Static Hosting

### Netlify (Recommended)
1. Push this folder to a GitHub repo
2. Go to [netlify.com](https://netlify.com) → "Add new site" → "Import from Git"
3. Set **publish directory** to the root (`/`)
4. Deploy! The `_redirects` file handles clean URLs automatically.

### Vercel
1. Push to GitHub
2. Import in [vercel.com](https://vercel.com)
3. The `vercel.json` handles URL rewrites
4. Deploy!

### GitHub Pages
1. Push to a GitHub repo
2. Go to Settings → Pages → Enable
3. Set source to main branch / root
4. The `404.html` provides SPA fallback for clean URLs

### Cloudflare Pages
1. Push to GitHub
2. Connect in [Cloudflare Pages](https://pages.cloudflare.com)
3. Deploy!

### Any Other Static Host
Just upload all files to the root directory. Every page works as a standalone `.html` file.

## File Structure

```
├── index.html              # Homepage
├── about.html              # About page
├── browse.html             # Browse all 749 resources
├── categories.html         # 32 category overview
├── roadmap.html            # Learning roadmap
├── daily.html              # Resource of the day
├── faq.html                # FAQ
├── favorites.html          # Favorites page
├── glossary.html           # Russian learning glossary
├── credits.html            # Credits
├── maruf.html              # About the creator
├── 404.html                # Error fallback (also SPA router)
├── category/               # 32 category pages
│   ├── grammar.html
│   ├── podcasts-and-audio.html
│   ├── youtube-and-video.html
│   └── ... (29 more)
├── learn/                  # Learning guide pages
│   ├── apps.html
│   ├── free.html
│   ├── grammar.html
│   ├── podcasts.html
│   ├── beginners.html
│   └── online.html
├── levels/                 # CEFR level pages
│   ├── A1.html
│   ├── A2.html
│   ├── B1.html
│   ├── B2.html
│   ├── C1.html
│   └── C2.html
├── assets/                 # Static assets
│   ├── styles-DXh7mJcr.css  # Main stylesheet (93KB)
│   └── *.js                  # JS bundles (not required)
├── _redirects              # Netlify URL redirects
├── netlify.toml            # Netlify config
├── vercel.json             # Vercel config
├── _routes.json            # Cloudflare Pages config
└── README.md               # This file
```

## Technical Notes

- The original site is a React SPA (Remix framework) with server-side rendering
- This mirror preserves the SSR HTML content which contains all 749+ resources
- CSS handles all styling and animations — no JavaScript needed for content display
- Vanilla JS provides theme toggle, search, favorites, share, and random resource functionality
- All internal links are converted from SPA routes (e.g., `/category/grammar`) to static HTML files (e.g., `category/grammar.html`)
- External links to resources (YouTube channels, apps, websites) still point to their original URLs
- React/Remix hydration scripts, TanStack Router, and Cloudflare challenge scripts have been removed
- Null bytes and invalid CSS selectors have been cleaned from all HTML files
- The `_redirects`, `vercel.json`, and `_routes.json` files provide clean URL support on Netlify, Vercel, and Cloudflare Pages respectively

## Size

| Component | Size |
|-----------|------|
| HTML pages | 8.3 MB |
| CSS | 93 KB |
| JS bundles | 1.3 MB (optional) |
| **Total** | **9.3 MB** |
| **Zipped** | **1 MB** |

---

*Original site by [Maruf Sultan](https://github.com/maruf009sultan) • Source: [GitHub](https://github.com/maruf009sultan/awesome-russian-language)*
