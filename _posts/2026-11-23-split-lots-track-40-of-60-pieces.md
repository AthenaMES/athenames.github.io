---
title: "Split lots: tracking 40 of 60 pieces without losing the rest"
description: "How to track split lots on the shop floor: give each part of a job card its own number, balance quantities at each stage, and never lose the pieces left behind."
date: 2026-11-23
author: Athena team
published: true
hold: false
email_thread: "1a201046faf9558c"
last_reply_id: "1a201046faf9558c"
---

A job card for 60 pieces leaves the turning section. Forty pieces go ahead to milling because the customer needs them first. Twenty stay behind, waiting for a tool or a second setup. On paper, the job card goes with the forty. The twenty are now pieces with no card.

This is how **split lots** go missing. Nobody loses them on purpose. A week later, the stores team finds a crate of half-finished parts in a corner. Nobody is sure which job card they belong to, which stage they finished, or whether they were inspected. Some are reworked, some are scrapped, and the job card quietly closes at 40 instead of 60.

Splitting a lot is normal and often the right decision. The problem is not the split. It is that the paper system has one card for one lot, and has no clean way to follow two parts of the same job.

## Why split lots get lost

Most plants that lose pieces in splits see the same causes.

- **One card, two places.** The original job card can only travel with one part of the lot. The other part is left with a chit, a chalk mark or nothing at all.
- **Quantities are not balanced.** The register says 60 in at turning and 40 out at milling. Nobody writes down where the other 20 are, so the gap is only noticed at month-end.
- **Splits happen for many reasons.** A part of the lot goes to rework, a part goes to an alternate machine, a part is held for inspection, a part goes to a vendor first. Each reason needs a different follow-up.
- **The split is decided verbally.** The supervisor tells the operator "send forty ahead". The decision is right, but there is no record of who split it, when, or why.
- **Merging back is not recorded.** When the 20 pieces catch up, they may join a different batch, and the link to the original job card is gone.

## The basic rule: every piece is always somewhere

The simplest way to track split lots is one rule that everyone can check:

> At every stage, pieces in = pieces out + pieces still at the stage + pieces rejected.

If this does not balance, something is missing. A supervisor can check it in two minutes per job card, on paper or on a screen.

The second rule: **every part of a split gets its own identity, linked to the parent job card.** If the job card is JC-118, the two parts become JC-118/A and JC-118/B. Each part has its own quantity, its own current stage and its own tag on the crate. Both still point back to JC-118, its material and its heat number.

## How to track split lots: step by step

1. **Decide who may split a lot.** Usually the area supervisor or the planner. Operators should not split lots on their own, because they cannot see the whole plan.
2. **Record the split at the moment it happens.** Write the parent job card number, the stage, the date, the quantity in each part and the reason: priority, tool not ready, rework, alternate machine, vendor, or quality hold.
3. **Give each part a child number.** Use a simple suffix: /A, /B, /C. Write it on the job card copy or tag that travels with each crate. Keep the parent number visible on every tag.
4. **Copy the history, not just the quantity.** Each child must carry the material grade, heat number and the stages already done. Our checklist on [what a job card should record at every stage]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) lists the fields that matter.
5. **Give each part its own due date.** The pieces that go ahead and the pieces that wait will not finish together. Plan the stage dates for each part, as explained in our article on [stage-wise production planning]({{ '/blog/stage-wise-production-planning-one-due-date/' | relative_url }}).
6. **Balance quantities every day.** At the end of the shift, check the rule for every open job card with a split. Any gap is followed up the same day, not at month-end.
7. **Record merges.** If two parts join again, write it down: which child numbers, at which stage, and the new quantity. Do not mix parts from different heat numbers without a record.
8. **Close the parent only when all children are closed.** The job card for 60 is complete only when 60 pieces are dispatched, rejected with a reason, or still clearly accounted for.

## A worked example

For example, take a sample job card (not a real customer): JC-118, 60 pinion shafts, one heat number. The route is cutting, turning, milling, heat treatment at a vendor, grinding, final inspection and dispatch.

At milling, the customer asks for 40 pieces early. The supervisor splits the lot. Later, 5 pieces from the second part fail inspection after grinding and go for rework.

| Child | Qty | Reason for split | Current stage | Status |
| --- | --- | --- | --- | --- |
| JC-118/A | 40 | Customer priority | Dispatched | Closed |
| JC-118/B | 15 | Waiting for milling tool | Final inspection | Open |
| JC-118/B1 | 5 | Rework after grinding | Grinding (rework) | Open |
| **Total** | **60** | | | |

Without the split record, the register would show 40 dispatched and the job card would look almost done. With it, anyone can see that 20 pieces are still in the plant, where they are, and why. When the customer asks about the remaining pieces, the answer takes one look, not a walk around the shop.

These figures are sample data, shown only to explain the method.

## Checklist for supervisors

- Every split has a parent job card number and child numbers.
- Every child has a quantity, a reason, a current stage and a due date.
- Heat number and material travel with every child.
- Pieces in and pieces out balance at every stage, every day.
- Rework and rejections are recorded as their own parts, not as notes in the margin.
- Merges are written down.
- The parent job card closes only when every piece is accounted for.

## A note on traceability

If your customers ask for traceability, split lots are where it usually breaks first. Quality standards such as [ISO 9001](https://www.iso.org/iso-9001-quality-management.html) include requirements on identifying outputs and tracing them where needed. What your customer or certification body expects in your case is something to confirm with them directly. The method above simply makes sure that each piece can still be linked to its job card, material and stages after a split.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. It records splits, rework, alternate machines and vendor delays as steps. Operators and supervisors record each action on a computer in their production area, and the semi-finished goods traceability module follows work in progress between stages. The quality management module records inspection, rejections and rework by stage.

## Your next step

This week, pick three open job cards that have been split. Count the pieces at each stage and check whether the totals match the job card quantity. If any pieces are missing from the count, start the split record described above with those three cards.

To see how Athena tracks split lots and rework from stage to stage, [book a demo]({{ '/#demo' | relative_url }}).
