# Hybrid Architecture

Use markdown for reasoning. Use a typed store for governable facts.

## Put In Markdown

- methods
- heuristics
- SOPs
- tradeoffs
- decisions
- synthesized claims
- handoffs
- postmortems

## Put In A Typed Store

- runtime state
- metrics
- experiment results
- provenance chains
- freshness timestamps
- many-to-many relations
- records that need joins, constraints, or updates

## Authority Rules

- Let source apps or APIs remain the ground truth when possible.
- Let the typed store hold structured extracts, identifiers, and provenance.
- Let markdown explain how to think, navigate, and act on the domain.

## Good Pattern

```text
source apps/apis -> typed store -> markdown skill graph
```

## Anti-Pattern

```text
source apps/apis -> copied markdown notes -> more copied markdown notes
```

That creates drift and makes freshness impossible to reason about.

## Deciding Questions

Ask:

- will this fact change often?
- does it need joins or aggregate queries?
- do I need authoritative status or freshness?
- is this primarily a method or a record?

If it is mostly a record, prefer the typed store.
If it is mostly a method, prefer markdown.
