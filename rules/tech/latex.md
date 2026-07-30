---
description: LaTeX formatting — ASCII dashes and one sentence per line; formatting only
globs:
  - "**/*.{tex,ltx}"
alwaysApply: false
---

# LaTeX Style (Apply **Only** to LaTeX Content)

## Applicability Gate (MUST be checked before applying)

These rules apply **exclusively** to LaTeX documents.

Apply this rule **only if at least one condition holds**:

1. The file being edited has the extension `.tex`.
2. The content clearly contains LaTeX syntax (e.g., `\begin{}`, `\section{}`, math mode `$...$`, `\cite{}`, etc.).

If the content is **not** LaTeX:
→ **Do not apply these rules. Ignore this document entirely.**

If unsure whether the content is LaTeX:
→ **Do not apply the rules.**

## Precedence

Explicit user instructions override these rules.

## Scope

These rules affect **formatting only**.
Do **not** rewrite wording, change semantics, or refactor structure.

## Rules

1. Always use ASCII dashes:
1.1. `---` for em dashes
1.2. `--` for en dashes
1.3. Never use Unicode dashes (`—`, `–`).
2. Write exactly **one sentence per line**.
2.1. A new line is inserted only after a true sentence terminator (`.`, `?`, `!`).
2.2. A semicolon (`;`) does **not** end a sentence and must **not** trigger a line break.
2.3. Do not join sentences onto the same line.
2.4. Do not reflow paragraphs into wrapped text.

## Non-Goals (Do NOT do this)

1. Do not introduce new packages.
2. Do not modify macros.
3. Do not change math formatting.
4. Do not "improve" prose or style.
5. Do not reorder content.
