---
title: "Stage-wise production planning: why one due date is not enough"
description: "One due date per job card hides delays until it is too late. Stage-wise production planning gives every stage its own date, so a slip shows up days earlier."
date: 2026-11-18
author: Athena team
published: true
hold: false
email_thread: "1a1e74443c56ec19"
last_reply_id: "1a1e74443c56ec19"
---

In most machine shops, a job card carries one important date: the day the customer needs the parts. The planner writes it at the top, the supervisor sees it, and everyone works towards it. That one date drives the whole job.

The problem is that a job card does not travel in one step. It goes through cutting, turning, milling, heat treatment at a vendor, grinding, inspection and packing. If the only date on the card is the final one, nobody knows on day three whether the job is on time or already late. The delay only becomes visible when the job reaches dispatch and is not ready.

Stage-wise production planning fixes this by giving every stage of the job card its own planned date. This article explains why one date is not enough, how to set stage dates without a complicated system, and how to use them every day.

## Why one due date hides problems

A single due date tells you where the job must finish. It does not tell you where the job should be today.

Think of a job with seven stages and fourteen days. On day six, the parts are still waiting at the turning stage. Is that a problem? With one due date, the honest answer is "we do not know". The supervisor may feel there is still plenty of time. The planner may assume the job has moved on. By the time someone notices, there are three days left for four stages, and one of them is a vendor stage that takes four days on its own.

One due date also creates three common habits:

- **Firefighting at the end.** Jobs are pushed hard in the last few days, often with overtime and setup changes that disturb other jobs.
- **Vendor surprises.** Heat treatment, plating or grinding at a subcontractor takes a fixed number of days. If the material reaches the vendor late, no amount of effort inside the factory can recover that time.
- **Arguments about blame.** When a job is late, every stage says it did its part. Without stage dates, there is no record of where the time was actually lost.

## What stage-wise production planning means

Stage-wise production planning means each stage of the routing has a planned start or finish date, worked out from the final due date. The job card then shows not just "due 28 November" but "turning done by 19 November, at the vendor by 21 November, back by 25 November".

This is often called backward scheduling: start from the date the customer needs the parts and work back, stage by stage. Many planning systems describe it the same way, for example [Oracle NetSuite's help page on backward scheduling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4001085919.html). You do not need special software to start. A planner with a pen and a calendar can do it for the urgent jobs.

## How to set stage dates: a step-by-step method

1. **List the stages in order.** Take the routing for the part. Write every stage, including inspection, packing and any vendor stage. Do not skip the small ones: a missed deburring step can hold a lot for a day.
2. **Write a realistic time for each stage.** Use what actually happens on your floor, not the ideal cycle time. Include waiting time before the machine, setup time, and transport between areas. For vendor stages, use the days the vendor really takes, door to door.
3. **Start from the dispatch date and work back.** Put the packing and dispatch stage on the final date. Subtract the time for each stage before it, one by one, until you reach material issue.
4. **Add a small buffer before risky stages.** Vendor stages and stages on a single bottleneck machine are where jobs usually slip. A day of buffer before them is better than a day of overtime after them.
5. **Check the start date.** If the first stage should have started yesterday, the job is already late on paper. Tell sales and the customer now, not on the due date.
6. **Write the stage dates on the job card.** The dates must travel with the job, where the supervisor and operator can see them, not only in the planner's sheet.
7. **Review stage dates daily.** Each morning, list the stages that were due yesterday and are not done. That short list is where attention should go today.

## A checklist for daily use

- Every open job card has a planned date for each stage.
- Vendor stages have a send date and an expected return date.
- The daily review looks at stages that are late, not only jobs that are late.
- When a stage slips, the planner moves the later stage dates and checks the dispatch date.
- Splits and rework are planned as their own steps, with their own dates.
- Late stages have a reason written down, so the same problem can be fixed next time.

If you are still deciding what a job card should hold at each stage, our checklist on [what a job card should record at every stage]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) is a good place to begin.

## A worked example

For example, take a sample order (not a real customer) of 80 flanges, due for dispatch on 28 November. The planner works back from the due date using the usual time for each stage in this sample shop:

| Stage | Usual time | Planned finish |
| --- | --- | --- |
| Material cutting | 1 day | 17 Nov |
| CNC turning | 2 days | 19 Nov |
| VMC drilling | 1 day | 20 Nov |
| Buffer before vendor | 1 day | 21 Nov |
| Heat treatment (vendor) | 4 days | 25 Nov |
| Grinding | 1 day | 26 Nov |
| Final inspection | 1 day | 27 Nov |
| Packing and dispatch | 1 day | 28 Nov |

On 20 November, the morning review shows that CNC turning, planned to finish on 19 November, is still running. Only 50 of the 80 flanges are done because a tool change took longer than expected.

With a single due date, this would look fine: there are still eight days left. With stage dates, the planner sees the risk at once. If the parts reach the vendor late, the four vendor days push grinding and inspection past 28 November.

The planner has two choices that day: move the remaining 30 pieces to an alternate machine, or send the first 50 to the vendor as a split lot so the vendor can start. Either way, the decision is made eight days before dispatch, not one.

These figures are sample data, shown only to explain the method.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its stage-wise planning module gives each stage of a job card its own plan, and vendor stages carry their own due dates with send and receive records. Splits, rework and alternate machines are recorded as steps, so a split lot like the one in the example stays traceable. Operators and supervisors record progress on a computer in their production area, with no IoT, sensors or new hardware, and job cards come in from your ERP through Excel or CSV files. You can see the full list of [Athena modules]({{ '/#modules' | relative_url }}) on our home page.

## Your next step

Pick your five most urgent job cards today. For each one, write the stages in order, add a realistic time for each, and work back from the due date. Tomorrow morning, check which stages are already behind. That one list will tell you more than the due dates alone.

If you would like to see how stage-wise planning works in Athena, [book a demo]({{ '/#demo' | relative_url }}).
