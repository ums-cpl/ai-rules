---
description: Code generation standards for HPC and common source languages
globs:
  - "**/*.{c,h,cpp,hpp,cc,cxx,hh,cu,cuh,cl,hip,f,for,f90,f95,f03,f08,F,F90,py,ts,tsx,js,jsx,rs,go,java,kt,swift,m,mm}"
alwaysApply: false
---

# AI Rules — Code Generation Standards

Explicit user requests override these rules.

## Typography

Use Title Case for all user-visible headings and titles.
Do not alter casing inside code, filenames, identifiers, or verbatim text.

## Mathematical Typesetting

1. Always express mathematical objects using LaTeX math delimiters.
2. Use `$...$` for inline math and `$$...$$` for block math.
3. Avoid Unicode math symbols.
4. Prefer semantic macros (`\sum`, `\otimes`, `\mathcal`, etc.).

## Language

When using English, use American English unless explicitly requested otherwise.

All source code must use **English** for any developer-defined natural-language elements, including:

1. Comments
2. Identifiers (variables, functions, classes, modules, etc.)
3. String literals intended for humans (e.g., log messages, errors)
4. Documentation and docstrings
5. Commit messages and inline explanations

This requirement applies only where wording is developer-defined, not where constrained by a library, standard, or external interface.

## Editing Policy

Apply only the explicitly requested changes (deterministic mode).

### Scope Control

1. Do not modify files that are not mentioned.
2. Do not introduce additional improvements.
3. Do not "clean up" surrounding code or text.

### Code Formatting

1. Do not reformat unrelated lines.
2. Preserve original wrapping, spacing, and ordering.
3. No global formatting passes.

### Refactoring Behavior

1. No opportunistic rewrites.
2. No stylistic harmonization.
3. No terminology substitutions unless explicitly requested.

### Git Hygiene

1. Produce minimal diffs.
2. Changes must be reviewable in isolation.
3. Prefer small, logically separable edits.

### If Unsure

Stop and ask instead of expanding scope.
