# Templates

Use these templates to create a small graph first, then grow it only when the domain proves it needs more structure.

## Minimal Repo Shape

```text
repo-root/
  README.md
  skill-name/
    SKILL.md
    agents/
      openai.yaml
    references/
      templates.md
      patterns.md
      anti-patterns.md
      example-graph/
```

## Minimal Graph Shape

```text
graph/
  index.md
  topic-moc.md
  node-a.md
  node-b.md
```

## Index Template

```markdown
---
name: domain-index
description: Entry point for the domain. Use it to orient the agent and route it to the right cluster.
type: index
---

# Domain Index

One paragraph explaining what the graph covers and what it does not.

## Main Clusters

- [[topic-moc]] - what this cluster covers
- [[operations-moc]] - what this cluster covers

## Current Focus

- [[important-node]] - why it matters now

## Open Questions

- what still needs to be resolved
```

## MOC Template

```markdown
---
name: topic-moc
description: Map of content for one cluster of related notes.
type: moc
---

# Topic MOC

Explain what belongs here and when to read this cluster.

## Core Notes

- [[first-node]] - why it matters
- [[second-node]] - why it matters

## Open Questions

- [[unknown-or-missing-node]]
```

## Atomic Node Template

```markdown
---
name: first-node
description: One complete claim, method, or tradeoff.
type: method
source_of_truth: path, API, table, or "curated synthesis"
---

# First Node

State the main idea in one paragraph.

Use wiki links in prose: follow [[second-node]] when the idea changes implementation detail, and read [[third-node]] when the main risk is structural instead of tactical.

## Key Rule

Write the operational rule here.

## Inputs

- what this note expects

## Outputs

- what this note changes, informs, or constrains
```

## Suggested Note Types

- `index`
- `moc`
- `method`
- `decision`
- `synthesis`
- `anti-pattern`
- `open-question`
