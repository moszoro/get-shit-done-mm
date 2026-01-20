---
created: 2026-01-20T01:41
title: Rewrite Phase 6 as repository contribution
area: planning
files:
  - ~/.claude/get-shit-done/references/security-compliance.md
  - ~/.claude/get-shit-done/references/tdd.md
  - ~/.claude/commands/gsd/new-project.md
  - ~/.claude/get-shit-done/workflows/verify-phase.md
  - ~/.claude/agents/gsd-planner.md
---

## Problem

Phase 6 (TDD-First Workflow & Security Compliance) was implemented directly to the GSD installation at `~/.claude/`. These changes need to be converted into proper repository contributions so they can be:
- Tracked in git with the main GSD repo
- Reviewed and merged via PR
- Available to other GSD users

Current implementation exists only in local GSD install, not in the get-shit-done-mm repository files.

## Solution

1. Copy modified files from `~/.claude/` to their corresponding locations in the repository
2. Update the repo's template/reference files to match GSD install structure
3. Create PR with Phase 6 changes:
   - references/security-compliance.md (new)
   - references/tdd.md (updated with test_categories)
   - commands/gsd/new-project.md (updated with security question)
   - workflows/verify-phase.md (updated with quality step)
   - agents/gsd-planner.md (updated with TDD-first enforcement)
