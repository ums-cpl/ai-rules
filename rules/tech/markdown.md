---
description: Markdown formatting rules — one sentence per line, formatting only
globs: "**/*.md", "**/*.markdown"
alwaysApply: false
---

# Markdown Style (Apply **Only** to Markdown Content)

## Applicability Gate (MUST be checked before applying)

These rules apply **exclusively** to Markdown documents.

Apply this rule **only if at least one condition holds**:
- The file being edited has the extension `.md` or `.markdown`.
- The content clearly uses Markdown syntax (e.g., headings with `#`, lists with `-` or `*`, code fences ` ``` `, links `[text](url)`, emphasis `` `…` `` / `` `…` ``, etc.).

If the content is **not** Markdown:
→ **Do not apply these rules. Ignore this document entirely.**

If unsure whether the content is Markdown:
→ **Do not apply the rules.**

## Precedence

Explicit user instructions override these rules.

## Scope

These rules affect **formatting only**.  
Do **not** rewrite wording, change semantics, or refactor structure.

## Rules

- Write exactly **one sentence per line**.
  - A new line is inserted only after a true sentence terminator (`.`, `?`, `!`).
  - A semicolon (`;`) does **not** end a sentence and must **not** trigger a line break.
  - Do not join sentences onto the same line.
  - Do not reflow paragraphs into wrapped text.

## Non-Goals (Do NOT do this)

- Do not change heading levels.
- Do not alter list structure.
- Do not add or remove emphasis.
- Do not rewrite link text or URLs.
- Do not "improve" prose or style.
- Do not reorder content.
