---
description: Coding standards: typography, language, deterministic editing
alwaysApply: true
---

# AI Rules — Code Generation Standards

Explicit user requests override these rules.

## Typography

Use Title Case for all user-visible headings and titles.
Do not alter casing inside code, filenames, identifiers, or verbatim text.

## Language

When using English, use American English unless explicitly requested otherwise.

All source code must use **English** for any developer-defined natural-language elements, including:

- Comments
- Identifiers (variables, functions, classes, modules, etc.)
- String literals intended for humans (e.g., log messages, errors)
- Documentation and docstrings
- Commit messages and inline explanations

This requirement applies only where wording is developer-defined, not where constrained by a library, standard, or external interface.

## Editing Policy

Apply only the explicitly requested changes (deterministic mode).

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
