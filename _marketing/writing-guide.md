# Athena blog: writing guide (for the daily article routine)

This folder starts with an underscore, so Jekyll does not publish it. It is the brief that every article follows.

## Who we write for
- Owners, plant heads, production planners (PPC), supervisors and quality heads of machine shops and component manufacturers.
- First markets: India, and developing economies where shop floor records are still kept on paper job cards, registers, Excel and WhatsApp (for example Bangladesh, Sri Lanka, Nepal, Vietnam, Indonesia, the Philippines, Kenya, Nigeria, Egypt and similar).
- They are practical, busy and sceptical of software hype. Many read English as a second language.

## Voice
- Simple, clear English. Short sentences. One idea per paragraph.
- Indian and British spelling (digitise, organise, colour).
- Practical first: steps, checklists, examples a supervisor could use tomorrow.
- Respectful of paper systems: they worked; the plant has outgrown them.
- No hype words: revolutionary, game-changing, cutting-edge, seamless, Industry 4.0 buzz, "unlock", "leverage".
- No em dashes. Use commas, colons or full stops.

## Structure (900 to 1,300 words)
1. Title with the main search phrase, under 65 characters.
2. Opening (2 or 3 short paragraphs): the real shop floor problem, in plain words.
3. Body with H2 headings: the why, then the how (numbered steps or a checklist).
4. One worked example with sample data. Label it clearly as an example ("For example, a job card for 60 pinion shafts..."). Never present it as a real customer.
5. A short "Where Athena fits" paragraph (3 to 5 sentences) using only the facts below. Do not turn the article into an advert.
6. Close with one practical next step and the demo link.

## SEO checklist
- Main phrase in the title, the first 100 words and at least one H2.
- `description`: 140 to 160 characters, written like the line under the title on Google.
- 2 or 3 internal links: other blog articles (`{{ '/blog/' | relative_url }}...`) or site sections (`{{ '/#modules' | relative_url }}`, `{{ '/#demo' | relative_url }}`).
- If you use an outside fact or number, link the source (government body, standards body, well-known publication). Otherwise do not use the number.
- Use the words buyers search: job card, production planning, shop floor, traceability, OEE, subcontracting, job work, dispatch, MES.

## Facts about Athena you may use (from the public website)
- Athena is shop floor software (MES) for machine shops, by NMTG. Built inside an operating factory, by manufacturers.
- Modules: stage-wise planning; shop floor and OEE (quantity, stops and tools recorded at the machine; OEE from those entries); semi-finished goods traceability; finished goods traceability; dispatch tracker and planning; subcontracting (vendor stages with due dates, send and receive records); tool management (issue, return, tool life); quality management (inspection, rejections, rework by stage); escalation matrix; analytics and reports the team builds itself, with Excel export.
- No IoT, no sensors, no new hardware. Operators and supervisors record each action on a computer in their production area; usually one computer per production area, shared by the operators of about four machines.
- OEE comes from operator entries, not live machine telemetry.
- Records splits, rework, alternate machines and vendor delays as steps.
- Labels, stop reasons and messages can be set up in the team's own language.
- Works alongside the ERP: job cards come in through Excel or CSV files today; deeper links reviewed during discovery.
- Implementation: detailed process mapping, setup and configuration, hands-on training on the shop floor role by role, go-live zone by zone, support after go-live.
- Pricing by proposal; local server or cloud decided together.

## Never
- Invent numbers, percentages, savings, customers, quotes, case studies or awards.
- Claim features beyond the list above (no AI predictions, no automatic machine data, no mobile app claims).
- Name or criticise competitors.
- Copy text from other websites.
- Give legal, tax or compliance advice as fact; point to the official body instead.

## Daily review by email
- Every new draft is emailed to Jinal (jinal@nmtgindia.com) the morning before it goes live.
- He replies in the same thread: changes at the top, edits in the text, or HOLD.
- The next morning's run applies his reply before publishing at about 7:45 AM IST, so the article is live by 8 AM.

## Front matter for a new draft
```yaml
---
title: "..."
description: "..."
date: YYYY-MM-DD            # the day it will go live
author: Athena team
published: false            # draft, not on the website yet
hold: false                 # Jinal sets true to stop auto-publish
auto_publish_on: YYYY-MM-DD # the next day
email_thread: "..."          # Gmail thread of the review email sent to Jinal
---
```
File name: `_posts/YYYY-MM-DD-short-slug.md` (same date as `date`). Slug: lowercase words joined with hyphens, 4 to 7 words.
