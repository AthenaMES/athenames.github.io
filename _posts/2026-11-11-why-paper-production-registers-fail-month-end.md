---
title: "Why paper production registers fail at month-end"
description: "Paper production registers work day to day but break at month-end. See why the numbers stop matching, and a simple checklist to close the month with confidence."
date: 2026-11-11
author: Athena team
published: true
hold: false
email_thread: "1a1c337899912bc9"
last_reply_id: "1a1c337899912bc9"
---

On the last day of the month, the production office in many machine shops changes. The planner, the supervisors and the accounts team sit with a stack of **paper production registers**, a calculator and an Excel sheet. For two or three days, everyone tries to answer one question: how much did we really produce?

The registers were filled in every shift. Nobody was careless. Yet the totals do not match the dispatch figures, the stores issue slips or the job cards. Some pieces seem to have vanished. Others seem to have been made twice.

This is not a people problem. It is the way paper production registers are built. They work well for recording one shift. They fail when you need to add up a month. This article explains why, and gives a practical checklist to make month-end closing faster, on paper or on a screen.

## What a production register is good at

A paper register is simple, cheap and always available. An operator or supervisor writes the date, shift, machine, part number and quantity. Nobody needs training or a login. When power or internet goes down, the register still works.

For a small shop with a few machines and a few products, this is enough. The supervisor knows every job by heart, and the register is just a backup to memory.

The trouble begins when the shop grows: more machines, more part numbers, more vendors and more shifts. The register still records each shift, but nobody can hold the whole month in their head any more.

## Why paper production registers fail at month-end

### 1. Each register tells only part of the story

Most plants keep several registers: one per machine or section, one for inspection, one for stores, one for vendor challans. Each is correct on its own. At month-end, someone must join them by hand. A job that appears in turning but not in inspection may be waiting, rejected, or simply not written down. The register cannot tell you which.

### 2. Quantities are written, but losses are not

Operators usually write the good quantity. Rejections, rework and short pieces are often written in the margin, in a separate book, or not at all. At month-end, the gap between what was issued and what was produced has no explanation.

### 3. Splits and rework break the count

When 60 pieces become a lot of 40 and a lot of 20, or when 5 pieces go back for rework, paper has no clean way to show it. The same pieces may be counted twice at the next stage, or not counted at all.

### 4. Vendor stages are outside the register

For subcontracting (job work), material leaves the plant on a challan and comes back days later. The shop floor register does not show what is still at the vendor, so the month-end work-in-progress figure is a guess.

### 5. Handwriting and copying add errors

Every time a figure is copied from a register to a summary sheet and then into Excel, there is a chance of a wrong digit, a missed line or a page counted twice. Nobody notices until the totals do not match.

### 6. The answers come too late

Even when month-end figures are finally correct, they describe a month that is already over. A machine that lost hours to stops in the first week shows up only in the next month's meeting, when it is too late to recover the dispatch.

## A month-end closing checklist

You can make month-end much easier, even before you change any system. Use this checklist with your supervisors and planner.

1. **Use one job card number everywhere.** Every register, challan and inspection entry should carry the job card number, so records can be joined.
2. **Record received, OK, rejected and rework at every stage.** The rule is simple: quantity received = OK + rejected + rework + still pending. Our [job card checklist]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) lists the fields stage by stage.
3. **Write splits as separate lots.** When a quantity splits, give each part its own line with its own quantity and stage.
4. **Keep a vendor register with balances.** For each challan, record quantity sent, quantity received back and the balance still at the vendor.
5. **Close each week, not just each month.** A short weekly check finds missing entries while people still remember what happened.
6. **Agree on fixed reasons.** A short list of rejection and stop reasons makes losses easy to add up.
7. **Decide who signs off each register.** One named person per section checks the totals before they go to the office.

## A worked example

For example, take a CNC turning section with four machines, running two shifts (sample data, not a real plant). At month-end, the planner finds this for one part:

| Source | Quantity |
| --- | --- |
| Material issued for job card JC-2210 | 500 pieces |
| Turning register, total OK | 470 |
| Inspection register, accepted | 452 |
| Sent to plating vendor (challans) | 400 |
| Received back from vendor | 360 |
| Dispatched | 340 |

The gaps are clear, but the reasons are not. Where are the 30 pieces between issue and turning? Some may be rejected at setup and never written down. The 18 between turning and inspection may be rework waiting at the machine. The 52 between inspection and the vendor may be waiting in the plant for a second challan. The 40 still at the vendor have no due date written anywhere.

With the checklist above, each gap would carry a reason and a date: "30 rejected in turning: 22 undersize, 8 chatter marks", "18 in rework, burr", "52 waiting for vendor dispatch", "40 at vendor, due on the 5th". The month-end meeting then becomes a review of decisions, not a search for pieces.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built inside an operating factory. Operators and supervisors record quantity, stops, rejections and rework at each stage on a shared computer in their production area, with no IoT or new hardware. Splits, rework, alternate machines and vendor delays are recorded as steps, and subcontracting keeps send and receive records for each vendor stage. Reports can be built by your own team and exported to Excel, so month-end figures come from the same entries made during the month. You can see the full list of [Athena modules]({{ '/#modules' | relative_url }}).

If you are planning to move from paper, our [30-day plan for moving from paper job cards to digital]({{ '/blog/paper-job-cards-to-digital-30-day-plan/' | relative_url }}) shows how to start one zone at a time. Indian MSMEs looking at support for digital adoption can also read the [Digital MSME scheme guidelines](https://dcmsme.gov.in/CLCS_TUS_Scheme/Digital_MSME_Scheme/Scheme_Guidelines.aspx) from the Office of the Development Commissioner (MSME), and check eligibility with that office directly.

## Your next step

Take last month's figures for one busy part number. Write the quantities from each register in a table like the one above, and count how many gaps have no written reason. That number shows how much of your month-end is guesswork.

If you would like to see how your own month-end figures would look in Athena, [book a demo]({{ '/#demo' | relative_url }}).
