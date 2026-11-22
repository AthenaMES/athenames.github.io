---
title: "Setting priorities by due date without daily firefighting"
description: "How to set shop floor priorities by due date without daily firefighting: one priority list, stage due dates, a simple ratio, and one short review each morning."
date: 2026-11-22
author: Athena team
published: true
hold: false
email_thread: "1a1fbde12f71b013"
last_reply_id: "1a1fbde12f71b013"
---

In many machine shops, the priority list changes every hour. A customer calls, the owner walks onto the floor, and the job that was third in line is suddenly first. The supervisor breaks a setup halfway, the operator moves to a new job card, and the job that was running now waits.

This is daily firefighting. Everyone is busy, but the same jobs keep becoming urgent, and the plant still misses dates. The problem is usually not effort. It is that nobody shares one clear way of setting priorities by due date.

This article shows a simple method a supervisor or planner can start using tomorrow: one priority list, built from stage due dates, checked once a day, and changed only for clear reasons.

## Why priorities keep changing on the shop floor

Firefighting has a few common causes. Most plants will recognise more than one.

- **Only the final due date is known.** The job card shows the dispatch date, but not when each stage must finish. A job looks safe until the last few days, and then it becomes urgent all at once.
- **The loudest request wins.** Priority goes to whoever calls or shouts last, not to the job that is truly at risk.
- **Each supervisor keeps a separate list.** Cutting, turning and grinding each work to their own idea of what is urgent, so a job is rushed at one stage and waits at the next.
- **Changes are not recorded.** When a job is pushed ahead, nobody notes which job was pushed back, so that job becomes the next emergency.
- **Setups are broken too often.** Every change in the middle of a run costs setup time, which makes the plant even later.

## Two simple rules for setting priorities by due date

You do not need complex scheduling software to set better priorities. Two well-known rules are enough to start.

**Earliest due date first.** Line up the jobs waiting at a stage and run the one with the nearest due date first. It is easy to explain and easy to check. Its weakness is that it ignores how much work is still left on the job.

**Critical ratio.** This rule compares the time left with the work left. A common textbook definition is: critical ratio = time remaining before the due date ÷ remaining processing time, and the job with the smallest ratio goes first ([University of Kentucky course notes on scheduling](https://www.uky.edu/~dsianita/300/schedule.html)). In plain words:

- A ratio below 1 means the job is already behind: there is less time left than work left.
- A ratio close to 1 means there is no spare time.
- A ratio well above 1 means the job has room.

Use earliest due date for simple stages with short jobs. Use the critical ratio when jobs have several stages left, because it shows which job is really at risk.

## How to set priorities without firefighting: step by step

1. **Give every stage its own due date.** A priority rule only works if each stage has a date. Our article on [stage-wise production planning]({{ '/blog/stage-wise-production-planning-one-due-date/' | relative_url }}) explains how to work back from the dispatch date.
2. **Keep one priority list for the whole plant.** The planner owns it. Each area works from the same list, filtered for its own machines.
3. **Count remaining work in days or hours.** For each open job card, add up the time for the stages still to be done, including vendor stages. Use real lead times for vendor work, as shown in our article on [planning vendor stages]({{ '/blog/plan-vendor-stages-real-lead-times/' | relative_url }}).
4. **Rank the list once a day.** At the start of the shift, sort jobs at each stage by due date or by critical ratio. Mark the jobs with a ratio below 1 clearly.
5. **Freeze the next few hours.** Once a machine has started a job, let it finish the run unless there is a real emergency. This protects setups and stops the plan from changing every hour.
6. **Agree what counts as an emergency.** Write it down: for example, a line-stop risk at the customer, or a safety or quality issue. A phone call alone is not an emergency.
7. **Record every change of priority.** When a job is moved up, note the reason and which job moves down. The planner checks the new due date of that job the same day.
8. **Review at the end of the week.** Look at how many priority changes there were and why. If the same reason keeps coming back, fix the cause, not the symptom.

## A worked example

For example, take a sample turning cell (not a real customer) on a Monday morning. Four job cards are waiting. The supervisor works out the days left to each job's dispatch date and the days of work still left, including the vendor stage for job C.

| Job card | Parts | Days to due date | Days of work left | Critical ratio | Order |
| --- | --- | --- | --- | --- | --- |
| A | 60 pinion shafts | 6 | 3 | 2.0 | 4 |
| B | 40 flanges | 4 | 4 | 1.0 | 2 |
| C | 80 bushes | 9 | 10 | 0.9 | 1 |
| D | 50 spacers | 3 | 2 | 1.5 | 3 |

If the cell used earliest due date only, it would run D first, then B, A and C. Job C would wait the longest, even though it is already behind: it still needs heat treatment at a vendor, so it has more work left than days left.

With the critical ratio, job C goes first, then B, then D, then A. Job A has the most spare time, so it can wait. The supervisor checks that C and B use similar tools, so the setup change between them is small.

These figures are sample data, shown only to explain the method. Use your own job cards and your own times.

## Checklist for the morning priority review

- Every open job card has stage due dates.
- Remaining work includes vendor stages at real lead times.
- Jobs are ranked by one agreed rule.
- Jobs with a ratio below 1 are marked and discussed first.
- Running jobs are not broken without an agreed emergency.
- Every priority change is written down with a reason.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its stage-wise planning module gives each stage of a job card its own date, and the subcontracting module keeps vendor stages with their own due dates and send and receive records. Operators and supervisors record each action on a computer in their production area, so the team sees where each job card actually is. The escalation matrix helps make sure a delay reaches the right person, and the dispatch tracker and planning module keeps dispatch dates in view. You can see all [Athena modules]({{ '/#modules' | relative_url }}) on our home page.

## Your next step

Tomorrow morning, take the job cards waiting at your busiest stage. Work out the days left and the work left for each one, and sort them by critical ratio. Compare that order with the order the floor is actually following, and talk about the differences in the morning meeting.

To see how stage-wise planning and dispatch tracking work together in Athena, [book a demo]({{ '/#demo' | relative_url }}).
