---
name: typed-stores-hold-live-state
description: Put changing facts, provenance, and query-heavy records in structured storage instead of handwritten notes.
type: method
source_of_truth: curated synthesis
---

# Typed Stores Hold Live State

When a fact changes frequently, needs freshness tracking, or participates in many-to-many relationships, a typed store is usually a better source of truth than a note. The graph should point to that system, not duplicate it.

Use [[markdown-stores-methods]] when the material is guidance rather than records, and use [[maintenance-keeps-mocs-trustworthy]] when the problem is no longer storage but graph upkeep.

## Key Rule

If the reader needs to query, aggregate, or trust the current value of something, store it in a structured system and let the graph explain how to use it.

## Inputs

- runtime state
- metrics
- identifiers and provenance
- frequently changing records

## Outputs

- clearer authority boundaries
- less drift
- better operational queryability
