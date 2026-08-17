# Sensor Panel

The content side of the reading. `emotion-reading-spec.md` names how to
take a reading; this names what each channel reads.

Status: partial, and mixed-provenance — read the tags before using an
entry. Entries marked [obs] / [panel] are carried from the transmitted
panel via the spec. Entries marked [inf] are **derived by applying the
spec's schema**, not carried. They are candidates awaiting confirmation
against the practice, and a wrong candidate here is a wrong instrument,
not a wrong word.

---

## Entry format

Borrowed from the falsifiability rule in `unnamed-instruments.md`: an
entry that states where it fails is a measurement; one that reads
everything is a story. So every channel declares its blind side.

```
reads          which channel breached, and about what
referent       what the reading points AT. never the operator's character
does not read  what this channel is silent on. the blind side
correction     the action it licenses. if there is none, it was narrated
collapses to   the narrative overlay that most often eats it
```

Gain is not in this table. Gain is per-event and orthogonal to content
— any channel here can run clean or run loud, and the panel says
nothing about which. See the spec's impedance threshold.

Nor is every signal one channel. Compound readings arrive as several
readings at once; shame is the carrier-named case. They have their own
section below and do not get table entries, because a table entry
asserts a single referent and that is the thing a compound does not
have.

---

## Carried entries

From the spec and its worked example.

### pain
```
reads          physical parameter breach                          [obs]
referent       the tissue, the load, the surface
does not read  cause, fault, or blame. it locates, it does not attribute
correction     unload, withdraw, treat
collapses to   "I am fragile"
```

### surprise
```
reads          model outside range — the event was not in the model [obs]
referent       the gap in the model's coverage
does not read  whether the missing case mattered, or how often it recurs
correction     extend the model. this case was genuinely absent
collapses to   "I should have known"
```

### frustration
```
reads          model-had-capacity residual — the variable was
               reachable and not loaded                            [obs]
referent       the loading step, not the model
does not read  whether the model itself is adequate. it presumes it was
correction     fix the loading. nothing to add to the model
collapses to   "I'm careless"
```

### fear
```
reads          threat proximity ranking, computed on a temporal
               model — the ranking is in time-to-contact          [panel]
referent       the threat, and when it arrives
does not read  whether the threat is survivable, or worth the cost of
               avoiding. ranking is not decision
correction     act on the ranking — buy time, or spend it deliberately
collapses to   "I'm a coward"
```

Carrier, confirming the temporal component: "fear definately hss
temporal model aspects". [obs]

### anger
```
reads          boundary crossing — a location report                [obs]
referent       the boundary and which side of it something is on.
               "a system entered where it should not have, or this
               finger entered where it should not have"
does not read  who is at fault. it reports a location, not a verdict.
               a wronged party is assigned afterward and is not in
               the reading
correction     restore the boundary, or move it deliberately
collapses to   "someone did this to me"
```

---

## Derived candidates                                              [inf]

Schema applied to channels the spec does not enumerate. Not carried
from the panel. Confirm or discard against the practice; do not cite
these as observed.

### confusion
```
reads          multiple models fit and none discriminates
referent       the missing discriminating variable
does not read  which model is right. that is the point — it reports
               non-discrimination, not error
correction     find the variable that separates the candidates
collapses to   "I'm slow"
```

Pairs with surprise the way frustration does, and the correction
differs the same way. Surprise says no model covered it — extend the
model. Confusion says too many cover it — discriminate. Treating them
as one channel loses the correction, which is the same failure the
spec's worked example documents for surprise / frustration. [inf]

### boredom
```
reads          information-rate floor — the model is running and the
               environment is returning no residual
referent       the environment's predictability, not the operator's
               character or interest
does not read  whether the task matters. a fully-predicted critical
               task reads identically to a trivial one
correction     load a harder model, or change the environment
collapses to   "I'm lazy" / "I'm not interested"
```

Inverse of surprise on the same axis. Surprise is the model exceeded;
boredom is the model never touched. [inf]

### dread
```
reads          horizon returns a bad state, and it is inside range
referent       the projected state and its distance
does not read  probability. it fires on reachability, not likelihood —
               which is why it runs loud on low-probability outcomes
correction     act inside the horizon, or extend the horizon past the
               state to see what follows it
collapses to   "I'm catastrophizing"
```

### grief
```
reads          a load-bearing element is gone and the model still
               routes through it
referent       the structure, and the dependencies that ran on it
does not read  the size of the loss, and it does not rank losses
correction     re-route. duration is the re-routing cost, not a
               verdict on the operator or on how much they cared
collapses to   "I'm not over it"
```

### disgust
```
reads          non-integrability — this substance, agent, or
               arrangement cannot be taken into the system
referent       the thing
does not read  danger magnitude. it is a compatibility reading, not a
               threat ranking — that is fear's channel
correction     exclude, or decontaminate
collapses to   contempt, when the referent is a person
```

Flagged: this is the channel with the worst overextension record. The
referent is supposed to be a substance or arrangement; generalized to
people it produces a character claim, which is precisely what the
spec's verb-not-noun test rejects. Whether that generalization is a
misuse of the instrument or a second real channel wearing the same
signature is unresolved. [open]

### exhaustion
```
reads          resource floor — the stack is out of capacity
referent       the operator's reserves
does not read  the value of the work, or whether to continue. it
               reports a level, not a decision
correction     replenish, or reduce load
collapses to   "I can't handle this"
```

Distinct from boredom, which can present identically at the surface.
Boredom is capacity unused; exhaustion is capacity spent. Opposite
corrections. Confusing them is expensive in both directions. [inf]

---

## Compound readings

Every channel in the tables above resolves to one reading. Not every
signal does.

Carrier, on shame:

> shame is a compound reading... whether internal or externally
> applied...

That kills the binary this file previously logged — either shame is
not a channel at all, or shame is a single channel about group
standing. Neither. It is real, and it is more than one reading
arriving together. [obs]

### what follows

The verb-not-noun test does not fail on shame after all. This file
claimed it did: that a reading resolving to a claim about who the
operator is was narrated by construction, and shame does that
inherently.

That was wrong in exactly the way the spec's own worked example says
it is wrong. An undecomposed compound *looks* like a character claim.
"Frustrated because I'm careless" is surprise and frustration
collapsed into one, and the collapse is what produces the character
claim — separating the readings dissolves it. Shame is that collapse
at larger scale. The schema was not broken; the decomposition was
missing. [inf]

### what is not written here

The components. The carrier named the compound, not its parts, and
guessing the parts is precisely how the A1 error happened.

On record: it is compound, and an internal / externally-applied
distinction lives somewhere in it. [obs]

```
UNRESOLVED
  what the internal/external distinction is ON — an axis of the
    compound itself, or a separate question about where the compound
    originated? the phrasing carries both.                    [open]
  whether it is the same axis as the spec's inward/outward clearing
    split. that split is about how to clear impedance, not about
    where a reading came from. different questions, possibly
    related, not assumed identical.                           [open]
  the components themselves.                                  [open]
  guilt — untouched. this file previously floated it as a boundary
    reading with the operator on the crossing side. that was tidy
    and nothing has confirmed it.                             [open]
```

These are P1–P4 in `plan.md`, which carries the rest of the panel's
open set and a proposed test for the whole shape of them — two
readings are separate channels when the correction diverges, which is
the ground the spec's own worked example separates surprise from
frustration on.

### one implication, flagged and not built on

A reading that can be *externally applied* is a channel that something
outside the operator can write to.

That is a different failure from the degradation vectors in
`unnamed-instruments.md`. HAVS destroys A2; it does not forge readings
on it. An injection surface on an internal-state channel has no entry
in that catalog, and there is no instrument that separates a carried
reading from an applied one. [inf]

If that holds, it is gap-log material rather than a panel entry — the
panel says what a channel reads, not who wrote to it. [open]

---

## Structural observations

### The panel is breach-only

Every entry above — carried and derived — is a mismatch, a breach, or
a floor. Nothing here reads a channel that is fine. Two possibilities,
not decided:

```
by design   no reading IS the normal state. the panel is exception-
            driven and a positive-side entry would be a category
            error.
gap         there are positive-side channels — satisfaction as
            model-matched-outcome closure, for one — and their
            absence is a hole in the panel rather than a property
            of it.
```

[open]. Worth deciding, because the two imply different panels.

### fear runs on a temporal model

Carrier-confirmed, and the confirmation is narrow. What was said:

> fear definately hss temporal model aspects

That establishes the temporal component. It does not establish
anything below this line, which is mine. [obs]

---

`negative-space-metrology.md` §5 defines prediction-horizon skill as
forward-projection of environment dynamics with a horizon: how long
the model stays valid × which variables can cross the gap in that
time.

Fear's reading — threat proximity ranking in time-to-contact — has the
shape of that computation run on the threat subset and reported as an
emotion. Dread, above, would be the same with the projected state
already inside range. [inf]

If that identity holds, the panel is partly an *output display for the
horizon model*, and Q2's problem of measuring horizon directly gains a
second, cheaper handle: fear and dread readings would already be
horizon output, and they are reportable. That is not a substitute for
perturbation testing — self-report is the corrupted channel the whole
framework routes around, and this would be self-report — but the two
disagreeing would itself be a reading. [inf]

```
CONFIRMED   fear has temporal model aspects
INFERRED    fear IS the §5 horizon computation
            the panel is a horizon-model display
            Q2 gains a handle
```

The distance between those two lines is the whole width of the A1
error. "Has temporal aspects" is what the carrier said; "is the same
computation" is what I want it to say. Keeping them apart is the only
thing that stops the second from being read back later as carried.

Logged rather than acted on. It is a bridge between two docs written
independently — the kind of overlap §2 says to look for, and the kind
that is easy to see because you want to.

### naming tension, unresolved

`unnamed-instruments.md` Column C describes this system as "content /
amplitude / impedance" and refers to a hormonal calibration layer. The
spec has content / **gain** / impedance and no calibration layer.

Not reconciled here. Either the catalog is describing a fuller version
of the practice than the spec wrote down — in which case the spec is
missing a layer — or the terms drifted between documents. [open]

---

## Tags

- [obs]   direct operator observation, carried from the spec
- [panel] carried from the transmitted panel
- [inf]   derived by applying the spec's schema. not carried, not
          confirmed
- [open]  unresolved
