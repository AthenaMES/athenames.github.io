---
title: "Heat number traceability from bar to dispatch, on a budget"
description: "Heat number traceability on a small budget: tag bars at receiving, carry the heat number through cutting and every stage, and link it to the box you dispatch."
date: 2026-11-27
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-27
email_thread: "1a2159f7ba404a21"
last_reply_id: "1a2159f7ba404a21"
---

Every bar of steel that enters your plant comes with a heat number. It is printed on the mill test certificate and often stamped or painted on the bar itself. It tells you which melt the steel came from, and so which chemistry and properties it should have.

The trouble starts the moment the bar is cut. The cut pieces do not carry the stamp. The offcut goes back to the rack with no mark. Two weeks later, a supervisor looks at a bin of turned parts and cannot say which heat they came from. **Heat number traceability** is the habit of keeping that link alive, from the bar at the gate to the box at dispatch.

You do not need expensive equipment to do this. Paint markers, metal tags, a simple register and a job card that has a field for the heat number will take you most of the way. This article shows how to build the chain link by link.

## Why heat number traceability matters

The heat number is the one record that connects your parts to the steel mill's test results. When something goes wrong, it is often the first question asked.

- **A customer complaint about cracks or hardness.** The first check is usually the material, and that needs the heat number.
- **A suspect material lot.** If a supplier warns you about one heat, you need to find every part made from it, inside the plant and already shipped.
- **Customer audits.** Many buyers ask to see that you can trace a finished part back to its material certificate.
- **Mixed material on the rack.** Two grades that look the same can be swapped by mistake. A visible heat number on every bar and offcut makes this much harder.

Mill test certificates for steel are often issued to [EN 10204](https://knowledge.bsigroup.com/products/metallic-products-types-of-inspection-documents?version=standard), the standard that defines types of inspection documents for metallic products. Which certificate type you need is set by your customer or drawing, so confirm it with them. Whatever the type, the certificate is only useful if you can match it to your parts.

## Where the chain usually breaks

In most machine shops the heat number is recorded well at receiving. The gaps come later.

1. **At cutting.** The bar is cut into blanks and the heat number stays with the stub, not the blanks.
2. **With offcuts.** Remnants go back to the rack unmarked and are used later for a different job.
3. **When lots are split or mixed.** Blanks from two heats go into one bin or one job card.
4. **At vendor stages.** Parts go out for heat treatment and come back in the vendor's crates with only the vendor's challan.
5. **At packing.** The box label shows part number and quantity, but nothing links it back to the job card.

Each break needs one simple record to close it.

## How to build the chain, step by step

1. **Check the certificate at receiving.** Match the heat number on the mill test certificate with the marking on the bars. If they do not match, quarantine the bars and ask the supplier.
2. **Write it in the stores register.** Record date, supplier, grade, size, heat number, quantity and certificate number. Keep the certificate in a file sorted by heat number.
3. **Mark every bar.** Use a paint marker or a punched metal tag at one end. Some plants also add a paint colour code for grade, which helps people see mix-ups from a distance.
4. **Issue material against a job card.** When stores issues bars for cutting, write the heat number on the job card and the job card number in the stores register. This is the link that matters most.
5. **Mark offcuts before they go back.** Every remnant gets the heat number and grade written on it with a paint marker. An unmarked offcut is scrap until someone proves what it is.
6. **One heat per job card.** If a job needs more bars than one heat can supply, open a second job card or split the job card so each part carries a single heat number. Our article on [split lots]({{ '/blog/split-lots-track-40-of-60-pieces/' | relative_url }}) shows how to keep the quantities right.
7. **Tag the bin, not only the paperwork.** Each bin or trolley of blanks carries a tag with job card number and heat number. The tag moves with the parts from stage to stage.
8. **Record vendor batches.** When parts go to a heat treater or plater, write the job card and heat number on the challan, and record the vendor's batch number against the job card when they return.
9. **Link the box to the job card at packing.** Write job card numbers and quantities for each box. From the job card you can reach the heat number. Our article on [finished goods traceability]({{ '/blog/finished-goods-traceability-customer-complaint/' | relative_url }}) covers packing records in detail.

## A worked example

For example, here is sample data for an order of 200 flange bolts (not a real customer or order). The plant receives 20 bars of 32 mm round in one grade, in two heats.

**Stores register (receiving):**

| Date | Grade | Size | Heat number | Bars | Certificate no. |
| --- | --- | --- | --- | --- | --- |
| 03 Nov | Sample grade A | 32 mm | H-5512 | 12 | MTC-881 |
| 03 Nov | Sample grade A | 32 mm | H-5530 | 8 | MTC-882 |

**Material issue:**

| Job card | Part | Qty | Heat number | Bars issued | Offcut returned |
| --- | --- | --- | --- | --- | --- |
| JC-421 | Flange bolt | 120 | H-5512 | 6 | 1 piece, marked H-5512 |
| JC-422 | Flange bolt | 80 | H-5530 | 4 | 1 piece, marked H-5530 |

Both job cards go through turning and threading, then out to a heat treatment vendor. The vendor's batch numbers are recorded on return: JC-421 in batch HT-71, JC-422 in batch HT-72. At packing, box 1 and box 2 hold 60 pieces each from JC-421, and box 3 holds 80 pieces from JC-422.

Three weeks later, suppose the supplier writes to say heat H-5530 may have a problem. The supervisor opens the stores register, finds H-5530 was issued only to JC-422, and sees one offcut still on the rack. JC-422 went into box 3 only. The check takes a few minutes, and only one box and one offcut need attention.

All numbers, grades and references above are sample data, used only to show the method.

## Low-budget checklist

- Mill test certificate checked against bar marking at receiving.
- Stores register with heat number and certificate number for every receipt.
- Every bar and every offcut marked with heat number and grade.
- Heat number written on the job card when material is issued.
- One heat number per job card, or a split job card for each heat.
- Bin tags with job card and heat number at every stage.
- Vendor batch numbers recorded against the job card.
- Packing record linking each box to its job cards.
- One trace test a month: pick a heat number and find every part made from it.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its semi-finished and finished goods traceability modules keep the link from job card and material through each stage to what is dispatched, and the subcontracting module records send and receive at vendor stages. Splits and rework are recorded as steps, so pieces stay linked to their job card. Operators record each action on a computer in their production area, with no sensors or new hardware, and you can see how the modules fit together on the [modules page]({{ '/#modules' | relative_url }}).

## Your next step

Walk to your material rack today and count the offcuts with no heat number on them. That number tells you where to start. Mark them or set them aside, then add a heat number field to your job card if it does not have one.

When you want to see how the whole chain can live in one system, [book a demo]({{ '/#demo' | relative_url }}).
