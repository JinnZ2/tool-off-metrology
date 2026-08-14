# tool-off-metrology

Exploration of missing measurement tools.

Seed repo. CC0. Repo name provisional.

---

## What this is

Detect when learning/skill is being designed out of a work environment,
using measurements the environment's own instruments cannot make.

The problem is not that skill loss is hard to see. It is that every
standard instrument pointed at it reads wrong in a specific, repeating
way:

```
self-report        corrupt exactly where it matters — the least skilled
                   are the most confident                          [lit:high]
tool-on metrics    measure performance WITH the tool; aided scores rise
                   while unaided scores fall                       [lit:med]
attention counting scores the NOVICE higher — the calibrated operator
                   samples sparsely and reads as disengaged        [inf]
```

When the standard instrument reads backwards, that IS the signal. So
the method reads skill off its shadow rather than off a dial: find
where accounted-for cost ≠ observed outcome (**residual**), where the
instrument scores competence backwards (**inversion**), and probe
cold-start first-trial-only, which is the sole honest direct test
(**tool-off**).

Absence of an instrument is logged as a finding in its own right, not
as a caveat.

Full argument, evidence, and open questions:
[`negative-space-metrology.md`](negative-space-metrology.md)

---

## Lineage tags

Every asserted edge carries one. Untagged claims are the defect.

```
[obs]     direct field / operator observation
[inf]     inference, untested
[lit]     literature, with confidence — [lit:high] [lit:med] [lit:low]
[open]    unresolved
[gap]     no instrument exists
```

Specs may add local tags and declare them in their own tag list
(`emotion-reading-spec.md` adds `[panel]`).

Tags do not get promoted. `[inf]` becomes `[lit]` when there is a
citation, and not before.

---

## Docs

```
negative-space-metrology.md   the framework. why direct measurement fails,
                              the three detectors, the decay clock, the FCE
                              residual, prediction-horizon skill, and the
                              open questions Q1–Q7

emotion-reading-spec.md       operator-side reading method: content × gain,
                              the impedance threshold with its inward/outward
                              split, the verb-not-noun test. a worked case of
                              a functional instrument that exists only on a
                              carrier clock

plan.md                       research roadmap. what each open question needs,
                              what would falsify it, what is blocked on what,
                              and what to do first

CLAUDE.md                     conventions for anyone (or anything) editing here
```

The `harness/` tree sketched in the framework's §9 is a sketch. No code
exists yet.

---

## How to read it

Nothing here is finished, and the tags say which kind of unfinished.
The repo has one known failure mode, named in the framework's §7:
calibrated reasoning underneath, inflated at the headline. "Convergence
across domains" is what the work supports; "general law" is not. If you
find that seam anywhere — including in text added later — strip it.

---

## License

CC0. See [`LICENSE`](LICENSE). Take it, use it, no attribution needed.
