# SEO / GEO / AEO Audit Plugin for Claude

Automatically audits any website across three dimensions of modern search visibility:

- **SEO** — Traditional search engine optimization (Google, Bing): title tags, meta descriptions, heading structure, schema markup, internal links, content quality
- **GEO** — Generative Engine Optimization for AI-powered search (Perplexity, ChatGPT Search, Google AI Overviews, Gemini): E-E-A-T signals, entity clarity, factual density, author authority
- **AEO** — Answer Engine Optimization for featured snippets and voice search: FAQ schema, HowTo schema, question-phrased headings, direct answer formatting

---

## How to use

Once installed, just give Claude a URL and ask about search performance:

> "Can you audit burningstickcreative.com for SEO?"
> "Check my site example.com — why isn't it ranking?"
> "Audit this URL for AI search readiness: example.com"
> "Run a full SEO, GEO, and AEO audit on my website"

Claude will ask whether you want a **Quick Audit** (top issues and scores — takes 1-2 minutes) or a **Full Audit** (comprehensive breakdown — takes 3-5 minutes), then crawl the site across multiple pages before delivering a structured report.

---

## How to install (Claude Code)

**Option 1 — from a marketplace (once listed):**
```
claude plugin install seo-geo-aeo
```

**Option 2 — from this directory:**
```
claude --plugin-dir ./seo-geo-aeo-plugin
```

**Option 3 — install to project scope (share with your team):**
```
claude plugin install seo-geo-aeo --scope project
```

---

## Plugin structure

```
seo-geo-aeo-plugin/
├── .claude-plugin/
│   └── plugin.json          ← Plugin manifest
├── skills/
│   └── seo-geo-aeo/
│       └── SKILL.md         ← Audit instructions
└── README.md
```

---

## Version history

**1.0.0** — Initial release
- Quick and Full audit modes
- Multi-page site crawl (up to 15 pages)
- SEO, GEO, and AEO scoring with priority recommendations matrix
