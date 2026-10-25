# mewleafs.github.io

Public pages for mewleafs' projects: promo pages, privacy policies, terms and anything else a
platform (Twitch, Google, app stores…) wants at a public URL. GitHub Pages builds the Markdown with
Jekyll (theme: Primer) from the `main` branch and serves it at https://mewleafs.github.io/.

## Layout

One folder per project, and its pages under it:

```text
_config.yml              site title and theme
index.md                 https://mewleafs.github.io/ (links to every project)
_includes/               snippets shared by pages, e.g. gw2-notice.html
gw2-armoury/             Twitch GW2 Armoury extension
  index.md               /gw2-armoury/
  privacy.md             /gw2-armoury/privacy/
```

## Adding a page

1. Create `<project>/<page>.md` with front matter: a `title` and a `permalink` ending in `/`
   (`/<project>/<page>/`).
2. Link it from the project's `index.md` and from the root `index.md`.
3. Push to `main`. The page is live a minute or two later.

## Project rules

- **GW2 Armoury**: ArenaNet's Content Terms of Use ask fan sites to say they're unofficial, in the
  title bar too, and to show their legal notice. Every page under `gw2-armoury/` has *(unofficial
  fansite)* in its `title` and ends with `{% include gw2-notice.html %}`.

## Preview locally (optional)

With Ruby installed: `gem install bundler jekyll github-pages`, then `jekyll serve` and open
http://localhost:4000/.
