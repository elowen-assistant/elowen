# Codex Workspace Guide

This directory is the workspace-level source of truth for Codex-specific guidance that applies across Elowen repositories.

Use this area for:

- shared instructions that apply to the whole Elowen system
- cross-repo development rules
- playbooks for recurring workflows
- skill definitions or skill drafts that are broader than one service repo

Keep service-specific guidance in the owning repository. Keep cross-repo guidance here.

## Layout

- `instructions/` - shared rules and operating guidance
- `playbooks/` - step-by-step workflows for recurring tasks
- `notes/` - dated session handoff notes and restart context
- `skills/` - workspace-level skills or skill drafts

## Maintenance Rule

When a new cross-repo convention or recurring workflow appears during development, update this directory in the same change or immediately after it. This repository should stay current with how Elowen is actually being built.
