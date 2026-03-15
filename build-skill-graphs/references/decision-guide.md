# Decision Guide

Use this note when you need to decide whether a domain should stay in one file, become a skill graph, or split into markdown plus a typed store.

## Keep One `SKILL.md`

Choose one file when:

- the workflow is short and mostly procedural
- the agent rarely needs alternative traversal paths
- examples are few enough to stay readable inline
- the domain can be scanned quickly without hidden depth

## Build A Skill Graph

Choose a graph when:

- the domain has multiple clusters that deserve separate navigation
- the agent needs MOCs, index notes, or route-specific reading paths
- examples, tradeoffs, and anti-patterns are crowding the entrypoint
- the main problem is understanding, not just remembering steps

## Use A Hybrid System

Choose markdown plus a typed store when:

- the domain mixes stable reasoning with changing operational facts
- freshness matters and the graph should not become the source of truth
- records need joins, identifiers, or query-heavy relationships
- the agent needs both guidance and governable live data

## Quick Test

Ask:

1. Is the main pain too much explanation in one place?
2. Does the agent need more than one good path through the material?
3. Are changing records being forced into markdown?

If the answer is:

- mostly no: keep one `SKILL.md`
- yes to 1 or 2: use a skill graph
- yes to 3: use a hybrid system
