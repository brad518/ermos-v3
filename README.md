# ERMOSV3

A from-scratch Ermos site in the deep-tech-minimalism direction distilled from odinn.com.
Static, single-file (`index.html` + `assets/`), no build step.

- **Design system + rules:** `docs/style-guide.md`
- **Theme:** token-driven. Flip `<html data-theme="light">` ↔ `"dark"`.
- **Type:** Space Grotesk (display/body) + Space Mono (labels), one weight.
- **Accent:** electric blue `#0032FF`, used sparingly.

## Run locally
Open `index.html` in a browser, or:
```
python3 -m http.server 8890
```

## Prompt file
Use `ERMOS-V3-BRIEF.md` as the Claude Code prompt for the homepage rebuild.

## Status
Starter scaffold only (hero + two section stubs + footer). Product renders and the
full section build-out are still to come. Separate from the Ermos v1/v2 site
(`../../Ermos/ermoswebsite`) and its own git repo.
