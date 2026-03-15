# Skill Graph Playbook

`skill-graph-playbook` is a small, portable repository for agents that need to design markdown skill graphs instead of stuffing everything into one `SKILL.md`.

The repo includes one installable skill, `build-skill-graphs/`, plus templates, patterns, anti-patterns, hybrid architecture guidance, and a small example graph you can adapt.

## Who This Is For

Use this repo if you are working with:

- agent skills that have outgrown a single instruction file
- knowledge-heavy domains that need orientation, tradeoffs, and traversal paths
- reusable operating knowledge that should stay legible in plain markdown
- hybrid systems where markdown holds methods and a database holds live state

## Why This Exists

Some skills are simple enough to fit in one file. Deeper domains are not.

Skill graphs let an agent work with:

- an entrypoint note that orients the task
- MOCs that group clusters of related knowledge
- atomic notes that each hold one method, tradeoff, or claim
- wiki links in prose that explain why the next note matters

This repo keeps that idea small and reusable instead of turning it into a full plugin or vault generator.

## When Not To Use Skill Graphs

Skill graphs are useful when an agent needs to move through a domain, not just store a checklist.

You probably do not need a skill graph if:

- the full workflow fits cleanly in one `SKILL.md`
- the task is mostly procedural and rarely changes
- you need live mutable records more than explanatory notes
- the extra linking and maintenance would outweigh the benefit of better navigation

## Repo Layout

```text
skill-graph-playbook/
  build-skill-graphs/
    SKILL.md
    agents/openai.yaml
    references/
      templates.md
      patterns.md
      anti-patterns.md
      hybrid-architecture.md
      example-graph/
        knowledge-work.md
        graph-structure-moc.md
        agent-cognition-moc.md
        hybrid-architecture-moc.md
        progressive-disclosure.md
        links-carry-reasons.md
        mocs-orient-attention.md
        markdown-stores-methods.md
        typed-stores-hold-live-state.md
        maintenance-keeps-mocs-trustworthy.md
```

## Install

### Codex

If the built-in skill installer is available, install directly from GitHub:

```bash
python "$CODEX_HOME/skills/.system/skill-installer/scripts/install-skill-from-github.py" --repo ksanjeevein-maker/skill-graph-playbook --path build-skill-graphs
```

Windows PowerShell example:

```powershell
python "$env:CODEX_HOME\\skills\\.system\\skill-installer\\scripts\\install-skill-from-github.py" --repo ksanjeevein-maker/skill-graph-playbook --path build-skill-graphs
```

### Antigravity / Gemini CLI

Copy the `build-skill-graphs/` folder into your workspace or global skills directory, such as `.agent/skills/` or `~/.gemini/antigravity/skills/`, then restart the agent session.

### Manual

Clone the repo and copy only the skill folder if you prefer:

```bash
git clone https://github.com/ksanjeevein-maker/skill-graph-playbook.git
```

## Quick Start Path

If you want the fastest path through the repo, read in this order:

1. `build-skill-graphs/SKILL.md`
2. `build-skill-graphs/references/templates.md`
3. `build-skill-graphs/references/patterns.md`
4. `build-skill-graphs/references/anti-patterns.md`
5. `build-skill-graphs/references/example-graph/knowledge-work.md`

That sequence gives you the framing, the construction pattern, the common traps, and a concrete example graph.

## Use It

Example prompts:

- `Use $build-skill-graphs to turn this oversized SKILL.md into a small graph.`
- `Use $build-skill-graphs to design an entrypoint, two MOCs, and five atomic notes for a legal workflow domain.`
- `Use $build-skill-graphs to decide what belongs in markdown versus SQLite for this company knowledge system.`
- `Use $build-skill-graphs to create a graph for an operations handbook where links explain why the next note matters.`

## Inspiration

This repo is inspired by the broader idea behind skill graphs and by knowledge-graph-native agent systems such as Ars Contexta, but the contents here are intentionally smaller and easier to remix.
