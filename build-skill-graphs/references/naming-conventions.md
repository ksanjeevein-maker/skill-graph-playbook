# Naming Conventions

Good naming keeps a graph scannable before a reader opens any file.

## File Names

- use lowercase kebab-case
- prefer names that describe the note's job, not just the topic
- keep names short enough to read in a list without wrapping badly

Good:

- `incident-review.md`
- `handoff-boundaries.md`
- `position-sizing.md`

Weak:

- `important-things.md`
- `notes-v2-final.md`
- `random-thoughts-about-risk.md`

## Note Titles

Titles should tell the reader what question the note helps answer.

Good:

- `Handoff Boundaries`
- `Queue Health Versus Root Cause`
- `Markdown Stores Methods`

Weak:

- `Operations`
- `Thoughts`
- `General Notes`

## MOCs And Entrypoints

- let entrypoints name the domain or use case
- let MOCs name the cluster they route through
- let atomic notes name the claim, method, or tradeoff they explain

That makes the path easier to predict before clicking through it.
