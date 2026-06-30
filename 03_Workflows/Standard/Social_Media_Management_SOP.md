---
tags: [workflow, sop, social-media, core]
status: draft
created: 2026-06-30
owner: Sam
---

# Social Media Management SOP

The end-to-end process for taking a client from onboarding to published content and ongoing account management. This is Sam's first deliverable — the goal is to run and debug it without Jon.

---

## Zone 1 — Setup (once per client)

### Step 1: Onboard Client + Build Profile

**What this is:** You're collecting everything you need to do good work for this client — who they are, what they sell, who their audience is, what platforms they're on, and what they've tried before. Without this, every decision downstream is a guess.

**How to do it by hand:**

1. Schedule a 30-minute intake call or send an async questionnaire (use the client profile template at `88_Templates/Client_Profile_Template.md`).
2. Collect these essentials:
   - Business name, industry, location, website
   - Point of contact name + email + phone
   - Current social media handles (Instagram, TikTok, Facebook, LinkedIn)
   - Target audience (who buys from them, age range, location, interests)
   - Brand assets they already have (logo files, brand colors, fonts, existing style guide)
   - Competitors they respect or want to differentiate from (2–3 names)
   - What they've tried before and what worked / didn't
   - Their goal: more followers, more sales, more foot traffic, brand awareness?
   - Budget and timeline expectations
3. Create a client folder at `05_Clients/Active/[Client_Name]/` with their profile saved as `profile.md`.
4. Save any brand assets (logos, photos) they send into `05_Clients/Active/[Client_Name]/assets/`.

**Output:** A completed client profile in their folder. This is the single source of truth for everything that follows.

**Agent/tool:** None yet — this is manual. *Future: a client-onboarding agent could pre-fill the profile from a website URL and social handles.*

---

### Step 2: Audit Brand + Social Presence → Score + Strategy

**What this is:** You're looking at what the client already has — their branding, their social media accounts, their content — and grading it honestly. Then you write a short strategy doc that says "here's where you are, here's where you should be, here's how we get there." This is the work that makes the client trust you before you've posted anything.

**How to do it by hand:**

1. **Brand audit** — Open their website and socials. Score these on a 1–5 scale:
   - Visual consistency (do their posts, website, and logo feel like the same brand?)
   - Bio/profile completeness (do they have a clear bio, profile pic, link in bio, highlights?)
   - Content quality (are the photos/videos professional or phone-snapped and blurry?)
   - Posting frequency (how often do they post? When was the last one?)
   - Engagement (likes, comments, shares relative to their follower count)
   - Hashtag / SEO usage (are they using relevant hashtags or keywords?)

2. **Competitor scan** — Look at the 2–3 competitors from their profile. Note what they do well that the client doesn't. Don't copy — identify the gap.

3. **Write the strategy brief** — A short document (1–2 pages) saved to `05_Clients/Active/[Client_Name]/strategy.md` containing:
   - Scorecard (the 1–5 scores above with one-line explanations)
   - Top 3 problems to fix (ranked by impact)
   - Recommended platforms to focus on (don't spread thin — usually 2 max to start)
   - Content pillars: 3–4 recurring content themes (e.g., behind-the-scenes, product showcase, tips/education, social proof/testimonials)
   - Posting cadence: how many posts per week, which days, what format (reel, carousel, static, story)
   - Quick wins: 2–3 things you can fix immediately (update bio, better profile photo, consistent highlight covers)

**Output:** `strategy.md` in the client folder, ready to present.

**Agent/tool:** The **branding agent** can help build or audit a brand kit if the client needs one. *Future: a social-media-audit agent could pull follower counts, engagement rates, and posting frequency automatically.*

---

### Step 3: [HUMAN GATE] Present Strategy → Client Approves

**What this is:** You don't start producing content until the client has seen your plan and said yes. This protects you (no wasted work) and builds trust (they feel heard). This is a hard gate — nothing moves forward without a thumbs up.

**How to do it by hand:**

1. Package the strategy brief into a clean, presentable format. For now, the markdown doc is fine for a walkthrough call; later, a one-page PDF or slide deck.
2. Walk the client through it on a call (15–20 min) or send it async with a Loom video explaining each section.
3. Ask for explicit approval: "Does this direction work for you? Anything you want to change before we start producing?"
4. Log their response and any changes in `05_Clients/Active/[Client_Name]/strategy.md` under a "Client Feedback" section with the date.
5. If they want changes, revise and re-present. If they approve, update the strategy status to `approved` and move to Zone 2.

**Output:** An approved strategy. You now have permission to create content.

**Agent/tool:** None — this is a human conversation.

---

## Zone 2 — Production (repeats every content cycle)

### Step 4: Run the Content Studio

**What this is:** This is Jon's system. It takes the approved strategy (content pillars, posting cadence, brand guidelines) and generates a batch of content — captions, image concepts, hashtag sets, and draft visuals. Jon's target is ~70% automated with zero AI slop, meaning the output is a strong starting point that still needs a human eye. You feed in the strategy; it outputs a content folder.

**How to do it by hand (until the studio is wired up):**

1. Open the client's strategy. Pull out: content pillars, posting cadence, brand voice, target audience.
2. Plan the content batch: decide how many posts for this cycle (e.g., 8 posts for 2 weeks at 4/week).
3. For each post, draft:
   - **Caption:** Write it in the client's brand voice. Hook in the first line. CTA at the end. Keep it concise.
   - **Visual concept:** Describe what the image or video should be (e.g., "flat lay of menu items on branded background" or "owner talking to camera, 15-second reel").
   - **Hashtags:** 15–20 relevant hashtags, mix of broad and niche.
   - **Format:** Static image, carousel, reel, or story.
   - **Scheduled date/time:** Based on the cadence in the strategy.
4. Save the batch as `05_Clients/Active/[Client_Name]/content/cycle_[date]/` with one file per post or a single batch doc.

**Output:** A content folder with draft captions, visual briefs, and a schedule.

**Agent/tool:** *This is where Jon's Antigravity + content studio pipeline goes. Future: a content-studio agent that takes a strategy and outputs a ready-to-review content batch. This is the biggest automation opportunity in the whole SOP.*

---

### Step 5: Sam's Review — Content Folder + Canva Edits + Post Copy

**What this is:** This is your craftsmanship step. You open each piece of content and make it good. You're checking that the copy is sharp (no slop), the visuals match the brand, and the Canva designs are polished. This is the step Jon wants you to own completely — it's where your eye and judgment matter most.

**How to do it by hand:**

1. **Review copy** — Read every caption out loud. Check:
   - Does the first line hook? Would you stop scrolling for it?
   - Is it in the client's voice, not generic AI voice?
   - Is the CTA clear?
   - Grammar, spelling, brand name spelled right?
   - Hashtags relevant and not spammy?

2. **Review/edit visuals in Canva** — Open each design. Check:
   - Colors match the brand palette
   - Fonts are consistent with the brand kit
   - Text is readable (contrast, size, not too much text on image)
   - Images are high quality (not pixelated, well-cropped)
   - Layout is clean and balanced
   - Logo placement is consistent across all posts
   - *For reels/video:* pacing, text timing, audio

3. **Photo edits** — If using real photos (product shots, team photos), edit in Canva or a photo editor:
   - Crop and straighten
   - Adjust brightness/contrast
   - Apply consistent filter or color grade that matches the brand
   - Remove distracting backgrounds if needed

4. Mark each post as reviewed in the batch doc. Flag anything that needs a second opinion for step 6.

**Output:** A polished content batch, ready for approval.

**Agent/tool:** Canva MCP is connected — designs can be edited programmatically. *Future: a design agent that applies brand-kit rules to Canva templates and flags inconsistencies.*

---

### Step 6: [HUMAN GATE] Sam or Jon Approves Content

**What this is:** Final quality check before anything goes live. Either you or Jon looks at the finished batch and gives the green light. Jon's standard: "no AI slop" — if it looks or reads like generic AI output, it doesn't ship.

**How to do it by hand:**

1. Share the content batch — either the folder link or a screen-share walkthrough.
2. Review criteria:
   - Would this embarrass the client if a competitor saw it? (If yes, redo.)
   - Does every post clearly serve one of the content pillars?
   - Is the visual quality at or above what the client currently posts?
   - Is the copy specific to *this* client, not interchangeable with any other business?
3. Approve, request changes, or reject with specific notes.
4. If changes are needed, loop back to step 5. If approved, move to Zone 3.

**Output:** Approved content, ready to publish.

**Agent/tool:** None — this is a human judgment call.

---

## Zone 3 — Delivery (repeats on schedule)

### Step 7: Publish via Metricool or Blotato

**What this is:** You take the approved content and schedule it to go live on the right platforms at the right times. You're using a scheduling tool (Metricool or Blotato — pick one and standardize) so you're not manually posting at 9am every Tuesday.

**How to do it by hand:**

1. Log into the scheduling tool (Metricool or Blotato).
2. Connect the client's social accounts if not already connected.
3. For each post in the approved batch:
   - Upload the final visual (export from Canva as PNG or MP4)
   - Paste the caption
   - Add hashtags (first comment for Instagram if that's the strategy)
   - Set the scheduled date and time
   - Select the target platforms
4. Double-check the preview — make sure nothing is cropped weirdly, caption isn't cut off, video plays correctly.
5. Confirm the schedule.
6. Save a screenshot or export of the schedule to `05_Clients/Active/[Client_Name]/content/cycle_[date]/schedule_confirmation.png`.

**Output:** All posts scheduled and confirmed.

**Agent/tool:** *Future: a publishing agent that pushes approved content to Metricool/Blotato via API. Metricool has an API; Blotato may need browser automation.*

---

### Step 8: Manage Account + Report Results (2 weeks)

**What this is:** Once posts are live, you're not done. You monitor the account — respond to comments and DMs (or flag them for the client), watch for anything going wrong, and after two weeks pull a performance report. The report is what proves your value and drives the conversation in step 9.

**How to do it by hand:**

1. **Daily (5 min):** Check the client's social accounts for:
   - New comments that need a reply (respond in brand voice, or flag to client if it needs their personal input)
   - DMs that need attention
   - Any post that failed to publish or looks broken

2. **At 2 weeks, pull a report** covering:
   - Posts published vs. planned
   - Reach and impressions per post
   - Engagement rate (likes + comments + shares / reach)
   - Follower growth (net new followers)
   - Top-performing post and why you think it worked
   - Worst-performing post and what to learn from it
   - Any notable comments or DMs
3. Save the report as `05_Clients/Active/[Client_Name]/reports/report_[date].md`.

**Output:** A 2-week performance report in the client folder.

**Agent/tool:** *Future: a reporting agent that pulls metrics from platform APIs or Metricool and generates the report automatically.*

---

### Step 9: Decide — Continue / Pivot / Add Layers

**What this is:** You sit down (with the client, or internally first) and look at the data. What worked? What didn't? Do you keep the current strategy, adjust it, or add something new (paid ads, new platform, influencer collabs)? This is where you start the next cycle and the SOP loops back to step 4 (or step 2 if the strategy needs a bigger overhaul).

**How to do it by hand:**

1. Review the report from step 8.
2. Identify: what content pillar performed best? What format got the most engagement? What flopped?
3. Decide:
   - **Continue:** Strategy is working. Keep the same pillars and cadence. Loop back to step 4 for the next content batch.
   - **Pivot:** Something isn't landing. Adjust 1–2 content pillars, try a different posting time, or shift platform focus. Update `strategy.md` and loop back to step 4.
   - **Add layers:** Ready to scale. Consider: paid promotion of top posts, adding a new platform, starting a newsletter, influencer partnerships. This may need a new strategy conversation (loop back to step 2–3).
4. Log the decision in `05_Clients/Active/[Client_Name]/reports/report_[date].md` under a "Next Cycle" section.

**Output:** A clear decision and an updated plan for the next cycle.

**Agent/tool:** None — this is strategic judgment. Chloe can help analyze the data and suggest pivots.

---

## What We Still Need to Build

These are flagged for the infrastructure chat. Build them one at a time as Sam masters each manual step.

| Priority | What | Type | Why |
|----------|------|------|-----|
| 1 | **Design agent** | Agent + Skill | Canva edits, brand-kit enforcement, template application. Unblocks step 5. |
| 2 | **Content studio agent** | Agent + Skill | Takes strategy → outputs content batch (captions, visual briefs, hashtags). Unblocks step 4. |
| 3 | **Social media audit agent** | Agent + Skill | Pulls metrics, scores presence, drafts strategy. Speeds up step 2. |
| 4 | **Publishing agent** | Agent + Skill | Pushes approved content to Metricool/Blotato. Automates step 7. |
| 5 | **Reporting agent** | Agent + Skill | Pulls platform metrics, generates 2-week report. Automates step 8. |
| 6 | **Client onboarding agent** | Agent + Skill | Pre-fills client profile from URL + social handles. Speeds up step 1. |

---

## How to Run This SOP

**New client:** Start at step 1, go through every step in order.
**Existing client, new content cycle:** Start at step 4, go through step 9.
**After a pivot:** Start at step 2 if the strategy changed significantly, otherwise step 4.

To run a step: open this document, go to that step, follow the "How to do it by hand" section. When an agent exists for that step, Chloe will tell you to delegate to it instead.
