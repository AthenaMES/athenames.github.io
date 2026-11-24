---
title: "Semi-finished goods traceability, explained simply"
description: "Semi-finished goods traceability in plain words: what to record between stages, how to tag work in progress, and how to answer where a piece is in one look."
date: 2026-11-25
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-25
email_thread: "1a20b509b6a91b3e"
last_reply_id: "1a20b509b6a91b3e"
---

A customer calls about a batch of flanges. One piece has a crack near the bore. The quality head wants to know three things: which bar it was cut from, which machine turned it, and whether any other pieces from the same lot are still in the plant. The finished goods record shows the invoice and the dispatch date. Everything that happened before final inspection is spread across registers, chits and memory.

This is the gap that **semi-finished goods traceability** fills. Semi-finished goods are pieces that have started their route but are not yet finished: cut blanks, turned parts waiting for milling, parts at a heat treatment vendor, pieces waiting for grinding. Most machine shops call this work in progress, or WIP.

Paper systems track the start and the end of a job well. The middle is where pieces wait, move, split and get mixed. That middle is what this article is about.

## What semi-finished goods traceability means

In simple words, it means that at any moment you can answer four questions about any piece that is not yet finished:

1. **Which job card does it belong to?**
2. **What material and heat number is it made from?**
3. **Which stages has it finished, on which machine, by whom, and on what date?**
4. **Where is it now, and what is the next stage?**

If you can answer these for every crate on the floor, you have semi-finished goods traceability. If you need to walk the shop and ask three people, you do not.

## Why it breaks on paper

Most plants lose WIP traceability in the same few places.

- **Pieces move without the card.** The job card sits in the supervisor's file while the crate moves to the next machine.
- **Registers are kept by area, not by job.** Turning has its register, milling has its own. Linking one job across them takes hours.
- **Splits and rework.** Part of a lot goes ahead, part waits, part goes for rework. Our articles on [tracking split lots]({{ '/blog/split-lots-track-40-of-60-pieces/' | relative_url }}) and [recording rework loops]({{ '/blog/rework-loops-record-no-piece-missing/' | relative_url }}) cover these in detail.
- **Vendor stages.** Pieces leave for heat treatment or plating and come back mixed with other lots, or with a different count.
- **Waiting areas.** Crates parked near a machine for days lose their tags, or the tag gets wet, torn or overwritten.

## The building blocks

You do not need complex systems to start. You need a few simple habits, used every time.

- **One identity per lot.** Every lot on the floor carries its job card number. If a lot is split, each part gets a child number linked to the parent.
- **A tag on every crate.** The tag shows the job card number, part number, quantity, heat number and the last stage finished. Use a strong card or a plastic sleeve so it survives oil and handling.
- **A record at every stage.** When a stage finishes, someone records the job card, quantity in, quantity good, quantity rejected or sent for rework, the machine and the operator.
- **Quantities that balance.** At every stage, pieces in must equal pieces out, plus pieces still at the stage, plus pieces rejected. A gap means something is missing.
- **Send and receive records for vendors.** Every vendor stage has a send record and a receive record, both with the job card number and quantity.

## How to set it up: step by step

1. **List your stages.** Write down the route for your main product families: cutting, turning, milling, drilling, heat treatment, grinding, inspection. Keep it short and use the names your operators use.
2. **Decide the fields for each stage record.** Job card number, date, machine, operator, quantity in, good, rejected, sent for rework. Add the heat number at cutting, so it is linked from the first stage.
3. **Make the tag standard.** One format for the whole plant. Print it, so nobody writes their own version.
4. **Record at the stage, not at the end of the day.** Records written from memory at 6 PM miss things. The best moment is when the operator finishes the quantity.
5. **Check balances daily.** The supervisor picks the open job cards and checks the balance rule. Any gap is followed up the same day.
6. **Do a weekly floor walk.** Pick ten crates at random. Check that each tag matches the stage record. Fix the habit, not just the tag.
7. **Practise a trace.** Once a month, pick one finished piece and trace it back to its heat number and machines. Time how long it takes. If it takes more than a few minutes, find the stage where the trail went cold.

## A worked example

For example, take a sample job card (not a real customer): JC-205, 80 flanges, material EN8, heat number H-4471. The route is cutting, turning, drilling, heat treatment at a vendor, and final inspection.

| Stage | Date | Machine / vendor | Qty in | Good | Rejected / rework | Still at stage |
| --- | --- | --- | --- | --- | --- | --- |
| Cutting | 3 Nov | Bandsaw 1 | 80 | 80 | 0 | 0 |
| Turning | 4 Nov | CNC lathe 2 | 80 | 76 | 2 rework, 2 rejected | 0 |
| Drilling | 5 Nov | Drill 1 | 76 | 50 | 0 | 26 |
| Heat treatment | 6 Nov sent | Vendor A | 50 | Not yet back | 0 | 50 (at vendor) |

Two rework pieces from turning are in a separate record, linked to JC-205. Twenty-six pieces are still waiting at drilling.

Now suppose one flange from this lot is found cracked. With these records, the quality head can see in one look: heat number H-4471, turned on CNC lathe 2 on 4 November, drilled on Drill 1. Twenty-six pieces from the same lot are still at drilling and can be held for checking before they move. The 50 at the vendor can be checked when they come back.

These figures are sample data, shown only to explain the method.

## Checklist for supervisors

- Every crate has a tag with job card number, heat number, quantity and last stage.
- Every stage has a record with machine, operator, date and quantities.
- Rework and rejections are recorded as their own entries, linked to the job card.
- Splits have child numbers that point back to the parent.
- Vendor stages have send and receive records with quantities.
- Quantities balance at every stage, every day.
- One trace test is done every month.

## A note on standards

Customers who ask for traceability often refer to quality management standards. [ISO 9001](https://www.iso.org/iso-9001-quality-management.html), for example, includes requirements on identifying outputs and on traceability where it is required. What your customer or certification body expects in your case is something to confirm with them directly. The habits above simply make sure every piece in the middle of its route can be linked back to its job card, material and stages.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its semi-finished goods traceability module follows work in progress between stages, and it records splits, rework, alternate machines and vendor delays as steps. Operators and supervisors record each action on a computer in their production area, with no sensors or new hardware. The subcontracting module keeps send and receive records for vendor stages, and finished goods traceability carries the trail through to dispatch.

## Your next step

Tomorrow, pick one finished part from your last dispatch and try to trace it back to its heat number, machines and dates. Note each place where you had to ask someone instead of reading a record. Those are the first stages to fix.

To see how Athena follows semi-finished goods from stage to stage, [book a demo]({{ '/#demo' | relative_url }}).
