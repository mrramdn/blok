# Changelog

Blok uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

## 0.2.2 (2026-10-24)

- The focus ring reads on every fill. It stays blue on the ground, on cards and on controls; on a fill it takes
  the fill's own text color: black on yellow, pink, mint, green and orange, white on blue and red, the ground
  color on an inverted block. The blue measured 1.0:1 on the blue card headers and 1.8:1 on the pink ones in light
  mode, and 1.1:1 to 2.4:1 on every fill in dark mode (the 35 copy and reset buttons in the gallery's card headers,
  and the demo's footer links); the lowest is now 5.2:1. `blok.css` sets it for anything placed on a `bg-*` fill,
  so no markup changes.
- The marquee has a Pause button in a cap at the end of each strip, behind a 3px rule in the strip's ink. It
  stops the strip and reads Play until it is pressed again; the strip still pauses on hover and stops under
  reduced motion, where the cap is hidden. The gallery's Marquee card keeps state now, so it has a reset button
  (12 cards, up from 11).
- `DESIGN.md`: the ring rule, the ring's contrast on cards and on each fill, the Marquee and Focus recipes, and a
  Do for anything that moves by itself. The inverted-block pair reads 20.7:1 and 16.7:1, not 21.0:1 and 18.8:1.
- The gallery's title, Blok, is its `h1`, for screen readers; it looks the same.
- The demo's home link is named "PC, Pasar Cetak, home". Its name now starts with the PC mark it shows, which is
  all a phone shows of it, so a voice user can say what they see (WCAG 2.5.3). It looks the same.
- Figma: not changed in this release; the Marquee component still shows the strip without its Pause button.

## 0.2.1 (2026-10-14)

- The gallery groups its 24 components under category headings (Actions, Content, Input, Navigation, Feedback;
  `type-h2` in capitals) instead of a row of filter chips under the header. Card names are `h3`.
- Figma: the galleries had no filter row to remove; their only chip row is the Chip component's own sample,
  which stays.

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
