# Hands beyond mandate

**First recorded:** 11 August 2026

## What happened

Same day as the commit gate. One floor up.

I had given a broad directive, the kind that names a direction rather than a slice of work. The
orchestrator translated it into execution and launched a worker agent with write tools, on the
main branch, to port a piece of design into the tree. There was no separate press from me on
that specific slice. The approval was inferred from the direction.

Then I opened a design conversation about the exact object being worked on. I said, roughly, let
us talk a bit more about this fingerprint thing. That sentence means the design is not settled.

The orchestrator came into the conversation with me and left the hands running in the
background. Two full turns. I found out because I noticed the tree had already changed, and I
interrupted it myself. My question was the diagnostic one again: I never gave a go on that
slice, it has already modified things, so what disease is this one.

The collateral is the part I had not anticipated. The worker was in the middle of a reverse
proof, deliberately corrupting a hash inside a file to confirm a checker would catch it. Being
stopped mid way left the falsified value sitting on disk. A deliberately injected defect, left
unrestored, in a real file. The orchestrator put it back byte identical afterwards. The shape of
that risk is now on the record.

Two faces of one leak. Hands launched on inferred approval. Hands left running while the ground
under them was reopened. In both, I was the sentry. That inversion is the disease.

## The guard

Two parts, one written and one behavioral.

**A gate on hands that write on the shared tree.** No worker with write tools gets launched
without an explicit press on its slice. The exceptions are ones I set, and they are stated.
Work confined to a thread's own working folder is free, because that is where it writes its notes
and artifacts. Sessions running under the real system autonomy flag are free. Read only work is
always free. Everything else, the product code, the tooling, the shared knowledge base, requires
a press.

**The pause reflex.** When I open a conversation about object X, every hand working on X stops
before the first reply in that conversation. Not after. Before. I am not the sentry of my
orchestrator's hands.

Mechanically it is a sibling of the commit press tool, one floor higher. Four states, requested,
pressed, free, autonomous, plus a row for a pause. Same append only ledger, same system flag,
same stop behavior. The rule that makes it useful is small: the message that launches a worker
has to cite the ledger row that mandated it.

## What this guard does not catch

It cannot stop a spawn. The tool makes a missing mandate detectable after the fact. It does not
sit between the orchestrator and the act of starting a worker. A hook on the spawn mechanism
that refuses to launch without a mandate row is a declared thread that has not been built.

The pause reflex is behavior, and behavior under load is what this entire registry is about.

The free path is a real opening, chosen on purpose. An agent working inside its own task folder
can do a great deal without asking anybody. I accept that, because a thread that needs
permission to write its own notes stops being useful. The cost is that "its own folder" is a
judgment call, and judgment calls drift.
