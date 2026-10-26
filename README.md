# mewleafs.github.io

Public pages for mewleafs' apps: each app's home page, privacy policy and terms of use, and anything
else a platform (Google, Twitch, app stores…) wants at a public URL. GitHub Pages builds the
Markdown with Jekyll (theme: Primer) from the `main` branch and serves it at
https://mewleafs.github.io/.

## Layout

One folder per app, with its pages under it:

```text
_config.yml              site title and theme
index.md                 https://mewleafs.github.io/ (links to every app)
_includes/               snippets shared by pages, e.g. gw2-notice.html
leafs-content/           Leafs Content (desktop app)
  index.md               /leafs-content/          home page
  privacy.md             /leafs-content/privacy/
  terms.md               /leafs-content/terms/
leafs-live/              Leafs Live (desktop app), same three pages
gw2-armoury/             GW2 Armoury (Twitch Extension), same three pages
```

## Keeping the pages true

The pages describe each app as it is today. They're not a changelog: no versions, no history, no
"now" or "no longer". When an app changes what it collects, stores, sends, asks permission for or
does, its pages here are rewritten to match and their *Last updated* date changes.

## Adding a page

1. Create `<app>/<page>.md` with front matter: a `title` and a `permalink` ending in `/`
   (`/<app>/<page>/`).
2. Link it from the app's `index.md` and from the root `index.md`.
3. Push to `main`. The page is live a minute or two later.

## App rules

- **GW2 Armoury**: ArenaNet's Content Terms of Use ask fan sites to say they're unofficial, in the
  title bar too, and to show their legal notice. Every page under `gw2-armoury/` has *(unofficial
  fansite)* in its `title` and ends with `{% include gw2-notice.html %}`.

## Preview locally (optional)

With Ruby installed: `gem install bundler jekyll github-pages`, then `jekyll serve` and open
http://localhost:4000/.
