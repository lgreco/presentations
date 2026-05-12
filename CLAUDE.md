# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A collection of course presentation slides authored in **Marp** — Markdown files with Marp frontmatter that render as slide decks. Slides are organized by course in subdirectories (e.g., `COMP/` for computing/programming courses).

## Rendering slides

Marp is not installed as a local package; use the CLI via `npx`:

```bash
# Live preview in browser
npx @marp-team/marp-cli --preview COMP/first_day_of_classes.md

# Export to HTML
npx @marp-team/marp-cli COMP/first_day_of_classes.md -o out.html

# Export to PDF
npx @marp-team/marp-cli COMP/first_day_of_classes.md -o out.pdf
```

Alternatively, install the **Marp for VS Code** extension for in-editor preview.

## Slide file conventions

Every presentation file starts with this frontmatter block:

```yaml
---
marp: true
theme: default
_class: lead
paginate: true
transition: fade
---
```

- Slides are separated by `---` (horizontal rule).
- The first slide is the title slide (uses `_class: lead`).
- Course-specific subdirectories group related decks (e.g., `COMP/` for Leo's computing courses).

## Authoring notes

- Leo Irakliotis is the instructor. Slides address students directly.
- The course uses **Ungrading**: self-evaluation and reflection replace traditional grading. Keep this framing consistent when editing or adding content.
- Anonymous feedback is a standing feature of the course — preserve references to it when restructuring slides.
