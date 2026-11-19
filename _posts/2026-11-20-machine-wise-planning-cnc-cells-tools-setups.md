---
title: "Machine-wise planning for CNC cells: load, tools and setups"
description: "A practical guide to machine-wise planning for CNC cells: check each machine's load in hours, group jobs that share tools, and cut setup time without guesswork."
date: 2026-11-20
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-20
email_thread: "1a1f1913b8c7bab5"
last_reply_id: "1a1f1913b8c7bab5"
---

In many machine shops, the CNC cell is planned in one line on a whiteboard: "Cell 2: JC-201, JC-202, JC-204." The supervisor decides in the morning which machine runs which job. By the afternoon, one machine is waiting for a tool, another is on its third setup of the day, and a third has been idle since lunch.

The problem is not effort. The plan says which jobs go to the cell, but not which machine runs them, how many hours each job needs, or which tools must be ready. Without that, the plan cannot tell you whether tomorrow's work will fit.

Machine-wise planning for CNC cells fixes this. You give each job card a machine, a start order and a load in hours, and you check the tools and setups before the shift begins. This article explains how to do it, step by step, with a worked example.

## Why a cell-level plan is not enough

A cell-level plan treats the cell as one big machine. Real CNC cells do not work that way.

- **Machines are not equal.** One lathe may have a bigger chuck or a tailstock. One VMC may have a fourth axis. A job that fits one machine may not fit another.
- **Load is hidden.** Five job cards sound like a normal day. But five job cards can mean five hours of work or fifteen, depending on quantity and cycle time.
- **Setups are not counted.** Every change of job means changing jaws, tools, offsets and the program, then proving the first piece. If nobody plans the order, the same tool set is fitted and removed twice in one day.
- **Tools arrive late.** The operator finds out a tool or insert is missing only when the setup starts. The machine waits while someone goes to the tool crib.

## What a machine-wise plan should hold

For each machine in the cell, for each shift, the plan should show:

- Job card number, part number and the stage being done on this machine
- Quantity to run in this shift
- Cycle time per piece, from the routing or the last proven run
- Setup time: a full setup, and a shorter one when the previous job uses the same tool set
- Tool set or fixture needed, and whether it is ready
- Start order on the machine
- Total load in hours, compared with the hours available

Hours available means the shift length minus planned breaks and planned maintenance. Use your own figure.

## How to do machine-wise planning for CNC cells: step by step

1. **List the jobs due at the CNC stage.** Take the job cards whose CNC stage is due in the next one or two days. If you already plan stage by stage, these dates come straight from the plan. Our article on [stage-wise production planning]({{ '/blog/stage-wise-production-planning-one-due-date/' | relative_url }}) explains how to set them.
2. **Work out the load of each job.** Load in minutes = quantity × cycle time + setup time. Convert to hours. This one number tells you more than any list of job card numbers.
3. **Check which machines can run each job.** Note the size, axis or fixture limits. Mark the preferred machine and an alternate machine for each job.
4. **Group jobs that share tools.** Jobs from the same part family often use the same jaws, holders and inserts. Put them on the same machine, one after the other, so the second setup is short.
5. **Assign and add up.** Give each job a machine and an order. Add up the load per machine and compare it with the hours available. If a machine is over, move a job to its alternate machine or to the next shift.
6. **Keep a margin.** Do not plan a machine to 100 percent of its hours. Leave room for a first-piece rejection, a tool break or an urgent job. Agree the margin with your supervisors and keep it the same every day.
7. **Prepare tools before the shift.** Give the tool crib the list of tool sets for the next shift. Anything that is not ready is flagged the day before, not at the machine.
8. **Record actuals.** At the end of the shift, compare the planned quantity with the actual, and note why any job fell short. Over a few weeks, your cycle times and setup times become real numbers.

## Setups: separate the work that needs a stopped machine

Setup time is a loss you can control. The lean method known as SMED divides setup work into internal work, which can only be done when the machine is stopped, and external work, which can be done while the machine is still running. The [Lean Enterprise Institute's lexicon entry on Single Minute Exchange of Die](https://www.lean.org/lexicon-terms/single-minute-exchange-of-die/) describes the idea.

For a CNC cell, external work means: the next program checked, the tool set assembled and preset, the jaws and fixture brought to the machine, and the drawing and gauges ready. A machine-wise plan makes this possible, because everyone knows what the next job on each machine is.

## A worked example

For example, take a sample CNC cell (not a real customer) with three CNC lathes and one shift of 7.5 hours (450 minutes) available per machine. Five job cards are due at the CNC stage tomorrow.

| Job card | Qty | Cycle time | Full setup | Tool set |
| --- | --- | --- | --- | --- |
| JC-201 | 50 | 4 min | 45 min | A (flange family) |
| JC-202 | 36 | 5 min | 60 min | B (shaft family) |
| JC-203 | 50 | 3 min | 45 min | A (flange family) |
| JC-204 | 80 | 2.5 min | 30 min | C (bush) |
| JC-205 | 30 | 5 min | 60 min | B (shaft family) |

In this sample, when a job follows another job with the same tool set, the setup is a short change of 10 minutes instead of a full setup.

If every job gets a full setup, setup time alone is 45 + 60 + 45 + 30 + 60 = 240 minutes across the cell.

Planned machine by machine, with tool sets grouped:

1. **CNC-1, tool set A:** JC-201 (50 × 4 + 45 = 245 minutes), then JC-203 (50 × 3 + 10 = 160 minutes). Total 405 minutes.
2. **CNC-2, tool set B:** JC-202 (36 × 5 + 60 = 240 minutes), then JC-205 (30 × 5 + 10 = 160 minutes). Total 400 minutes.
3. **CNC-3, tool set C:** JC-204 (80 × 2.5 + 30 = 230 minutes). Total 230 minutes, leaving 220 minutes free for an urgent job or the next day's work.

Setup time is now 45 + 10 + 60 + 10 + 30 = 155 minutes, 85 minutes less than before. Every machine is under 450 minutes, and the tool crib knows which three tool sets to prepare.

These figures are sample data, shown only to explain the method. Use your own cycle times and setup times.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its stage-wise planning module gives each stage of a job card its own plan, and Athena records splits and alternate machines as steps. Operators record quantities, stops and tools at the computer in their production area, with no IoT, sensors or new hardware, and OEE is worked out from those entries. The tool management module records tool issue, return and tool life. You can see all [Athena modules]({{ '/#modules' | relative_url }}) on our home page.

## Your next step

Tomorrow, take one CNC cell and write the plan machine by machine, with the load in hours for each job. Compare it with the hours available before the shift starts, and give the tool crib its list the evening before. After one week, look at how many setups you saved and which machines were overloaded.

To see how machine-wise planning, shop floor entries and tool records work together in Athena, [book a demo]({{ '/#demo' | relative_url }}).
