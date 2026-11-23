---
title: "Rework loops: recording them so no piece goes missing"
description: "How to record rework loops on the shop floor: tag every rework piece, link it to its job card, re-inspect it and balance quantities so nothing goes missing."
date: 2026-11-24
author: Athena team
published: false
hold: false
auto_publish_on: 2026-11-24
email_thread: "1a2062a8d7025eec"
last_reply_id: "1a2062a8d7025eec"
---

Eight pieces fail inspection after grinding. The inspector marks them "rework" and puts them in a red crate. The operator who can fix them is busy on another job, so the crate waits. Two days later it is moved to make space. A week later, nobody can say which job card those eight pieces came from.

This is how **rework loops** swallow pieces. The rework itself is usually simple: re-grind a diameter, remove a burr, correct a thread. The trouble is that the piece leaves the normal route, and on paper there is no clear way to follow it out and bring it back.

Most plants record rework as a note in the margin of the job card, or a line in the quality register that nobody links back to production. This article shows a simple method to record rework loops so that every piece is either back on its route, rejected with a reason, or clearly waiting somewhere.

## Why rework loops lose pieces

When pieces go missing in rework, the causes are usually the same.

- **The job card moves on without them.** The good pieces go ahead with the card. The rework pieces stay behind with a chalk mark or a slip of paper.
- **Rework is recorded in a different book.** Quality writes it in the rejection register. Production writes nothing. The two books never meet.
- **Nobody owns the rework crate.** The inspector found the problem, the operator will fix it, and the supervisor plans the machine. Each assumes someone else is following it up.
- **Reworked pieces skip re-inspection.** The piece is corrected and sent straight on, so nobody confirms the fix worked.
- **Rework is counted as good output twice.** A piece produced, rejected, reworked and produced again can appear twice in the output figures if the loop is not recorded.
- **Repeat rework is invisible.** If the same defect comes back every week, nobody sees the pattern because each case lives on a separate slip.

## The basic rule: rework is a step, not a note

The simplest way to record rework is to treat it as a proper step on the route, with its own quantity in and out. The balance rule from our article on [tracking split lots]({{ '/blog/split-lots-track-40-of-60-pieces/' | relative_url }}) applies here too:

> At every stage, pieces in = pieces passed + pieces sent to rework + pieces rejected + pieces still at the stage.

And for the rework loop itself:

> Pieces sent to rework = pieces reworked and passed + pieces reworked and rejected + pieces still in rework.

If either line does not balance, a piece is missing. A supervisor can check both in a few minutes per job card.

## How to record rework loops: step by step

1. **Record the defect at the moment it is found.** Write the job card number, the stage, the quantity, the defect (for example "OD oversize") and who found it. Use a short, fixed list of defect names so the same problem is always written the same way.
2. **Give the rework pieces their own tag.** If the job card is JC-204, the rework part can be JC-204/R1. The tag travels with the crate and always shows the parent job card number, material and heat number.
3. **Decide the rework route.** Which machine or operator will correct it, and which stage it returns to. Some rework goes back one stage; some needs a different machine. Write it down, do not leave it as a verbal instruction.
4. **Give the rework a due date and an owner.** One person follows the crate until it is closed. Without a date, rework waits behind every new job.
5. **Re-inspect after rework.** Every reworked piece is checked again before it rejoins the route. Record the result: passed, rejected, or needs a second rework (for example JC-204/R1-2).
6. **Record the return.** When pieces pass, write how many rejoin the main lot and at which stage. Do not let them join a different job card or heat number without a record.
7. **Count output once.** Production output should count good pieces finished at a stage, not every attempt. Record rework hours separately, because they use machine time.
8. **Close the job card only when every piece is accounted for.** Dispatched, rejected with a reason, or clearly waiting in a named rework step.
9. **Review repeat defects every week.** List rework by defect, stage and machine. The same defect appearing again is a process problem to fix at its root, not a rework job to keep repeating.

## A worked example

For example, take a sample job card (not a real customer): JC-204, 80 flanged bushes, one heat number. The route is cutting, turning, drilling, grinding, final inspection and dispatch.

At final inspection after grinding, 9 pieces fail: 7 for an oversize outer diameter and 2 for a bore with a visible mark. The supervisor sends the 7 to rework as JC-204/R1 and the 2 as JC-204/R2. After re-grinding and re-inspection, 6 pass and rejoin the lot. One piece is still oversize and becomes JC-204/R1-2 for a second rework. The 2 bore pieces are checked and cannot be saved, so they are rejected with a reason.

| Tag | Qty | Defect | Rework step | Result |
| --- | --- | --- | --- | --- |
| JC-204 (main) | 71 | None | None | Passed, dispatched |
| JC-204/R1 | 6 | OD oversize | Re-grind OD | Re-inspected, passed, dispatched |
| JC-204/R1-2 | 1 | OD still oversize | Second re-grind | Waiting, due Thursday |
| JC-204/R2 | 2 | Bore mark | Not reworkable | Rejected with reason |
| **Total** | **80** | | | |

Check the balance: 71 dispatched + 6 reworked and passed + 1 still in rework + 2 rejected = 80. Every piece is accounted for. Without the rework record, the register would show 71 dispatched and 80 started, and the 9 missing pieces would be a mystery at month-end.

These figures are sample data, shown only to explain the method.

## Checklist for supervisors and quality heads

- Every rework has a job card number, stage, quantity, defect name and the person who found it.
- Every rework crate has its own tag linked to the parent job card and heat number.
- Every rework has a route, an owner and a due date.
- Reworked pieces are re-inspected and the result is recorded.
- Returns to the main lot are recorded with the quantity and stage.
- Output counts good pieces once; rework time is recorded separately.
- Quantities balance at every stage and in every rework loop.
- Repeat defects are reviewed every week.

## A note on quality standards

Quality standards such as [ISO 9001](https://www.iso.org/iso-9001-quality-management.html) include requirements on controlling outputs that do not meet requirements, and on checking them again after they are corrected. What your customer or certification body expects in your case is something to confirm with them directly. The method above simply makes sure each reworked piece stays linked to its job card, material and inspection result. Our checklist on [what a job card should record at every stage]({{ '/blog/what-job-card-should-record-every-stage/' | relative_url }}) lists the other fields worth keeping.

## Where Athena fits

Athena is shop floor software (MES) for machine shops, built by NMTG inside an operating factory. It records splits, rework, alternate machines and vendor delays as steps, so a rework loop stays linked to its job card. The quality management module records inspection, rejections and rework by stage, and the semi-finished goods traceability module follows work in progress between stages. Operators and supervisors record each action on a computer in their production area, with no sensors or new hardware.

## Your next step

This week, walk the shop floor and find every crate marked rework or hold. For each one, write down the job card number, quantity, defect and owner. Any crate you cannot link to a job card is the first gap to close.

To see how Athena records rework loops from inspection back to the route, [book a demo]({{ '/#demo' | relative_url }}).
