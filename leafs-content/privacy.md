---
title: "Leafs Content: privacy policy"
permalink: /leafs-content/privacy/
---

# Leafs Content: privacy policy

*Last updated: 25 October 2026*

Leafs Content is a desktop app for Windows for planning, writing, editing and preparing YouTube
videos. This page explains what data it handles and where that data goes.

**In short:** Leafs Content has no server of its own, no Leafs account, no analytics, no ads and no
tracking. The developer receives no data from it. Your work stays in a workspace folder on your PC.
Data leaves your PC only for the AI features you use, the web searches and downloads they make, and,
if you connect it, read-only YouTube data from Google.

## On your PC

- **Your workspace** is a folder you choose. It holds your ideas, structures, scripts, timelines,
  thumbnails and images, the footage, pictures, music and other files you add to the library, their
  transcripts, research notes, your channel's intro and rules, settings and the YouTube numbers the
  app has fetched. You can back it up, move it or delete it like any other folder.
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
YouTube titles and numbers the app has fetched. The tool sends it to its provider under your own
account, and that provider's terms and privacy policy apply. The AI tools can also search the web
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

Leafs Content uses YouTube API Services. You connect YouTube in Settings with your own Google
OAuth client, which you create in Google Cloud; Leafs Content doesn't ship one. It asks for two
read-only permissions: `youtube.readonly` and `yt-analytics.readonly`.

- **What it reads:** your channel's name, and for the published videos you link in the app: title,
  publish date and length, views, watch time, average view duration, audience retention, likes,
  comments, subscribers gained, impressions and click-through rate. To get impressions and
  click-through rate it asks YouTube's Reporting API to prepare a daily reach report for your
  channel. It never uploads, edits or deletes anything on YouTube.
- **How it's used:** to show the numbers in the app, and as context for the AI features you use
  (see above). It isn't used for advertising, sold or shared with anyone else.
- **Where it's kept:** in your workspace's database on your PC, until you delete it or the
  workspace.
- **Disconnecting:** *Disconnect* in Settings revokes the sign-in at Google and deletes it from your
  PC. You can also remove the access at any time on Google's
  [third-party access page](https://myaccount.google.com/connections).

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
