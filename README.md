# AI Rules

Project rules for AI coding assistants. Markdown (`.md`) with YAML frontmatter for portability across tools and editors.

## Structure

```
.
├── README.md
├── LICENSE
└── rules/
    ├── formatting-and-language.md
    ├── editing-policy.md
    └── latex-style.md
```

- **rules/** — Markdown rule files with optional YAML frontmatter (e.g. `description`, `globs`, `alwaysApply`).

## Usage

Clone the repo and use the rules as needed for your editor or AI assistant. Copy files from `rules/` into your project's rules directory, or reference them as documentation.

**Example (Cursor):** `Rules → New → Add from GitHub → enter this repo's URL`. Rules are installed into `.cursor/rules/`.

## Rules Overview

| Rule | Description |
|------|-------------|
| formatting-and-language | Typography (Title Case for headings); language (American English, code in English) |
| editing-policy | Deterministic editing: minimal diffs, scope control, no opportunistic changes |
| latex-style | LaTeX formatting: em/en dashes, sentence-per-line |

## Adding Rules

Add new `.md` files under `rules/`. Example frontmatter:

```yaml
---
description: Short description (shown in rule picker)
globs: "**/*.py"   # optional: only when these files are open
alwaysApply: false # true = apply in every session
---

# Rule Title

Rule content...
```

## License

MIT (see [LICENSE](LICENSE)).
