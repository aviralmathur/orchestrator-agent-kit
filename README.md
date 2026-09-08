# Orchestrator Agent Kit

A portable chief-of-staff orchestrator agent for Claude Code, extracted from a live
deployment running daily since August 2026.

**`SKILL.md`** is the whole thing — self-contained, no external files required.

## Install (3 steps)

1. Copy the folder into your skills directory:

   ```bash
   cp -r orchestrator-agent-kit ~/.claude/skills/orchestrator
   ```

2. Open `SKILL.md` and replace the seven placeholders in §0 (`{{AGENT}}`,
   `{{PRINCIPAL}}`, `{{ORG}}`, etc.). Nothing else needs editing to get a working agent.

3. Start a Claude Code session and say *"brief me"* — or invoke it as
   `/orchestrator`. Rename the folder and the frontmatter `name:` if you want a
   different invocation.

## What to read first

- **§3 Prime directives** — the safety envelope. Do not relax these.
- **§6.1 The never-miss list** — fill this in before your first run. It has the
  shortest path to a real failure.
- **§9 Failure modes** — the most valuable section, and the one you have to earn.
  Add to it every time something goes wrong.

## Recommended posture for week one

Run it **draft-only, no send**. Relax to per-item send approval once the drafts are
consistently good. Never relax past per-item.

## Splitting it up later

§1 explains the three-layer structure (pointer → charter → shared fleet rules) that
the source deployment uses across fourteen agents. Start as one file; split once you
have a second agent, because the moment a rule lives in two places one of them is
already wrong.
