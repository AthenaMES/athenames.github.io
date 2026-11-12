---
title: "One computer per production area: shop floor data entry setup"
description: "A simple, low-cost setup for shop floor data entry: one shared computer per production area. Where to place it, who uses it, and how to keep entries on time."
date: 2026-11-13
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-13
email_thread: "1a1cd841e97caa54"
last_reply_id: "1a1cd841e97caa54"
---

When a factory decides to move from paper to a screen, the first question is often about hardware. Do we need a tablet for every operator? A screen on every machine? Sensors and cables? For most machine shops in India and other growing economies, the answer is much simpler: **one computer per production area** is enough for good **shop floor data entry**.

This sounds almost too basic. But many digital projects fail not because the software is wrong, but because the entry point is in the wrong place. The computer sits in the supervisor's cabin, far from the machines, and entries are made at the end of the shift from memory. The result looks digital but behaves like a paper register.

This article explains how to set up one shared computer per production area so that operators actually use it, entries happen close to the work, and the data can be trusted.

## Why one shared computer works

A machine shop is usually organised in areas: cutting, turning, VMC or HMC, grinding, heat treatment handover, inspection, packing and dispatch. Each area has a few machines and a small group of operators who already work as a team.

A shared computer in each area fits this pattern:

- **It is close to the work.** An operator can walk a few steps, record the quantity or a stop, and go back to the machine.
- **It keeps cost and maintenance low.** A handful of computers is easier to buy, protect and support than one device per person.
- **It creates a habit.** When everyone in the area uses the same screen, entries become part of the routine, like the old register on the table.
- **The supervisor can see it.** Missing entries are noticed during the shift, not at month-end.

In practice, one computer can usually serve the operators of about four machines. If machines are spread out, or one area runs many short jobs with frequent changes, you may need a second one.

## How to set up shop floor data entry, step by step

### 1. Draw your production areas

Take a plan of the shop floor and mark each area. Group machines that are near each other and run related stages. Count the machines in each group. If a group is larger than about four machines, or the walk to the computer is long, split it.

### 2. Choose the spot for each computer

Good places have four things in common:

1. Within a short walk of every machine in the area.
2. Away from coolant splash, chips and direct heat.
3. Visible to the supervisor during the shift.
4. Near a stable power point, with space for a small table or wall mount.

Avoid placing it inside a closed cabin. If the operator has to open a door and wait, entries will slip to the end of the shift.

### 3. Protect the hardware simply

You do not need expensive equipment to start. A standard desktop or mini PC, a keyboard and mouse, and a screen are enough. Protect them with a simple enclosure or cabinet, a keyboard cover against oil and dust, and a small UPS so a power dip does not lose an entry. Keep the screen at standing height so operators do not need to sit down.

### 4. Plan the network

Each area computer needs a reliable link to the server, whether the server is in your plant or in the cloud. Test the connection at the exact spot before you fix the computer there. Thick walls, metal racks and large machines can block wireless signals, so a cable may be the better choice in some areas.

### 5. Decide who enters what

Write down, for each area, who records each action:

- **Operator:** job card started, quantity produced, stops and their reasons, tool changes.
- **Inspector:** OK, rejected and rework quantities.
- **Supervisor:** splits, transfers to another machine, sending material to a vendor.

Our [job card checklist]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) lists the fields to capture at each stage.

### 6. Make entries quick

Operators will use the computer only if each entry takes very little time. Keep the screen simple. Use pick lists for stop and rejection reasons instead of free text. Set up labels in the language your operators read most easily.

### 7. Agree on when to enter

Fix clear moments for entries: when a job starts, when a stop happens, and when a job or lot is completed. "At the end of the shift" is too late, because people forget stops and small rejections.

### 8. Give each person their own login

Even on a shared computer, each user should log in with their own name. This shows who made each entry and builds responsibility. Keep logins simple, and log out after each entry.

## A worked example

For example, take a sample machine shop (not a real plant) with 14 machines in five areas:

| Area | Machines | Computers | Who uses it |
| --- | --- | --- | --- |
| Cutting | 2 band saws | 1 | 2 operators, stores helper |
| CNC turning | 4 lathes | 1 | 4 operators, setter |
| VMC | 3 machines | 1 | 3 operators |
| Grinding and deburring | 3 machines, 1 bench | 1 | 4 operators |
| Final inspection and packing | 1 table | 1 | 2 inspectors, packer |

That is five computers for 14 machines. In the CNC turning area, the computer stands on a wall mount between lathe 2 and lathe 3, about ten steps from each machine. An operator records "job card JC-3105 started" at 8:10, a 25-minute stop for "waiting for insert" at 10:40, and 120 pieces completed at 1:30. The supervisor sees the stop on the same screen and arranges inserts for the next job before it happens again.

Before this setup, the same information reached the office the next morning, written in a register, without the stop.

## Common mistakes to avoid

- **Putting the computer in the office.** Entries become end-of-shift guesswork.
- **Asking for too many fields.** Start with quantity, stops and rejections. Add more later.
- **Sharing one login.** Nobody knows who entered what.
- **Skipping training at the spot.** Train each operator at the actual computer, on a real job card.
- **Removing paper on day one.** Run paper and screen together for a short period in one area, then move to the next.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. It is designed for exactly this setup: no IoT, no sensors and no new hardware, with operators and supervisors recording each action on a computer in their production area, usually one computer shared by the operators of about four machines. Quantities, stops and tools recorded at the machine feed OEE and reports, and labels, stop reasons and messages can be set up in your team's own language. Implementation includes process mapping, hands-on training role by role on the shop floor, and go-live zone by zone. You can see all [Athena modules]({{ '/#modules' | relative_url }}).

## Your next step

Print a plan of your shop floor this week. Mark your production areas, count the machines in each, and choose one spot per area using the four rules above. If you want the wider picture first, read our guide on [how to digitise shop floor records without IoT or sensors]({{ '/blog/digitise-shop-floor-records-without-iot-sensors/' | relative_url }}).

If you would like to see how this would work in your plant, [book a demo]({{ '/#demo' | relative_url }}).
