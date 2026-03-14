# Skill Graph Playbook

`skill-graph-playbook` is a small, portable repository for agents that need to design markdown skill graphs instead of stuffing everything into one `SKILL.md`.

The repo includes one installable skill, `build-skill-graphs/`, plus templates, patterns, anti-patterns, hybrid architecture guidance, and a small example graph you can adapt.

## Why This Exists

Some skills are simple enough to fit in one file. Deeper domains are not.

Skill graphs let an agent work with:

- an entrypoint note that orients the task
- MOCs that group clusters of related knowledge
- atomic notes that each hold one method, tradeoff, or claim
- wiki links in prose that explain why the next note matters

This repo keeps that idea small and reusable instead of turning it into a full plugin or vault generator.

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

### Antigravity / Gemini CLI

Copy the `build-skill-graphs/` folder into your workspace or global skills directory, such as `.agent/skills/` or `~/.gemini/antigravity/skills/`, then restart the agent session.

### Manual

Clone the repo and copy only the skill folder if you prefer:

```bash
git clone https://github.com/ksanjeevein-maker/skill-graph-playbook.git
```

## Use It

Example prompts:

- `Use $build-skill-graphs to turn this oversized SKILL.md into a small graph.`
- `Use $build-skill-graphs to design an entrypoint, two MOCs, and five atomic notes for a legal workflow domain.`
- `Use $build-skill-graphs to decide what belongs in markdown versus SQLite for this company knowledge system.`

## Inspiration

This repo is inspired by the broader idea behind skill graphs and by knowledge-graph-native agent systems such as Ars Contexta, but the contents here are intentionally smaller and easier to remix.
