# atlas-splitter-site

Static marketing + legal + support pages for **Atlas Splitter** (Mac).

**Do not** put any game engine / app source code in this repository.

Contents:

- `index.html` — product landing (Creem Buy link)
- `privacy/` — Privacy Policy
- `terms/` — Terms of Service
- `support/` — Support hub + localized guides
  - `support/en/` English
  - `support/zh/` 中文
  - `support/ja/` 日本語
  - `support/ko/` 한국어

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
- https://atlassplitter.com/support/zh/
- https://atlassplitter.com/support/ja/
- https://atlassplitter.com/support/ko/

## Local preview

```bash
open /Users/hushiwei/Desktop/atlas-splitter-site/support/index.html
```

## Notes

- Only this static site is published; never push `GameEngine` / `atlas_splitter` source.
- App Help / Connect URLs should point at `https://atlassplitter.com/support/` and `https://atlassplitter.com/privacy/` (not Notion) once updated.
