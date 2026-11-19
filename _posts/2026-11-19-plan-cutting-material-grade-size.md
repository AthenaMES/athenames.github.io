---
title: "How to plan cutting by material grade and size"
description: "A simple way to plan cutting by material grade and size: group job cards by bar, cut in the right order, track the leftover ends and keep heat numbers clear."
date: 2026-11-19
author: Athena team
published: true
hold: false
email_thread: "1a1ec6ae98a3b045"
last_reply_id: "1a1ec6ae98a3b045"
---

In many machine shops, cutting is the first stage of every job card and the least planned. The saw operator picks up whichever job card is on top, finds a bar, cuts the pieces and moves on. An hour later, another job card for the same material grade and diameter arrives, and the same bar is pulled out of the rack again.

This looks harmless, but it costs time and material every day. The saw is set up again and again for the same size. Short leftover ends pile up in a corner because nobody knows which grade they are. And when a customer asks which heat a part came from, the cutting register cannot always say.

Planning cutting by material grade and size is a simple fix. Instead of cutting job card by job card, you group the day's cutting by grade and size, cut in a sensible order, and record what was used. This article shows how to do it with a daily cutting plan, a checklist and a worked example.

## Why cutting job card by job card causes problems

Cutting is where material turns into work in progress. Mistakes here travel through every stage after it.

- **Repeated setups.** Each change of size means adjusting the saw stop and often the blade or the vice. Cutting the same size three times in a day means three setups instead of one.
- **More waste.** Every bar ends with a piece too short to use for that job. If the next job of the same grade needs shorter pieces, that end could have been used. Cut at random times and it ends up as scrap.
- **Wrong grade issued.** Bars of different grades often look the same. When the operator is hunting for material for one job card at a time, the risk of picking the wrong grade goes up.
- **Lost heat numbers.** If the heat or batch number is not written down at the time of cutting, the link between the raw material certificate and the finished part is broken from the first stage.

## What a cutting plan should hold

A cutting plan is a short list for the saw, made once a day or once a shift. For each line it should show:

- Job card number and part number
- Material grade (for example EN8 or 20MnCr5)
- Size: diameter or section, and the cut length per piece
- Quantity of pieces required
- Planned date for cutting, taken from the job card's stage dates
- Heat number or batch of the bar to be used
- Space to record pieces actually cut, bars used and leftover length

The cut length is not just the finished length of the part. It needs an allowance for the saw cut and for facing on the machine. Industry guidance such as this [Production Machining article on how much stock is required](https://productionmachining.com/blog/post/how-much-stock-is-required) explains why every piece needs this extra material. Use the allowance your process engineer has set for each part, and write it into the routing so the saw operator does not guess.

## How to plan cutting by material grade and size: step by step

1. **Collect the job cards due for cutting.** Take every open job card whose cutting stage is due in the next one or two days. If you already plan stage by stage, this list comes straight from the stage dates.
2. **Group by grade, then by size.** Sort the list first by material grade, then by diameter or section. All the 40 mm EN8 jobs sit together, then the 50 mm EN8 jobs, and so on.
3. **Within each group, sort by priority.** Put the job card with the earliest due date first. Grouping should save setups, not delay an urgent job.
4. **Plan the bars.** For each group, add up the length needed, including allowances. Decide which bars to use, and start with leftover ends of the same grade and heat before opening a new bar.
5. **Check the material before cutting.** Confirm the grade and heat number on the bar against the plan. If the plan says one heat and the rack has another, the supervisor decides, not the operator.
6. **Cut in plan order.** Do one setup per size and cut all lines for that size before changing.
7. **Record what was used.** For each line, write the pieces cut, the bar and heat used, and the leftover length.
8. **Label and store leftover ends.** Mark each usable end with its grade, size, heat number and length. Store them by grade so tomorrow's plan can use them first.

## A short checklist for the saw area

- Today's cutting plan is printed or on screen before the shift starts.
- Lines are grouped by grade and size, with urgent jobs first in each group.
- Each bar is checked for grade and heat number before the first cut.
- Pieces cut are counted and written against the job card, not from memory at the end of the shift.
- Leftover ends are labelled and returned to a fixed place.
- Any shortage is reported to the planner the same day.

If you are not yet sure what each stage of the job card should record, see our checklist on [what a job card should record at every stage]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}).

## A worked example

For example, take a sample shop (not a real customer) where bars come in 3,000 mm lengths. Four job cards need cutting tomorrow. The cut lengths below already include the allowance for the saw cut and facing.

| Job card | Grade | Diameter | Cut length | Pieces | Due |
| --- | --- | --- | --- | --- | --- |
| JC-101 | EN8 | 40 mm | 125 mm | 30 | 24 Nov |
| JC-102 | 20MnCr5 | 50 mm | 210 mm | 20 | 25 Nov |
| JC-103 | EN8 | 40 mm | 95 mm | 40 | 26 Nov |
| JC-104 | EN8 | 50 mm | 160 mm | 12 | 27 Nov |

Cut in the order the job cards arrived, the saw would change size three times: 40 mm, then 50 mm, then 40 mm again, then 50 mm again in a different grade.

Grouped by grade and size, the plan becomes:

1. **EN8, 40 mm:** JC-101 first (earlier due date), then JC-103. Total length is 3,750 mm for JC-101 and 3,800 mm for JC-103, so 7,550 mm in all. Three bars cover it, and the third bar leaves a usable end of about 1,385 mm.
2. **EN8, 50 mm:** JC-104, 1,920 mm. The store has a labelled 2,100 mm end of the same grade, size and heat, so no new bar is opened.
3. **20MnCr5, 50 mm:** JC-102, 4,200 mm, from two bars of one heat number.

The saw now has three setups instead of four, the leftover end is used, and the heat number is written against each job card at the moment of cutting. The 1,385 mm end of EN8, 40 mm is labelled and stored for the next plan.

These figures are sample data, shown only to explain the method.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its stage-wise planning module gives each stage of a job card its own plan, including cutting. Operators and supervisors record quantities at the computer in their production area, with no IoT, sensors or new hardware. The semi-finished goods traceability module keeps the link from each job card to the stages it has passed through, and reports can be exported to Excel. You can see all [Athena modules]({{ '/#modules' | relative_url }}) on our home page.

## Your next step

Tomorrow morning, take the job cards due for cutting and sort them by grade and size before the saw starts. Count how many setups you save, and label every usable leftover end. After a week, you will know how much this one habit is worth on your floor.

To see how stage-wise planning and traceability work together in Athena, [book a demo]({{ '/#demo' | relative_url }}).
