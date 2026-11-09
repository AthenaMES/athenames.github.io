---
title: "What a job card should record at every stage: a checklist"
description: "A practical checklist of what a job card should record at every stage of a machine shop, from material issue to dispatch, so no lot or piece goes missing."
date: 2026-11-10
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-10
email_thread: "1a1be11f0867747c"
last_reply_id: "1a1be11f0867747c"
---

Every machine shop has a job card. Some are printed forms, some are a page in a register, some are a row in Excel. But ask three supervisors what a job card should record, and you will often get three different answers.

That is where most shop floor confusion starts. If one stage writes the quantity and another does not, or one operator writes the machine and the next writes nothing, the card stops telling the full story. Later, when a customer asks about a lot, or month-end figures do not match, nobody can trace what happened.

This article gives a simple checklist of **what a job card should record at every stage**, so the card carries the same facts from material issue to dispatch, whether it is on paper or on a screen.

## Why a fixed set of fields matters

A job card is not paperwork for its own sake. It is the only record that travels with the work. When it is filled in the same way at every stage, three things become possible:

- **You can find any lot.** You know which stage it is at, how many pieces, and since when.
- **You can count losses.** Rejections, rework and stops are written where they happen, not guessed at month-end.
- **You can trace back.** If a customer reports a problem, you can go from the finished part back to the machine, the operator, the date and the material.

Without a fixed set of fields, each person records what they think is important. The card then answers some questions at some stages, and none at others.

## The header: what to record once

These facts are written when the job card is opened, usually by production planning (PPC). They do not change from stage to stage.

1. **Job card number.** One unique number per card. Never reuse it.
2. **Part number and revision.** The drawing revision matters when a design changes mid-order.
3. **Customer and sales order or work order number.** This links the shop floor back to what was promised.
4. **Planned quantity.** How many pieces this card is meant to produce.
5. **Material details.** Grade, size and the heat number or batch number from the material certificate.
6. **Route.** The list of stages in order, with each one marked in-house or vendor.
7. **Due date.** The date the job must be ready for dispatch.

## At every stage: the checklist

These are the fields to record each time the work passes through a stage. Keep them the same for every stage, so the card reads like a clear timeline.

| Field | Why it matters |
| --- | --- |
| Stage name | Shows where the work is in the route |
| Machine (or vendor) | Needed when the job moves to an alternate machine |
| Operator or person responsible | Tells you whom to ask, without blame |
| Date and shift, start and end | Shows how long work waited and how long it ran |
| Quantity received at the stage | The starting count for this stage |
| Quantity completed (OK) | The good pieces that move on |
| Quantity rejected, with reason | Losses written where they happen |
| Quantity sent for rework, with reason | So rework pieces do not disappear |
| Stops, with reason and duration | The raw input for OEE and loss analysis |
| Tool used | Helps trace a quality problem to a tool |
| Inspection result and inspector | Proof that the stage was checked |

A simple rule holds the whole table together: **quantity received = OK + rejected + rework + still pending**. If those numbers do not add up at any stage, something is missing.

## Special cases the card must handle

The checklist above covers the normal flow. Real shop floors are not normal for long. Make sure your job card has a clear way to record these:

- **Splits.** When only part of the quantity moves on, record the split as two lots, each with its own quantity, stage and date. Do not let one card carry two stories.
- **Rework loops.** Record where the rework pieces went, and when they came back to the main flow.
- **Alternate machines.** If the job moves to a different machine, write the new machine at that stage, not just in the margin.
- **Vendor stages.** For subcontracting (job work), record the vendor name, the date and quantity sent, the challan number, the due date and the date and quantity received back.
- **Hold.** If a lot is stopped for a quality decision, record who put it on hold, why and when it was released.

## A worked example

For example, take a job card for 80 flange blanks (sample data, not a real customer order):

- **Header:** JC-1045, part FL-220 rev B, planned quantity 80, material EN8, heat number H-7731, route: cutting, turning, drilling, zinc plating (vendor), final inspection, dispatch.
- **Turning:** received 80, OK 76, rejected 2 (undersize diameter), rework 2 (burr on face), one stop of 25 minutes for an insert change.
- **Drilling:** received 76, OK 50 on day 1. The other 26 wait for a free machine and move to an alternate drilling machine the next day. The card shows two lots: 50 and 26.
- **Zinc plating:** 50 pieces sent to the vendor with a challan number and a due date. The 26 follow two days later. The 2 rework pieces, once deburred and drilled, rejoin the second lot, so 28 go in the second dispatch to the vendor.

Now the arithmetic checks out: 76 + 2 rework back = 78 good pieces in two lots, plus 2 rejected = 80. If a customer later asks about a flange from the second lot, you can trace it to the alternate drilling machine, the rework, the vendor and heat number H-7731.

## How to bring this checklist into your shop

1. **Collect your current job cards.** Take one real card from each product family and list every field the team actually fills in.
2. **Compare with the checklist.** Mark what is missing and what is written but never used.
3. **Agree on a short list of reasons.** Write rejection, rework and stop reasons in the words operators already use, and in their language.
4. **Decide who records each field.** Operators, inspectors, stores and PPC each own a part of the card.
5. **Try it on one product family first.** Run it for two weeks, then fix what did not work.

If you work to a quality standard such as [ISO 9001](https://www.iso.org/iso-9001-quality-management.html), check its requirements on identification and traceability with your certification body. The checklist here is a practical starting point, not a compliance guide.

If you are still deciding how to move from paper, our [30-day plan for moving from paper job cards to digital]({{ '/blog/paper-job-cards-to-digital-30-day-plan/' | relative_url }}) explains how to start one zone at a time.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built inside an operating factory. Operators record quantity, stops and tools at the machine on a shared computer in their production area, with no IoT or new hardware. Splits, rework, alternate machines and vendor delays are recorded as steps, so semi-finished and finished goods stay traceable. Rejections and rework are recorded by stage, and labels and stop reasons can be set up in your team's own language. You can see the full list of [Athena modules]({{ '/#modules' | relative_url }}).

## Your next step

Pick one job card from last week and check it against the stage checklist above. Count how many fields are missing at each stage. That count tells you where your shop loses track of work.

If you would like to see how your own job card would look in Athena, [book a demo]({{ '/#demo' | relative_url }}).
