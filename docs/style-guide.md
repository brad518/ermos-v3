# ERMOSV3 — Style Guide

A from-scratch site in the **deep-tech minimalism** language distilled from odinn.com,
applied to Ermos (sovereign, on-premises AI appliance).

## Design thesis
The hardware is the hero. Sell it like a museum object, not a product photo.
Restraint is the luxury signal: one typeface family, one weight, near-monochrome,
a single accent used sparingly. Whitespace and slow reveals do the talking; copy is
sparse, confident, and spatial.

## Open decision — palette direction
- **Light (ODINN-faithful):** near-white ground, near-black ink, one electric-blue accent.
- **Dark (Ermos-brand):** midnight ground, off-white ink, electric-blue accent.
The scaffold is token-driven (`:root` vars + `[data-theme]`) so this is a one-line flip.
Default in the current scaffold: **light**. Confirm before the full build.

## Color (tokens)
Light:  `--bg #FAFAFA` · `--surface #FFFFFF` · `--ink #0A0A0A` · `--muted #6B6B6B` · `--line rgba(0,0,0,.12)`
Dark:   `--bg #0B0F14` · `--surface #10151D` · `--ink #F2F5F9` · `--muted #8B93A1` · `--line rgba(255,255,255,.12)`
Accent (both): `--accent #0032FF` (ODINN electric blue) — reserve for **one** moment per view.
Deep accent (optional): `#01004A`.

## Type
- Display/body: **Space Grotesk** (technical grotesque; stands in for ODINN's "NewScience").
- Labels/nav/eyebrows/specs: **Space Mono** (monospace = instant deep-tech credibility).
- **One weight discipline:** 400 as default; 500 only for the rare emphasis. No bold.
- Hierarchy comes from **size + contrast**, not weight. Headings modest (hero ~clamp 40–64px).
- No uppercasing tricks and minimal letter-spacing — the mono face carries the "engineered" tone.

## Product-shot rules
- Desaturated / clay-render treatment, shot **large and cropped**, on a plain ground.
- Prefer **video** (muted, looped, or scroll-scrubbed) for beauty shots and reveals.
- One product moment per section; never busy.

## Motion
- Slow, deliberate scroll reveals (fade/rise). Respect `prefers-reduced-motion`.
- No scattered effects; one orchestrated moment per section.

## Voice
- Proprietary + curated framing (™ terms, "two iconic products").
- Benefits as **places/objects**: "in your building", "on your desk", "off the cloud entirely".
- Short, declarative, confident. Cut ~30% of what you'd normally write.

## What to keep from Ermos
- The security/sovereignty story needs **more proof + persuasion** than ODINN's gallery approach.
- Dominion box is already the natural hero object.
- Deploy pattern (when ready): new public repo under `brad518` + GitHub Pages (as with `ermos-preview`).
