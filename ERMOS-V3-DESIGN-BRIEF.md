# ERMOS-V3-DESIGN-BRIEF.md — Visual Design Brief (companion to ERMOS-V3-BRIEF.md)

Save this in the repo root next to `ERMOS-V3-BRIEF.md`. At the start of each Claude Code session say: "Read ERMOS-V3-BRIEF.md and ERMOS-V3-DESIGN-BRIEF.md before any work."

---

## ROLE

You are the design lead on the Ermos Dominion v3 homepage rebuild (`rebuild-fullbleed` branch). Use the `frontend-design` skill. The narrative brief (ERMOS-V3-BRIEF.md) owns the copy, the six-beat structure, and the section order — you do not change those. This brief owns everything visual.

## FIRST TASK: CRITIQUE BEFORE YOU BUILD

Brad does not like the current build. Before writing any code:

1. Screenshot the current state of the branch (or render it locally and inspect).
2. List, specifically, everything that reads as an AI/template default rather than a choice made for this subject — palette, type pairing, spacing rhythm, card patterns, gradient accents, icon usage, hero treatment.
3. Present that critique plus your revised design plan (token system below) to Brad for approval BEFORE building. Do not skip this gate.

## THE SUBJECT (pinned — do not re-derive)

- **Product:** a physical AI appliance — a real box that sits inside the client's office. Sovereign, on-premises, physically incapable of leaking.
- **Audience:** managing partners and practice principals at 10–30 person Australian law, accounting, medical, and financial advice firms. Risk-averse, time-poor, allergic to startup hype. They buy from people who look like they'll still exist in ten years.
- **The page's single job:** get a sceptical principal to book a consult (secondary: the gated PDF download).
- **Mood in five words:** permanent, physical, discreet, engineered, Australian-professional.

## DESIGN DIRECTION

The distinctive material here is that Dominion is PHYSICAL in a category full of vapour. Cloud AI companies design with gradients, glassmorphism, floating abstractions — because their product doesn't exist anywhere. Dominion exists. It has mass. The design language should borrow from the world where this product lives and the world the buyer trusts:

- Engineering spec sheets, not SaaS landing pages
- The brass plate beside a chambers door, not a neon glow
- A vault door, a deed, a sealed envelope — objects with weight and provenance
- The product photography (full-bleed hero, per the five hard rules already agreed) is the proof: show the box

This is direction, not a token list. Do the frontend-design skill's two-pass process properly: brainstorm the token system (4–6 named hex values, display + body + utility faces, layout concept, one signature element), then critique it against the defaults below before showing Brad.

## BANNED LOOKS (hard rules)

1. No cream/#F4F1EA background + high-contrast serif + terracotta accent (the Claude-default look).
2. No near-black + single acid-green or vermilion accent.
3. No broadsheet/hairline-rules/zero-radius newspaper pastiche.
4. No purple-blue gradients, glassmorphism, floating 3D blobs, or particle fields — that's the cloud-AI vernacular this product exists to reject.
5. No generic SaaS card grids with icon + heading + two lines, repeated six times.
6. No stock icons standing in for meaning. If a structural device (numbering, dividers, eyebrows) doesn't encode something true about the content, cut it.
7. Inter/Roboto/Open Sans as the display face is a fail. Body face is your call if it earns its keep.

## HERO RULES (carried over — already agreed, do not relitigate)

1. Full-bleed product shot, hero headline "ChatGPT for firms that can't use ChatGPT" legible over it at all viewports.
2. Mobile crop must keep the product recognisable.
3. Headline + primary CTA above the fold on a 1366×768 laptop.
4. Overlay scrim no heavier than needed for WCAG AA contrast.
5. One restrained load animation maximum. No scroll-jacking.

## SIGNATURE ELEMENT

Propose exactly ONE memorable element that embodies "your data never leaves the building" — and keep everything else quiet. Candidates to spark thinking (choose your own if better): a spec-plate/engraved-plaque treatment for the pricing block; a section divider drawn as a literal boundary line ("everything below this line stays in your building"); the comparison table rendered as a compliance register. One. Not three.

## QUALITY FLOOR (build silently, don't announce)

- Responsive to 360px. Test the hero crop at 360, 768, 1366, 1920.
- Visible keyboard focus states. `prefers-reduced-motion` respected.
- Real Australian English throughout (per narrative brief).
- Watch CSS specificity collisions between section-level and element-level selectors — this bit the earlier build.

## DRIFT CHECK (run before every commit, report ✅/❌)

1. Does every colour and type decision trace back to the approved token system?
2. Is the signature element still singular?
3. Have any banned looks (1–7) crept in?
4. Do the five hero rules still hold at all four test widths?
5. Does the page still pass the narrative brief's own five-point drift check?

If any check fails, fix before committing. If a change genuinely requires breaking a rule, stop and ask Brad.

## OUT OF SCOPE

Copy changes, section order, backend, forms, the Scatter Tax PDF. Visual system and componentry only.
