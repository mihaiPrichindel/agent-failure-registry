# The false green

**First recorded:** 9 August 2026

## What happened

Three of them in one day, all in the same corner of my system.

The definition first, because the name misleads. A false green is not a broken gate. A broken
gate is easy. A false green is a gate working perfectly, on something other than the object the
reader believes it is protecting.

**Case one.** A checking tool reported green over the second document in a series. What it had
actually done was verify the second document's lines against the anchor of the first. They
passed by accident. The bodies had not changed between the two commits, so the wrong comparison
came out right. What caught it was not the verdict. It was a small count printed beside the
verdict, saying the run had covered one document, when the series by then had two.

**Case two.** A report claimed there were zero occurrences of a forbidden form inside a
directory. True as a statement of intent. False as a sentence. Seven lines contained it. All
seven were quotations of the forbidden form, written down in order to explain it, which is
exactly why the person who wrote the check believed the claim. What caught it was reading the
lines one by one. Counting had already answered zero.

**Case three.** A sweep reported the whole registry green. Underneath, a set of rows had been
read as one kind of record when they were another, and an entire class had been silently
overwritten. What caught it was a count that failed to return to its earlier value after a
restore.

Three greens. All three caught by numbers printed next to the verdict. None caught by the
verdict.

## The guard

Two rules came out of that day, plus one law of reporting.

**Reverse proof is mandatory.** A gate does not earn trust by passing. It earns trust by being
seen failing. You break the thing deliberately, in a scratch copy, and the gate must go red. A
guard that has never been observed going red is decoration. What gets counted now is how many
gates have been proven capable of failing, not how many passed.

**Every verdict cites the version of the gate that produced it.** Without that, an old green
becomes unfalsifiable in retrospect. You cannot tell which gate said it, so you cannot tell what
it measured.

**A report must print the number from which a reader can deduce what was measured.** That last
one is the rule that changed the shape of every report here. A verdict on its own is not
falsifiable by the person reading it. All three greens that day were caught this way, so the
rule is not a preference. It is the observed catching mechanism, promoted into a requirement.

## What this guard does not catch

The reverse proof only proves a gate can fail on the defect you thought to inject. It says
nothing about the defects you did not think of.

Worse, and this is the part that keeps the entry open: a gate aimed at the wrong object will
pass its own reverse proof cleanly. Break the thing it is actually looking at, and it goes red
exactly as promised. You walk away more confident, not less. The reverse proof tests a gate's
mechanics. It does not test its aim.

And the auxiliary number only helps if somebody reads it. Everything in this pattern happens on
fast turns, where reports get read at the verdict line and nowhere else. The rule pushes the
evidence in front of the reader. It cannot make the reader slow down.
