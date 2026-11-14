---
title: "Writing stop reasons that operators will actually use"
description: "A practical guide to writing machine stop reasons operators will actually pick: a short list, plain words, their language, and a monthly review of Others."
date: 2026-11-15
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-15
email_thread: "1a1d7d10efa0ab31"
last_reply_id: "1a1d7d10efa0ab31"
---

Every machine shop knows the feeling. The machine stood for forty minutes, the register says "stop", and nobody can say why. Or the stop reason column says "Others" on half the lines. When a factory starts recording stops, on paper or on a screen, the quality of the **stop reasons** decides whether the data is useful or just noise.

The problem is rarely the operator. It is usually the list. A list written in the office, with forty codes, technical words and two options that mean nearly the same thing, will not be used well at the machine. People pick the first option, the vague option, or nothing.

This article shows how to write stop reasons that operators will actually use: short, clear, in their language, and tied to the action someone will take.

## Why stop reasons matter more than stop minutes

Recording that a machine stopped tells you there is a loss. Recording why it stopped tells you who can fix it. "Waiting for material" goes to stores or the cutting section. "Waiting for setter" goes to the supervisor. "Insert breakage" goes to the tool room.

Stop reasons are also the base of availability in OEE. The Lean Enterprise Institute describes OEE as a measure built from availability, performance and quality losses ([Lean Enterprise Institute: Overall Equipment Effectiveness](https://www.lean.org/lexicon-terms/overall-equipment-effectiveness/)). If the reasons are vague, you can calculate a number, but you cannot act on it.

## What goes wrong with most stop reason lists

- **Too many options.** Operators scroll past what they cannot read quickly and choose something near the top.
- **Office words.** "Unplanned maintenance event" means little on the floor. "Machine breakdown" is clearer.
- **Overlapping reasons.** "No material" and "Material shortage" and "Waiting for RM" split one problem three ways.
- **A big "Others" option.** It is the easiest choice, so it becomes the most common.
- **No owner.** Nobody reviews the list, so it never improves.

## How to write stop reasons, step by step

### 1. Start from real stops, not from a template

Before writing anything, look at what actually stops your machines. Take two weeks of paper registers or supervisor notes and list every stop with a short description. Group them. Often, a few causes take up most of the stop time. Those are the reasons that must be easy to find.

### 2. Keep the list short

Aim for about 10 to 15 reasons for operators in one area. If you need more detail, use two levels: a group (for example "Tool") and a reason inside it (for example "Insert breakage", "Tool not available"). An operator should find the right reason in a few seconds.

### 3. Use the words people say on the floor

Write each reason the way an operator would say it to the supervisor. "Waiting for setter", "Waiting for inspection", "Power cut", "Drawing not clear". If your team speaks Hindi, Marathi, Tamil, Bengali, Bahasa or Swahili on the floor, write the reasons in that language too. A reason they can read at a glance is a reason they will pick.

### 4. One reason, one owner

Each reason should point to one person or team who acts on it. If a reason has no clear owner, it will not lead to action. This also helps you spot overlaps: two reasons with the same owner and the same fix can usually become one.

### 5. Separate planned stops from losses

Lunch, tea breaks, planned maintenance and "no plan for this machine" are not the same as breakdowns. Keep them as separate reasons so they do not hide real losses, and agree in advance which ones count as planned time.

### 6. Put "Others" on a short leash

Keep an "Others" option, because some stops are new. But ask for a few words of description when it is used, and review those entries every week. If the same description appears again and again, it deserves its own reason.

### 7. Review the list once a month

Sit with one supervisor and one operator from each area for 30 minutes. Look at the most used reasons, the least used reasons, and the "Others" entries. Add, merge or rename. When you change a reason, tell the operators at the machine, not by circular. Our guide on [training operators who have never used software]({{ '/blog/train-operators-never-used-software/' | relative_url }}) explains how to do short, task-by-task sessions.

## A worked example

For example, take a sample CNC turning area (not a real plant) with four machines. The first stop list, written in the office, had 32 reasons. After two weeks of real stops, the supervisor rewrote it as 12 reasons in six groups:

| Group | Stop reason (as written on screen) | Owner |
| --- | --- | --- |
| Material | Waiting for material | Stores |
| Material | Wrong material or size | Cutting section |
| Setup and tools | Setup or changeover | Setter |
| Setup and tools | Waiting for setter | Supervisor |
| Setup and tools | Insert or tool breakage | Tool room |
| Setup and tools | Tool not available | Tool room |
| Machine | Machine breakdown | Maintenance |
| Machine | Power cut | Maintenance |
| Quality | Waiting for first piece inspection | Quality |
| Quality | Drawing or program not clear | Planning |
| Planned | Break or shift change | (planned) |
| Other | Others (write a few words) | Supervisor |

In the first week of using it, the sample area records the following stops on one machine in one shift:

| Time | Minutes | Reason |
| --- | --- | --- |
| 08:40 | 25 | Setup or changeover |
| 10:15 | 15 | Waiting for first piece inspection |
| 12:30 | 30 | Break or shift change |
| 14:05 | 20 | Waiting for material |
| 15:50 | 10 | Others: coolant low |

Out of 100 minutes of stops, 30 are planned and 70 are losses, each with a clear owner. The "Others" entry is coolant. If coolant appears several times in the weekly review, it becomes a reason of its own under "Machine".

## Common mistakes to avoid

- **Copying a long list from another plant.** Their stops are not your stops.
- **Changing reasons every week.** Review monthly so the data stays comparable.
- **Blaming operators for "Others".** It usually means a reason is missing.
- **Recording stops at the end of the shift.** Memory fades. Record at the time, at the machine. Our article on [digitising shop floor records without IoT or sensors]({{ '/blog/digitise-shop-floor-records-without-iot-sensors/' | relative_url }}) covers how this works with operator entries.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Operators record quantity, stops and tools at the machine, on a computer in their production area, and OEE is calculated from those entries, with no IoT, sensors or new hardware. Labels, stop reasons and messages can be set up in the team's own language. During implementation, the team maps your process in detail and trains each role on the shop floor. You can see the full list of [Athena modules]({{ '/#modules' | relative_url }}).

## Your next step

This week, take two weeks of stop records from one area and write them as a list of 10 to 15 reasons, each with an owner, in the words your operators use. Try it on one machine for a week and review the "Others" entries on Friday.

If you would like to see how stop reasons are recorded in Athena, [book a demo]({{ '/#demo' | relative_url }}).
