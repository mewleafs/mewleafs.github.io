---
title: Leafs Live
permalink: /leafs-live/
---

# Leafs Live

A desktop app for Windows for live streamers. It reads your Twitch and YouTube chats in one place,
lets you answer from either account, lets you delete messages and time out, ban or unban viewers
from the same feed, lets you allow or deny the messages Twitch's AutoMod holds, keeps a log of
every moderation action in your chats with an undo for timeouts and bans, runs chat commands typed in the message box (`/ban`, `/slow`, `/raid`…), shows
each chat's modes (slow mode, followers-only, members-only…) with a switch for Twitch's and a raid
shield button that turns on the protections you picked and back off, and drives customizable OBS
overlays (chat, featured message, alerts, chat race, poll, giveaway, credits) and an OBS dock
from a server that runs only on your PC. Simple rules can hide, dim, highlight or tag messages,
and, once you turn them on, delete messages or time out or warn their authors (blocked words,
links, shouting in capitals, too many emotes, the same text again), never touching you, your
moderators or your bots. Reader mode shows the chat in pages, in the app and the dock, so you
read every message in order: a page moves on only when you press Next, and it skips the messages
your rules dim but never a follow, sub, raid or other alert. Alerts thank viewers in chat when they follow, subscribe, gift subs,
cheer, raid, redeem a channel points reward or use a Power-up on Twitch, cheer on Twitch hype
trains as they start, level up and end, and thank viewers who send a Super Chat, a Super Sticker,
a Jewels gift, become a member or gift memberships on YouTube: each type is off until you turn it
on, with your own messages and variables, amount tiers, a minimum, rewards picked from your
channel's list with messages of their own, and one line for a burst of them, sent as your bot
account when you have one. Viewer commands answer what viewers type in either chat (`!discord`,
`!uptime`, `!followage`, `!lurk`, `!so @friend`, `!8ball`, a `!deaths` counter…) in that chat, once
you turn them on: every command can be edited, turned off or deleted, with your own replies and
variables, who can use it, cooldowns and a gentler pace on YouTube to spare its daily quota, and
you can add your own. Timed messages post your lines (your Discord, your socials, a reminder of
the commands…) in each of your live chats every few minutes, taking turns in your order, once you
turn them on, and only after enough viewers have written since the last one, so a quiet chat isn't
spammed. The same alerts play on stream in an Alerts widget, one at a time, with your own
text, picture, GIF or video and sound from your PC, and you can skip or replay them from the app or
the dock. A chat race shows who got to your stream first: each viewer's first message, follow,
sub, redeem or other support takes the next place, gold, silver and bronze first, on stream as a
leaderboard, a ticker or one arrival at a time, with an all-time board of who came first most
often; it starts with each stream (or when you start it), leaves out your own accounts and known
bots, and lists everyone in the app and the dock with a *Said hi* tick, so you can greet each one
while getting ready. Polls run in both chats at once: one choice, several choices or an open
answer, voted by typing an option's number or text (or `!vote`), one vote per account on each
platform, with a time or until you end it, who can vote, the result live on stream or only at the
end (Twitch and YouTube shown apart if you like) and, if you choose, a line in chat when it starts
and ends; you start, end or cancel them from the app or the dock, save polls to run again and see
past ones with their results. Giveaways also run in both chats at once: viewers enter with a
keyword like `!join`, a name that matches a pattern (such as a Guild Wars 2 account name, kept as
their entry) or any message, one entry per account, and a name counts once; subscribers and
members get more chances (×2 unless you change it), and you can limit it to some platforms, to
subscribers or higher, to Twitch followers or Twitch accounts of a certain age, and leave
moderators out. You close the entries (or they close at their time), draw a winner weighted by
those chances, reroll, and can ask the winner to answer in chat within a time; the giveaway shows
on stream with its prize, how to enter, the time left, a shuffle of names and the winner, and,
if you choose, lines in chat when it opens, before it closes and for the winner. Past giveaways
keep their winners and a draw log with each draw's seed and entries, so a draw can be checked.
Credits roll at the end of a stream with everyone who supported it: Twitch subscribers (not gifted
subs), gifters with their totals, bits, the hype train's top contributors and raids, YouTube
members, gifted memberships, Super Chats and Stickers (names only) and Jewels, and if you like your
moderators and top chatters; each section can be turned off, renamed and reordered, with your own
title and end text, a speed or a total time, and a loop. You roll them from the app, the dock or
the overlay editor; they never include follows.
Stream ideas keep a list of things to do on stream (ideas, topics, things to
react to or read), each with a note, a kind, links to open or copy and an optional day from which
it's important: important ones come first, and the dock's button counts them with a small bounce
when one comes due; search, filter by kind, drag to reorder, tick them done. They're in the app and
the dock, never on stream. Stream info sets your stream's details on both platforms from one
form, in the app and the dock: a title shared by both or one for each, Twitch's category (search
by name), tags, language, content classification labels and branded content, and the YouTube
broadcast's description, category, visibility, made for kids and a thumbnail from your pictures,
for the live broadcast, an upcoming one or a new one you schedule on a stream key; save it as a
preset ("Guild Wars 2 night") to apply again with one click. One Play / Pause / Stop control, in the app's header and the dock's, holds or drops
everything that can interrupt the stream: alerts on stream, featured messages and, if you choose,
the thank-you messages and the channel points rewards Leafs Live's Twitch app created, which it
pauses on Twitch itself. A simulator makes fake chat messages, follows, subs, raids, Super Chats, bans,
AutoMod holds and more, one at a time or as saved sequences, so you can try your alerts, overlays
and rules without a stream: they happen in simulated chats, nothing of them is saved, and the lines
they would send to chat are only shown unless you choose to really send them. The interface works
in English and Spanish.

Everything runs on your streaming PC. There's no Leafs account and no Leafs server: the app talks
only to Twitch and YouTube for the accounts you connect, and to Google Fonts when you add a font.

## Google and YouTube

Connecting YouTube is optional. If you connect it, Leafs Live asks Google for `youtube.readonly`
to find your live streams and read their chat. Only if you choose to send messages to YouTube chat
(*Allow sending*, or a bot account) does it also ask for `youtube.force-ssl`, which it uses only to
post the messages you write, the thank-you messages you turn on, the answers to the viewer
commands you turn on and the timed messages you turn on, and to carry out the moderation you click or type in your own chat
(deleting a message, timing out, banning or unbanning a viewer, adding or removing a chat
moderator) or that a moderation rule you turned on does (deleting a message, timing out its
author). It never uploads or deletes videos, and it moderates only when you do or one of
your rules does. With the same permission it changes your live or upcoming broadcast's title,
description, category, visibility, audience setting and thumbnail, and schedules a new broadcast,
only when you press *Update the stream* or apply a stream info preset. Details are in the
[privacy policy](privacy/).

- [Privacy policy](privacy/)
- [Terms of use](terms/)
