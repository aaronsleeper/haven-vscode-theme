# Haven VS Code Theme

VS Code color theme extension derived from the Haven brand design system.

## Source of truth

All color values come from `../cena-health-brand/_tokens/color.md` and the
accessibility audit at `../cena-health-brand/audits/accessibility-audit.md`.

## Key constraints

- Editor background is `#FBFAF8` (light) / `#0D322D` (dark) — never pure white or neutral gray
- All syntax colors must pass WCAG AA (4.5:1) against their respective backgrounds
- Interactive fill uses teal-400 (`#1B685E`), not teal-500 (`#3A8478`) — per audit R1
- Syntax hue logic: teal = structure (keywords, types, tags), sage = organic (functions, decorators), warm amber = values (strings), slate blue = constants (numbers)
- ANSI magenta slots use warm red — the brand has no purple

## Files

- `themes/cena-health-light.json` — light theme (warm off-white ground)
- `themes/cena-health-dark.json` — dark theme (chromatic dark ground)

## Testing

1. Open this folder in VS Code
2. Press F5 to launch Extension Development Host
3. Cmd+K Cmd+T → select "Haven Light" or "Haven Dark"

## Do not

- Use `#FFFFFF` or `#000000` anywhere — always use brand chromatic values
- Use teal-500 (`#3A8478`) for text at normal sizes — fails AA
- Add non-brand purples or bright colors to the ANSI palette
