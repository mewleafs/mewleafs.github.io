---
title: "Leafs Content: privacy policy"
permalink: /leafs-content/privacy/
---

# Leafs Content: privacy policy

*Last updated: 25 October 2026*

Leafs Content is a desktop app for Windows for planning, writing, editing and preparing YouTube
videos. This page explains what data it handles and where that data goes.

**In short:** Leafs Content has no server of its own, no Leafs account, no analytics, no ads, no
cookies and no tracking. The developer receives no data from it. Your work stays in a workspace folder on your PC.
Data leaves your PC only for the AI features you use, the web searches and downloads they make, and,
if you connect it, read-only YouTube data from Google.

## On your PC

- **Your workspace** is a folder you choose. It holds your ideas, structures, scripts, timelines,
  thumbnails and images, the footage, pictures, music and other files you add to the library, their
  transcripts, research notes, your channel's intro and rules, settings and the YouTube data the
  app has fetched (see below). You can back it up, move it or delete it like any other folder; the
  app's own backups leave the YouTube data out.
- **Transcription, voice cleanup, background removal and spell check** run on your PC.
- **App settings and caches** are kept in the app's data folder (`%LOCALAPPDATA%`), or next to the
  app in its portable version.
- **The YouTube sign-in**, if you connect YouTube, is kept in Windows Credential Manager, outside
  the workspace and its backups.

## AI features

Leafs Content doesn't run an AI service. Its AI features drive the official command-line tools you
install and sign in to yourself:

- Claude Code (`claude`), from Anthropic: [privacy policy](https://www.anthropic.com/legal/privacy)
- Codex CLI (`codex`), from OpenAI: [privacy policy](https://openai.com/policies/privacy-policy/)

When you use an AI feature, the tool you picked receives what that task needs, for example the
video's idea, structure and script, transcripts, descriptions of library files, frames of your
edit, your channel's intro and rules, and, for tasks that compare ideas with your past videos, the
titles and numbers of those videos. YouTube's numbers are included only if you turn on *Let AI
tasks use the YouTube numbers* (see below); otherwise the AI sees only numbers you typed in
yourself. The tool sends it to its provider under your own account, and that provider's terms and
privacy policy apply, including whether it may use your conversations to train its models: both
let you turn that off (Claude: *Help improve Claude*; ChatGPT: *Improve the model for everyone*). The AI tools can also search the web
and open web pages. They work only through Leafs Content's own tools: they can read and propose,
but nothing changes until you accept it. Your scratchpad notes are never given to them.

## Downloads

- **Media tools:** the app downloads ffmpeg, whisper.cpp, Node.js and its speech and cutout models
  from their publishers (GitHub, nodejs.org, Hugging Face) and checks each file before use. The
  first video export downloads a headless Chrome browser used for rendering.
- **Pictures from the web:** when you paste a link, or accept pictures the AI found, the app
  downloads them from those websites. It only connects to public internet addresses.

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
  API). It asks Google for those fields only, and never uploads, edits or deletes anything on
  YouTube.
- **How it's used:** to show those numbers in the app exactly as YouTube returns them, next to the
  video they belong to; numbers you type in yourself are marked as yours. If you turn on *Let AI
  tasks use the YouTube numbers* (off until you choose; the first task that could use them asks),
  they're also sent to the AI tool you use with the tasks that compare ideas with your past videos
  (see above). YouTube data isn't used for advertising, sold, or shared with anyone else.
- **Where it's kept:** in your workspace's database on your PC, and never in the app's backups.
  Every refresh checks that each linked video still exists on your channel and updates its facts;
  a video that's gone loses its YouTube data.
- **When it's deleted:** right away when you press *Delete YouTube data* or *Disconnect* in
  Settings, or when Google says the sign-in has expired or was revoked; and automatically when the
  app hasn't been able to check the data with YouTube for 30 days. Deleting it in the app doesn't
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
