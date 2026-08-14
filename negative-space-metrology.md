# Negative-space competence metrology

The core framework. Seed doc.
Sibling to `field-curiosity-loop` — same residual-router spine, pointed at
institutional/skill data instead of sensor data.

Lineage tags: [obs]=direct field observation · [inf]=inference, untested ·
[lit]=literature, with confidence · [open]=unresolved · [gap]=no instrument exists

---

## 0. Purpose (one line)

Detect when learning/skill is being designed out of a work environment,
using measurements the environment's own instruments cannot make.

---

## 1. Why direct measurement fails

The reporting channel is the corrupted one. You cannot ask.

```
self-report        → corrupt exactly where it matters
                     Gillen 2008: 100% of airline pilots claimed raw-data
                       capability; ALL failed it in sim              [lit:high]
                     Davis 2006 JAMA: 13/20 comparisons null-or-inverse;
                       worst calibration = least-skilled + most-confident [lit:high]
tool-on metrics    → measure performance WITH the tool; mask atrophy
                     Budzyn 2025: overall ADR rose while unaided ADR fell [lit:med]
attention counting → scores the NOVICE higher (measurement inversion)  [inf]
                     expert samples sparsely under a model of the system;
                     any eyes-on-task / glances-per-min metric reads
                     the calibrated operator as disengaged
```

Same inversion recurs: yellow-vest saturation, safety-reporting numbers,
FCE lifting scores, attention metrics. When the standard instrument reads
backwards, that IS the signal.

---

## 2. Framework — negative-space competence metrology

You can't read skill off a dial. You read it off its shadow.

```
THREE DETECTORS
  residual    : where accounted-for cost ≠ observed outcome
                the gap names the missing variable
  inversion   : where the standard instrument scores competence backwards
  tool-off    : cold-start, first-trial-only probe — the only honest direct test

METHOD (exploratory, not confirmatory)
  do NOT define observables first — that smuggles in the answer
  run multiple sims from different angles
  look for where their residuals / negative-space shadows OVERLAP
  convergence across substrates = the evidence
  harness stays agnostic about what it's hunting

INSTRUMENT-GAP RULE
  absence of an instrument is data, logged as a finding in its own right —
  not an apology, not a caveat
```

---

## 3. The measurement method (solves the no-self-report problem)

```
COLD-START PROBE                                                    [lit:high]
  score the FIRST retest trial only (everything after = relearning)
  the probe IS the maintenance dose — measure and train in one act (CI-2)
  → distinguishes read-it-and-tried-it from did-it-for-years
    BEFORE the failure, not after                                  [inf→testable]

DECAY CLOCK (the function the sims assumed)          Tatel & Ackerman 2025 [lit:high]
  procedural-motor: −0.08 SD/mo accuracy, −0.06/mo speed
  half of acquisition gains gone ~6.5 mo (acc) / ~13 mo (speed)
  real-world decays SLOWER than lab (labs overstate)
  HARD LIMIT: only 2% of data > 1yr — "half-life" folk numbers extrapolate

REACQUISITION ASYMMETRY                                             [lit:high]
  relearning << learning; 40-min refresher reversed 35% multi-month deficit
  BUT savings dies with the carrier (no living bearer → no savings)
```

---

## 4. The residual worth chasing first — FCE

Buried in swarm-2 RTW literature, reported flat, connection unmade:

```
Gross & Battie 2004:  better FCE (lifting-capacity) score → HIGHER recurrence [lit]
Gross 2006:           higher lifting perf → faster claim closure, but
                      NO FCE indicator predicted recurrence (r²=1.2–11%)      [lit]
```

Reading:
- the instrument that measures the assumed cause (strength) has ~no
  predictive power over the outcome (re-injury)                    [inf]
- kills the strength model of return-to-work injury; does not prove
  the replacement                                                  [inf]
- the replacement candidate: stale prediction-horizon (§5), not lost fitness [inf]
- textbook residual: accounted cost (strength) ≠ outcome (re-injury);
  the gap is where the missing variable lives                      [inf]

---

## 5. Prediction-horizon skill (undiagnosed; not in either swarm)

```
DEFINITION
  forward-projection of environment dynamics with a HORIZON:
  how long the model stays valid × which variables can cross the gap in that time
  looking away = evidence OF a model, not absence of one
  constant monitoring = brute-force fallback for those WITHOUT the model

SAME OPERATION ACROSS DOMAINS                                       [obs]
  traffic: closure rates vs following distance — "not within distribution distance"
  felling: stored tension / wobble — when to pull the chain vs wait
  different physics, identical computation → general skill, not domain trick

CLOSES THE RETURN-TO-WORK LOOP                                     [inf]
  horizon is the fast-decaying, most environment-specific piece
  calibrated to THIS yard / traffic / machine's time constants; goes stale on layoff
  predicts: injury spike after break = stale model, not lost strength
  sharp counterintuitive test: familiar work after layoff MORE dangerous
    than unfamiliar work (unfamiliar → continuous monitoring, no stale horizon relied on)

ADJACENT BUT NOT THE SAME
  Eva & Regehr "knowing when to look it up" = seek external info (opposite polarity) [lit]
  vigilance/complacency lit treats reduced monitoring as DEFICIT — inverted from this
```

---

## 6. Findings carried from swarm-1, confirmed by swarm-2

```
F1 skill requirement discovered DOWNSTREAM of installation, never before [lit:med]
   Kokhanok 7yr dormant until 3 locals trained; Wales legacy-infra mismatch
F2 remediation sized to what's AUDITABLE → fix inherits the measurement
   limit that caused the problem                                   [inf, strong lit support]
   Naval Academy celestial nav = 3hr module skipping sight reductions
   credential windows encode convention, not decay data (CI-5)     [lit:high]
F3 skill-carrier half-life vs duration of demanding condition;
   mismatch predicts lapse                                         [inf→testable]
   wood gas abandoned 1945 (no carrier) vs Cuba persisted via law + elders
   grant cycles = 2–4yr carrier bolted to 20yr infrastructure
```

---

## 7. The overclaim seam (both swarms, same failure)

```
exec summary: recurrence "upgrades this to a general LAW of human–tool
              systems. Confidence: high."                          → overclaim
convergence CI-8: "decay is continuous, modest monthly, design- and
              task-moderated."                                     → defensible
```

Work supports CONVERGENCE across domains, not a law. Universality claim
never run through the scientific method. Calibrated underneath, inflated at
the headline — same seam in both packets. Strip at audit.

---

## 8. Open questions to explore

```
Q1  FCE thread: has anyone connected functional-capacity's PREDICTIVE
    FAILURE to skill rather than fitness? trace the citation graph.     [next]
Q2  prediction-horizon: measure it directly — ask operator max look-away,
    perturb environment at varying delays, find where prediction breaks.
    yields seconds/domain/experience-level. does it decay on the clock? [design]
Q3  is horizon exactly what alarm-based automation destroys? (promise to
    warn → stop computing horizon → can't when the alarm fails)         [design]
Q4  displaced local optima: do displaced practices CLUSTER in high-variance
    environments (cold, remote, off-grid, irregular load) where local
    optimum diverges most from aggregate? castor oil, wood gas as cases. [untested]
    NB: displacement is on distribution cost, not performance.          [inf]
Q5  "critical thinking decline" — do NOT assume it extrapolates. instead
    audit the MIXEDNESS: what moderates it? construct validity (does the
    horizon skill even load on the test)? sample dynamics (urban/suburban
    undergrads = population with variance already gone)?                 [open]
Q6  micro-skills (handwriting, micrometer, screwdriver, lifting mechanics)
    — do they share ONE decay curve, or separate? swarm has the motor
    clock but hasn't tested the common-substrate hypothesis.            [open]
Q7  the instrument gap itself: enumerate skills with NO instrument that
    distinguishes competent from absent before failure. that list is a
    finding.                                                            [gap]
```

---

## 9. Architecture sketch

```
harness/
  sims/            multiple exploratory models, different angles, agnostic target
  residual_router  find where sims' negative-space shadows overlap
  detectors/
    residual.*     accounted cost ≠ outcome
    inversion.*    instrument scores competence backwards
    tool_off.*     cold-start first-trial probe + decay-clock scoring
  gap_log.*        skills with no distinguishing instrument (absence = data)
  claim_lineage.*  [obs]/[inf]/[lit]/[open]/[gap] on every asserted edge
```

Assumed by `thermo-pm` and `labor-thermodynamics`; neither has it. This is
the sensing layer both were missing.

