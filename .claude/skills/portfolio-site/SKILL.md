---
name: portfolio-site
description: Plan and build a one-page personal portfolio website from a brand kit — hero, work showcase, about, and contact — written in the brand voice and ready to deploy. Use when building or rebuilding a portfolio site like kovision.com.
---

# Skill: portfolio-site

The recipe the web-builder agent (or Sam) follows to build a one-page portfolio. Work top to bottom. Keep it slop-free and brand-driven.

## Inputs to gather first
- The brand kit (`05_Clients/Ko Vision/Brand_Kit.md`) — colors, fonts, voice. If missing, stop and run the branding agent.
- 3–6 pieces of work to showcase (images, links, or short case notes). If Sam has none yet, the site launches with placeholders and his own socials become piece #1.
- One headshot and one sentence about who he helps.
- Contact: email and the one button you want visitors to click (e.g. "See my work" or "Work with me").

If an input is missing, ask Sam one sharp question rather than guessing.

## Decide the stack (one choice, then move on)
- **Recommended v1:** single static `index.html` + `style.css` in the repo, deployed free on GitHub Pages.
- **Alternative:** no-code (Framer / Webflow) if Sam wants visual drag-and-drop.
Pick one. Don't reopen it.

## Build the page, section by section (show each before the next)
1. **Hero** — name, one-line elevator ("Ko Vision is Samuel Ko's creative portfolio…"), headshot, primary button.
2. **Work** — a clean grid of the showcase pieces. The work is the loudest thing on the page.
3. **About** — 2–3 sentences, first person, in the brand voice. Who he helps and why.
4. **Contact** — email + button. One clear action, no clutter.
5. **Polish** — mobile layout, fast load, favicon, page title/meta.

## Output & gate
Build it in the repo. Show Sam the result. The site is a draft until he approves it (human gate). On approval, deploy (GitHub Pages) and point kovision.com at it. End with Sam's next minimum viable floor.
