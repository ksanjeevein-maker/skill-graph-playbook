---
name: progressive-disclosure
description: Stage graph traversal so the agent can decide what to load before reading full files.
type: method
source_of_truth: curated synthesis
---

# Progressive Disclosure

The graph should reveal itself in layers. Start with an index, follow a relevant MOC, then open the atomic notes that answer the current question.

Use [[links-carry-reasons]] when the next hop needs justification in prose, and use [[mocs-orient-attention]] when the graph is large enough that routing itself needs its own note.

## Key Rule

Do not make the agent load a full cluster when a short description and one well-placed link can make the same routing decision.

## Inputs

- an entrypoint note
- short descriptions on important files
- a current task or question

## Outputs

- fewer unnecessary reads
- lower context cost
- more reliable traversal decisions
