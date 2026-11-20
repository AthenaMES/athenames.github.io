---
title: "Planning vendor stages around real lead times"
description: "Plan vendor stages like heat treatment and plating around real lead times: record send and receive dates, find the true days per vendor, and plan with margin."
date: 2026-11-21
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-21
email_thread: "1a1f6b775f3c1676"
last_reply_id: "1a1f6b775f3c1676"
---

Most machine shops send some stages outside: heat treatment, plating, grinding, gear cutting, painting. On paper, the plan gives each of these vendor stages a fixed number of days, often "one week", because that is what the vendor said when the work started. Then a lot of shafts comes back after twelve days, and the dispatch date slips.

The problem is not only the vendor. The plan uses a lead time that someone remembers, not the lead time that actually happens. Nobody has the send and receive dates in one place, so nobody can say how long that vendor really takes.

Planning vendor stages around real lead times fixes this. You record when material goes out and when it comes back, you work out the true days for each vendor and each type of work, and you plan with those numbers. This article shows how, step by step, with a worked example.

## Why vendor stages cause so many late jobs

Inside the plant, a supervisor can see a job card waiting at a machine. Once material leaves the gate, it disappears from view until it comes back.

- **The lead time in the plan is a promise, not a record.** "Five days" was agreed once. The real time may be longer in the busy season or when the vendor's furnace is down.
- **Travel and waiting are not counted.** The time a lot waits at your gate for a vehicle, and the time it waits after return for incoming inspection, both belong to the vendor stage.
- **Small lots wait for batches.** A heat treatment vendor may hold your 40 pieces until the furnace load is full.
- **Partial returns are not tracked.** The vendor sends back 50 of 60 pieces. The job card shows "received" and the 10 missing pieces are forgotten until dispatch.
- **Delays are found late.** Nobody checks the lot until the next stage is waiting for it.

## What to record for every vendor stage

For each lot sent out, keep these details together with the job card:

- Job card number, part number and the stage being done outside
- Vendor name and type of work (for example, case hardening, zinc plating)
- Quantity sent and the date it left the gate
- Due date given to the vendor
- Quantity received, the date it came back, and any short or rejected quantity
- Date it cleared incoming inspection and was ready for the next stage

The challan or delivery document is still needed. But the challan shows that material went out. It does not tell the planner when it is due back or how late it is.

In India, GST rules also set conditions and time limits for goods sent for job work. The [GST Council's flyer on job work](https://www.gstcouncil.gov.in/sites/default/files/e-version-gst-flyers/Job_Work.pdf) explains the rules. Check the current position with your tax adviser; this article does not give tax advice.

## How to plan vendor stages around real lead times: step by step

1. **Start recording send and receive dates today.** Use one register or one sheet for all vendor stages. Every lot gets one line, from the day it leaves to the day it is ready for the next stage.
2. **Measure lead time from gate to ready.** Count the days from the date the material left your gate to the date it cleared incoming inspection. This is the lead time that matters to your plan, not only the vendor's working days.
3. **Group by vendor and type of work.** Heat treatment at one vendor and plating at another will have different lead times. Keep them separate.
4. **Look at the usual time and the slow time.** After a few weeks, you will have several lots for each vendor. Note the typical lead time and the longer times you see now and then. Plan with a figure close to the slow end, not the best case.
5. **Give each vendor stage its own due date.** In a stage-wise plan, the vendor stage gets a send date and a receive date like any other stage. Our article on [stage-wise production planning]({{ '/blog/stage-wise-production-planning-one-due-date/' | relative_url }}) explains how to set dates stage by stage.
6. **Plan the stage before and after.** If the lead time is long, finish the machining stage earlier so the lot leaves on time. Book the next machine for the realistic return date, not the hopeful one.
7. **Check open lots every day.** Make a short list of lots that are due back in the next two days, and lots that are already late. Call the vendor before the due date, not after.
8. **Track partial returns.** If only part of a lot comes back, keep the balance open against the vendor until it is received or written off.
9. **Review each vendor every month.** Count how many lots came back by the due date and how many were late. Share the facts with the vendor. A plain record makes the conversation easier for both sides.

## A worked example

For example, take a sample machine shop (not a real customer) that sends shafts to one vendor for case hardening. The plan has always used 5 days for this stage. The planner records the last six lots:

| Lot | Qty sent | Left gate | Ready after inspection | Days |
| --- | --- | --- | --- | --- |
| 1 | 60 | 2 Oct | 8 Oct | 6 |
| 2 | 40 | 6 Oct | 13 Oct | 7 |
| 3 | 80 | 9 Oct | 15 Oct | 6 |
| 4 | 50 | 14 Oct | 23 Oct | 9 |
| 5 | 60 | 20 Oct | 27 Oct | 7 |
| 6 | 30 | 24 Oct | 3 Nov | 10 |

In this sample, no lot came back within the 5 days in the plan. Four of the six lots took 6 or 7 days. Lots 4 and 6 took 9 and 10 days. Lot 6 was the smallest lot, which suggests it may have waited for a full furnace load. The planner checks this with the vendor before drawing a conclusion.

The planner now makes three changes:

1. **Plan 8 days for this stage**, instead of 5. Most lots fit inside this, and the plan stops promising dates it cannot keep.
2. **Send small lots together where possible**, so they do not wait at the vendor for a batch.
3. **Ask for a fixed furnace day** for urgent lots, and agree it in writing.

These figures are sample data, shown only to explain the method. Use your own records.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its subcontracting module gives vendor stages their own due dates and keeps send and receive records against each job card. Athena records vendor delays, splits and rework as steps, so a partial return can be recorded as a split instead of being forgotten. The dispatch tracker and planning module helps the team keep dispatch dates in view. You can see all [Athena modules]({{ '/#modules' | relative_url }}) on our home page.

## Your next step

This week, pick the vendor stage that delays you most often. Write down the send date and the ready date for every lot, and after one month compare the real lead time with the number in your plan. Change the plan to match what you find.

To see how vendor stages, send and receive records and stage-wise planning work together in Athena, [book a demo]({{ '/#demo' | relative_url }}).
