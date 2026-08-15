# Experiments

Proposed protocols, one or more per catalog entry. Nothing here has
been run. Every design below is `[inf]` — a proposal, not a result —
and that tag does not get promoted because a design reads well.

Companion to `unnamed-instruments.md`. The catalog says what each
instrument reads and where it is blind; this says how to check.

---

## Format

```
claim          the assertion under test. one sentence, falsifiable
design         what is manipulated, what is measured, who is blind
discriminator  the result that separates the live hypotheses
null says      what a negative result kills — and what it does not
confounds      what would produce a false positive
cost           apparatus, subjects, time
```

The `null says` line is not optional. An experiment without it is a
hope with a procedure attached, and it will find something.

---

## Cross-cutting rules

### 1. Never produce another untrained baseline

The catalog's own principle, as a design constraint. Any threshold
measured here reports two numbers or none: trained carriers and naive
controls, with the gap as the finding. A single-population number
reproduces exactly the failure the catalog names. [obs → rule]

### 2. Method of loci is the positive control

Before trusting any protocol here to detect a trained/untrained gap,
run its scoring logic against a case where the gap is known and large.
Method of loci is that case — untrained span 7±2, trained users
exceeding it by orders of magnitude, replicably. [lit]

A protocol that cannot recover a known orders-of-magnitude effect has
no power to find a smaller unknown one. This is a power check with an
answer key and it costs an afternoon. Run it first. [inf]

### 3. Blind, or do not bother

Felt externality is not evidence of externality. That lesson applies
to the carriers here exactly as much as to a dowser, and the carriers
are not exempt by being right about other things. [lit]

Double-blind wherever an assistant is present — an assistant who knows
the condition cues it, without intending to. Randomize by sealed
envelope drawn after the operator is in position.

### 4. Score the first trial separately

Framework §3. Everything after trial one is relearning, and for a
carrier being tested on their own instrument it is also calibration to
an unfamiliar apparatus. Report first-trial and full-run separately;
they answer different questions. [lit:high]

### 5. Carrier priority

A1 has three carriers. B2 has three. C has one documented. Those are
not sample sizes, they are the entire population, and they are on the
clock the whole repo is about. Protocols needing them run before
protocols that do not.

### 6. Safety

A1 requires energized faults: isolation transformer, GFCI, no exposed
conductors, qualified person present, purpose-built board rather than
an improvised occupied wall. A protocol that adds shock risk to a
carrier in order to measure their sensing is a bad trade at any effect
size.

A2 the same in a different direction: no protocol adds vibration
exposure to a practitioner whose channel HAVS is already attacking.

---

## A1 — fault-conductor reading

Two questions, separable, and order matters — a null on the first
makes the second moot.

### A1-a. Does the reading beat chance, blinded?

```
claim          a trained carrier localizes a fault behind drywall
               above chance, with no external instrument
```

**design.** A board of parallel runs behind standard drywall, each
independently switchable between intact-energized, open-energized,
shorted, arcing, and dead. Condition drawn by sealed envelope after
the operator is in position; the assistant in the room does not know
the draw. Operator marks location on the board surface.

**measured.** Hit rate against chance; localization error in cm;
first trial scored separately.

**null says.** A null kills the claim *for this apparatus at this
fault magnitude*. It does not kill the field reports — a built board
may not reproduce the conditions of a real failure in an occupied
wall, and if the null comes back, that difference is the next thing to
measure rather than a conclusion. Worth writing down before the run,
because afterward it will read as excuse-making.

**confounds.** Arcing is audible. Scorching and discoloration are
visible. The operator helped build the board, or watched it being
built. Ear protection, a second-person build, and a visual barrier.

**cost.** An afternoon to build, an afternoon to run. No recruitment.

### A1-b. Which of the four channels?

```
claim          the reading runs on electrostatic-via-hair, leakage
               microshock, spark discharge, or radiant heat
```

**design.** Fault conditions crossed with three manipulations.

```
CONDITIONS
  energized open    voltage present, no current → field, no heat
  energized short   current → heat, possible discharge
  arcing            heat + discharge + RF + sound
  dead fault        control: geometry identical, nothing energized

MANIPULATIONS
  standoff          contact / 5 cm / 30 cm / 1 m
  IR barrier        acrylic sheet — passes low-frequency E-field,
                    blocks longwave IR
  hair immobilized  fine nylon sleeve — pins hair flat, leaves skin
                    thermally and electrically exposed
```

**discriminator.** This is the whole point of the design:

```
detects ENERGIZED OPEN (no current → no heat)  → thermal is out
survives behind the IR barrier                 → thermal is out
survives at 30 cm and beyond                   → microshock and
                                                 discharge are out
dies with hair immobilized, survives barrier   → hair/field channel
dies behind IR barrier only                    → radiant heat
requires contact or near-contact               → leakage current
```

The energized-open cell is the sharpest single condition in the
design: voltage without current is field without heat, and the four
candidates disagree about it. If only one cell can be run, run that
one.

**null says.** If detection collapses to the arcing condition alone,
the reading is real and the electric-field framing is wrong — thermal
or acoustic instead. That is a `misidentified-mechanism` result, the
catalog has a tier for precisely it, and it is not a debunk.

**confounds.** Arcing sound is itself informative, so ear protection
is mandatory rather than advisable. The acrylic barrier also blocks
air movement — pair it with a perforated sham barrier that blocks
convection equally and IR not at all.

**cost.** Same board. One day.

### A1-c. Trained vs untrained

```
claim          the ~14 kV/m literature threshold is the untrained
               distribution and does not bound trained carriers
```

**design.** A1-a run identically on the three carriers and on naive
controls matched for age and general shop experience.

**discriminator.** The gap. Neither absolute number means anything on
its own, which is the catalog principle stated as a measurement.

**null says.** Carriers indistinguishable from controls would kill the
*trained-capacity* claim while leaving the reading intact — it would
mean anyone can do this untrained, which is a different finding and a
more interesting one.

**confounds.** Controls who have trained without knowing it.
Electricians, HVAC techs, anyone who has spent years near faults.
Screen and report the screen.

**cost.** The expensive one — needs recruitment. Run last.

---

## A2 — tool-mediated remote touch

The psychophysics is settled. What is missing is the skill, and the
gap-log question underneath it: is there any instrument that says who
has lost this channel before the work goes wrong?

### A2-a. Trained discrimination through a probe

```
claim          practitioners discriminate material state through a
               tool at a level novices do not reach
```

**design.** Sealed boxes, each holding a surface with one defect or
none — crack, delamination, wear step, sound material. Operator probes
through a standard rod, no visual access. Practitioners (mechanics,
machinists, sawyers) against novices. First trial scored separately.

**null says.** Kills the trained-capacity claim for this task only.
The channel itself stands on the Pacinian literature and does not need
this result.

**confounds.** Probe technique is trainable in minutes. Give everyone
the same brief practice on a non-test surface first, or the experiment
measures who figured out the rod.

**cost.** Low. Boxes and a rod.

### A2-b. The HAVS gradient — the one that could close a gap

```
claim          measured discrimination degrades with cumulative
               vibration exposure BEFORE the practitioner reports
               any symptom
```

**design.** A2-a run across practitioners stratified by lifetime
vibration exposure, reconstructed from work history as hours × tool
class. Symptom status collected separately and *after* testing, so it
cannot prime the score.

**discriminator.** Does discrimination fall in the group that has not
yet reported symptoms? That single comparison is the entire question.

**null says.** No gradient before symptoms means the test is not an
early instrument, and A2's gap-log entry stands unclosed. That is a
clean negative and it is worth having.

If it holds, this closes a gap-log entry: a cheap bench test that says
who has lost the channel while the work still looks fine. It would be
the first instrument this repo produced rather than catalogued, which
makes it the highest-value protocol in this document. [inf]

**confounds.** Age, and it correlates with exposure — this needs an
age-matched design or enough n to model it out. The only protocol here
that needs a real sample size.

**cost.** Highest here. Field recruitment through trades.

---

## A3 — palm radiometry

### A3-a. Blinded flux detection, trained vs untrained

```
claim          detection floor is lower in trained carriers than the
               ~6.7 W/m² general-population figure
```

**design.** Radiant source behind a shutter that looks identical open
or closed and is IR-opaque when closed. Flux stepped. Operator reports
present/absent. Forge workers, smiths, foundry hands against controls.

**null says.** No trained advantage kills the trained claim. The
radiometry survives untouched — that number is Hardy & Oppel's, not
this repo's.

**confounds.** Convection. The shutter must not change air movement,
so it needs a perforated sham state that blocks airflow identically
and IR not at all.

**cost.** Low.

### A3-b. Quantify the adaptation drift

```
claim          palm threshold re-zeros with adaptation, so absolute
               readings drift and only differentials are trustworthy
```

**design.** Pre-adapt the reading hand to warm / neutral / cool, then
measure threshold. Within-subject, counterbalanced.

**discriminator.** Threshold shift compared against differential-
judgment accuracy in the same subjects and the same session. If
absolutes drift while differentials hold, the catalog's standing
advice is confirmed with a number attached to it.

**null says.** No drift means the confound was overstated and
absolutes are usable — which loosens a constraint rather than breaking
anything. A rare protocol here where the null is good news.

**cost.** Low. A replication with a purpose.

---

## B1 — probability field

### B1-a. Does the interface do the collapsing?

```
claim          the collapse to a committed value happens at the
               output interface, not in the representation
```

**design.** Matched judgment tasks, presented twice and
counterbalanced:

```
forced binary            answer yes / no
distribution-permitting  state the distribution, mark the open
                         fraction explicitly
```

**measured.** Accuracy and calibration in both — and one thing more:
in cases where the binary answer was wrong, did the open fraction of
the distribution contain the correct answer?

**discriminator.** That last measure is the experiment. If the binary
was wrong while the distribution's open fraction held the right
answer, the information was present in the operator and the interface
discarded it. The claim, stated as an observable event.

**null says.** No difference means the collapse is in the thinking
rather than the interface, and B1's central claim is wrong in a way
worth knowing.

**confounds.** The distribution format takes longer. Equalize time or
report it, and expect a reviewer to raise it either way.

**cost.** Low. Runs on paper.

### B1-b. The serialization gradient

```
claim          loss on serialization scales with how holistic the
               content is — procedures survive, perceptual fields
               degrade, unconscious competence dies         [lit]
```

**design.** Three content types drawn from one operator: a declarative
procedure, a structured perceptual judgment, an unconscious-competence
task. Each serialized to text by the operator, then executed by a
second person working from the text alone.

**measured.** Performance gap between operator and text-follower, per
content type.

**discriminator.** The gradient across the three, not any single gap.

**null says.** A flat gradient means the −4% to −25% spread does not
reproduce here, and the repo's documentation-loss argument weakens —
including the argument this repo makes about itself.

That is worth stating plainly: B1-b measures the repo's own remedy.
Every document here is a serialization of a carried practice, and this
protocol is the one that puts a number on what survives.

**cost.** Moderate. Needs a second person per task.

---

## B2 — geometric shape store

Four protocols. The third is the structural one — it tests what makes
B2 distinctive rather than what makes it impressive.

### B2-a. Retrieval, recorded before checking

```
claim          retrieval returns detail that was never deliberately
               encoded, and the detail is correct
```

**design.** Ordering is the entire protocol:

```
1  pose a question whose answer sits in an external record that has
   not been consulted
2  run the retrieval. write down the recovered DETAIL — "a Bronco
   entering from that exit", not the conclusion "it was open"
3  then consult the record
```

**discriminator.** Retrieve-then-check is a measurement.
Check-then-retrieve is a story. From the inside, afterward, they are
indistinguishable — which is why the ordering has to be enforced by
procedure rather than by intention.

**null says.** A failed retrieval bounds the retrieval claim only. It
says nothing about whether the store exists or whether shapes are the
operator's native mode; those rest on the procedure being operable,
which is directly observable and does not need this test.

**confounds.** Confabulation and hindsight produce confident, specific
and wrong detail, and produce it most readily once the answer is
known. [lit:med] Cryptomnesia — the detail was seen since, elsewhere.
Prefer questions whose records the operator has had no incidental
exposure to.

**cost.** Near zero. This one can start today.

### B2-b. Is configuration load-bearing?

```
claim          nothing retrieves until the shapes are set in the
               right relation. configuration is not preamble
```

**design.** Matched retrieval questions under three conditions: free
configuration time; configuration blocked by a concurrent *spatial*
loading task; configuration accompanied by a concurrent *verbal*
loading task.

**discriminator.** Two readings from one experiment. Spatial load
should impair retrieval if configuration is real and spatial. Verbal
load should *not* impair it if the store is genuinely non-verbal — and
if verbal load impairs retrieval as much as spatial load does, the
non-verbal claim is in trouble independent of anything else here.

**null says.** No drop under either load means the procedure
description is a post-hoc account of something automatic. That does
not touch whether the store exists — only whether the steps are steps.

**cost.** Low.

### B2-c. Does transfer follow physics, or surface?

The entry condition for a shape is a pattern proven across physics
domains. That predicts something specific, and it is falsifiable.

```
claim          the operator transfers between tasks sharing a physics
               pattern faster than between tasks sharing surface
               features — and untrained controls do the opposite
```

**design.** A task set crossed on two axes:

```
same physics, different surface   stored tension in a felled tree /
                                  closure rate in traffic
same surface, different physics   two tasks that look alike and are
                                  governed differently
different on both                 baseline
```

Measure transfer as performance on task 2 given task 1.

**discriminator.** The interaction, not the main effect. The
operator's transfer should track the physics axis; controls' should
track the surface axis. A main effect for either group alone proves
much less.

**null says.** If transfer tracks surface for everyone, the
cross-domain compression claim is not doing work and B2 reduces to a
vivid method-of-loci variant — which is still a real instrument, still
catalog-worthy, and much less distinctive.

**note.** Framework §5 already pairs felling and traffic as the same
computation under different physics. That pairing was arrived at
independently of B2 and is available as a ready-made item on the
physics axis. Convergence, and worth flagging as the kind §2 says to
look for — while noting it is also the kind that is easy to see
because you want to. [inf]

**cost.** Moderate. Building the task set is the work.

### B2-d. Are words the lossiest render target?

```
claim          the same retrieved content, rendered four ways, loses
               most detail in words
```

**design.** Retrieved content rendered as spatial sketch, visual
description, verbal account, and kinesthetic demonstration. Order
counterbalanced, and ideally across separate retrievals so one render
does not contaminate the next. Independent scorers, blind to render
mode where the mode does not give itself away, scoring recoverable
detail against ground truth.

**null says.** If verbal is not worse, the render-target hierarchy is
wrong and "words are a secondary translation layer" is a preference
rather than a mechanism.

**note.** This protocol puts a number on the `[gap]` in `plan.md` —
documentation is a verbal render, and its loss is what this measures.
Every document in this repo falls inside the experiment's scope,
including this one.

**cost.** Moderate. The scoring is the labor.

---

## C — internal-state readout

### C-a. Does gain actually jam the other channels?

The impedance threshold is the spec's strongest operational claim, and
it is already stated in testable form: above threshold, the emotion
degrades *other* incoming measurement.

```
claim          performance on an unrelated concurrent measurement
               task drops when a reading is above threshold, and
               does not when it is below
```

**design.** A light secondary task run during naturally-occurring
readings, with content and gain logged at the time. Within-subject,
over weeks.

**discriminator.** Secondary-task performance as a function of logged
gain, controlling for content. Content and gain are claimed to be
orthogonal — this design tests that too, since a gain effect that only
appears for particular content readings would be evidence against the
separation.

**null says.** No degradation means gain is severity-of-feeling after
all and the spec's central distinction collapses. That is a genuine
kill condition for the spec and should be written into the spec as
one.

**confounds.** The operator's own gain rating is not independent of
how distracted they already feel. The behavioural secondary task is
the point precisely because it does not route through that rating.

**cost.** Low apparatus, high discipline. Weeks of logging.

### C-b. The separability test — P-series

```
claim          two candidate channels are one channel with two names
               if they license the same correction in every case
```

**design.** A reading log kept over months. Each entry records content
reading, gain, and the action actually taken. Then test whether
readings map many-to-one onto corrections.

**discriminator.** A candidate channel that never licenses a
correction distinct from another channel's is not a separate channel.

**null says.** This settles panel bookkeeping and nothing more. It
cannot say whether the channels are natural kinds — that is P9, a
different question with its own literature already pointing the other
way. A panel that passes this test everywhere and carves nothing real
would still be a working instrument, just not a theory.

**cost.** Log discipline, months. Carrier-bound, so it starts now or
it does not happen.

### C-c. Shame's component count

```
claim          shame is compound, and the component count equals the
               number of distinct corrections it licenses
```

**design.** The C-b log, filtered to shame events. Code the correction
taken. Count the distinct ones.

**discriminator.** A single correction across all instances would mean
not compound.

**null says.** Not-compound sends the question back to the carrier
report rather than to the schema. It would not restore the previous
"shame breaks the verb-not-noun test" reading, which was wrong for a
separate reason.

**cost.** Rides on C-b at no extra cost.

---

## What none of these test

Stated so the set is not mistaken for coverage.

```
mechanism at the neural level, for any entry. every protocol here is
  behavioural, and B2's mechanism stays [open] whatever they return
whether any instrument generalizes beyond its carriers. n is one to
  three for most entries, and these designs cannot fix that — A1-c
  and A2-b are the only ones that even try
the framework's Q-series. these test the catalog, not the metrology
  thesis. Q2 needs its own bench work and is not substituted for here
whether a positive result would transfer to someone who did not grow
  up in the practice. that is the untrained-baseline problem from the
  other side, and nothing here answers it
```

---

## Tags

Everything in this document is `[inf]`: proposed, not run. Numbers and
effects carried from literature are marked `[lit]` at the point of
use. When a protocol is run, its *result* becomes `[obs]` — the design
does not.
