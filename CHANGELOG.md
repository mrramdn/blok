# Changelog

Blok uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

## 0.2.0 (2026-10-14)

A blank component sheet and an example screen.

- The gallery is a blank template: every card shows neutral placeholder content ("Save", "Email", "Option A",
  "Plan name", "00") instead of the invented print fair, and shows the variants and states its recipe defines
  (disabled toggle, slider, radio and checkbox, the error and disabled field, six badge statuses). 24 live
  components, up from 22, with copy on every card and reset on the 11 that keep state.
- `DESIGN.md` has 24 recipes, up from 22, with the same neutral markup as the gallery. New: Button variants
  (destructive, ghost, small, disabled) and Text field states (error, disabled). The front matter gains
  `button-destructive`, `button-ghost`, `button-ghost-hover` and `button-small`.
- `preview/demo.html`: an event landing page for an invented two-day print and zine fair in Bandung, built only
  from the recipes (17 kinds of component). `preview/input.css` scans it too.
- Figma: neutral text in the components, both galleries and the cover. Button gains the Destructive and Ghost
  variants (40 variants, up from 24), Badge gains Success, Destructive and Outline (8 tones), Single selection
  gets a Show figure property, and Progress shows its own value. 26 components with 116 variants. A new page
  Example holds `Example/Light` and `Example/Dark`, the landing page rebuilt from 53 instances each.
- Fixes: squares on the yellow marquee are `bg-primary-foreground`, so they stay black in dark mode; the
  newsletter field no longer collapses when the button sits under it in a narrow container; card headers in
  the gallery line up with the 24px body padding; a field error is a red block with white text, because red
  text on the dark card reaches only 3.4:1.

## 0.1.0 (2026-10-14)

First beta.

- Tokens in light and dark mode, in `blok.css` (Tailwind CSS v4, shadcn/ui token names, plus `pink`, `blue`,
  `mint`, `grid` and the three hard shadows) and in the front matter of `DESIGN.md`.
- `DESIGN.md` with the rules, the measured contrast of both modes and 22 recipes.
- A component gallery in `preview/` with 22 live components for an invented print fair, category filters, copy on
  every card and reset on the 11 that keep state.
- The Figma library "Blok Design System": 81 variables in four collections, 12 text styles (8 bound to the font
  variables; the four expanded ones keep Archivo's width axis instead), 3 shadow styles, 26 components with
  97 variants (the 22 recipes plus the Tab, List item, Accordion item and Step building blocks), 13 Lucide
  icons, a foundations page, and a light and a dark gallery built from instances.
