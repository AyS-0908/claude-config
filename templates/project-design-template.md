# Template — Project design.md

## Purpose
Use this template to generate a `/project/design.md` for any new web/frontend project.
Ask the user each question below, then produce the file using the Google Labs Design.md standard.

---

## Questions to ask the user

1. **Project name** — Used as the `name` token in the YAML front matter.
2. **Color palette** — Primary, secondary, accent, neutral. Hex values if known; otherwise describe the desired mood (e.g. "dark and serious", "warm and human", "bright and minimal").
3. **Typography** — Heading font and body font. Style preference: serif, sans-serif, or monospace. Any specific font names (Google Fonts, system fonts)?
4. **Visual ambiance** — Choose one or describe: épuré/minimal · chaleureux/humain · corporate/institutionnel · audacieux/créatif · autre.
5. **Logo / brand assets** — URL, file path, or textual description. If none, say so.
6. **UI references or inspirations** — Sites, apps, or screenshots the user finds appealing.
7. **Border radius** — Sharp (0–2 px) · Soft (4–8 px) · Rounded (12 px+).
8. **Spacing density** — Compact · Standard · Airy.
9. **Any do's and don'ts** — Explicit visual rules (e.g. "no gradients", "never use red", "always left-align text").

---

## Output format

Generate `design.md` following the Google Labs Design.md standard (https://github.com/google-labs-code/design.md):

```markdown
---
name: ProjectName
colors:
  primary: "#XXXXXX"
  secondary: "#XXXXXX"
  accent: "#XXXXXX"
  neutral: "#XXXXXX"
typography:
  h1:
    fontFamily: "Font Name"
    fontSize: "3rem"
    fontWeight: 700
    lineHeight: 1.2
  h2:
    fontFamily: "Font Name"
    fontSize: "2rem"
    fontWeight: 600
  body-md:
    fontFamily: "Font Name"
    fontSize: "1rem"
    lineHeight: 1.6
  label:
    fontFamily: "Font Name"
    fontSize: "0.75rem"
    fontWeight: 500
rounded:
  sm: 4px
  md: 8px
  lg: 16px
spacing:
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.md}"
    padding: "12px 24px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.accent}"
    border: "1px solid {colors.accent}"
    rounded: "{rounded.md}"
    padding: "12px 24px"
  card:
    backgroundColor: "{colors.neutral}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
---

## Overview
[Describe the visual identity in 2–3 sentences: what feeling it conveys, what references inspired it.]

## Colors
[Explain each color's role and usage.]

## Typography
[Explain font choices and hierarchy rationale.]

## Layout
[Grid system, max-width, column structure, responsive breakpoints.]

## Elevation & Depth
[Shadow usage, z-index conventions, layering approach.]

## Shapes
[Border radius usage, any geometric motifs.]

## Components
[Usage guidance for key components: buttons, cards, forms, navigation.]

## Do's and Don'ts
[Explicit visual rules derived from user answers.]
```

---

## Rules after generation
- `design.md` is the single source of truth for all frontend decisions.
- Every color, font, spacing, and component style must reference its tokens.
- Do not deviate without updating `design.md` first and confirming with the user.
