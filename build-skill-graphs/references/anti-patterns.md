# Anti-Patterns

## The Giant Skill File

If one `SKILL.md` is trying to contain every framework, edge case, template, example, and exception, the skill has already become a graph in disguise.

Fix:

- move detail into linked notes
- keep the entrypoint focused on orientation

## Link Dumps

Lists of bare links create navigation without meaning.

Fix:

- put links inside prose
- explain what question or decision each linked note helps with

## Fragmentation Without Synthesis

Tiny notes are only useful when their boundaries are meaningful.

Fix:

- merge notes that always travel together
- add synthesis notes when the real value is in how several ideas combine

## Stale MOCs

An old MOC can quietly become misinformation because it still looks authoritative even after the graph changes around it.

Fix:

- update the relevant MOC whenever you add a new cluster
- keep MOCs short enough to maintain

## Markdown As Database

Do not force changing facts, queue state, metrics, or operational records into handwritten notes just because the graph is convenient.

Fix:

- keep live data in a typed store
- let markdown explain methods, meaning, and routing

## Deep Folder Mazes

Heavy nesting makes traversal harder for both humans and agents.

Fix:

- start flat
- add folders only when they reflect a real domain boundary

## Fake Completeness

A graph becomes brittle when it hides uncertainty behind polished structure.

Fix:

- create `open-question` notes
- state missing sources and unresolved tradeoffs directly
