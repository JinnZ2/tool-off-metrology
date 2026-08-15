# plan.md

Research roadmap for the open questions in `negative-space-metrology.md`
§8. For each: what it needs, what would falsify it, what it is blocked
on, and the hazard that would make a wrong answer look right.

No build plan here. The `harness/` sketch in §9 stays a sketch until a
question actually needs code — most of these do not.

Status: seed. Sequencing is a claim too, and it is `[inf]`.

---

## Sequencing rule — cost is the wrong sort order

The obvious ordering is cheap-first. It is wrong here, in one specific
way.

Desk work waits. Carrier-dependent work does not.

Any question whose evidence lives in a live carrier — a transmitted
practice, an elder operator, an undocumented method — is on a clock
that no literature question is on. A citation graph will still be there
in five years. A carrier may not be, and §6 F3 is the whole reason this
repo exists.

```
SORT KEY
  carrier-sourced evidence   → expiry, not cost. front-load regardless.
  everything else            → cost and unblocking value.
```

This applies to Q7 entries and to any Q2 / Q4 material sourced from
operators rather than from papers. [inf]

---

## Q7 — instrument-gap enumeration                          [gap] [do first]

Enumerate skills with no instrument that distinguishes competent from
absent *before* failure. The list is the finding.

```
NEEDS      a log with a fixed entry format. nothing else.
COST       near zero. additive. needs no permission and no subject.
BLOCKED ON nothing.
```

Entry format, revised — the last two fields come from
`unnamed-instruments.md`, which arrived at the same problem from the
other side and solved it better:

```
skill                what it is, in operator terms
carriers             who still has it; roughly how many; transmitting or not
failure it precedes  what breaks when it is gone, and how long after
instrument that
  would distinguish  what would have to be measurable to catch it early
search bound         where you looked for that instrument and did not find it
operating range      the regime where the skill actually applies
cannot read          what it is blind to, inside its own regime
carrier's words      the operating range in the carrier's own phrasing,
                     verbatim, recorded before any analysis of it
```

The range fields are not decoration. They separate a catalogued
instrument from a claim that works everywhere. An entry without them is
not an entry. [inf]

The verbatim field is there because of how A1 went wrong. The carrier
had stated the range correctly on first telling — "open" wire, a
"problem" — and the analysis layer imported a broader scenario,
attached it to them, and then narrowed it back as though correcting
them. Without the carrier's words on record there is nothing to check
the paraphrase against, and the entry lands in the wrong tier with the
error looking like rigor. See the provenance correction in
`unnamed-instruments.md`. [obs]

Two parallel catalogs already exist and should converge on this format
rather than being merged:

```
unnamed-instruments.md   instruments with no NAME. tiered by evidence.
sensor-panel.md          one instrument's channels, decomposed
```

Neither is the gap log. The gap log's question is narrower — no
instrument exists to distinguish competent from absent *before
failure* — and an entry can be well-named, well-characterized, and
still belong in it. A2 (tool-mediated remote touch) is the sharp case:
fully quantified, named channel, documented kill mechanism in HAVS,
and still no instrument that says which practitioner has lost it until
the work goes wrong. That is a gap-log entry with none of the
namelessness. [inf]

Seed entries already written elsewhere: the reading method in
`emotion-reading-spec.md` (household transmission, no formal name, no
external record, no instrument that prices its absence in advance), and
A2 above.

Why first: it is the only output on this list that is complete at every
moment — ten entries is a finding, forty is a better one, and there is
no half-finished state. It also forces the frame to be concrete. You
cannot write an entry without naming the failure and the missing
instrument, which is exactly where hand-waving would otherwise survive.

```
FALSIFIER  (for the frame, not the question)
  if candidate entries keep turning out to HAVE an instrument that the
  author simply did not know about, the negative-space framing is
  decoration and the gap claim is weaker than §2 states.
  the search-bound field is what makes this detectable.
```

---

## Q1 — FCE thread: has anyone connected the predictive failure to skill?

Forward-citation trace on Gross & Battie 2004 and Gross 2006. Screen
for anyone attributing functional-capacity's predictive failure to a
model/skill variable rather than to fitness.

```
NEEDS      citation-graph trace. desk work, days.
COST       low.
BLOCKED ON nothing.
UNBLOCKS   §4 → §5. whether the replacement candidate is unclaimed.
```

Decision rule, both directions:

- connection already made → read their model, adopt it or locate
  precisely where it stops. either is progress and neither is a loss.
- bounded search comes up empty → log as `[gap]`, state the bound, stop.
  do not keep searching for an absence.

```
HAZARD
  absence of citation is weak evidence and degrades fast with search
  effort. a bound stated up front ("these databases, these years,
  these terms") keeps the null honest. without it the null is just
  fatigue. [inf]
```

---

## Q5 — audit the mixedness of "critical thinking decline"      [open]

Not "does it extrapolate." What moderates it. Pull the mixed results,
code the moderators, and check two things the headline skips:

```
CONSTRUCT VALIDITY  does the horizon skill even LOAD on the instrument
                    used? if the test cannot see it, a null on the test
                    says nothing about it.
SAMPLE DYNAMICS     urban/suburban undergrad samples may be a population
                    with the variance already gone. a floor effect reads
                    as a null.
```

```
NEEDS      literature audit. desk work, weeks.
COST       low-medium.
BLOCKED ON nothing.
```

Value here is de-claiming, not claiming. It is the direct defense of the
§7 seam, applied to a claim the repo would otherwise be tempted to lean
on. The likely outcome — "the literature does not support extrapolation"
— is a finding and gets written as one. Negative results do not get
shelved for being negative; that is how the seam reopens.

---

## Q2 — measure prediction-horizon directly                  [design] [hinge]

The load-bearing question. §5 stands or falls here, and §4's
replacement candidate goes with it.

Operator states max look-away; perturb the environment at varying
delays; find where prediction breaks. Yields seconds × domain ×
experience level.

```
NEEDS      an instrument that does not exist yet. operators. a
           perturbable environment. safety review.
COST       high — the highest on this list.
BLOCKED ON nothing formally, but see the bench step.
UNBLOCKS   Q3 entirely.
```

Bench step first. Build a screen task with controllable dynamics and no
injury surface, and establish that the measurement shape works at all
before anyone goes near a yard or a road. If the shape fails on the
bench it fails in the field, more expensively and with worse
consequences.

```
CONFOUND — design against this from the start
  self-selected look-away duration may be measuring risk appetite, not
  model quality. two operators with identical horizons and different
  risk tolerance return different numbers, and the metric silently
  scores nerve as skill.
  → the honest measure is perturbation DETECTION at a delay, not
    look-away duration. run both; the gap between them is its own
    reading. [inf]
```

```
FALSIFIERS
  experts and novices show the same tolerance
    → horizon is not the discriminating variable. §5 falls.
  horizon does not decay on a clock
    → the layoff prediction falls, and the stale-model account of
      §4 loses its mechanism.
```

Note the sharp test §5 already offers and keep it: familiar work after
a layoff should be MORE dangerous than unfamiliar work. It is
counterintuitive enough that a confirmation is worth something and a
disconfirmation is cheap to read.

---

## Q3 — is horizon what alarm-based automation destroys?     [design]

```
BLOCKED ON Q2. hard block, no partial credit.
```

You cannot test the destruction of a quantity you cannot measure. Every
version of this question that does not wait for Q2 is an inference
wearing an experiment's clothes.

```
FALSIFIER   (once unblocked)
  alarm-supported operators show intact horizon on probe → the
  mechanism is wrong, whatever else automation is doing.
```

Flagged because this is the question with the most policy weight
attached, which makes it the one under the most pressure to be answered
early on inference alone. Answering it early is how §7's seam gets
written into something that matters. Wait.

---

## Q4 — do displaced practices cluster in high-variance environments?

```
NEEDS      a case set with inclusion criteria written BEFORE cases are
           gathered. otherwise you gather confirmations.
COST       medium. desk work plus carrier interviews — the interview
           portion is on the expiry clock, see sequencing rule.
BLOCKED ON nothing.
```

Hold §8's own note in front: displacement is on distribution cost, not
on performance. A practice that lost on merit is not evidence here, and
the criteria have to separate the two before the cases arrive.

```
HAZARD — survivorship, and it inflates rather than deflates
  you only hear about displaced practices somebody recorded. recording
  correlates with the practice having had a champion. champions cluster
  in exactly the marginal, high-variance environments the hypothesis
  predicts. so a positive result is consistent with a pure recording
  artifact.
  the fix is a denominator — practices displaced FROM low-variance
  environments — which is precisely what nobody logged.        [gap]
  → until that denominator exists, a positive result caps at [inf].
    write it that way or not at all.
```

```
FALSIFIERS
  displaced practices distributed evenly across environment variance
  a high-variance environment where the aggregate optimum won on merit
```

---

## Q6 — do micro-skills share one decay curve or several?        [open]

Handwriting, micrometer, screwdriver, lifting mechanics. The swarm has
the motor clock but has not tested the common-substrate hypothesis.

```
NEEDS      cross-task retest data at the INDIVIDUAL level. re-analysis
           of the existing motor-decay corpus if per-task granularity is
           published or obtainable; new collection if not.
COST       medium if the data exists, high if it must be collected.
BLOCKED ON data availability. check before designing anything.
```

```
INHERITED LIMIT — carry it into any claim
  only 2% of the corpus runs past one year. any common-substrate result
  is a claim about the first year and must say so in the sentence, not
  in a footnote. [lit:high]
```

```
FALSIFIER
  per-task decay slopes differ beyond measurement error → separate
  curves, common-substrate hypothesis dead.
```

---

## Dependencies

```
Q7  ─────────────────────────────────────────►  additive, never blocked
Q1  ─────────────────────────────────────────►  unblocks §4→§5 reading
Q5  ─────────────────────────────────────────►  defends §7
Q4  ────────────────► capped at [inf] until the denominator gap closes
Q6  ────?────────────► gated on whether per-task data exists at all
Q2  ═══════════════════════════════════╗
                                       ╚═════►  Q3   (hard block)
```

---

## Next three

```
1  Q7   start the gap log. fixed entry format, one entry already
        written. front-load any entry whose carriers are aging —
        expiry, not cost.
2  Q1   bounded citation trace. state the bound before starting.
3  Q5   mixedness audit. expect a negative result and publish it as one.
```

Q2's bench step runs in parallel if there is capacity for it — it is the
hinge, and it is the longest pole. Everything downstream of it waits.

### Off-roadmap — the cheapest empirical test in the repo

Not in §8. `unnamed-instruments.md` A1 proposes a blinded test of
arm-hair fault detection: known-faulted vs known-intact runs, operator
blind to which. Shop-runnable, no subjects to recruit, no safety
review, no apparatus that does not already exist.

It is worth pulling forward out of proportion to its topic, because it
is the only place in the repo where a felt reading gets checked against
ground truth cheaply — and the confound it tests for (felt externality
is not evidence of externality) applies to every `[obs]` entry in
`sensor-panel.md` and every operator report Q2 would collect. A
positive result is a small finding about wiring. A negative result is a
large finding about the whole observational base. [inf]

---

## Kill conditions for the frame

Stated up front so they cannot be renegotiated later.

```
K1  the cold-start first-trial probe fails to separate
    read-it-and-tried-it from did-it-for-years
      → the only honest direct test is not one. §3 falls.

K2  prediction-horizon does not separate by experience (Q2)
      → §5 falls, and §4's replacement candidate goes with it.

K3  gap-log entries keep turning out to have instruments after all (Q7)
      → the negative-space framing is decoration.
```

None of these kill the residual and inversion detectors. Those stand on
the documented cases — the FCE predictive failure and the attention
inversion — independent of whether the horizon account is right. Worth
knowing which parts are load-bearing before a result comes in and the
temptation is to save everything. [inf]
