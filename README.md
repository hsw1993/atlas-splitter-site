# atlas-splitter-site

Static marketing + legal + support pages for **Atlas Splitter** (Mac).

**Do not** put any game engine / app source code in this repository.

Contents:

- `index.html` — product landing (Creem Buy link)
- `get/` — **How to get the product** (buy → download `.dmg` → activate) for Creem compliance
- `privacy/` — Privacy Policy
- `terms/` — Terms of Service
- `support/` — Support hub + localized guides
  - `support/en|zh|ja|ko/` — **latest** help (editable; may document the next release)
  - `support/versions/` — index of frozen help per shipped app build
  - `support/versions/{ver}-{build}/{lang}/` — **read-only** snapshot (e.g. `1.0.0-4`)

Version id matches the notarized DMG: `AtlasSplitter-{CFBundleShortVersionString}-{CFBundleVersion}.dmg`.

Live: https://atlassplitter.com/

## Publish with GitHub Pages

Repo: https://github.com/hsw1993/atlas-splitter-site  
Pages: Deploy from branch `main` / `(root)`. Custom domain `atlassplitter.com`.

```bash
cd /Users/hushiwei/Desktop/atlas-splitter-site
git status
git add -A && git commit -m "…" && git push
```

After deploy, spot-check:

- https://atlassplitter.com/support/
- https://atlassplitter.com/support/en/
- https://atlassplitter.com/support/versions/
- https://atlassplitter.com/support/versions/1.0.0-4/zh/

## Freeze help on each ship

When uploading a new Creem / MAS build:

1. Finish editing `support/{en,zh,ja,ko}/` for that build.
2. Copy into `support/versions/{ver}-{build}/{lang}/`.
3. Fix relative links (`guide.css` → `../../../guide.css`; home/privacy up four levels).
4. Add a `.version-bar` (historical snapshot) and a row on `support/versions/index.html`.
5. Do **not** edit archived trees afterward.

Engineering notes: GameEngine `atlas_splitter/docs/123-*-官网Support按版本冻结归档.md`.

## Local preview

```bash
open /Users/hushiwei/Desktop/atlas-splitter-site/support/index.html
open /Users/hushiwei/Desktop/atlas-splitter-site/support/versions/index.html
```

## Notes

- Only this static site is published; never push `GameEngine` / `atlas_splitter` source.
- App Help / Connect URLs should point at `https://atlassplitter.com/support/` and `https://atlassplitter.com/privacy/` (not Notion).
