# Blok

A neo-brutalist design system: thick black outlines, hard offset shadows without blur, flat loud fills and square corners, set in Archivo and Space Mono. The same tokens exist as a Tailwind CSS v4 theme, a `DESIGN.md` that people and coding agents follow, and a Figma library.

"Blok" is a working name.

## Files

| File | What it is |
| --- | --- |
| `blok.css` | Tailwind CSS v4 theme: color tokens (light and dark), the hard shadows, radius 0, type utilities, the `blok-press` physics and the slider, checkbox, radio and grid utilities. Token names follow shadcn/ui. |
| `DESIGN.md` | The rules, the measured contrast of both modes and the component recipes, in the [design.md](https://github.com/google-labs-code/design.md) format. |
| `preview/index.html` | Component gallery built with the theme: 22 live components for a print fair, a dark mode switch, category filters, and copy and reset buttons per component. |
| `CHANGELOG.md` | What changed in each version. |

Figma: [Blok Design System](https://www.figma.com/design/XcVs9c9Dpbd7N9AIzbY5Ia) (pages Cover, Foundations and Components).

## Use it in a project

1. Load Archivo as a variable font with its width axis, and Space Mono 400 and 700. From Google Fonts:

   ```html
   <link href="https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@62..125,100..900&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet" />
   ```

   With `next/font/google`, pass `axes: ["wdth"]` for Archivo. The display and heading utilities set `font-stretch: 125%`, which only works when the width axis is loaded.

2. Copy `blok.css` next to your main stylesheet and import it after Tailwind:

   ```css
   @import "tailwindcss";
   @import "./blok.css";
   ```

3. Copy `DESIGN.md` to the project root so coding agents follow the same rules.
4. Dark mode is the `.dark` class on `<html>`.

The theme removes the default Tailwind palette, radii and shadows on purpose. Use the semantic tokens (`bg-card`, `text-muted-foreground`, `bg-primary`, `bg-pink`, `bg-blue`, `bg-mint`), the three hard shadows (`shadow-xs` on controls, `shadow-sm` on cards, `shadow-lg` on floating surfaces), `blok-press` for the lift on hover and the sink on press, and the `type-*` utilities for type.

## Preview

```sh
pnpm install
pnpm build   # writes preview/preview.css from the classes in preview/index.html
pnpm dev     # same, watching for changes
```

Then open `preview/index.html` in a browser. Copy needs a secure context, so serve the folder (`python3 -m http.server -d preview`) if the clipboard button does nothing over `file://`.

`npx @google/design.md lint DESIGN.md` checks the token file. It reports no errors. The warnings are component sub-tokens the format does not know yet (`borderColor`, `borderWidth`, `shadow`, which the recipes need), tokens that only the prose uses, and `fontStretch` on the four expanded type roles.

## Versions

The version is in `package.json`, `CHANGELOG.md` says what changed, and every release is a git tag. To release:

1. Change the files and run `pnpm build`, so `preview/preview.css` matches the gallery.
2. Raise `version` in `package.json` and add an entry to `CHANGELOG.md`.
3. Commit, tag `v<version>` (`git tag -a v0.2.0 -m "Blok 0.2.0"`) and push with `git push --follow-tags`.
4. On the design site, sync this folder and add the version to Blok's record. The site's tests fail while the
   record states a different version from the synced files.

## Where the look comes from

The look is original. It takes the vocabulary of neo-brutalist launch pages and indie product sites (thick outlines, hard shadows, flat saturated fills, heavy type) and fixes it to a small set of values: five fills, two shadow offsets, one outline color, no radius, one focus color. Archivo's width axis gives the display type its expanded shape, and Space Mono sets everything that is a label or a figure. No reference screenshot was measured; every value was chosen for this system and its contrast was computed. The demo content is an invented print and zine fair.
