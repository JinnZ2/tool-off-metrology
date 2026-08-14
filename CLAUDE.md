# CLAUDE.md

Guidance for working in this repo.

## What this is

A documentation repo, not a codebase. Seed docs on negative-space
competence metrology: measuring skill and skill-loss with instruments the
measured environment does not itself have. No build, no tests, no
dependencies. The deliverable is prose that holds up under audit.

`README.md` is the spine. Other root-level `*.md` files are specs that
hang off it (e.g. `emotion-reading-spec.md`). §9 of the README sketches a
`harness/` tree — it is a sketch, not existing code. Do not treat it as
present, and do not scaffold it unless asked.

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
`[panel]`). Declare any added tag in that file's own tag list.

Rules that follow from the convention:

- Do not promote a tag. `[inf]` does not become `[lit]` because it sounds
  right. Cite or leave it.
- Do not launder uncertainty in prose. If a claim is untested, the tag
  says so and the sentence does not hedge around it.
- Absence of an instrument is a finding, logged as `[gap]` — not an
  apology and not a caveat.

## Register

Match the existing files. Terse, declarative, field-note density. ASCII
blocks in fenced code for structured material; prose only where the
argument needs connective tissue. Roughly 72-column wrapping in the
existing docs — keep it.

Terms are field terms: definition, signs, axis. Not narrative vocabulary,
not metaphor doing load-bearing work.

## The overclaim seam

README §7 names the repo's own recurring failure mode: calibrated
reasoning underneath, inflated at the headline. "Convergence across
domains" is defensible; "general law" is not. When editing or adding,
strip that seam wherever it appears — including in text you just wrote.

Corollary: do not summarize a document into a stronger claim than the
document supports. Do not add executive summaries.

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
