# Migration Playbook

Use this playbook when one large `SKILL.md` has become hard to scan, hard to update, or too expensive for an agent to read every time.

## Step 1: Mark The Current Boundaries

Before splitting anything, identify:

- what the current file does well
- which sections are stable methods
- which sections are examples or optional detail
- which sections are actually live facts or operational state

Do not split blindly. Start from the real fault lines in the document.

## Step 2: Draft The Entry Point

Create one index note that answers:

- what this graph covers
- what it does not cover
- which clusters exist
- where the agent should start for the current task

This note replaces the old habit of reading the whole file.

## Step 3: Create The First MOC

Add only the MOC that is needed right now.

Most migrations do not need three or four MOCs on day one. One well-written MOC is often enough to break the monolith safely.

## Step 4: Split Only The Highest-Pressure Sections

Move out the sections that most obviously deserve their own note:

- repeated decisions
- large examples
- anti-patterns
- domain-specific methods

Leave low-value detail in place until there is a reason to separate it.

## Step 5: Replace Headings With Links That Carry Reasons

When moving content out of the original file, do not leave behind bare headings and dead stubs.

Replace them with links in prose that say why the next note matters.

## Step 6: Mark Open Questions

If the old file hid uncertainty, the migration should make that visible instead of polishing it away.

Create `open-question` notes or a short unresolved section in the index or MOC.

## Step 7: Stop Early

The goal is not "fully decomposed."

The goal is "easy to traverse for the next real task."
