# Patterns

## Progressive Disclosure

Skill graphs work best when the agent can decide what to read before loading full files.

Preferred path:

`index -> description -> MOC -> node -> section`

That keeps context cost low and prevents the graph from feeling like a hidden monolith.

## Link Semantics

Use wiki links in sentences so the reason for the connection is visible at the point of use.

Good:

- "Use [[position-sizing]] when confidence should change exposure."
- "Read [[kill-switches]] when uncertainty should stop execution."

Weak:

- "Related: [[position-sizing]], [[kill-switches]], [[confidence]]."

## Note Type Discipline

Different note types should do different jobs.

- `index` orients
- `moc` groups and routes
- `method` teaches a procedure
- `decision` records a choice and why it was made
- `synthesis` explains how several notes fit together
- `open-question` makes uncertainty explicit

If every note is trying to do all of those things at once, the graph is not really decomposed.

## Authority And Freshness

When a note refers to changing facts, point to the system of record.

Examples:

- `source_of_truth: analytics warehouse`
- `source_of_truth: ops/config.yaml`
- `source_of_truth: curated synthesis from references`

The graph should explain how to think and where to look. It should not pretend to be a live database.

## Repo Shapes

Use the smallest layout that supports the work.

### Flat

```text
references/example-graph/
  knowledge-work.md
  graph-structure-moc.md
  atomic-note.md
```

Good for tiny graphs and examples.

### Clustered

```text
knowledge/
  index.md
  strategy/
    strategy-moc.md
    bayesian-scoring.md
    position-sizing.md
  operations/
    operations-moc.md
    incident-review.md
```

Good when the graph has real subdomains.

### Hybrid

```text
knowledge/
  index.md
  decisions/
  methods/
data/
  runtime.sqlite
  metrics.db
```

Good when stable markdown knowledge and volatile structured facts need different homes.

## Delivery Heuristic

When expanding a graph, add:

1. one entrypoint update
2. one MOC if needed
3. two to five atomic nodes

That is usually enough to improve the system without overfitting it on day one.
