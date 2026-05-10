---
name: Design.md global rule — scaffold via templates
description: Global CLAUDE.md triggers project scaffolding via templates in ~/.claude/templates/ — don't put heavy content in the global file itself.
type: feedback
---

Global CLAUDE.md is lean (~50 lines). It contains only:
- Karpathy 4 principles
- Communication style
- Bootstrap trigger rules pointing to templates

Templates live in `~/.claude/templates/` and are read only once per project:
- `project-claude-template.md` → generates `/project/CLAUDE.md`
- `project-design-template.md` → generates `/project/design.md` (Google Labs standard)

**Why:** Global CLAUDE.md loads on every message; keeping it lean minimizes token cost. Heavy content (YAML examples, long question lists) belongs in templates that are read once.

**How to apply:** On any new project without a CLAUDE.md or design.md, read the relevant template, ask the questions, generate the file. After that, use only the project files.
