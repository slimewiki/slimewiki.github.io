# slimewiki.github.io

The root site for the **slimewiki** GitHub org. It exists only to redirect the
bare domain to the wiki:

- `https://slimewiki.github.io/` → `https://slimewiki.github.io/slime-character-wiki/`

`index.html` does the redirect (meta-refresh + JS `location.replace`, preserving
any `#hash`). `.nojekyll` stops GitHub from running Jekyll on the files.

## Publish

This repo must be named exactly **`slimewiki.github.io`** and live under the
**`slimewiki`** org (or user). Then:

1. Push these files to the `main` branch.
2. Repo → **Settings → Pages** → Source: **Deploy from a branch**, Branch:
   `main` / `/ (root)` → Save.

Within a minute, `https://slimewiki.github.io/` will redirect to the wiki.
