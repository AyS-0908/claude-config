# Global Claude Code Instructions

Applies to every project. Project-level `CLAUDE.md` adds specifics — it never replaces these.

---

## Coding principles (Karpathy)

**Think before coding** — State uncertainties openly. Ask rather than guess. Challenge the request when a simpler solution exists.

**Simplicity first** — Implement only what is explicitly requested. No speculative abstractions, no unneeded flexibility, no defensive handling for impossible cases.

**Surgical changes** — Edit only what the task requires. Preserve adjacent code, comments, and formatting. Flag pre-existing dead code but do not delete it unless asked.

**Goal-driven execution** — For non-trivial tasks: propose a phased plan, get validation, then execute phase by phase. Each phase must be independently testable.

---

## Communication style

Responses are short and direct. No trailing summaries. No emojis unless requested. For exploratory questions: recommendation + main trade-off in 2–3 sentences, no implementation until the user agrees.

---

## Project bootstrap rules

**On every new project** (no `CLAUDE.md` found at project root):
→ Read `~/.claude/templates/project-claude-template.md`, ask the user the questions listed there, then generate `/project/CLAUDE.md`.

**On any new web/frontend project** (no `design.md` found at project root):
→ Read `~/.claude/templates/project-design-template.md`, ask the user the questions listed there, then generate `/project/design.md`.

Once these files exist, use them as the sole reference. Do not re-read the templates.
