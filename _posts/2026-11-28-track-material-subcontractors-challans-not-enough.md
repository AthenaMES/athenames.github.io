---
title: "Track material at subcontractors: why challans are not enough"
description: "How to track material at subcontractors: why delivery challans alone lose pieces, and a simple send and receive record that shows what each vendor holds today."
date: 2026-11-28
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-28
email_thread: "1a21ac4a88ed96d0"
last_reply_id: "1a21ac4a88ed96d0"
---

Most machine shops send work outside. Heat treatment, plating, grinding, gear cutting and painting often go to a vendor down the road. The material leaves the gate with a delivery challan, and the challan copy goes into a file.

A month later, the planner asks a simple question: how many pieces of this part are at the heat treater right now? Nobody can answer quickly. Someone opens the challan file, someone calls the vendor, and the two numbers do not match. This is the daily problem of trying to **track material at subcontractors** with paper alone.

The challan is a necessary document. It is just not a tracking system. This article explains why, and shows a simple way to know what every vendor holds, by job card, on any day.

## What a challan does well, and what it does not

A delivery challan records that goods left your plant for job work. In India, the GST law has specific rules for sending goods to a job worker, including how they are documented and how long they may stay out. The [GST Council's job work guide](https://www.gstcouncil.gov.in/sites/default/files/e-version-gst-flyers/Job_Work.pdf) and [CBIC Circular 38/2018](https://gstcouncil.gov.in/sites/default/files/2024-06/jobwork_circular_38_of_2018.pdf) explain these rules. For what applies to your plant, check with your tax adviser or the official sources.

So the challan answers a tax and movement question: what left, when and to whom. It does not answer the production questions:

- **Which job card do these pieces belong to?** One challan often carries pieces from three or four job cards.
- **How many came back, and when?** Material returns in parts, often on the vendor's own challan with a different number.
- **How many are still at the vendor?** This needs every send and every receive added up, per job card.
- **Did anything come back rejected or short?** A return of 96 against 100 sent is easy to miss in a file.
- **Which stage comes next?** The challan does not tell the shop floor where the pieces go after they return.

## Why material goes missing at vendors

Pieces are rarely lost on the road. They go missing in the records. The usual reasons:

- **Partial returns.** The vendor sends 60 today and 40 next week. The second return is never matched to the first send.
- **Mixed job cards.** Two job cards of the same part travel together and come back as one lot.
- **Different numbers on each side.** Your challan number, the vendor's return challan and the job card number are never written on the same page.
- **Rejections held at the vendor.** A few pieces fail at the vendor and stay there, but your records still show them as "sent".
- **No one owns the balance.** Stores records the movement, planning wants the date, and nobody checks the open quantity each week.

## How to track material at subcontractors: step by step

You do not need new hardware for this. You need one record that links the challan to the job card and keeps a running balance.

1. **Write the job card number on every challan line.** If one challan carries three job cards, use three lines, each with its own quantity.
2. **Keep a send and receive record per job card and vendor stage.** Columns: job card, part, stage, vendor, challan number, date sent, quantity sent.
3. **Record every return against the same line.** Add the vendor's return challan number, date received, quantity received, and quantity rejected or short.
4. **Calculate the balance at the vendor.** Balance = sent minus received minus rejected at vendor. This number is the answer to "what is at the vendor right now?"
5. **Give each vendor stage a due date.** When you send, write the date it should come back. Our article on [planning vendor stages around real lead times]({{ '/blog/plan-vendor-stages-real-lead-times/' | relative_url }}) shows how to set this from your own history.
6. **Treat a partial return as a split.** The returned pieces move to the next stage, the rest stay open at the vendor. See [split lots]({{ '/blog/split-lots-track-40-of-60-pieces/' | relative_url }}) for how to record this without losing pieces.
7. **Inspect on receipt and record the result.** Count, check and write the result before the pieces move on.
8. **Review open balances every week.** One list: every vendor, every job card with a balance above zero, and how many days it has been out. Call the vendor with this list in hand.
9. **Reconcile with the vendor once a month.** Send them your open list and ask them to confirm. Differences found early are easy to settle.

## A worked example

For example, here is a sample send and receive record for one heat treatment vendor. This is sample data, not a real customer.

| Job card | Part | Challan | Sent | Qty sent | Return challan | Received | Qty received | Rejected | Balance |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| JC-405 | Pinion shaft | CH-221 | 3 Nov | 100 | V-118 | 10 Nov | 60 | 0 | 40 |
| JC-405 | Pinion shaft | CH-221 | 3 Nov | | V-124 | 14 Nov | 36 | 2 | 2 |
| JC-409 | Pinion shaft | CH-221 | 3 Nov | 80 | V-124 | 14 Nov | 80 | 0 | 0 |
| JC-412 | Gear blank | CH-230 | 12 Nov | 150 | | | | | 150 |

Look at what the challan file alone would show: two challans, CH-221 and CH-230, with 330 pieces sent. That is all.

The record shows much more. JC-409 is complete. JC-412 is fully at the vendor, still within its due date. JC-405 came back in two parts, two pieces were rejected, and **two pieces are still unaccounted for**. Without the balance column, those two pieces would quietly disappear, and the job card would be short at dispatch.

With this record, the planner's weekly call to the vendor takes two minutes: "We show two pieces of JC-405 still with you, and 150 of JC-412 due on 19 Nov. Can you confirm?"

## Checklist for stores and planning

- Every challan line carries a job card number and quantity.
- Every return is recorded against the line it came from.
- The vendor's return challan number is written next to your challan number.
- Rejections and shortages at the vendor are recorded, not ignored.
- Every vendor stage has a due date.
- The balance at each vendor is visible per job card.
- Open balances are reviewed every week.
- Each vendor confirms the open list once a month.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its subcontracting module records vendor stages with due dates and keeps send and receive records against each job card. Splits and vendor delays are recorded as steps, so a partial return does not break the trail, and the quality management module records inspection and rejections by stage. Supervisors record each action on a computer in their production area, with no sensors or new hardware, and reports can be exported to Excel.

## Your next step

This week, pick your busiest vendor. List every job card you have sent them in the last two months, and add up sent minus received for each. Compare the list with the vendor's own count. The gaps you find will show you exactly why the challan file is not enough.

To see how Athena tracks job work at vendors by job card, [book a demo]({{ '/#demo' | relative_url }}).
