# Claude Code Prompt — Ermos Dominion v3 Homepage Rebuild

Copy everything below the line into Claude Code as your opening prompt (or save as `ERMOS-V3-BRIEF.md` in the repo root and tell Claude Code to read it before any work).

---

## ROLE

You are rebuilding the Ermos Dominion homepage (v3) on the `rebuild-fullbleed` branch. Use the `frontend-design` skill. This brief is the single source of truth for narrative structure and copy priorities. If any existing page content, component, or your own instinct conflicts with this brief, **the brief wins**. Do not "improve" the narrative order. Do not add sections not listed here without flagging it and asking first.

## THE BUYER (write for this person only)

Principal of a 10–30 person Australian law firm, medical practice, accounting firm, or financial advice practice. They sit on data they legally cannot leak. They cannot afford a $500k enterprise AI deployment, but they can afford $6,500 up front and $2,499/month. They are sceptical of AI hype and inflated ROI claims. Every sentence on the page must survive contact with this person's scepticism.

## THE NON-NEGOTIABLE NARRATIVE — SIX BEATS, IN THIS ORDER

The top of the page must walk the buyer through these six beats in this exact sequence. Each beat earns the next. The price appears LAST, only after the enterprise anchor has been set.

1. **You sit on data you're not allowed to leak.**
   Privileged matters, patient records, client financials. Name the verticals. This is identity, not features.

2. **So your firm has quietly banned AI — or thinks it has.**
   Staff are pasting client material into free ChatGPT on their phones anyway. All the risk of AI, none of the benefit. (Shadow AI — keep it visceral, one or two sentences.)

3. **The firms that solved this spent serious money.**
   Sovereign on-premises AI has been an enterprise purchase — six figures of hardware plus a dedicated IT function. Fine for a bank, not for a 20-person practice.
   ⚠️ Phrasing rule: use "six figures plus a dedicated IT function" or similar. Do NOT state "$500k" as a hard claim unless a citable comparable is provided.

4. **Dominion is that same class of capability, sized and priced for a firm.**
   A box in your office. Your files, your matters, your house style. Nothing ever leaves the building. Not cloud-hosted "private" — physically incapable of leaking.

5. **You don't run it. We do.**
   Installed in two weeks, managed for the life of the agreement, no IT hire, no per-seat licences, hardware replaced if it fails.

6. **The price, framed against a salary.**
   $6,500 one-time, $2,499/month, whole firm, unlimited users (Core; Growth $7,995 / $3,999 for 15–30 staff). Frame: "less than one part-time admin salary for every person in the building to have AI they're actually allowed to use."

## KEEP (these already work — do not lose them)

- Headline: **"ChatGPT for firms that can't use ChatGPT."** This stays as the hero. Do not replace it.
- The three-paths decision framing (use public AI / ban AI / Dominion) — this maps to beats 1–3 and can be the visual treatment of them.
- Visible pricing. Never hide prices behind "contact us".
- The honest FAQ tone, including the "a frontier cloud model may edge it" admission. Honesty is the brand voice.
- Security section: "your data is as safe as your building" framing.
- Australian sovereignty markers (onshore, ABN, 1300 number).

## DEMOTE OR CUT (objection generators — remove from homepage)

- **The $2.7M / $1.8M productive-capacity model.** Remove from the homepage entirely. It belongs in the gated Scatter Tax PDF where an already-interested reader will tolerate a planning model. On the homepage it spikes scepticism and undermines everything after it.
- **The full "AI scattered vs consolidated" comparison table.** Same destination — gated PDF. On the homepage, it may survive only as ONE line: "Firms that consolidate AI capture 80–95% of the knowledge that currently walks out the door" with a link to the full report.
- **The five "Why businesses choose Ermos" cards (25 bullets).** Cut or compress to a single tight section of max 5 bullets total. Kill generic SaaS language: "empower your people", "scale smarter and faster", "drive real business outcomes" — banned phrases.

## COPY RULES

- Australian English throughout.
- Short sentences. No hype adjectives ("revolutionary", "game-changing", "cutting-edge" — banned).
- Every claim must be either verifiable, clearly framed as a planning model, or cut.
- One CTA repeated: "Book a confidential consultation." Secondary CTA: the gated download (security brief or Scatter Tax PDF — check with Brad which one before wiring it).
- The price must never appear on the page before beat 3 (the enterprise anchor) has been established in the reading order.

## DRIFT CHECK — RUN BEFORE EVERY COMMIT

Before committing any homepage change, verify and state in the commit message:
1. Do the first six sections of the page still follow the six beats in order? ✅/❌
2. Does the enterprise/six-figure anchor still appear before any price? ✅/❌
3. Is the productivity dollar model still absent from the homepage? ✅/❌
4. Is "ChatGPT for firms that can't use ChatGPT" still the hero? ✅/❌
5. Any banned phrases introduced? ✅/❌

If any check fails, fix it before committing. If a change genuinely requires breaking one of these rules, stop and ask Brad — do not decide unilaterally.

## OUT OF SCOPE FOR THIS PROMPT

Backend, forms handling, the security-brief page internals, and the Scatter Tax PDF itself. Homepage narrative and copy only, plus whatever component restructuring the six-beat order requires.