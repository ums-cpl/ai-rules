---
description: Base rules: typography, language, deterministic editing
alwaysApply: true
---

# Base Rules

Explicit user requests override these rules.

## Typography

Use Title Case for all user-visible headings and titles.
Do not alter casing inside code, filenames, identifiers, or verbatim text.

## Language

When using English, use American English unless explicitly requested otherwise.

All source code---including comments, identifiers, strings (e.g., error messages), and documentation---is to be written in English unless explicitly requested otherwise.

## Editing Policy (Deterministic Mode)

Apply only the explicitly requested changes.

### Scope Control

- Do not modify files that are not mentioned.
- Do not introduce additional improvements.
- Do not "clean up" surrounding code or text.

### Code Formatting

- Do not reformat unrelated lines.
- Preserve original wrapping, spacing, and ordering.
- No global formatting passes.

### Refactoring Behavior

- No opportunistic rewrites.
- No stylistic harmonization.
- No terminology substitutions unless explicitly requested.

### Git Hygiene

- Produce minimal diffs.
- Changes must be reviewable in isolation.
- Prefer small, logically separable edits.

### If Unsure

Stop and ask instead of expanding scope.
