---
tags: [meta, stack, tools]
status: living
updated: 2026-06-30
---

# SamKo OS — Stack & Tools

The registry of tools in (or evaluated for) the stack: what each is for, install status, how to finish setup, and how to use it. Keep this current when tools are added.

## Core (live)
Claude Code (brain) · Chloe + agents (branding, web-builder, design, social-media) + skills · Notion (Mission Control + Progress Log) · GitHub (private OS repo + public `thekovision` site) · Canva · Gmail · Google Calendar · Apify (free tier — limited runs).

---

## Scraping & research

### Firecrawl — general web → markdown/JSON  ·  ADDED (needs key)
For research and scraping normal websites (client sites, competitor sites, articles). Added as an MCP in `.mcp.json` (runs via `npx -y firecrawl-mcp`).
- **Finish setup (you):** sign up free at **firecrawl.dev**, copy your API key, paste it into `.mcp.json` in place of `PASTE_YOUR_FIRECRAWL_API_KEY_HERE`, then restart the session. (`.mcp.json` is git-ignored so your key never gets committed.)
- **Use for:** "research X," "scrape this website," pulling a client's/competitor's site copy for a brand audit.
- **Not for:** Instagram (auth-walled, anti-bot).

### Scrapling — Python stealth scraper (backup to Firecrawl)  ·  DEFERRED
The heavy-duty backup for anti-bot / Cloudflare-protected sites Firecrawl can't crack.
- **Blocked by:** your system Python is 3.9; Scrapling needs 3.10+. Also needs Homebrew.
- **Install when needed:** `brew install python@3.12` → `pip3.12 install "scrapling[fetchers]"` → `scrapling install`. Only worth it once a real scrape actually needs it.

### Instagram brand analysis — the plan
Apify's free tier is limited, and Firecrawl/Scrapling are weak on Instagram (auth wall). Cheapest reliable path: **Apify free runs, used sparingly**, plus manual review. Never automate your *own* logged-in IG to bulk-scrape — account-ban risk. A `social-audit` skill will wrap whichever source we settle on (SOP step 2).

---

## Web design & build

### Impeccable — anti-generic design guidance  ·  INSTALL (plugin)
Keeps AI-built sites and HTML decks from looking like every other SaaS template; also for HTML presentations you export to PDF.
- **Install (you):** in Claude Code, run `/plugin marketplace add pbakaus/impeccable`, then `/plugin install impeccable`, then `/impeccable init` once per project.
- **Use for:** thekovision.com, client sites, and HTML decks → PDF.

### Ponytail — leaner code from agents  ·  INSTALL (plugin)
Makes AI agents write less/simpler code — useful when you start building sites and micro-apps.
- **Install (you):** `/plugin marketplace add DietrichGebert/ponytail`, then `/plugin install ponytail`.

---

## Video / motion

### Remotion — programmatic video & motion-graphic overlays  ·  ON DEMAND
React framework for making videos/overlays from code — great for social motion graphics.
- **Start a project when needed:** `npx create-video@latest` (Node is installed).
- **⚠️ License:** free for individuals and small teams, but a **paid company license** is required for commercial/agency use above the free threshold. Sort the license before shipping any client video.

---

## Documents / agency polish
Use the built-in skills already available: `pdf`, `docx`, `pptx`, `artifact-design`. **Plan:** a branded Ko Vision document template (warm greige, gold, Inter + Cormorant) that all proposals, brand audits, and decks pour into, so every deliverable looks agency-grade and consistent. Impeccable covers the HTML-deck-to-PDF route.

---

## Fun
### spank  ·  INSTALLED
macOS novelty — plays audio when the laptop's accelerometer feels a smack. Binary at `~/.local/bin/spank`.
- **Run:** `sudo spank --sexy` (needs sudo for accelerometer access).
