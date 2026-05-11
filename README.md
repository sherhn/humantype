# HumanType

**Strip AI typography. Write like a human.**

HumanType detects and replaces the typographic symbols that AI language models habitually produce – em dashes, curly quotes, ellipses, non-breaking spaces, and more – substituting plain ASCII equivalents that read as naturally human-written text.

🌐 **Live site:** https://humantype.sherhn.space/

---

## What it does

AI-generated text is littered with typographic "tells": the em dash (—), curly quotes (""), the Unicode ellipsis (…), non-breaking spaces, legal symbols (® ™ ©), and typographic arrows (→ ⇒). AI detection tools look for exactly these patterns. HumanType replaces them all in one click.

## Features

- **19 replacement rules** across 7 categories: dashes, ellipsis, quotes, special spaces, fractions, legal symbols, arrows
- **Selective rules** — enable or disable any individual rule or entire category
- **Live symbol counter** — shows how many replaceable symbols are in your input before you click Replace
- **Detailed stats** — see exactly which symbols were replaced and how many
- **One-click copy** — copy the cleaned result straight to your clipboard
- **Keyboard shortcut** — `Ctrl+Enter` / `Cmd+Enter` to replace instantly
- **No server, no data sent** — everything runs locally in your browser

## File structure

```
index.html       # Main application (single self-contained file)
robots.txt       # Search engine crawler rules
sitemap.xml      # XML sitemap for SEO
humantype-logo.svg  # Standalone SVG logo
README.md        # This file
```

## Deployment

Upload all files to your web server root. The app is fully static — no backend required.

```bash
# Example: deploy via rsync
rsync -av index.html robots.txt sitemap.xml humantype-logo.svg user@yourserver:/var/www/humantype/
```

## SEO

- Full `<meta>` tags: description, keywords, author, robots, canonical URL
- Open Graph tags for social sharing
- Twitter Card metadata
- JSON-LD structured data (`WebApplication` schema)
- Inline SVG favicon (no external file dependency)
- `robots.txt` allowing all crawlers
- `sitemap.xml` pointing to the canonical URL

## License

MIT — free to use, modify, and deploy.
