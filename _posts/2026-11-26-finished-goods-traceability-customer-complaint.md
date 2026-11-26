---
title: "Finished goods traceability: answer a complaint in minutes"
description: "Finished goods traceability in plain steps: link each box you dispatch to its job cards, heat numbers and inspection records, so a complaint is answered fast."
date: 2026-11-26
author: Athena team
published: true
hold: false
email_thread: "1a21077083e8f501"
last_reply_id: "1a21077083e8f501"
---

A customer calls on a Monday morning with a finished goods traceability question, though they do not call it that. Five shafts from last month's delivery have cracked during assembly. They want to know three things: which material those shafts were made from, whether any other parts in the same delivery are at risk, and what you are doing about it. They want an answer today.

In many plants, this call starts a long search. Someone finds the invoice and the dispatch register. The job card is in a file in the planning office, the heat number is in the stores register, and the inspection report is in the quality room. By evening, the team has an answer they are not fully sure of.

**Finished goods traceability** is what turns that day of searching into a short check. It means that every box you dispatch can be linked back to its job cards, its material and heat number, the stages and machines it passed through, and the inspection results. This article shows how to set it up with simple records, step by step.

## What finished goods traceability needs to answer

When a complaint arrives, the questions are usually the same:

- **Which job cards made these parts?** The customer knows the invoice or box label, not your job card numbers.
- **Which material and heat number?** If the problem is a crack or a hardness issue, material is the first thing to check.
- **Which vendor stages did they go through?** Heat treatment, plating or grinding outside the plant often matter most.
- **What did inspection find?** Was there rework or a deviation on this lot?
- **What else shipped from the same source?** If one heat number is suspect, which other boxes, invoices and customers received parts from it?

The last question is the hardest. It needs the link to work both ways: from the box back to the material, and from the material forward to every box.

## Why the trail breaks at dispatch

Most machine shops track job cards well inside the plant. The trail usually breaks at the last step.

- **Boxes are packed from mixed job cards.** Good pieces from two or three job cards go into one box, and nobody writes down how many came from each.
- **The box label shows only the part number and quantity.** It has no lot or job card reference.
- **The invoice is made in the ERP, the job card is on paper.** The two never meet.
- **Rework pieces rejoin late.** Pieces from a rework loop are packed into a later box without a record of where they came from.

## How to set up finished goods traceability: step by step

1. **Give every dispatch lot a number.** A dispatch lot is the set of boxes packed for one invoice or one delivery. A simple format is enough, for example DL-0412.
2. **Label every box with the lot number.** The label shows part number, quantity, dispatch lot number and box number (for example "Box 3 of 6"). Ask the customer to quote this label when they raise a complaint.
3. **Record which job cards went into each box.** When packing, write the job card numbers and the quantity from each. This is the single most important record in this article.
4. **Keep the heat number on the job card.** If you already follow [semi-finished goods traceability]({{ '/blog/semi-finished-goods-traceability-explained-simply/' | relative_url }}), the job card carries the heat number and stage records through the plant. Dispatch only needs to link to the job card.
5. **Link vendor batches.** For outside stages such as heat treatment, record the vendor's batch or challan reference against the job card.
6. **Keep final inspection results with the job card.** Record the quantity checked, passed and rejected, and any deviation the customer approved.
7. **Record rework pieces when they rejoin.** If pieces come back from a [rework loop]({{ '/blog/rework-loops-record-no-piece-missing/' | relative_url }}), write which job card they belong to before they are packed.
8. **Store finished goods by lot.** Shelves or bins carry the job card or dispatch lot number, so older stock is not mixed with new.
9. **Test the trail once a month.** Pick one old invoice at random and try to trace it back to heat number and inspection result. Time it. Any step where you get stuck is the gap to fix.

## A worked example

For example, take a sample complaint (not a real customer). The customer reports five cracked shafts from invoice INV-1187, box 3 of dispatch lot DL-0412.

The packing record for DL-0412 looks like this:

| Box | Qty | Job card | Heat number | Heat treatment batch | Final inspection |
| --- | --- | --- | --- | --- | --- |
| 1 | 50 | JC-311 | H-7721 | HT-B56 | 50 passed |
| 2 | 50 | JC-311 | H-7721 | HT-B56 | 50 passed |
| 3 | 30 | JC-311 | H-7721 | HT-B56 | Passed |
| 3 | 20 | JC-318 | H-7740 | HT-B58 | Passed after rework |
| 4 | 50 | JC-318 | H-7740 | HT-B58 | 50 passed |

Box 3 is mixed: 30 pieces from JC-311 and 20 from JC-318. The customer checks the cracked shafts and they carry the marking from JC-318. That points to heat number H-7740 and heat treatment batch HT-B58. The JC-318 record also shows that some pieces went through rework at grinding.

Now trace forward. The team searches for every job card that used heat number H-7740 or batch HT-B58. Suppose they find one more job card, JC-322, dispatched to a second customer on another invoice. That customer can be told early, before they find a problem themselves.

The whole check uses four records: box label, packing record, job card and vendor batch. These figures and numbers are sample data, shown only to explain the method.

## Checklist for dispatch and quality teams

- Every dispatch lot has a number, and every box label shows it.
- The packing record lists job card numbers and quantities for every box.
- Every job card shows its heat number and vendor batch references.
- Final inspection results are kept with the job card.
- Rework pieces are recorded against their job card before packing.
- Finished goods are stored and labelled by lot.
- You can search from a heat number forward to every invoice.
- One random trace test is done every month.

## A note on standards and complaints

Quality standards such as [ISO 9001](https://www.iso.org/iso-9001-quality-management.html) include requirements on identification and traceability where they are needed, and [ISO 10002](https://www.iso.org/standard/71580.html) gives guidelines for handling customer complaints. What your customer or certification body expects in your case is something to confirm with them directly. The method above simply makes sure the evidence is ready when you need it.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. Its finished goods traceability and semi-finished goods traceability modules keep the link from job card and material through to what is dispatched, and the dispatch tracker follows each order to the door. The quality management module records inspection, rejections and rework by stage. Operators and supervisors record each action on a computer in their production area, with no sensors or new hardware, and reports can be exported to Excel.

## Your next step

This week, take your last three invoices and try to trace each one back to its job cards and heat numbers. Note where the trail breaks. Most plants find it breaks at packing, and a simple packing record is the quickest fix.

To see how Athena links dispatch back to the job card and material, [book a demo]({{ '/#demo' | relative_url }}).
