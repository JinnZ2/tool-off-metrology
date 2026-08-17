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

### 1. Two numbers or none — and say which kind of gap it is

The catalog's own principle, as a design constraint. Any threshold
measured here reports two numbers or none: trained carriers and naive
controls, with the gap as the finding. A single-population number
reproduces exactly the failure the catalog names. [obs → rule]

Second half of the same rule, from the catalog's standing counter-case
— a measured group difference can be either of two things, and they
are not distinguishable without objective instrumentation:

```
threshold difference   the instrument itself performs differently
reporting difference   the instrument performs the same and the
                       attention, vocabulary or willingness to
                       report differs
```

The konenki case is the worked warning: a large, robust, replicated
cross-cultural difference in reported hot flashes that moved with
diet and biomedicalization over twenty years, and vanished when the
Hilo study measured skin conductance instead of asking. [lit]

Design consequence, and it is not a caveat: **every protocol here that
compares trained carriers to controls must have an objective readout,
not a report.** A protocol whose dependent variable is what the
operator says cannot tell the two apart, and will find the effect
either way. Where a design does use self-report — G1-a's prediction
step — the report must be the *predictor* and something instrumented
must be the *outcome*.

### 1b. Name the axis the training targets, before testing it

A trained population exceeds baseline on the axis it trains and can
look identical to untrained on an adjacent one. So a trained-vs-control
protocol must state, in advance, which axis the training is supposed to
move — or state that it does not know.

The worked failure is in the catalog at G2: long-trained meditators,
~4,947 hours, tested on cardiac beat-counting under pharmacological
amplification, null at every dose. Read as "the training does not
sharpen interoception." Read against what the tradition actually
trains — decoupling the *response* from the content, not the content
signal — the null lands on an axis nobody claimed. [lit]

Applied to the protocols here: A1-c, A2-a and A3-a all compare trained
carriers to controls, and each must name its axis before running.
A1-c's axis is fault detection, not field sensitivity in general.
A2-a's is defect discrimination through a tool, not tactile acuity.
A3-a's is flux detection at low differentials, not thermal comfort.
Write it down; a null on an unnamed axis is unreadable afterward.

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

### 7. For anything in the open tier, transduce before hunting

The catalog's resolution path, as a design rule. A vibrotactile
magnetic-north belt worn for seven weeks produced a reported new sense
of spatial perception in 8 of 9 wearers — and the finding is explicit
that it was *not* perception of the magnetic field, but differentiated
changes in the perception of space. [lit]

Two uses here, and they are different:

```
as capability   if the goal is a person who can use field
                information, the device is the answer and no receptor
                needs to exist
as control      if the goal is to test an unaided reading, the belt
                is the positive control that separates "this field
                information is usable by a human at all" from "this
                person reads it unaided"
```

It is also the cleanest positive demonstration of rule 1b: a real
capacity was gained, on a different axis than the label claimed.

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

**what this protocol is for, in catalog terms.** A1 currently sits in
`mechanism-open`, which is a state rather than a verdict, and this
experiment is what moves it:

```
a candidate channel confirmed        → real-quantified
the reading runs on a channel other
  than the one it was told as        → misidentified-mechanism
no channel survives the design       → back to A1-a. the reading is
                                       established by use, so a
                                       four-way null means the design
                                       missed the channel, not that
                                       the reading is absent
```

The third row is the one to write down beforehand. It is the outcome
most likely to be read as a debunk and it is the one that says least.

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

**framing — do not lose this one.** The defensible mechanism is graded
prefrontal impedance under chemical load (Arnsten 2009). The pop
"amygdala hijack" version is rejected (LeDoux; Pessoa & Adolphs), and
a positive result here will be *offered* that framing by anyone
summarizing it. Graded, not seized. The catalog's Column C flags this
as a landmine and it is one at write-up time, not at design time. [lit]

**cost.** Low apparatus, high discipline. Weeks of logging.

### C-d. Does the spec's split differentiate Frijda, or conflate him?

```
claim          amplitude and impedance are two axes corresponding to
               two transitions Frijda kept distinct — not one axis
               he already had
```

**design.** Rides on the C-a and C-b logs at no extra cost. Code every
reading twice:

```
amplitude    did it cross into overt action?
             (Frijda's readiness → action)
impedance    did it degrade the concurrent secondary task?
             (the spec's signal → stack corruption)
```

**discriminator.** Dissociation. A reading that crossed into action
without degrading the secondary task — or degraded it without crossing
into action — is evidence the axes separate. Neither case appearing
across a long log is evidence they are one thing.

**null says.** Perfect co-occurrence means the spec has one axis under
two names, and Frijda's single graded control-precedence covers it.
That simplifies the spec rather than breaking it, and the spec should
say so rather than keeping a distinction the log did not support.

**cost.** Zero beyond C-a and C-b.

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

---

## G — the gap log

The catalog's G-entries are named absences rather than instruments.
Two of them can be attacked directly. The other two cannot be attacked
by this repo at all, and that is a finding about the protocol rather
than an obstacle to it.

### G1-a. Differential channel sensitivity across the neurosteroid axis

```
claim          neurosteroid state shifts the RELATIVE sensitivity of
               sensory channels, and a trained operator can predict
               which channel is up and which is down before measuring
```

**design.** Within-subject and longitudinal — one cycle minimum,
three better. Each session:

```
1  anchor the session to time-since-wake. the wake-cycle axis is
   validated, faster and larger, and will otherwise swamp this one
2  operator logs the PREDICTION first — an ORDERING across channels
   plus a direction per channel, not a single "sharper today"
3  then measure, using the catalog's own quantified instruments as
   the readout: A3 palm-radiometry threshold, A2 tool-mediated
   discrimination, plus a standard auditory or visual threshold as a
   channel the practice makes no claim about
4  salivary assay where affordable, cycle-day where not
```

**the second axis, from dim24.** Cortisol and the neurosteroid axis do
not add; they multiply. Cortisol alone did nothing to GnRH pulsatility
in ovariectomized ewes, and fell 70% with estradiol and progesterone
co-administered — the same stressor lands differently depending on
where the neurosteroid axis sits. [lit, animal]

Design consequence: salivary cortisol is sampled alongside, and the
analysis carries an interaction term rather than treating stress as
noise to control away. A design that regresses sensitivity on the
neurosteroid gradient alone will attribute an interaction to the main
effect and get the shape of the curve wrong. Log stressors as events,
not as a covariate mean. [inf]

Scope kept attached: the direct pulse-causality work is ewe, monkey
and mouse. Human evidence is correlational plus exogenous-glucocorticoid
studies, with proof-of-mechanism only at the extreme (functional
hypothalamic amenorrhoea). Use the coupling to shape the design; do not
predict an effect size from it. [lit]

**sampling — the part dim23 changes.** The driver is the *rate of
change*, not the level. [lit:high] A design that bins sessions into
three or four cycle phases cannot see a rate, and will average across
exactly the transition that carries the signal. Sessions must be
daily or near-daily, and dense through the luteal decline where the
kinetics differ most between people. The analysis variable is the
derivative, not the level.

**analysis — the second thing dim23 changes.** Gain is *altered*, and
can inverse across the range: less sensitive at low doses, more at
luteal-range and above, with paradoxical worsening. [lit:high] A model
that fits "sensitivity rises with X" will miss a sign change and score
it as noise. The analysis has to allow non-monotonic response, and the
prediction has to be recorded in a form that can be wrong in that way
— which is why step 2 asks for direction per channel rather than a
scalar.

**discriminator.** Does the *ordering* in the prediction match the
ordering in the measurement, above chance? Not "was the operator
sharper today" — that is the performance frame, and the performance
frame is the one that already came back null.

**why this design satisfies the counter-case.** Cross-cutting rule 1
requires an objective readout wherever trained capacity is claimed.
Here the self-report is the predictor and the instrumented threshold
is the outcome, so a pure attention-and-reporting difference cannot
produce a match — the operator's report has to track something a
radiometer and a probe can measure. That structure is what separates
this from the konenki failure mode. [inf]

**why the existing null does not settle this.** A scalar performance
index averages across channels. If one channel rises while another
falls, the average moves toward zero and a study looking for
worse-today finds nothing while a real differential shift runs
underneath it. That is a residual in the framework's own sense — the
aggregate measure hides the structure — and it is structurally the
same failure §4 documents for FCE, where the instrument measuring the
assumed cause had no predictive power over the outcome. [inf]

**null says.** No prediction/measurement match kills the
read-as-instrument claim, which is the claim at issue. It leaves the
neuroendocrinology untouched — that stands on its own literature and
never needed this.

**confounds.**

```
expectancy   the operator knows their cycle day and the prediction is
             not blind to it. this is exactly why the measurements
             must be objective and the prediction recorded BEFORE
             them, by procedure rather than by intention
wake axis    validated, faster, larger. anchor or lose the signal
life         sleep, load, illness. log them — they are the first
             alternative explanation anyone will offer, and they will
             be right to offer it
borrowed     every effect size in this literature comes from
magnitudes   symptomatic samples. use it for the VARIABLE — gradient,
             not level — and not for how big the effect should be in
             a healthy carrier. importing a magnitude from a disorder
             sample is how a null gets called a failure
```

**a note on what not to copy.** Schmidt 1998 established the premise
by suppressing the axis with GnRH and adding hormones back. That is
the causal design and it is the reason the premise is solid — and it
is pharmacological, invasive, and entirely wrong for a healthy carrier
reading their own instrument. Cite it for the premise. Do not model
the protocol on it.

**cost.** Low apparatus, high discipline, months. Carrier-bound.

### FM-a. The field modifier, tested as a modifier

The catalog's compound field-modifier entry states why isolation
testing returns null: strip the other channels to test this one
cleanly and you have removed the thing being measured. Its
discriminator follows from that, and it is a good one. This adds the
part that makes it separable from the obvious alternative.

*(ID provisional — this is the one catalog entry with no number. It
needs one.)*

```
claim          readings on the OTHER channels shift with local field
               structure, in a long-resident trained holder
```

**design.** Same holder, on and off Precambrian shield terrain, other
channels intact — and a magnetometer logging actual local field
gradient and variance at every site. Orientation and spatial-judgment
tasks run at each.

**discriminator — and this is the whole design.** Not the terrain
comparison. Shield-vs-not is confounded with everything about a place:
topography, vegetation, sound, sightlines, weather, and above all
familiarity, since long residence is a stated precondition. A
place-level effect is exactly what plain familiarity predicts.

What familiarity does not predict is covariation with a magnetometer
reading the holder cannot see. So the test is the *within-site*
correlation between measured field structure and the holder's readings,
at novel locations inside each terrain type. That converts a place
comparison into a dose-response and leaves familiarity with nothing to
explain.

**positive control, from the catalog's own resolution path.** Run the
vibrotactile belt on the same holder. If the belt-delivered field is
usable and the unaided reading is not, that separates "field
information is usable by this person" from "this person reads it
unaided" — which is the actual question, and neither arm alone answers
it. [inf]

**null says.** No covariation with measured field structure means the
reading is not tracking the field. It does not kill the reading — the
entry claims a modifier on other channels, and a modifier could be
tracking terrain structure through topography, acoustics or light
without any field component. That would move the entry toward
misidentified-mechanism, which is a tier the catalog has and now has an
occupant for.

**confounds.** Familiarity, above. Season and weather across a
multi-site protocol. The holder's own knowledge of which terrain they
are on — unavoidable, and the reason the discriminator is the
within-site correlation rather than the between-terrain difference.

**cost.** Moderate: travel, a magnetometer, a belt. Carrier-bound —
the entry specifies a holder born and raised in the terrain.

### G2 is closed — what that leaves

The catalog closes G2: the vedanānupassanā mapping is real, it is
structural rather than thematic, and it lands on the response axis.
There is no search left to run there, and this document should not
pretend otherwise.

Two things survive as work:

```
the female-monastic lead   the textual traditions that carry the
                           mapping are largely male-monastic and
                           celibate — richly mapped on the daily
                           axis, structurally near-blind to the
                           slower one. that lead is untouched by the
                           closure and rolls into the G3 search
                           below                              [lead]
the quarantined candidate  G2's continuous-spatial-percept
                           possibility — that a trained observer's
                           percept is of distribution or extent
                           rather than a count, and so scores as
                           absence on a counting task. filed with
                           magnetoreception, not catalogued as
                           working, and testable only after G4-a
                           produces a task that is not a count [open]
```

The second is worth one line of design attention because it is
cheap once G4-a exists: if the percept is of the wrong *shape* for
the task, a discrimination or localization measure should show the
difference the counting task missed. Khalsa's own study already found
a body-map localization difference it was not looking for. That is a
lead, not a result. [inf]

### G3-a. Where to look, and what would count

Not experiments. Searches — and a search needs a stopping rule and a
criterion as much as an experiment needs a null.

```
claim          calibration knowledge of the neurosteroid axis is
               described somewhere in a trained-perceiver tradition
```

**scope, corrected.** The earlier version of this claim added "and
reads as absent because of who did the documenting." dim27 does not
support that as a premise — it supports it as one possible explanation
among others, and the search has to be able to come back empty without
that explanation absorbing the result. Search first. Explain after.

**do not walk these.** Refuted as historical carriers and struck from
the lead list: the contemporary Red Tent movement (invented tradition,
1997 novel, the author says so herself), the generic Goddess-milieu
"moon lodge" (modern pan-Indian syncretism), and menstrual synchrony
as supporting folklore (the largest dataset found cycles diverging).
Anyone searching this area will meet all three early and they look
like leads. [lit]

**search the tribally-specific, never the category.** This is dim27's
operative instruction and it changes the unit of search. "Menstrual
seclusion" is not one object — documented instances carry opposite
purposes, and the best hormone-verified case in the record (Strassmann's
Dogon work) is read by its own investigator as paternity surveillance
rather than rest or instruction. A search run at category level will
average real practices with invented ones and with a case that points
the other way.

**what would count as positive**, roughly strongest first:

```
living carrier says so, unprompted, to an open question — strongest,
  and the only route that does not depend on what got written
community's own publication says so. the Wabanaki material is a
  community/revival publication, not an outsider ethnography. read
  what communities have published about themselves before reading
  what was published about them
vocabulary residue — terms for states or timings with no documented
  practice attached. a language keeps words for what it used to do
outsider description with unexplained structure — a schedule read as
  taboo by the ethnographer that tracks something physiological they
  were not tracking
```

**one inference dropped.** The earlier version listed "prohibition
residue — a rule against X implies X." Keep the first half and lose
the second: a documented rule is evidence of the *behavior* and not of
its *meaning*, which is exactly the distance the Dogon case measures.
Seclusion is well attested there and the calibration reading is not
what it was for. [lit]

**what would count as negative** — two tests, and the second is new:

```
1  traditions where women DID hold the pen. bhikkhunī literature,
   Christian women contemplatives, women's Hindu and Jain ascetic
   writing. if the axis is absent there too, the who-held-the-pen
   explanation fails and something else is going on.

2  the best-documented case, read directly. Frisbie 1967 on Kinaaldá
   is 400+ pages with song texts and a top primary-data rating. if
   calibration content is absent from an ethnography that thorough,
   "undocumented rather than absent" is much weaker than a thin
   record makes it look.
   caveat that cuts the other way: Kinaaldá is a first-menses
   puberty rite, not a cyclic practice. absence of a cyclic
   calibration axis in a non-cyclic rite is weak evidence about a
   cyclic axis. run the test, then discount it accordingly.
```

**null says.** An empty search bounds the search, not the question —
same discipline as Q1. State where you looked, state that you stopped,
and do not keep searching for an absence. Note that this null is now
easier to reach honestly than it was, because the scope correction
above removes the explanation that used to absorb it.

**cost.** Desk work, plus someone who reads the source languages. The
`[lead]` tags in the catalog are load-bearing here: none of those
traditions is attested to hold this, and the search is what would
change that.

### G4-a. Invalidity, or inversion?

G4 says the heartbeat-counting task rewards norm-knowledge over
sensing. That claim has two strengths and the catalog states the
stronger one:

```
INVALIDITY  the task measures something other than interoception
            — established. arithmetic passes it, expectation
            predicts it at r=0.78, strict instructions halve
            scores, and the three standard tasks disagree with
            each other                                     [lit:high]
INVERSION   the task ranks a true perceiver BELOW a non-perceiver
            who knows population norms — not established. it
            follows from the mechanism, and following from a
            mechanism is not the same as being measured    [inf]
```

The difference matters to this repo specifically. §1's detector list
is a list of *inversions*, not of bad instruments, and the two carry
different weight. One measured comparison settles it.

```
claim          heartbeat-counting score ranks interoceptive
               accuracy backwards once norm-knowledge is measured
               alongside it
```

**design.** Three measures on the same participants:

```
a  a discrimination task — judge whether a tone train is
   synchronous with own heartbeat. cannot be passed by counting
   or by estimating from a known rate, which is the point
b  knowledge of own resting heart rate, asked directly and
   checked against measurement
c  the standard heartbeat-counting task
```

**discriminator.** Regress c on a and b. Invalidity predicts b
dominates and a contributes little. Inversion predicts something
stronger and rarer — a negative partial for a, meaning that among
people matched on norm-knowledge, the better perceivers score *worse*.
Then look directly at the corner cases: high-a/low-b against
low-a/high-b, and see which the standard task ranks higher.

**null says.** No negative partial means invalidity without inversion.
The `[lit:high]` on the inversion framing in §1 comes down to `[inf]`
and the detector list keeps its count rather than gaining one.

Stated at the field's landing, not past it: the catalog's own dim25
correction says the counting task is *compromised*, not broken —
Zimprich 2020 reanalyzed the critique's data and argued much of the
defect is an artifact of correlating ratio variables, and the field
settled on don't-abandon-don't-trust, prefer discrimination and
phase-adjustment tasks. So a null here does not license "the objective
channel is unusable." It licenses "this task is a poor measure and the
better ones are the ones this design already uses." [lit]

**confounds.** The discrimination task has its own literature and its
own critics; it is better than counting, not clean. Report which
variant and its own reliability rather than treating it as ground
truth.

If this design is ever extended to a *training* effect rather than a
group difference, Murphy & Bird 2025 is the checklist: seven distinct
mechanisms all present as improved interoceptive accuracy and only one
is a genuine perceptual gain — attentional cueing, labelling,
perceptual boosting by breath-holding or muscle tensing, learning the
task mapping, heart-rate knowledge, composite-measurement confounds,
and reduced anxiety lowering heart rate. It also explains the
Meyerholz d=1.21 vs Rominger preregistered d=0.15 split: counting-task
gains survive, discrimination-task gains vanish. Any training claim
must be measured on a task unaffected by rate knowledge, which is the
same requirement this design already imposes for a different reason.
[lit]

**cost.** Low. Standard psychophysiology kit, one session per
participant, no carrier dependency — this is the one protocol here
that anyone could run.

### C-e. Detecting out-of-range operation

The catalog now gives Column C an operating range and a failure
regime, which it previously lacked. The failure is overshoot: the
trained operation decouples response from content, the dose-response
is non-monotonic, and past a point the decoupling runs into
depersonalization and anhedonia — adverse-event prevalence around
8.3%. More training makes the reading worse. [lit]

```
claim          past a threshold of response decoupling, readings stop
               resolving to actions — and that is detectable by the
               spec's own criterion rather than by a clinical one
```

**design.** Rides on the C-b log. Code each reading for whether it
resolved to an action or to a label, and plot that rate against
cumulative practice within-subject and across subjects at different
practice volumes.

**discriminator.** A rising noun-output rate at high practice volume
is out-of-range operation. The spec already says a noun output means
the instrument was not used; this applies that criterion to a dose
axis.

**null says.** Flat noun-rate across practice volume means either the
overshoot does not occur in this population or the spec's criterion
does not detect it. The two are not separable by this design alone,
and saying so beforehand keeps a flat result from being read as
safety.

**this one is not only a measurement.** Unlike everything else in this
file, the phenomenon under study is a documented adverse outcome. A
protocol that observes it must have a route out — someone to refer to,
a stopping rule, and no incentive to keep a subject in the condition
to complete the dose curve. Observational only; do not induce.

**cost.** Rides on C-b. The care costs more than the measurement.

### What G4 does and does not do to the Column C protocols

G4 says there is no instrument capable of testing a content-field
claim: the objective side rewards arithmetic, the report side rewards
credentialed vocabulary. That is a real problem and it lands unevenly
on the protocols above.

```
C-a  survives. the outcome is a behavioural secondary task, and the
     gain rating is the predictor. same structure as G1-a — a
     vocabulary effect cannot produce a match against an
     instrumented outcome
C-b  survives, and for a reason worth naming. the outcome is the
     ACTION TAKEN, not a report about a feeling. the spec's own
     verb-not-noun rule is what makes this measurable, and it
     sidesteps the report-channel failure that the interoception
     literature is stuck in                                    [inf]
C-c  rides on C-b, same footing
C-d  rides on C-a and C-b, same footing
```

That is a genuine methodological advantage and it should not be
oversold. The spec solves the *report* channel by resolving readings
to actions. It does nothing for the objective channel, where G4's gap
is untouched — nothing here measures whether the reading corresponds
to an internal state at all, only whether it predicts what the
operator then does.

Cross-link: B2-d is the relevant test of the render-target half of
G4's report-channel argument. If verbal rendering loses most detail,
then a questionnaire is close to the worst available instrument for a
non-verbal store, and the interoception field has been using nothing
else. [inf]

### Standing constraint — no neural substrate

Do not attach the spec or the panel to an anatomical seat. The insula
version is already disposed of: bilateral insula, ACC and amygdala
destruction left pain affect, emotion and self-awareness intact
(Feinstein 2016), and anterior insula activation accompanies anything
salient, so it discriminates nothing. [lit:high]

This is a standing constraint rather than a protocol because the
temptation arrives at write-up, when a behavioural result wants a
mechanism attached to make it feel solid. The result is the result.

### The constraint that changes the design

This repo's frame is that naming moves a practice off the carrier
clock. For G2 and G3 that premise does not straightforwardly hold, and
the difference is structural rather than procedural.

```
restricted        some traditions restrict transmission by
knowledge         initiation, sex, or kin. documenting it is not
                  neutral preservation — for that tradition it can
                  be the exact harm the restriction exists to prevent

extraction        a catalog entry is an extraction unless the carrier
                  community decides it is not. "cataloguing is the
                  first move off the clock" is a claim the frame
                  makes, and it is made from outside

whose question    the difference between asking a community what they
                  hold and asking them to fill a gap in your catalog
                  is visible from their side even when it is not
                  visible from yours
```

Practical consequence: G2 and G3 are the only items in this document
that should not be run by this repo alone. They need someone inside
the tradition, and the correct outcome may be that the knowledge is
confirmed to exist and is deliberately not written down here. That is
a successful result, not a failed one.

dim27 makes this concrete rather than abstract. The documented cases
are Navajo and Wabanaki — living communities, and in the Wabanaki case
the source is the community's own 2025 publication. That is a
community already speaking about its own practice, on its own terms
and its own schedule. The first move is reading what they chose to
publish, not arriving with a question about a gap in someone else's
catalog.

The tension with the catalog's frame is real and is left standing. The
naming-is-the-intervention case was built on proprioception, where
nobody owned the sense and no one was harmed by its being named. It
does not transfer unexamined to knowledge somebody's grandmother held
under a rule about who gets told. [open]

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
whether the G3 structural finding is right. G2/G3-a searches for the
  knowledge; it does not test the claim that documentation and
  capacity came apart on a particular axis. that claim is about the
  historical record and would need a historian's instrument, not a
  psychophysical one
```

---

## Tags

Everything in this document is `[inf]`: proposed, not run. Numbers and
effects carried from literature are marked `[lit]` at the point of
use. When a protocol is run, its *result* becomes `[obs]` — the design
does not.
