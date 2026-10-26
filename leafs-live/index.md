---
title: Leafs Live
permalink: /leafs-live/
---

# Leafs Live

A desktop app for Windows for live streamers. It reads your Twitch and YouTube chats in one place,
lets you answer from either account, lets you delete messages and time out, ban or unban viewers
from the same feed, keeps a log of every moderation action in your chats with an undo for timeouts
and bans, runs chat commands typed in the message box (`/ban`, `/slow`, `/raid`…), shows
each chat's modes (slow mode, followers-only, members-only…) with a switch for Twitch's and a raid
shield button that turns on the protections you picked and back off, and drives customizable OBS
overlays (chat, featured message) and an OBS dock
from a server that runs only on your PC. Simple rules can hide, dim, highlight or tag messages. The
interface works in English and Spanish.

Everything runs on your streaming PC. There's no Leafs account and no Leafs server: the app talks
only to Twitch and YouTube for the accounts you connect, and to Google Fonts when you add a font.

## Google and YouTube

Connecting YouTube is optional. If you connect it, Leafs Live asks Google for `youtube.readonly`
to find your live streams and read their chat. Only if you choose to send messages to YouTube chat
(*Allow sending*, or a bot account) does it also ask for `youtube.force-ssl`, which it uses only to
post the messages you write and to carry out the moderation you click or type in your own chat
(deleting a message, timing out, banning or unbanning a viewer, adding or removing a chat
moderator). It never uploads, edits or deletes videos, and
it never moderates on its own. Details are in the [privacy policy](privacy/).

- [Privacy policy](privacy/)
- [Terms of use](terms/)
