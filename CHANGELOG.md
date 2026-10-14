# Changelog

Blok uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

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
