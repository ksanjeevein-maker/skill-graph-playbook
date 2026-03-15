---
name: build-skill-graphs
description: Design and extend markdown skill graphs made of index notes, MOCs, and atomic linked nodes. Use when a domain is too deep for one SKILL.md, when the user wants a wiki-linked knowledge system, or when you need to separate stable methodology from live operational data.
---

# Build Skill Graphs

## Overview

Use this skill to turn one oversized skill or knowledge dump into a graph of small markdown notes that an agent can traverse progressively. The default path is:

`index -> MOC -> node -> section`

Most routing decisions should happen before reading full files.

## When To Use This Skill

Use it when:

- the domain no longer fits cleanly in one `SKILL.md`
- the user wants a second-brain style skill library or knowledge graph
- the work involves MOCs, entrypoints, note types, or traversal rules
- the team needs a boundary between stable markdown knowledge and live system state

## Core Workflow

1. Define the graph boundary.
   Decide what the graph should answer, what its main entrypoint is, and what stays out of scope.

2. Separate stable knowledge from live state.
   Put methods, heuristics, claims, decisions, and synthesized patterns in markdown.
   Put volatile facts, runtime state, provenance chains, metrics, and join-heavy relations in a typed store.

3. Create the entrypoint first.
   Start with one index note that names the main clusters and points attention.

4. Add MOCs only when a topic is large enough.
   Use MOCs to orient the reader. Do not use them as giant link dumps.

5. Write atomic nodes.
   Each node should hold one complete thought, method, tradeoff, or claim.

6. Use links inside prose.
   A wiki link should explain why the next note matters, not just prove that it exists.

7. Encode trust and freshness.
   Mark note type, state the source of truth, and make uncertainty explicit when the graph is incomplete.

8. Keep traversal cheap.
   Prefer one or two hops from the entrypoint over deep hidden chains.

## What Belongs In Markdown

- methods
- heuristics
- decision rules
- synthesized claims
- curated examples
- stable operating guidance

## What Belongs In A Typed Store

- changing records
- metrics and dashboards
- provenance chains
- runtime state
- query-heavy relations
- facts that are likely to drift

## References

Read these files as needed:

- `references/templates.md` for entrypoint, MOC, and node templates
- `references/patterns.md` for traversal rules, note types, and repo layouts
- `references/anti-patterns.md` when the graph feels too big, too flat, or too stale
- `references/hybrid-architecture.md` when the markdown versus database boundary is unclear
- `references/decision-guide.md` when the main question is whether a graph is needed at all
- `references/migration-playbook.md` when splitting one oversized skill into a graph
- `references/review-checklist.md` when checking whether the graph is ready to use
- `references/maintenance-checklist.md` when the graph is starting to drift
- `references/naming-conventions.md` when note and file names are getting muddy
- `references/example-graph/knowledge-work.md` for a small working example
- `references/example-graph-business-ops/operations-knowledge.md` for a business-operations example

## Delivery Pattern

When building a graph for a user:

1. Create or update the entrypoint first.
2. Add only the next few notes needed for the current task.
3. Name the next nodes worth reading.
4. Keep open questions visible instead of pretending the graph is complete.
5. Point to the system of record whenever facts are operational or time-sensitive.
