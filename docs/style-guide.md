# Ermos V3 — Style Guide (Compliance-Plate System)

The approved visual system for the Ermos V3 site. Supersedes the earlier ODINN-derived
scaffold guide. Companion to `ERMOS-V3-DESIGN-BRIEF.md` (banned looks, hero rules,
drift checks) and `ERMOS-V3-BRIEF.md` (narrative, copy) — the briefs win on any conflict.

## Design thesis

Dominion is PHYSICAL in a category full of vapour. The design borrows from the two
paper worlds the buyer already trusts: the spec plate riveted to a machine, and the
deed in the safe. Permanent, physical, discreet, engineered, Australian-professional.
No cloud-AI vernacular: no gradients, glassmorphism, glows, floating abstractions.

## Colour tokens (approved)

| Token     | Hex       | Role |
|-----------|-----------|------|
| Limestone | `#EBEAE6` | Page ground — plinth / spec-paper grey. Not SaaS white, not cream. |
| Plate     | `#EFEEEA` | Plate/surface fill (pricing plates). |
| Gunmetal  | `#191C1F` | Ink; the single dark "vault" band; hero stage is `#111316`. |
| Graphite  | `#54595F` | Secondary text. |
| Brass     | `#8A6D3B` | THE accent — used as engraved material (plate borders, register numbers, markers, key data). Never as glow, gradient or button fill. |
| Rule      | `#B8B5AE` | Solid section rules. Spec sheets use real lines, not 12% hairlines. |

## Type

- **Display: Libre Caslon Text** — the letterform of deeds and contracts. Headlines,
  register headings, plate price figures, FAQ questions.
- **Body: Source Sans 3** — plain, engineered, invisible. Weight 400; 600 only for
  buttons/brand.
- **Data: IBM Plex Mono** — DATA ONLY (serials, ABN, prices, time codes, spec labels,
  register numbers). Never decorative eyebrows.

## Structure

- Full-bleed photographic hero (five hard rules in the design brief).
- Below the hero the page runs as a **numbered register 01–06** matching the six
  narrative beats. Numbering encodes the agreed sequence — that is why it is allowed.
- Square corners. Solid rules. No shadows. No pills. No icons.
- One dark band per page (security = the vault). Everything else on limestone.
- **Signature element (singular): pricing as engraved compliance plates** — model
  header strip, small-label/big-value spec pairs, EVERYTHING INCLUDED list with brass
  square markers, labelled price rows with large serif figures, agreement note.

## Reference board (added 2026-07-13, from Brad)

Two brand references Brad supplied as the target look and feel. Both confirm the
current direction; capture their ideas for future work:

**1. "Cognition" — modular mark, engineering-sheet layout**
- Solid near-black geometric logomark (modular hexagon cluster) over warm off-white.
- Lowercase grotesque wordmark; thin vertical hairline dividers between lockups;
  full-width ruled bands framing section titles.
- Ideas to use: a **partner/trust strip** of single-colour lockups separated by
  vertical rules; ruled title bands; the modular-cluster motif suits "concentrated
  intelligence" if Ermos ever wants a secondary mark.

**2. "Accumulate" — roundel cube mark, serif wordmark**
- Solid black roundel containing a white isometric **cube with a directional facet**
  — almost literally "a box", perfect precedent for a Dominion product mark.
- High-contrast serif wordmark (Caslon-adjacent) — independent validation of our
  Libre Caslon display choice.
- Ideas to use: a **Dominion logomark** = isometric box, single colour (gunmetal on
  limestone, reversed on the vault band), bare or in a roundel. Could sit in the nav,
  the plate header, and as favicon.

**Colours extracted from the references**
- Bone `#F2F0EB` — warm paper ground seen in both. Adopted as an *optional warm
  surface* variant sitting between Limestone and Plate; use for reference boards,
  print, or the security-brief document styling. Do not replace Limestone on the site
  without a deliberate pass.
- Mark black `#121212` — flat ink for logomarks (slightly deeper than Gunmetal text).
- Chartreuse sliver (~`#C8D92E`, visible as an edge rule in the Accumulate board) —
  **NOT adopted.** The design brief's banned look #2 rules out an acid-green accent,
  and Brass is the committed accent. Recorded here only as provenance. If Brad ever
  wants chartreuse instead of brass, that is an explicit brief change he must call.

## Logo / lockup rules (new, derived from the references)

- Marks are always single-colour, flat, geometric. No gradients, outlines or glows.
- Wordmark: letterspaced caps (current nav treatment) or Caslon for print contexts.
- On limestone: mark black `#121212`. On gunmetal/vault: paper `#F3F1EC`.
- One mark per surface; never mark + decorative graphic together.

## Product imagery

- Hero: full-bleed shot, desaturated, no blue glow (current 640px render is seated on
  a matching dark stage and edge-masked — replace when real photography exists).
- Wanted: the box in a real office, natural light, timber/plaster context.

## Motion & quality floor

- One restrained load animation (hero). Scroll reveals are opacity-only, 0.7s.
- `prefers-reduced-motion` respected (video pauses, reveals off).
- Responsive to 360px; hero tested at 360 / 768 / 1366 / 1920.
- Visible keyboard focus: 2px brass outline.
- Australian English. No em-dashes in visible copy. No hype adjectives.

## Deploy

- Work on `main`; push to `main` auto-deploys https://brad518.github.io/ermos-v3/
  (rebuild ~60–90s). The `ERMOS-V3` branch and its Actions workflow are stale/broken —
  do not use without fixing.
