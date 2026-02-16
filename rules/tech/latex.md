---
description: LaTeX formatting rules for dashes and line breaks
globs: "**/*.tex"
alwaysApply: false
---

# LaTeX Style (Apply **Only** to LaTeX Content)

## Applicability Gate (MUST be checked before applying)

These rules apply **exclusively** to LaTeX documents.

Apply this rule **only if at least one condition holds**:
- The file being edited has the extension `.tex`.
- The content clearly contains LaTeX syntax (e.g., `\begin{}`, `\section{}`, math mode `$...$`, `\cite{}`, etc.).

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

- Always use ASCII dashes:
  - `---` for em dashes
  - `--` for en dashes
  Never use Unicode dashes (`—`, `–`).

- Write exactly **one sentence per line**.
  - A new line is inserted only after a true sentence terminator (`.`, `?`, `!`).
  - A semicolon (`;`) does **not** end a sentence and must **not** trigger a line break.
  - Do not join sentences onto the same line.
  - Do not reflow paragraphs into wrapped text.

## Non-Goals (Do NOT do this)

- Do not introduce new packages.
- Do not modify macros.
- Do not change math formatting.
- Do not “improve” prose or style.
- Do not reorder content.