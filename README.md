# cannonballdigitalworks.com

The Cannonball Digital Works website. One plain HTML page — no build step, no framework. GitHub Pages serves this repository's `main` branch as-is at **cannonballdigitalworks.com** (set by the `CNAME` file), the same way `cohesync-site` serves cohesync.com and `worklynq-site` serves worklynq.com.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page: styles (in the `<style>` block at the top), content, and the small script at the bottom that switches the service tabs. |
| `assets/cannonball-logo.png` | The logo. |
| `CNAME` | Tells GitHub Pages to serve this site at cannonballdigitalworks.com. Don't delete it. |
| `.nojekyll` | Tells GitHub Pages to serve files exactly as they are. |

## Making a change

1. Edit `index.html` — on GitHub's web editor or locally.
2. To check locally, run `python3 -m http.server` in this folder and open http://localhost:8000.
3. Commit to `main`. GitHub Pages republishes in a minute or two.

**Service tabs:** each tab is a `<button class="tab" data-tab="…">`, paired with a `<div class="panel" id="panel-…">`. The `data-tab` value must match the panel's id after `panel-`. The tab and panel marked `active` show first.

## Known gaps (as imported)

- The **"Get started"** buttons are plain buttons with no link or action, so they don't do anything yet.
- There is no `<meta name="viewport">` tag, so phones show a shrunken desktop layout.
- No favicon.

## History

Previously hosted by the old contractor on an AWS server (`52.200.230.134`). The live page was copied into this repo in October 2026 (commit "Import live cannonballdigitalworks.com page from AWS"); the only change since is moving the embedded logo out into `assets/`, verified pixel-identical.
