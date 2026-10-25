---
title: "GW2 Armoury (unofficial fansite): privacy policy"
permalink: /gw2-armoury/privacy/
---

# GW2 Armoury: privacy policy

*Last updated: 25 October 2026*

GW2 Armoury is a Twitch Extension that shows a streamer's current Guild Wars 2 build (gear, traits,
skills, pets and legends) in a panel, on the video and in the Twitch mobile app. This page explains
what data it handles and where that data goes.

**In short:** the extension has no server of its own, no analytics, no ads, no cookies and no
tracking. The developer receives no data from it. The streamer's GW2 API key stays in the streamer's
own browser.

## Streamers

- **Your GW2 API key** is stored only in your browser's local storage, on the extension's Twitch
  page. It's used only to read your build from the official Guild Wars 2 API
  (`api.guildwars2.com`), and only from your browser while one of the extension's broadcaster pages
  is open. It's never sent to Twitch, to viewers or to the developer. The extension only needs a key
  with the read-only permissions `characters`, `builds` and `inventories`. You can delete the key
  at any time on ArenaNet's account page, or by clearing your browser's site data.
- **What gets published:** your settings (which game modes and sections to show, the language and
  where the overlay's button goes) and a snapshot of your build: the character's name, profession,
  specializations, build name, and the game's ID numbers for your traits, skills, equipment and
  upgrades, with the time it was read. This is saved in Twitch's Extension Configuration Service and
  sent to viewers through Twitch, so anyone who can view your channel's extension can see it. It
  never contains your API key, your account name or anything else from your account.

## Viewers

- The extension doesn't ask for your Twitch identity and doesn't store or send any information
  about you. Twitch gives every extension your language, the light or dark theme and the state of
  the video player; GW2 Armoury uses these only to show the build in your language and theme and to
  stay out of the way of the player's controls.
- To show item, trait and skill names and icons, your browser downloads public game data from
  `api.guildwars2.com` and images from `render.guildwars2.com`, both run by ArenaNet. Like any
  website, those servers can see your IP address; see ArenaNet's privacy policy.
- That public game data and the last build shown are cached in your browser's local storage so the
  extension loads faster and makes fewer requests. It holds no personal data, and you can clear it
  at any time by clearing your browser's site data.
- **Copy build code** writes the in-game build code to your clipboard only when you click it. The
  extension never reads your clipboard.

## Third parties

The extension runs inside Twitch and uses ArenaNet's public API:

- Twitch: [privacy notice](https://www.twitch.tv/p/legal/privacy-notice/)
- ArenaNet: [privacy policy](https://www.arena.net/en/legal/privacy-policy)

GW2 Armoury is an unofficial fan extension. It isn't affiliated with, endorsed, sponsored or approved
by ArenaNet or NCSOFT. Guild Wars 2 names, images and data belong to ArenaNet, LLC.

## Children

The extension doesn't knowingly collect data from anyone, including children under 13.

## Changes

Changes to this policy are published on this page with a new date.

## Contact

Questions: use the support email on the extension's Twitch page.

{% include gw2-notice.html %}
