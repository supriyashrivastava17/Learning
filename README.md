# Living Things — landing page

Static landing page built from the Figma design (`Desktop - 3`, 1440 × 4585).

## Running it

No build step — `index.html` is self-contained. Serve the folder over HTTP:

```bash
ruby -run -e httpd -- -p 4322 .
```

Then open <http://localhost:4322>. Any static server works
(`python3 -m http.server 4322`, `npx serve`, etc.).

## Layout

| Path | Purpose |
| --- | --- |
| `index.html` | The whole page — markup, CSS and JS inline |
| `.claude/launch.json` | Dev-server config for the Claude Code browser pane |

## Sections

Nav → Hero → Results → Our Services → Our Values → Footer.

## Notes

- Type is Poppins with Playfair Display italic for the serif accents
  (`Technology`, `Future`, `Improve`, `Air`, `Efficiency`, `Principles`).
  That sans/serif contrast is the design's signature.
- The page background carries an SVG grain texture to match the Figma paper.
- **Imagery is hand-authored SVG, not the Figma exports.** The design's
  photographs (leaf branch, energy column, four landscapes, footer figure)
  could not be exported — the file was only reachable signed out, so Dev Mode
  and asset export were unavailable. The SVGs are deliberate stand-ins and
  should be swapped for the real assets.
- Colours and spacing are read from the canvas by eye, not from Dev Mode, so
  they are close but not token-exact.
- Copy is transcribed from the design, including its own placeholder text
  ("At Living Thing, we craft experiences…") and the footer's `ALL right
  reivied 2020` typo.
- Nav links and buttons are anchors to on-page sections; nothing posts anywhere.
