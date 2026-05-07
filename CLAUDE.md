# Claude Code Install Guide — Project Instructions

## Purpose
Internal step-by-step install guide for Claude Code at 84.51º / Kroger, published via GitHub Pages.
Audience: non-technical Mac users, primarily designers with little or no terminal experience.

## Audience & Tone
- Users may be nervous or unfamiliar with Terminal and Claude Code
- Claude Code and Terminal often give vague or no feedback — the guide should acknowledge this and tell users what to expect (e.g., "a lot of text will scroll by — that's normal", "it may look like nothing is happening — be patient")
- The goal is to instill confidence: users should feel like they know what's happening and what to do if something looks unexpected
- Language should be plain, direct, and reassuring — not technical

## File Structure
- `claude-code-content.txt` — the editable source of truth for all page content
- `index.html` — the rendered page; updated by applying changes from the txt file

## Workflow
1. Edit `claude-code-content.txt` or ask Claude to apply the changes to `index.html.'
2. Changes need to be synced to other file that was not initially edited.ß
3. Push to GitHub — the live site updates automatically via GitHub Pages

## Content Format (claude-code-content.txt)
- `---STEP---` marks a new numbered step block
- `---FINAL---` marks the closing section
- `---FOOTER---` marks the footer
- Steps are auto-numbered via CSS counters — never manually renumber when adding or removing steps
- Do not change or remove `---` section markers

## Key Details
- KrAIG UI URL: https://ai-model-proxy.aks-ur-prd-internal.8451.cloud/ui/
- Corporate proxy (Zscaler) requires SSL cert setup — this is covered in the "Kroger Network Certificates Setup" step
- The `.claude` folder is hidden in Finder — revealed with Command + Shift + Period
- `settings.json` uses the KrAIG base URL, not Anthropic's default
- Live site: https://claysealkr.github.io/claude-code-install/
