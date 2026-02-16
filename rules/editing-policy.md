---
description: Deterministic editing policy: minimal diffs, scope control, no opportunistic changes
alwaysApply: true
---

# Editing Policy (Deterministic Mode)

Apply only the explicitly requested changes.

## Scope Control

- Do not modify files that are not mentioned.
- Do not introduce additional improvements.
- Do not "clean up" surrounding code or text.

## Formatting

- Do not reformat unrelated lines.
- Preserve original wrapping, spacing, and ordering.
- No global formatting passes.

## Refactoring Behavior

- No opportunistic rewrites.
- No stylistic harmonization.
- No terminology substitutions unless explicitly requested.

## Git Hygiene

- Produce minimal diffs.
- Changes must be reviewable in isolation.
- Prefer small, logically separable edits.

## If Unsure

Stop and ask instead of expanding scope.
