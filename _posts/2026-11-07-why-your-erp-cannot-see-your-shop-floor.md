---
title: "Why your ERP cannot tell you where a job card is"
description: "Your ERP knows the order, the stock and the invoice. It does not know which stage a job card is at, what is waiting for a vendor, or why output dropped yesterday. Here is why, and what to do about it."
date: 2026-11-07
author: Athena team
image: /assets/img/og-image.png
image_alt: "A job card splitting between two heat treatment vendors"
---

Ask your ERP where job card 204718 is right now, and it will most likely say "Released". That answer is correct on paper and useless on the floor.

An ERP is built to run the business: orders, purchase, stock, invoices and tax. It records what *should* happen and what was *billed*. It is not built to record what happens between the cutting machine and the dispatch dock.

## What happens between release and dispatch

In a machine shop, a single job card rarely moves in a straight line:

- **Quantities split.** 40 of 60 pieces finish gear hobbing today. The other 20 follow tomorrow, as a separate lot.
- **Work goes outside.** Heat treatment or plating happens at a vendor, with its own lead time and its own delays.
- **Machines change.** A breakdown on one grinder moves the job to another.
- **Pieces come back.** Inspection sends two pieces to rework, and they loop back a stage.

Each of these is a normal day. None of them fits into one "status" field.

## Why this matters for dispatch dates

When the system only knows "Released" and "Dispatched", everything in between lives in WhatsApp chats, Excel sheets and phone calls. The plant head finds out a vendor lot is late on the day of dispatch. The customer finds out after that.

The real question is not "is the order open?" but **"which stage is each lot at, and what is it waiting for?"**

## What a shop floor system adds

A manufacturing execution system (MES) sits next to your ERP and records the floor as it really runs:

1. **Every stage is recorded** by the operator who did the work: quantity made, stops and their reasons, tools used.
2. **Splits, rework and vendor work are steps**, not exceptions, so no piece goes missing.
3. **Dispatch dates follow real progress**, so a late lot is flagged while there is still time to act.

You keep your ERP for money and stock. The shop floor finally has its own record.

## Where to start

You do not need sensors or machine connections. Start with one product family, record every stage for two weeks, and look at where work waits. In most plants, one stage (often a vendor) holds most of the delay.

*Want to see this on your own job cards? [Book a demo]({{ '/#demo' | relative_url }}).*
