# AI Rules

Project rules for AI coding assistants.
Markdown (`.md`) with YAML frontmatter for portability across tools and editors.

## Structure

```
.
├── README.md
├── CONTRIBUTING.md
├── LICENSE
└── rules/
    ├── global/
    │   └── coding-standards.md    # Typography, language, editing policy
    └── tech/
        ├── cpp.md           # C++ style (applies when .cpp files are open)
        ├── latex.md         # LaTeX formatting (applies when .tex files are open)
        ├── markdown.md      # Markdown formatting (applies when .md / .markdown files are open)
        └── python.md        # Python style (applies when .py files are open)
```

- **rules/global/** — Cross-cutting rules applied in every session.
- **rules/tech/** — Tech-specific rules (globs) applied when matching files are open.
  Each tech rule follows the same structure: Applicability Gate, Precedence, Scope, Rules, Non-Goals.

## Rule Modes

| Mode | Frontmatter | When Applied |
|------|-------------|--------------|
| Always | `alwaysApply: true` | In every session |
| Auto Attached | `alwaysApply: false`, `globs: "**/*.tex"` | When matching files are open |
| Manual | `alwaysApply: false`, no globs | Only when explicitly referenced (e.g. `@ruleName`) |

## Usage

Clone the repo and use the rules as needed for your editor or AI assistant.
Copy files from `rules/` into your project's rules directory, or reference them as documentation.

**Example (Cursor):** `Rules → New → Add from GitHub → enter this repo's URL`.
Rules are installed into `.cursor/rules/`.

## Rules Overview

| Rule | Description |
|------|-------------|
| global/coding-standards | Typography (Title Case), language (American English, code in English), deterministic editing |
| tech/cpp | *C++* style and conventions (placeholder; auto-attached for `**/*.cpp`) |
| tech/latex | *LaTeX* formatting (dashes, one sentence per line; auto-attached for `**/*.tex`) |
| tech/markdown | *Markdown* formatting (one sentence per line; auto-attached for `**/*.md`, `**/*.markdown`) |
| tech/python | *Python* style and conventions (placeholder; auto-attached for `**/*.py`) |

## Adding Rules

Add new `.md` files under `rules/global/`, `rules/tech/`, or a new category.
Each rule should state that explicit user requests override it.

Example frontmatter:

```yaml
---
description: Short description (shown in rule picker)
globs: "**/*.py"   # optional: only when these files are open
alwaysApply: false # true = apply in every session
---

# Rule Title

Rule content...
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT (see [LICENSE](LICENSE)).
