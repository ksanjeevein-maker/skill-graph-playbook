---
name: mocs-orient-attention
description: Use MOCs to route attention through a cluster instead of restating every note in the graph.
type: synthesis
source_of_truth: curated synthesis
---

# MOCs Orient Attention

An MOC is not a backup copy of the graph. It is a compact guide that helps the reader decide which local region is worth exploring next.

Read [[progressive-disclosure]] when the graph needs better staged loading, and rely on [[links-carry-reasons]] when the MOC should point outward to notes that justify the next step.

## Key Rule

If an MOC is growing into a long catalog, split the cluster or reduce the list to the notes that best orient the current domain.

## Inputs

- a cluster with enough notes to need a hub

## Outputs

- faster routing
- less graph sprawl
- clearer local navigation
