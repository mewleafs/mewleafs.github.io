---
title: "Leafs Live: privacy policy"
permalink: /leafs-live/privacy/
---

# Leafs Live: privacy policy

*Last updated: 26 October 2026*

Leafs Live is a desktop app for Windows that reads a streamer's Twitch and YouTube chats, sends the
streamer's replies, carries out the moderation actions the streamer clicks, the chat commands
the streamer types and the moderation rules the streamer turns on, and shows chat on OBS overlays. This page explains what data it handles and where that data goes.

**In short:** Leafs Live has no server of its own, no Leafs account, no analytics, no ads and no
tracking. The developer receives no data from it. Your accounts, chat history and overlays stay on
your PC. The app talks only to Twitch and Google (YouTube) for the accounts you connect, and to
Google Fonts when you add a font.

## On your PC

- **Each profile** is a folder you choose. Its database holds the accounts you connected (login,
  display name, picture link and permissions, never passwords or tokens), your rules with their
  blocked words and allowed links, overlays, fonts and pictures, and the chat history (below).
- **Sign-ins** (Twitch and Google tokens) are kept in Windows Credential Manager, never in the
  profile folder.
- **Overlays and the dock** are served only to your own PC (`127.0.0.1`), for OBS. They never get
  your sign-ins.
- **Logs and diagnostics** stay on your PC. *Save diagnostics…* writes a text file only when you ask
  for it, without sign-ins or chat history, and it's up to you whether to share it.

## Chat history and viewers

To show chat, search it, keep a "to answer" list and recognise first-time chatters, Leafs Live
stores the chat messages and events it reads (names, user IDs, messages, badges, cheers,
Super Chats, subs, raids and memberships) in the profile's database, with a log of the moderation
that happened in your chat (deleted messages, timeouts, bans, warnings, lifted ones and cleared
chats: who did it, you, a moderator or one of your rules, to whom, the reason, and the message it
was about).
For each viewer it keeps a short record (name, user ID, first and last seen, message count and any
note you write).

- **Twitch:** messages and moderation log entries are deleted after 90 days by default; you can
  change that in Settings, or keep them forever. Viewer records stay until you delete the profile.
- **YouTube:** messages and moderation log entries are deleted after 30 days, and viewer records
  30 days after they were last seen, or sooner if your Settings say so. A viewer who chats again is
  seen again.

**If you chat on a channel that uses Leafs Live:** your public chat messages are read through
Twitch's or YouTube's official API and kept only on that streamer's PC, as described here. They're
never sent to the developer.

## Twitch

You sign in with Twitch's device code login. For your streamer account Leafs Live asks for:

- `user:read:chat` (to read your channel's chat) and `user:write:chat` (to send the messages you
  write);
- `moderator:manage:chat_messages` and `moderator:manage:banned_users`, to delete a message, time
  out, ban or unban a viewer when you click it, and to delete a message or time out its author
  when it matches a rule you set up to do that;
- `moderator:read:blocked_terms`, `moderator:read:chat_settings`, `moderator:read:unban_requests`,
  `moderator:read:warnings`, `moderator:read:moderators` and `moderator:read:vips`, which Twitch
  requires to tell the app who took each moderation action in your chat (Leafs Live uses only that
  part);
- `moderator:manage:chat_settings`, to turn slow mode, followers-only, subscribers-only,
  emote-only or unique chat on or off when you type the command (`/slow`, `/followers`…), switch it
  in the chat's Modes menu or press the raid shield;
- `moderator:manage:shield_mode`, to see whether Twitch's Shield mode is on and to turn it on or
  off when you type `/shield` or `/shieldoff`, switch it in the Modes menu or press a raid shield
  set to use it;
- `moderator:manage:announcements`, `moderator:manage:shoutouts` and `moderator:manage:warnings`,
  to post an announcement, shout out a channel or warn a viewer when you type `/announce`,
  `/shoutout` or `/warn`, or warn a viewer whose message matches a rule you set up to do that;
- `channel:manage:moderators`, `channel:manage:vips` and `channel:manage:raids`, to add or remove a
  moderator or a VIP and to start or cancel a raid when you type `/mod`, `/vip`, `/raid` or their
  opposites;
- `channel:manage:broadcast`, used only to add a stream marker when you type `/marker`;
- `moderator:manage:automod`, to see the messages Twitch's AutoMod holds for review in your chat
  and to allow or deny one when you click Allow or Deny.

A bot account gets only `user:write:chat`. Leafs Live reads your channel's chat messages, chat
events, chat modes (slow mode, followers-only and the rest, and Shield mode), moderation actions,
the messages AutoMod holds for review, and whether your stream goes online. Held messages are kept
only in memory while the app runs, never saved. It posts only the messages you send, and it
moderates or changes your chat only when you click Delete, Timeout, Ban or Unban, allow or deny a
held message, switch a chat mode, press the raid shield or type a chat command in the message box
(such as `/ban`, `/slow` or `/raid`), or when a message matches a moderation rule you turned on
(to delete it, time its author out or warn them), always as your streamer account. Moderation
rules are off until you turn them on, act once when a message arrives, and never act on you, your
moderators, your own accounts or known bots, nor on VIPs and members unless you choose so. The raid shield's choices, and which modes it turned on so it can turn
them back off, are kept in the profile's database. To find someone a command names who hasn't written in your chat, it looks their
name up on Twitch. See Twitch's [privacy notice](https://www.twitch.tv/p/legal/privacy-notice/).

## YouTube

Leafs Live uses YouTube API Services. You sign in with Google in your browser, using Leafs Live's
own Google client or, if you choose, your own.

- **Permissions:** `youtube.readonly` for your streamer account. `youtube.force-ssl` only if you
  choose *Allow sending* (it lets you send and moderate), and for a bot account, which only sends.
- **What it reads:** your channel's ID, handle, name and picture; your live and upcoming streams,
  to find their chats; and those chats' messages and events, including the senders' channel names,
  pictures and badges. For a stream link you paste, the video's title and live details.
- **What it writes:** only the chat messages you send, and the moderation you click or type in
  your own chat: deleting a message, timing out, banning or unbanning a viewer, and adding or
  removing a moderator of the chat (`/mod`, `/unmod`; to remove one it first reads the chat's list
  of moderators), plus deleting a message or timing out its author when it matches a moderation
  rule you turned on, always as your streamer account. It never uploads, edits or deletes videos,
  and moderates only when you do or one of your rules does.
- **Bans:** to be able to lift a ban later, it keeps the ID YouTube gives each ban it makes, with
  the banned channel's ID, in the profile's database (deleted with the rest of the YouTube data).
- **How it's used:** only to show and answer your chat in the app, the dock and your overlays. It
  isn't used for advertising, sold or shared with anyone else.
- **Where it's kept:** in the profile's database on your PC, for at most 30 days, as described
  above. Your channel's name and picture are fetched again every week.
- **Agreeing:** the Accounts screen and the first-run setup say that connecting YouTube agrees to
  the YouTube Terms of Service and this policy, with links to both and to the Google Privacy
  Policy.
- **Disconnecting:** *Disconnect* on the Accounts screen revokes the sign-in at Google, deletes it
  from your PC, and deletes the profile's YouTube chat history, moderation log entries and YouTube
  viewer records (for a bot account, its name on the known bots list). You can also remove the
  access at any time on Google's [third-party access page](https://myaccount.google.com/connections);
  Leafs Live then can't sign in, and the account and its YouTube data are deleted within 30 days. Deleting data in Leafs Live
  doesn't touch what YouTube itself keeps.

Leafs Live's use and transfer of information received from Google APIs adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements. See also the
[Google Privacy Policy](https://policies.google.com/privacy) and the
[YouTube Terms of Service](https://www.youtube.com/t/terms).

## Pictures and fonts

Your overlays and the dock show viewers' pictures, emotes and badges from Twitch's and YouTube's
image servers. When you add a Google font, the app downloads it once from Google Fonts. Like any
download, those servers can see your IP address.

## Children

Leafs Live doesn't knowingly collect data from anyone, including children under 13.

## This page

This policy describes Leafs Live as it is today. The date at the top is the last time it was checked
against the app.

## Contact

Questions: email [mewleaf1@gmail.com](mailto:mewleaf1@gmail.com).
