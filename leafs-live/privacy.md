---
title: "Leafs Live: privacy policy"
permalink: /leafs-live/privacy/
---

# Leafs Live: privacy policy

*Last updated: 29 October 2026*

Leafs Live is a desktop app for Windows that reads a streamer's Twitch and YouTube chats, sends the
streamer's replies, the thank-you messages the streamer turns on, the answers to the viewer
commands the streamer turns on, the timed messages and the now playing line the streamer turns on and the lines of the polls and giveaways the streamer runs, carries out the moderation actions the streamer clicks, the chat commands
the streamer types and the moderation rules the streamer turns on, manages the Twitch channel points rewards the streamer makes in it, gives and takes Twitch VIP for the VIP Stamps the streamer turns on, posts the stream notifications the streamer sets up in their Discord server, and shows chat and the song playing on the PC on OBS overlays. This page explains what data it handles and where that data goes.

**In short:** Leafs Live has no server of its own, no Leafs account, no analytics, no ads and no
tracking. The developer receives no data from it. Your accounts, chat history and overlays stay on
your PC. The app talks only to Twitch and Google (YouTube) for the accounts you connect, to Discord for
the stream notifications you set up, to Google Fonts when you add a font, and to 7TV, BetterTTV and
FrankerFaceZ for their emotes.

## On your PC

- **Each profile** is a folder you choose. Its database holds the accounts you connected (login,
  display name, picture link and permissions, never passwords or tokens), your rules with their
  blocked words and allowed links, your viewer commands with their counters and how many times
  each was used, your timed messages, your saved polls and giveaways, your stream ideas (with their notes, links and days), your
  Discord stream notifications (their messages, the roles they mention, what Discord said about
  each webhook and the ID of each stream's message), overlays
  with their fonts, pictures, videos and sounds (with how loud each sound is, measured on your PC so
  they play at the same level), which third-party emote providers are on, and the chat history
  (below). The profile folder also keeps the third-party emotes' pictures (below). A stream idea's link
  opens in your own web browser when you click *Open*; the app itself doesn't visit it.
- **Sign-ins** (Twitch and Google tokens) and the **Discord webhooks** of your stream
  notifications are kept in Windows Credential Manager, never in the profile folder.
- **Overlays and the dock** are served only to your own PC (`127.0.0.1`), for OBS. They never get
  your sign-ins.
- **Remote control** is off until you turn it on. Then the app answers calls from your own PC
  (`127.0.0.1`) that carry its key, which is kept in the app's settings file on your PC; calls from
  websites are refused. What an action does on Twitch or YouTube (a line in chat, a chat mode, a
  stream marker, an ad, stream info) is sent by the app the same way as from its own buttons. It
  never gives out your sign-ins, and the list of the latest calls it shows in Settings is kept in
  memory only.
- **Simulated events** (the app's simulator, to try alerts and overlays) are made on your PC, in
  simulated chats, and are never saved. Nothing about them reaches Twitch or YouTube, except that
  while you turn on *Really send to chat* the chat messages they lead to (such as thank-yous) go to
  your real chat. Moderation in a simulated chat is never sent, and a counter a viewer command
  changes there changes only in memory.
- **Now playing** reads what's playing from Windows' media controls on your PC (the app it plays
  in, the title, artist and album, its cover, where it is, and whether it plays): only for the
  Now playing view, the dock and your overlays, kept in memory, never saved, and sent nowhere.
  The profile keeps which apps you picked and the names of the apps it has seen there. It reaches
  your chat only when you turn its chat line on or a viewer uses a command that says it (`!song`),
  sent like any other line. Its Play, Pause, Next and Previous buttons act on that app only.
- **Logs and diagnostics** stay on your PC. *Save diagnostics…* writes a text file only when you ask
  for it, without sign-ins or chat history, and it's up to you whether to share it.

## Chat history and viewers

To show chat, search it, keep a "to answer" list, remember how far you read in reader and important mode, the names reader mode skips and what
important mode holds, and
recognise first-time chatters, Leafs Live stores the chat messages and events it reads (names,
user IDs, messages, badges, cheers, Super Chats, subs, raids and memberships) in the profile's database, with a log of the moderation
that happened in your chat (deleted messages, timeouts, bans, warnings, lifted ones and cleared
chats: who did it, you, a moderator or one of your rules, to whom, the reason, and the message it
was about), and a list of alert events (Twitch follows, subs, gifted subs, cheers, raids, channel
points redemptions with the reward and what the viewer typed with it, hype trains with their level,
points and top contributors, and bits spent on Power-ups; YouTube Super Chats, Super Stickers,
memberships, gifted memberships and Jewels gifts: who, what, how much, and the thank-you message
sent for it, if any), which also keeps each one from being thanked twice. To group the chat by
stream, it also keeps when each of your streams was live on each platform (its start and end).
For the chat race (who got to your stream first), it keeps each race and each viewer's place in
it: their name, user ID, picture link, name color, badges, what brought them in (a message, a
follow, a sub, a Super Chat…), the chat, when, and whether you ticked them off as greeted; the
counts of first places and streams in a row are worked out from those races.
For polls, it keeps each poll you run (its question, options and settings, when it ran and its
result: each option's votes from each platform, and for an open answer the answers viewers wrote)
and each viewer's vote in it: their name, user ID, what they voted and when. A poll you cancel is
deleted with its votes.
For giveaways, it keeps each giveaway you run (its prize and settings, when it opened, closed and
ended) with each viewer's entry: their name, user ID, what they entered (such as a Guild Wars 2
account name), their chances and when; and each draw, with the random seed it used, every entry
it drew from and the winner, so the draw can be checked again. A giveaway you cancel is deleted
with its entries.
For the word game, it keeps each round you play (its level, language, letters and words, its goal,
when it ran and how it ended) and the points viewers scored in it: their name, user ID, the word they
found (or the round's bonus), the points and when. The boards of this stream's and all-time points
are worked out from those, with accounts you linked as one person counted together. These are kept
apart from the chat history, like viewer stats. The word lists come with the app.
For VIP Stamps (Twitch only), it keeps each stamp a viewer got (their name, user ID, the stream,
the month and when), each stream's stamp icon, the viewers it made VIP or you made permanent VIPs
(name, user ID, the month they're VIP for and whether the app gave it), who was welcomed in each
stream, the welcome sound you give a VIP (their name, user ID, a copy of the sound file you picked for them,
kept in the profile folder outside your library, its volume and whether their welcome is on), and a report of each month change (who gained, kept or lost VIP, with
their stamps). These stay until you delete the profile.
For viewer stats, it keeps, for each viewer and each of your streams, when they were first and last
there, when they first wrote or showed up with an alert in it (or that they were only in the chat,
watching), how many messages they sent and what brought them in, and what they gave in it: bits,
subs and gift subs with their tier and months, Super Chats and Super Stickers in their own
currency, memberships and gifted memberships, Jewels, channel points redemptions by reward and
raids, and when they followed. These are kept apart from the chat history, so how often someone comes is still known after
the messages are gone.
For stream recaps, it keeps for each of your streams how many messages came each minute on each
platform (counts, not the messages), the viewer counts it read while you were live, and the stream
markers you made, the channels you raided and the ad breaks, with their times.
For each viewer it keeps a short record (name, user ID, first and last seen, message count, the
first message they wrote in your chats, any note you write, and the other accounts you linked to
them as the same person).

- **Twitch:** messages, moderation log entries, alert events, chat race places, polls with their votes, giveaways with their entries and stream times are deleted after 90 days by
  default; you can change that in Settings, or keep them forever. Viewer records, viewer stats,
  stream recaps and word game rounds and points stay until you delete the profile.
- **YouTube:** messages, moderation log entries, alert events, chat race places, poll votes (and the polls YouTube viewers voted in), giveaway entries (and the giveaways YouTube viewers entered) and stream times are deleted after 30 days, viewer stats and YouTube's part of stream recaps 30 days after the stream they're about, word game points 30 days after they were scored, and viewer records
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
  requires to tell the app who took each moderation action in your chat; Leafs Live also uses
  `moderator:read:blocked_terms` to list your channel's blocked terms and
  `moderator:read:unban_requests` to list and hear the unban requests viewers send;
- `moderator:manage:chat_settings`, to turn slow mode, followers-only, subscribers-only,
  emote-only or unique chat on or off when you type the command (`/slow`, `/followers`…), switch it
  in the chat's Modes menu or press the raid shield;
- `moderator:manage:shield_mode`, to see whether Twitch's Shield mode is on and to turn it on or
  off when you type `/shield` or `/shieldoff`, switch it in the Modes menu or press a raid shield
  set to use it;
- `moderator:manage:announcements`, `moderator:manage:shoutouts` and `moderator:manage:warnings`,
  to post an announcement, shout out a channel or warn a viewer when you type `/announce`,
  `/shoutout` or `/warn`, shout out the channel a viewer command such as `!so` names when you
  allow its users to, or warn a viewer whose message matches a rule you set up to do that;
- `channel:manage:moderators`, `channel:manage:vips` and `channel:manage:raids`, to add or remove a
  moderator or a VIP and to start or cancel a raid when you type `/mod`, `/vip`, `/raid` or their
  opposites, and, once you turn VIP Stamps on, to read your channel's moderators and VIPs and to
  add or remove the VIPs it gives at each month change and the permanent VIPs you add;
- `channel:manage:broadcast`, to add a stream marker when you type `/marker`, and to set your
  stream's title, category, tags, language, content classification labels and branded content
  when you press *Update the stream* or apply a stream info preset;
- `moderator:manage:automod`, to see the messages Twitch's AutoMod holds for review in your chat
  and to allow or deny one when you click Allow or Deny;
- `moderator:manage:automod_settings`, to show your AutoMod levels and change them when you save
  them in Moderation;
- `moderator:manage:blocked_terms`, to add a term to your channel's blocked terms or remove one
  when you do it in Moderation, or copy your Leafs Live blocked words there;
- `moderator:manage:unban_requests`, to approve or deny an unban request, with the note you write,
  when you click Approve or Deny;
- `moderator:read:followers`, to show on a viewer's card since when they've followed your channel,
  to answer the `!followage` viewer command, and to hear new follows so the app can thank them in
  chat when you turn that on;
- `moderator:read:chatters`, to see who is in your chat while your stream is live, those who only
  watch included, for the viewer stats;
- `channel:read:redemptions`, to hear when a viewer redeems one of your channel points rewards and
  to list your channel's rewards, so you can pick which ones to thank or show on stream;
- `channel:read:hype_train`, to hear when a hype train starts, reaches a new level and ends;
- `bits:read`, to hear the bits spent in your channel (the app uses only the bits spent on
  Power-ups: cheers already come through the chat) and, for credits that name everyone who
  supports you, to read your channel's all-time bits leaderboard;
- `channel:read:subscriptions`, to list who is subscribed to your channel now, and who gifted each
  gifted sub, for credits that name everyone who supports you;
- `channel:manage:redemptions`, to make, change, pause, turn off and delete the channel points
  rewards you set up in Leafs Live, to list what viewers redeemed on them and complete or refund
  those redemptions when you click Complete or Refund (Twitch lets an app change only the rewards
  it created, and only their redemptions), and, when you turn on pausing rewards in alert control,
  to pause those rewards while alert control is paused or stopped and unpause them when you press
  Play;
- `channel:read:ads`, to show when your next ad break comes, how long it is and how many snoozes
  you have left, and to hear when an ad break begins;
- `channel:manage:ads`, to snooze the next ad when you click Snooze;
- `channel:edit:commercial`, to run an ad when you click Run an ad.

A bot account gets only `user:write:chat`. Leafs Live reads your channel's chat messages, chat
events, chat modes (slow mode, followers-only and the rest, and Shield mode), moderation actions,
the messages AutoMod holds for review, unban requests (who sent them, when and what they wrote)
and when one is answered or taken back, new follows, channel points redemptions, hype trains, bits
spent on Power-ups, when an ad break begins, and whether your stream is live, since when, and when it goes online or offline. When you open a viewer's card it asks
Twitch when that account was made and since when it has followed your channel, to show them there,
and when you set up channel points alerts it asks for your channel's list of rewards. When a
viewer command's answer or a timed message needs them, it asks Twitch for your stream's title and category, or when
the viewer who typed it (or the one they name) made their account and since when they've followed
your channel. When a giveaway you run takes only followers or accounts of a certain age, it asks
Twitch, as each viewer enters, when their account was made and since when they've followed your
channel. Once you turn VIP Stamps on, at each month change, when you preview one and when you
add a permanent VIP, it asks Twitch for your channel's moderators and VIPs (kept only in memory),
and to add a permanent VIP, or a VIP's welcome sound, by a name the app hasn't seen it looks the
name up on Twitch. When you open Channel points, it asks Twitch for your channel's rewards with their
settings, and for the redemptions waiting on the rewards Leafs Live created (who redeemed them,
when and what they typed); it hears when one of those is completed or refunded on Twitch. When you
open Stream info, it asks Twitch for your channel's title, category, tags,
language, content classification labels and branded content, and searches Twitch's categories by
the name you type. When you open Moderation, it asks Twitch for your AutoMod levels, your
channel's blocked terms and the unban requests waiting for an answer. When your streamer account
connects, when your stream goes live or offline, every few minutes while it's live, after an ad
break, and when you open Stream info or the dock's ads, it asks Twitch for your channel's ad
schedule (the next ad break, its length and the snoozes left). While your stream is live, every
few minutes, it asks Twitch for the list of who is in your chat (their names and user IDs) and
keeps that each of them was at that stream, for the viewer stats. When you open or roll credits
for everyone who supports you, it asks Twitch for your channel's subscribers (their names, user
IDs and who gifted a gifted sub) and its all-time bits leaderboard (the top 100 names and their
bits), kept only in memory for ten minutes. While your stream is live, every
minute, it asks Twitch for your stream's viewer count and keeps it with that stream, for its
recap. Once a Discord stream
notification that posts for Twitch is on, while your stream is live, it asks Twitch for your stream's title, category,
viewer count and the category's box art each time the notification's message is posted or updated
(and your channel's title and category when a stream ends after the app was restarted during it). Held messages, unban
requests, the AutoMod levels, the blocked terms, the ad schedule and ad breaks, account dates, follow dates, the title, the category, the
stream info Twitch gives, the list of rewards and the waiting redemptions are kept only in memory while the app runs, never
saved (a reward you pick is saved by its ID and title; a stream info preset you save keeps what you
put in it, in the profile's database). It posts only the messages you send; once you turn viewer commands on (they're off
until you do), the answer to a command a viewer types in your chat, in that chat, for the commands
that are on and the viewers each one allows, as the account the command sends as (your bot account
by default, when you have one), with a shoutout as your streamer account for a command set to do
that; once you turn timed messages on (they're off until you do), your timed messages in your live
chat, as the account each one sends as (your bot account by default, when you have one); once you
turn the now playing line on (it's off until you do), a line naming each new track once it has
played for the seconds you set, in your live chats, as the account you pick (your bot account by
default, when you have one); for a
poll you start with its chat lines on, a line when it starts and one when it ends, as your bot
account when you have one; for a giveaway you start with its chat lines on, a line when it opens,
one a minute before it closes and one for each winner drawn, as your bot account when you have
one; for the alert types
you turn on (every type is off until you do), a thank-you message in your chat when someone
follows, subscribes, gifts subs, cheers, raids, redeems a reward or uses a Power-up, or when a hype
train starts, reaches a new level or ends, as your bot account when you have one, else your
streamer account; and once you turn VIP Stamps on, a welcome line when one of its VIPs first
shows up in a stream (its alert type is on with VIP Stamps; you can turn it off), the thank-you
messages for a stamp or a reached goal when you turn those on, and, if you choose, a line naming
the new VIPs after a month change, as your bot account when you have one. At each month change
VIP Stamps makes Twitch VIPs of the viewers who reached your amount and takes VIP away from the
viewers it made VIP who didn't, unless it's on vacation; it never takes VIP from someone you made
VIP on twitch.tv or a permanent VIP, and never makes a moderator a VIP. It makes a permanent VIP
you add a VIP right away, and takes that VIP away only when you remove them and choose so. It makes, changes, pauses, turns on or off or deletes a channel points reward
only when you do it in Channel points, and completes or refunds a redemption only when you click
Complete or Refund, always as your streamer account, except the reward you pick for VIP Stamps,
when it's one Leafs Live created: a redemption that gives a stamp is completed, and one that
doesn't (a second one in the same stream, or one with no stream) is refunded. It changes your AutoMod levels, adds or
removes a blocked term, and approves or denies an unban request only when you do it in Moderation,
always as your streamer account; a blocked term you copy into Leafs Live joins the profile's
blocked words in its database. It snoozes or runs an ad only when you click Snooze or Run an ad, as your streamer account, and
says an ad break is coming only when you click Tell chat: the line you set (or the default one)
in your Twitch chat, as your bot account when you have one and choose so; your ads settings (the
heads-up, pausing alerts during ad breaks and that line) are kept in the profile's database. When you turn on pausing rewards in alert control, it asks Twitch for the
rewards it may change, pauses those that are on when you press Pause or Stop and unpauses them when
you press Play; the IDs of the rewards it paused are kept in the profile's database until then. It
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
  choose *Allow sending* (it lets you send, moderate and change your broadcasts), and for a bot
  account, which only sends.
- **What it reads:** your channel's ID, handle, name and picture; your live and upcoming streams,
  to find their chats and when each one went live; and those chats' messages and events, including the senders' channel names,
  pictures and badges. For a stream link you paste, the video's title and live details. When you
  open Stream info, your live and upcoming broadcasts' titles, descriptions, categories,
  visibility, audience setting (made for kids or not), scheduled times and the stream key each is
  bound to, and YouTube's list of video categories; when you schedule a broadcast, the names of
  your channel's stream keys (never the keys themselves). Once a Discord stream notification that posts
  for YouTube is on, while you're live on YouTube, your live broadcast's title and viewer count each
  time its message is posted or updated (the app's last look at it when that's at most a few
  minutes old). These are kept only in memory while the app runs. Once you turn on YouTube stats
  (the live stats' + menu, or Viewers → Settings; off until you do), while you're live on YouTube,
  your live broadcast's viewer count, likes and views every 2 minutes, in one request: the viewer
  count is kept with that stream for 30 days, for its recap, and the likes and views only in memory
  while the app runs, for the live stats.
- **What it writes:** only the chat messages you send; once you turn viewer commands on (they're
  off until you do), the answer to a command a viewer types in your chat, in that chat, with the
  answers asked for within a few seconds of each other sent together as one message, at most one
  such message per chat in the time you set, and none once a quarter of the day's quota is left,
  as the account the command sends as (your bot account by default, when you have one); once you
  turn timed messages on (they're off until you do), your timed messages in your live chats, as
  often as you set for YouTube, none once
  half of the day's quota is left, as the account each one sends as (your bot account by
  default, when you have one); once you turn the now playing line on (it's off until you do), a
  line naming each new track once it has played for the seconds you set, none once half of the
  day's quota is left, as the account you pick; for a poll you start with its chat lines on and
  its YouTube lines left on, a line when it starts and one when it ends, as your bot account when
  you have one; for a giveaway you start with its
  chat lines on, a line when it opens, one a minute before it closes and one for each winner
  drawn, as your bot account when you have one, and, with its entry confirmations on, a line
  telling the viewers who entered within a few seconds of each other that they're in (or in
  already), none once a quarter of the day's quota is left, as your bot account when you have one,
  else your streamer account; for the alert types you turn on (every
  type is off until you do), a thank-you message in your chat for a Super Chat, Super Sticker, new
  member, membership milestone, gifted memberships or Jewels gift, none sent by itself once a
  quarter of the day's quota is left, as your bot account when you have one, else your streamer
  account; and the moderation you click or type in your own chat: deleting a message, timing out, banning or unbanning a viewer, and adding or
  removing a moderator of the chat (`/mod`, `/unmod`; to remove one it first reads the chat's list
  of moderators), plus deleting a message or timing out its author when it matches a moderation
  rule you turned on, always as your streamer account; and, when you press *Update the stream* or
  apply a stream info preset, the title, description, category, visibility and audience setting of
  the live or upcoming broadcast you picked (for the category, through the broadcast's video when
  the broadcast itself doesn't take it), its thumbnail when you pick a picture from the profile's
  library, and a new scheduled broadcast bound to the stream key you choose, as your streamer
  account. It never uploads or deletes videos, changes your broadcasts only when you press
  *Update the stream* or apply a preset, and moderates only when you do or one of your rules does.
- **Bans:** to be able to lift a ban later, it keeps the ID YouTube gives each ban it makes, with
  the banned channel's ID, in the profile's database (deleted with the rest of the YouTube data).
- **How it's used:** only to show and answer your chat in the app, the dock and your overlays,
  to show and change your broadcasts' details in the app and the dock, and for the viewer stats
  and stream recaps the app shows you. It isn't used for
  advertising, sold or shared with anyone else.
- **Where it's kept:** in the profile's database on your PC, for at most 30 days, as described
  above. Your channel's name and picture are fetched again every week.
- **Agreeing:** the Accounts screen and the first-run setup say that connecting YouTube agrees to
  the YouTube Terms of Service and this policy, with links to both and to the Google Privacy
  Policy.
- **Disconnecting:** *Disconnect* on the Accounts screen revokes the sign-in at Google, deletes it
  from your PC, and deletes the profile's YouTube chat history, moderation log entries, alert events, chat race places, poll votes (and the polls YouTube viewers voted in), giveaway entries (and the giveaways YouTube viewers entered), stream times, viewer stats, word game points, YouTube's
  part of stream recaps and YouTube viewer records (for a bot account, its name on the known bots list). You can also remove the
  access at any time on Google's [third-party access page](https://myaccount.google.com/connections);
  Leafs Live then can't sign in, and the account and its YouTube data are deleted within 30 days. Deleting data in Leafs Live
  doesn't touch what YouTube itself keeps.

Leafs Live's use and transfer of information received from Google APIs adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements. See also the
[Google Privacy Policy](https://policies.google.com/privacy) and the
[YouTube Terms of Service](https://www.youtube.com/t/terms).

## Discord

Leafs Live posts to Discord only through the webhooks you paste into its Discord view, and only for
the notifications you turn on. It needs no Discord account or login: a webhook's URL is what lets
it post in one channel, so the app keeps it in Windows Credential Manager and never shows it on a
page, in the log or in diagnostics. When you add a webhook, the app asks Discord for its name and
its channel's and server's IDs. When one of the notification's platforms goes live, it posts the
message you wrote, filled with your name and picture link, your stream's title, category, viewer
counts and links, and the stream's picture, which the app downloads from Twitch's and YouTube's
image servers and uploads with the message. Only the roles you picked are mentioned. While you're
live it edits that message every so often (every 30 minutes unless you pick another time), and when
the stream ends it edits, deletes, leaves or replaces it, as you picked. For a notification whose
stream recap you turn on (off until you do), when a stream ends it posts the recap message you
wrote once, filled with that stream's numbers (messages, chatters, new and returning viewers,
follows, subs, bits, memberships, Super Chats per currency, raids, peak viewers) and, where you put
them, the names of the five Twitch viewers who wrote most and the chat race's Twitch podium; the
recap page's *Post to Discord* posts it again. YouTube viewers' names never go to Discord.
*Send a test* posts a test message, which you can delete from the app. Nothing else about your
viewers or your chat is sent to Discord. What's posted is in your Discord server, under
[Discord's privacy policy](https://discord.com/privacy). Deleting a notification in Leafs Live
forgets its webhook; messages already posted stay in Discord until you delete them there, and you
can delete a webhook itself in Discord's channel settings at any time.

## Third-party emotes

So that 7TV, BetterTTV and FrankerFaceZ emotes show in the chat, the dock and your overlays, Leafs
Live asks each of them for its emotes for everyone and for your Twitch channel's, by your Twitch
channel's public user ID (no account or sign-in is used), when a profile opens, when you change your
streamer accounts or press *Refresh*, and again every so often. 7TV also tells the app when your
channel's emotes change, over a connection that stays open while the app runs. When you've linked
your YouTube channel in your 7TV account, the app uses the emotes 7TV lists for it there; your
YouTube channel's ID isn't sent. The emote lists are kept only in memory. Each emote's picture is
downloaded once from that provider's image server and kept in the profile folder, so your overlays
load it from your PC. Each provider has a switch in Settings → Chat, all on to begin with; one
turned off isn't asked again. Like any download, those servers can see your IP address. Nothing
about your viewers or your chat is sent to them. Their own privacy policies are on their sites:
[7TV](https://7tv.app), [BetterTTV](https://betterttv.com) and
[FrankerFaceZ](https://www.frankerfacez.com/privacy).

## Pictures and fonts

Your overlays and the dock show viewers' pictures, Twitch's and YouTube's own emotes and badges
from Twitch's and YouTube's image servers (third-party emotes come from your PC, above), and Stream info shows the box art of the Twitch categories you search for from
Twitch's. When you add a Google font, the app downloads it once from Google Fonts. Like any
download, those servers can see your IP address. The pictures, videos and sounds you add for alerts
are copied into the profile folder, and your overlays load them from your PC; they're sent nowhere,
unless you export a template, which then carries them in its file, or you pick one as a YouTube
broadcast's thumbnail, which uploads it to YouTube.

## Children

Leafs Live doesn't knowingly collect data from anyone, including children under 13.

## This page

This policy describes Leafs Live as it is today. The date at the top is the last time it was checked
against the app.

## Contact

Questions: email [mewleaf1@gmail.com](mailto:mewleaf1@gmail.com).
