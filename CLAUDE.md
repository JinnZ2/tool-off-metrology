# CLAUDE.md

Guidance for working in this repo.

## What this is

A documentation repo, not a codebase. Seed docs on negative-space
competence metrology: measuring skill and skill-loss with instruments the
measured environment does not itself have. No build, no tests, no
dependencies. The deliverable is prose that holds up under audit.

```
README.md                    front door: purpose, tag legend, doc map.
                             orientation only — no argument lives here
negative-space-metrology.md  the framework. the spine everything hangs off
emotion-reading-spec.md      operator-side reading method
sensor-panel.md              content side of that method, per channel
unnamed-instruments.md       catalog of real, unnamed sensing instruments
experiments.md               proposed protocols against the catalog entries
plan.md                      research roadmap over the framework's Q1–Q7
```

Protocols in `experiments.md` carry a `null says` line stating what a
negative result kills and what it leaves standing. A protocol without
one is not designed, and it will find something.

The gap log lives in `unnamed-instruments.md` (G-entries), not in a
file of its own. Keep it there — one log, not two.

Some gaps are gaps in the record rather than in instrumentation, and
they touch living communities and restricted knowledge. Where they do,
the repo's own frame — naming is the intervention — is a claim made
from outside, and cataloguing can be the harm the restriction exists
to prevent. That tension is logged in `experiments.md` and stays
unresolved. Do not write around it.

`sensor-panel.md` mixes provenance on purpose: carried entries are
`[obs]`/`[panel]`, schema-derived candidates are `[inf]`, and they live
in separate sections. Never move an entry up a column. A derived
candidate becomes carried when the practice confirms it, not when it
reads well.

New specs go at root as their own file and get a line in the README doc
map. Keep the README thin: when the framework changes, the README changes
only if the compressed thesis or the doc map is now wrong.

§9 of the framework sketches a `harness/` tree — it is a sketch, not
existing code. Do not treat it as present, and do not scaffold it unless
asked.

## Claim lineage — required

Every asserted edge carries a tag. This is the repo's core convention;
untagged claims are the defect.

```
[obs]    direct field / operator observation
[inf]    inference, untested
[lit]    literature, with confidence: [lit:high] [lit:med] [lit:low]
[open]   unresolved
[gap]    no instrument exists
```

Individual specs may add local tags (`emotion-reading-spec.md` uses
`[panel]`; `unnamed-instruments.md` uses `[lead]`). Declare any added
tag in that file's own tag list — an undeclared tag is the same defect
as an untagged claim.

`[lead]` in particular is not a weak `[inf]`. It marks a place to look,
and it carries no claim that the place holds anything. Writing about a
lead as though it were evidence is the failure the tag exists to
prevent.

Rules that follow from the convention:

- Do not promote a tag. `[inf]` does not become `[lit]` because it sounds
  right. Cite or leave it.
- Do not launder uncertainty in prose. If a claim is untested, the tag
  says so and the sentence does not hedge around it.
- Absence of an instrument is a finding, logged as `[gap]` — not an
  apology and not a caveat.

## Instrument entries declare their blind side

Any doc that catalogs an instrument — `unnamed-instruments.md`,
`sensor-panel.md`, and the Q7 gap log when it exists — states, per
entry, the regime the instrument works in and what it cannot read.

This is the line between a measurement and a story, and it is load-
bearing: it is what keeps A1 (arm-hair fault detection) on a different
footing from dowsing. An entry that reads everything, everywhere, has
not been specified. Its blind side is not a caveat to add at the end —
it is half the entry.

The blind side is not always an out-of-range. A detector fails by
being off-scale; a store fails at the boundary of what it holds. B2 is
the worked case — no out-of-range failure, because it is not a
detector, and its edge is the uncoalesced layer instead. Find the
entry's actual failure boundary rather than forcing every entry into
the transducer shape.

## Trained-carrier claims say which kind

An entry claiming a trained carrier outperforms the general population
states whether that is a *threshold* difference or a *reporting*
difference — or states that it does not yet know. The catalog's
konenki counter-case is why: a large replicated cross-cultural
difference that moved with diet over twenty years and vanished under
skin conductance. Only objective instrumentation separates the two, so
a claim resting on what someone says cannot tell them apart.

## Carrier words before paraphrase

When a claim is carried from an operator, record their words verbatim
before writing the analysis, and keep the two in separate columns.

A paraphrase can widen an operating range. Once widened, the widening
is invisible — it reads back as the carrier's own claim, and any later
narrowing reads as the analyst locating the carrier's overclaim rather
than their own. `unnamed-instruments.md` A1 is the worked case: the
carrier said "open" and "problem" in the first sentence, the
intact-wiring scenario was imported from elsewhere and attached to
them, and the record then showed them being corrected into a range they
had stated correctly from the start.

The cost is not just to the carrier. It puts the entry in the wrong
evidentiary tier, which is the one thing the tier system exists to
prevent.

## Register

Match the existing files. Terse, declarative, field-note density. ASCII
blocks in fenced code for structured material; prose only where the
argument needs connective tissue. Roughly 72-column wrapping in the
existing docs — keep it.

Terms are field terms: definition, signs, axis. Not narrative vocabulary,
not metaphor doing load-bearing work.

## The overclaim seam

`negative-space-metrology.md` §7 names the repo's own recurring failure
mode: calibrated
reasoning underneath, inflated at the headline. "Convergence across
domains" is defensible; "general law" is not. When editing or adding,
strip that seam wherever it appears — including in text you just wrote.

Corollary: do not summarize a document into a stronger claim than the
document supports. Do not add executive summaries.

Second corollary: do not attach a neural substrate to anything here.
The seat-of-feeling version is already disposed of in the catalog's G4,
and the temptation arrives at write-up — a behavioural result wanting
an anatomy bolted on to make it feel solid. The result is the result.

## Editing existing docs

- Preserve author voice and phrasing. These are the author's field notes;
  copy-editing them into neutral prose destroys the signal they carry.
- Preserve tags on any line you touch.
- Add rather than rewrite when the content is new.
- Do not reconcile apparent tensions between docs by smoothing them. An
  unresolved tension gets `[open]`.

## Git

- License: CC0 (see `LICENSE`). No attribution headers on new files.
- Develop on the branch named in the task; create it if absent.
- Push with `git push -u origin <branch>`.
- Do not open a pull request unless explicitly asked.
