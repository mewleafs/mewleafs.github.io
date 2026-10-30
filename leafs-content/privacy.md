---
title: "Leafs Content: privacy policy"
permalink: /leafs-content/privacy/
---

# Leafs Content: privacy policy

*Last updated: 30 October 2026*

Leafs Content is a desktop app for Windows for planning, writing, editing and preparing YouTube
videos. This page explains what data it handles and where that data goes.

**In short:** Leafs Content has no server of its own, no Leafs account, no analytics, no ads, no
cookies and no tracking. The developer receives no data from it. Your work stays in a workspace folder on your PC.
Data leaves your PC only for the AI features you use, the web searches and downloads they make, the
link to OBS Studio if you point it at another computer, and, if you connect it, read-only YouTube
data from Google.

## On your PC

- **Your workspace** is a folder you choose. It holds your ideas, structures, scripts, timelines,
  thumbnails and images, the footage, pictures, music and other files you add to the library, their
  transcripts, research notes, your channel's intro and rules, settings and the YouTube data the
  app has fetched (see below). For a stream recording you add, it also holds the link to the stream
  you type in, the loudness and other moments the app found in the recording, the moments you
  kept or passed, with the reasons you gave and the layout picked for each, where your avatar
  sits on your recordings if you mark it, and, if you use it, a copy of the stream data Leafs
  Live saved for that stream (see below). You can back it up, move it or delete it like any other folder; the
  app's own backups leave the YouTube data out.
- **Transcription, voice cleanup, background removal, spell check and finding the loud and lively
  moments of a stream recording** run on your PC.
- **App settings and caches** are kept in the app's data folder (`%LOCALAPPDATA%`), or next to the
  app in its portable version.
- **The YouTube sign-in**, if you connect YouTube, is kept in Windows Credential Manager, outside
  the workspace and its backups.
- **The OBS password**, if you connect the app to OBS Studio, is kept in Windows Credential Manager
  too, and OBS's host and port in the app's settings, outside the workspace.
- **The Leafs Live folder**, if you choose one, is kept in the app's settings, outside the
  workspace.

## AI features

Leafs Content doesn't run an AI service. Its AI features drive the official command-line tools you
install and sign in to yourself:

- Claude Code (`claude`), from Anthropic: [privacy policy](https://www.anthropic.com/legal/privacy)
- Codex CLI (`codex`), from OpenAI: [privacy policy](https://openai.com/policies/privacy-policy/)

When you use an AI feature, the tool you picked receives what that task needs, for example the
video's idea, structure and script, transcripts, descriptions of library files, frames of your
edit, your channel's intro and rules, and, for tasks that compare ideas with your past videos, the
titles and numbers of those videos. To find Shorts in a stream recording, it gets the recording's
transcript in parts of about 25 minutes, the moments the app found in each part, frames of the
recording, the titles of the moments you kept or passed on your streams, with your reasons, and,
if you use Leafs Live's data for that stream, its hype moments with the chat messages around each
(the messages' text only, no names), the chat's messages per minute, your markers and the viewers'
clips. YouTube's numbers are included only if you turn on *Let AI
tasks use the YouTube numbers* (see below); otherwise the AI sees only numbers you typed in
yourself. The tool sends it to its provider under your own account, and that provider's terms and
privacy policy apply, including whether it may use your conversations to train its models: both
let you turn that off (Claude: *Help improve Claude*; ChatGPT: *Improve the model for everyone*). The AI tools can also search the web
and open web pages. They work only through Leafs Content's own tools: they can read and propose,
but nothing changes until you accept it. Your scratchpad notes are never given to them.

## OBS Studio (optional)

To record B-roll while the script's voice plays, you can connect the app to OBS Studio's WebSocket
server in Settings, at the host and port you enter (OBS on the same PC is `localhost`). While the
connection is on, the app connects whenever OBS is running. It answers OBS's password challenge
(the password itself is never sent), asks OBS once whether it's recording, and then only listens
for OBS starting, pausing and stopping a recording. It never starts, stops or changes anything in
OBS, and the recordings stay wherever OBS saves them. *Disconnect* in Settings ends the connection;
*Remove* and *Connect again* delete the saved password.

## Leafs Live stream data (optional)

Leafs Live, the developer's streaming app, saves a file for each stream when it ends, in its own
profile folder on your PC. Leafs Content reads those files from that folder (the one Leafs Live's
settings list, or one you choose in Settings → Connections) when it opens, when you add a stream
or change its link, and when you open a stream's Harvest. It only reads them, never changes them, and nothing is sent
anywhere to get them: the two apps never connect to each other. A file holds when the stream was
live on Twitch and YouTube and the IDs of its videos there, the moments the chat got excited about
with counts (messages, laughter, raids, gifts and the like) and the chat messages around each, as
text only, without names, the chat's messages per minute, your Twitch markers, and the viewers'
Twitch clips, without who made them.

When a file matches a stream you added (its video is the stream's link, or the stream was live
when your recording started), the stream's Harvest asks whether to use it. Only if you choose
*Use it* is a copy kept with that stream in your workspace, and its moments shown along the stream
and given to the AI as described above. *Stop using it* deletes the copy. The parts that came from
YouTube (its chat messages and counts, Super Chats and memberships, and its times) are deleted from
the copy once 30 days have passed since the stream started on YouTube (the next time the app looks
for stream data), as Leafs Live deletes them from its own files, and the app's backups never carry
them.

## Downloads

- **Media tools:** the app downloads ffmpeg, whisper.cpp, Node.js and its speech and cutout models
  from their publishers (GitHub, nodejs.org, Hugging Face) and checks each file before use. The
  first video export downloads a headless Chrome browser used for rendering.
- **Pictures from the web:** when you paste a link, or accept pictures the AI found, the app
  downloads them from those websites. It only connects to public internet addresses.
- **Update check:** once a day the app reads
  [`latest.json`](https://mewleafs.github.io/leafs-content/latest.json) on this site (GitHub Pages)
  to see whether a newer version is out. It downloads or installs nothing, and sends nothing with
  the request.

Like any download, the servers involved can see your IP address. No personal data is sent with
these downloads.

## YouTube (optional)

Leafs Content uses YouTube API Services. You connect YouTube in Settings by signing in with Google
in your browser, after agreeing to this policy and the
[YouTube Terms of Service](https://www.youtube.com/t/terms). The app uses its own Google OAuth
client, so there's nothing to set up. It asks for two read-only permissions:
`youtube.readonly` and `yt-analytics.readonly`. The requests go straight from your PC to Google;
they don't pass through any Leafs server.

- **What it reads:** your channel's name, and for each published video you link in the app: its
  channel, publish date and length (YouTube Data API), and views, average view duration, average
  percentage viewed, likes, comments and subscribers gained per time window (YouTube Analytics
  API). For a stream whose YouTube video you link, when you ask for it: that video's channel,
  publish time and the time the live started (YouTube Data API), and its audience retention:
  how much of the audience was watching at each point of the video, and how that compares with
  similar videos (YouTube Analytics API), only for videos on your connected channel. Each time
  you open *New stream*: your channel's list of uploads and, for each of its videos, its title,
  length and, for a past live, when it went live and ended (YouTube Data API). It asks
  Google for those fields only, never uploads, edits or deletes anything on YouTube, and never
  downloads videos.
- **How it's used:** to show those numbers in the app exactly as YouTube returns them, next to the
  video they belong to; numbers you type in yourself are marked as yours. A stream's retention is
  drawn along the stream, and the time the live started is used once to suggest how far your
  recording is from the stream's video, which you can apply or ignore. *New stream* lists your
  past lives, newest first, and sets apart the ones that are already a stream in your workspace
  (by its link, or by when its recording started); picking one fills in its title and link,
  which you can change before adding the stream. If you turn on *Let AI
  tasks use the YouTube numbers* (off until you choose; the first task that could use them asks),
  they're also sent to the AI tool you use with the tasks that compare ideas with your past videos
  and, for a stream, with the task that finds Shorts in it (see above). YouTube data isn't used for advertising, sold, or shared with anyone else.
- **Where it's kept:** in your workspace's database on your PC, and never in the app's backups.
  The list of past lives in *New stream* isn't kept at all: it's read again each time the dialog
  opens and gone when it closes; only a title and link you add a stream with stay, as that
  stream's own.
  Every refresh checks that each linked video still exists on your channel and updates its facts;
  a video that's gone loses its YouTube data.
- **When it's deleted:** right away when you press *Delete YouTube data* or *Disconnect* in
  Settings, or when Google says the sign-in has expired or was revoked; and automatically when the
  app hasn't been able to check the data with YouTube for 30 days. A stream's retention is also
  deleted 30 days after it was fetched unless you fetch it again, and when you change the stream's
  link. Deleting it in the app doesn't
  change anything on YouTube. Numbers you typed in and your own notes stay.
- **Revoking access:** *Disconnect* in Settings revokes the sign-in at Google and deletes it from
  your PC. You can also remove Leafs Content's access at any time on Google's
  [security settings page](https://security.google.com/settings/security/permissions).

Leafs Content's use and transfer of information received from Google APIs adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements. See also the
[Google Privacy Policy](https://policies.google.com/privacy) and the
[YouTube Terms of Service](https://www.youtube.com/t/terms).

## Children

Leafs Content doesn't knowingly collect data from anyone, including children under 13.

## This page

This policy describes Leafs Content as it is today. The date at the top is the last time it was
checked against the app.

## Contact

Questions: email [mewleaf1@gmail.com](mailto:mewleaf1@gmail.com).
