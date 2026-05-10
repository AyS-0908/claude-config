# Template — Project CLAUDE.md

## Purpose
Use this template to generate a `/project/CLAUDE.md` for a new project.
Ask the user each question below, then produce the file using their answers.
Omit any section that does not apply to this project.

---

## Questions to ask the user

1. **Project name and one-sentence description** — What is this project and what does it do?
2. **Target audience** — Who uses it? (CEOs, developers, end consumers…)
3. **Tech stack** — Language(s), framework(s), runtime, package manager.
4. **Entry point and build commands** — How do you start the dev server? How do you build? How do you run tests?
5. **Key files or directories** — Any non-obvious structure worth knowing (e.g. where pages live, where config lives)?
6. **Hard constraints** — What must never be done? (e.g. no CDN, single HTML file, no database, specific browser support)
7. **Deployment target** — Where does it run? (Vercel, VPS, local only…)
8. **Phased plan** — Should implementation follow a validated phase-by-phase approach? (default: yes)

---

## Output format

Generate the file as follows, filling in the user's answers:

```markdown
# CLAUDE.md — [Project Name]

## Project
[One-sentence description. Target audience.]

## Stack
[Language, framework, runtime, package manager]

## Commands
- Dev: `[command]`
- Build: `[command]`
- Test: `[command]`

## Structure
[Key files/directories if non-obvious]

## Hard constraints
[List constraints — one per line]

## Deployment
[Target environment]

## Workflow
[Phase-by-phase if applicable: describe the phases and validation gates]
```
