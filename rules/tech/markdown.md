---
description: Markdown formatting — one sentence per line; formatting only
globs:
  - "**/*.{md,markdown}"
alwaysApply: false
---

# Markdown Style (Apply **Only** to Markdown Content)

## Applicability Gate (MUST be checked before applying)

These rules apply **exclusively** to Markdown documents.

Apply this rule **only if at least one condition holds**:

1. The file being edited has the extension `.md` or `.markdown`.
2. The content clearly uses Markdown syntax (e.g., headings with `#`, lists with `-` or `*`, code fences, links `[text](url)`, emphasis, etc.).

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

1. Write exactly **one sentence per line**.
1.1. A new line is inserted only after a true sentence terminator (`.`, `?`, `!`).
1.2. A semicolon (`;`) does **not** end a sentence and must **not** trigger a line break.
1.3. Do not join sentences onto the same line.
1.4. Do not reflow paragraphs into wrapped text.

## Non-Goals (Do NOT do this)

1. Do not change heading levels.
2. Do not alter list structure.
3. Do not add or remove emphasis.
4. Do not rewrite link text or URLs.
5. Do not "improve" prose or style.
6. Do not reorder content.
