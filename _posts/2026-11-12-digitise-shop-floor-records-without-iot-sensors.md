---
title: "How to digitise shop floor records without IoT or sensors"
description: "You do not need sensors or machine connections to digitise shop floor records. A practical guide to moving job cards, stops and rejections to a screen."
date: 2026-11-12
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-12
email_thread: "1a1c85eec9a9bb79"
last_reply_id: "1a1c85eec9a9bb79"
---

Many factory owners want to **digitise shop floor records**, but stop when they hear what it seems to need: sensors on every machine, PLC connections, gateways, new cables and a long project. For a machine shop with a mix of old manual lathes, a few CNC machines and a vendor network, that sounds expensive and risky.

The good news is that most of the value does not come from the machine. It comes from the people who already write the job card, the production register and the rejection slip. If those same people record the same facts on a screen instead of on paper, you get searchable, joined-up records from day one.

This article explains what you can digitise without IoT or sensors, what you give up, and a simple step-by-step way to start.

## Why sensors are not the first step

Sensors are good at one thing: telling you whether a spindle is turning and how many cycles it ran. They cannot tell you which job card is on the machine, why it stopped, whether the pieces passed inspection, or which vendor has the next stage.

Those are the questions a plant head, planner or quality head actually asks every day. The answers live in people's heads and on paper. So the real gap in most plants is not machine data. It is a lack of clean, joined-up records of what people already do.

There are also practical reasons to start without hardware:

- **Mixed machines.** Older manual and conventional machines often have nothing to connect to.
- **Cost and time.** Hardware, wiring and integration take budget and months before anyone sees a report.
- **Ownership.** When operators make the entries, they own the data and learn to trust it.
- **Vendor stages.** Heat treatment, plating and grinding at a subcontractor happen outside your plant. No sensor in your shop can see them.

## What you can digitise with simple operator entries

Almost everything on your paper job card and registers can move to a screen:

1. **Job card start and finish** at each stage, with machine and operator.
2. **Quantity** received, OK, rejected, sent for rework and still pending.
3. **Stops** with a reason from a short fixed list (setup, no material, tool change, breakdown, waiting for inspection).
4. **Tools** issued and returned, with the job they were used on.
5. **Inspection results** and rejection reasons by stage.
6. **Splits and rework**, recorded as separate lots or steps.
7. **Vendor stages**: quantity sent on challan, quantity received back, due date.
8. **Dispatch**: what left the plant, against which order.

Our [job card checklist]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) lists the fields for each stage in more detail.

## What you give up, honestly

Operator entries are not the same as machine signals. Short stops of a minute or two will often go unrecorded. Cycle counts depend on the operator entering the quantity, not on a counter. Timings are as accurate as the moment the operator presses the button.

For most growing machine shops this is a fair trade. A stop of 40 minutes for "no material" matters far more than a 90-second pause, and only a person can tell you the reason. You can always add machine connections later, on the machines where they make sense, once your records are clean.

## A step-by-step way to start

### Step 1: Map one zone on paper first

Pick one production area, for example the CNC turning cell. Walk the floor with the supervisor and write down every record that is kept today: job card, register, rejection slip, tool book. Note who writes each one and when.

### Step 2: Decide the few things every entry must have

Keep it short. Job card number, stage, machine, operator, quantity OK, quantity rejected, and stop reason. If an entry needs more than a minute, operators will skip it.

### Step 3: Fix the lists before you start

Agree on a short list of stop reasons and rejection reasons with the supervisors. Write them in the words operators already use, in their own language if needed. Long lists with vague items like "other" make the data useless.

### Step 4: Put one computer where the work happens

A shared computer in the production area, close to the machines, works better than a computer in the office. Operators should not need to walk far or wait for a supervisor to type for them.

### Step 5: Train at the machine, role by role

Train operators on their own entries only, at their own machines, with real job cards. Train supervisors separately on checking and correcting entries. Short sessions over a few days work better than one long classroom session.

### Step 6: Run paper and screen together for a short time

For the first one or two weeks, keep the paper register as a backup. Each day, the supervisor compares the two. Once they match, stop the paper in that zone.

### Step 7: Review the data every day

Use the entries in the daily production meeting from the first week. When people see their own entries used to solve problems, entry quality improves quickly. Then move to the next zone.

## A worked example

For example, take a turning cell with four CNC machines and one shared computer (sample data, not a real plant). On one shift, the operator of machine T-03 makes these entries for job card JC-3105, a batch of 120 flange bushes:

| Time | Entry |
| --- | --- |
| 07:10 | Start JC-3105, stage: turning OP10 |
| 08:05 | Stop: tool change (insert worn) |
| 08:20 | Resume |
| 10:40 | Stop: waiting for inspection approval |
| 11:15 | Resume |
| 14:30 | Quantity: 96 OK, 4 rejected (undersize bore), 20 pending |
| 14:35 | Tool returned, insert issued for next shift |

No sensor was used. Yet by the end of the shift, the supervisor can see that 35 minutes were lost waiting for inspection, that 4 pieces were rejected for one clear reason, and that 20 pieces are still pending on this stage. The planner knows the job card is not ready for the next stage. On paper, the same facts would be spread across a register, a rejection slip and a tool book, if they were written at all.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. It needs no IoT, no sensors and no new hardware: operators and supervisors record each action on a computer in their production area, usually one computer shared by the operators of about four machines. OEE is calculated from those operator entries, and splits, rework, alternate machines and vendor delays are recorded as steps. Labels and stop reasons can be set up in your team's own language, and go-live happens zone by zone with hands-on training at the machine.

If month-end is where paper hurts most today, read [why paper production registers fail at month-end]({{ '/blog/why-paper-production-registers-fail-month-end/' | relative_url }}) for a closing checklist you can use now.

## Your next step

Choose one zone and list every paper record kept there today, with who writes it and when. That list is your starting point for going digital without any new hardware.

If you would like to see how operator entries become shop floor reports in Athena, [book a demo]({{ '/#demo' | relative_url }}).
