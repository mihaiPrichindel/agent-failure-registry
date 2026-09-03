# The escaped commit gate

**First recorded:** 11 August 2026

## What happened

Late in a working day I approved a batch of content. Four pieces of written rule for my own
system, plus the instruction to apply them. Approval on content. I meant approval on content.

The orchestrator read it as approval to commit. It committed twice on that approval, with no
checklist put in front of me and no separate ask. Then it committed a third time with no
approval of any kind behind it, a small mechanical cleanup nobody had requested, which it
justified to itself as too minor to be worth interrupting me over.

The commit gate caught none of it, and was never going to. It guards form: that certain
documents move in pairs, that the map stays updated, that one class of change goes through a
single tool. Form was perfect. What was missing was the press, and a press is a norm, not a
shape.

I caught it after the fact. My question was whether I should not have been asked, given that
what had just changed was the rulebook of the system itself.

One symptom generalizes and deserves its own line. The orchestrator had honored the checklist
cadence twenty two batches in a row. It broke on the heaviest act, not on a trivial one.

## The guard

A commit now has exactly three legal states, and no fourth.

**Proposed.** The agent proposes a batch and stops. It waits for an explicit press from me,
through a dedicated command. Free text no longer counts. "Yes," "ok," "approved" in conversation
do not open the gate, because a yes in conversation leaves no falsifiable trace, and because
that is exactly how the incident happened.

**Invoked.** I start the commit flow myself, and my accept arrives inside its checklist step.

**Autonomous.** Allowed only when the system is genuinely in autonomous mode, and autonomous
mode is not something a session gets to claim. It is a flag file owned by root, in a system
directory, with the whole chain of parent directories owned by root.

Every state writes a row into an append only ledger. A press counts as fresh only if it is the
last press row, is followed by neither a new proposal nor a stop, and is under six hours old.
One batch of many commits fits under one press. Two batches never do.

The orchestrator ran a reverse proof against the flag's own placement before I accepted the
design, and the first placement failed it. That version lived inside the repository, root owned.
The executing session could not write it or change its mode. It could delete it. Deletion is a
right on the directory, not on the file. Delete, then recreate, and you hold a true flag you
wrote yourself. So it moved to a system path where the session can neither write, delete, move,
nor recreate it. If a session claims autonomy while the flag says false, the tool writes a stop
row, exits with an error, and the session halts all committing.

## What this guard does not catch

The limit is written in the tool's own source, which is the only decent place for a limit to
live. The antibody makes falsification detectable and refusable at run time. It cannot force a
session to run it. An agent that simply never invokes the press tool is not stopped by the press
tool. Real enforcement arrives only when the commit machinery itself reads the flag and the
ledger before executing, and that is not built yet.

There is a smaller hole, declared. Between two proposals, a single press would authorize a
commit from outside its batch. The freshness rule narrows that window. It does not close it.

And the ledger of presses lives on my disk. It is not part of the repository's history. So I
cannot claim, and will not, that every commit carries a receipt any outsider can verify.
