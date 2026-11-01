# videoFn MCP

**Video editor for your AI assistant. Builds, checks and renders edits on your Mac.**

videoFn gives Claude, ChatGPT, Codex or any MCP client the tools to edit video
on your Mac. Your assistant builds the edit, checks its own work and fixes the
problems it finds. You watch the live preview, give notes in plain English and
export the finished MP4.

This repository publishes the videoFn connector for Claude Desktop
(`videoFn.mcpb`) and the metadata for the
[MCP Registry](https://registry.modelcontextprotocol.io). The videoFn app itself
is at [videofn.com](https://videofn.com).

## What it does

videoFn is a native video editor for Apple Silicon Macs with a built-in MCP
server. You brief your AI assistant, and it uses videoFn's tools to build the
edit from your footage, screen recordings, photos, music or documents.

- **It checks its own work.** videoFn measures text legibility against moving
  backgrounds, cut pacing, speech cuts, audio and visual sync, and the exported
  file. The assistant fixes what the checks find.
- **You stay in control.** The live preview shows the edit as it takes shape.
  Give notes in plain English, or change timing yourself in the editor.
- **Rendering happens on your Mac.** No uploads, no render queue.
  Transcription, voiceover, noise reduction, subject tracking and image
  background removal also run on the device. Your assistant receives
  transcripts, measurements and the preview frames it asks for, under its
  provider's terms.
- **Buy it once.** videoFn is free to try with a watermark on exports. One
  purchase removes the watermark. No account, no subscription, no credits.
  Your AI assistant is billed separately by its provider.

## What people make with it

- Product demos and launch videos from screen recordings
- App Store preview videos
- Release notes and changelog videos
- Vertical social clips with captions from longer recordings
- Explainers from a script, a PDF, a Word document or a spreadsheet
- Talking-head cleanup: remove filler words and long pauses, add subtitles
- Beat-synced edits, lyric videos, music videos from photos, YouTube intros

## Example prompts

- "Make a 30-second launch video from the screen recording in my Downloads
  folder. Add captions and some upbeat music."
- "Cut the ums and long pauses from this interview and add subtitles."
- "Turn this PDF report into a two-minute narrated explainer with animated
  charts."
- "Make a vertical clip of the best 45 seconds of this podcast recording."

## Requirements

- An Apple Silicon Mac
- The videoFn app
- An MCP client: Claude Desktop, Claude Code, ChatGPT, OpenAI Codex or another
  client

## Install

1. Download videoFn from [videofn.com/download](https://videofn.com/download)
   and open it.
2. On the launch screen, select **Connect** for your assistant.
3. Ask your assistant for a video.

**Claude Desktop only:** you can also install the connector first. Download
`videoFn.mcpb` from the
[latest release](https://github.com/stevejhiggs/videofn-mcp/releases/latest)
and open it. The connector needs the videoFn app. Until the app is installed,
it tells Claude where to download it.

## How the connector works

`videoFn.mcpb` contains a small launcher and no editor code. The launcher
starts the MCP broker inside the installed videoFn app, so the connector always
matches the app version you have. The broker starts the app when your
assistant first needs it.

## Links

- Website: [videofn.com](https://videofn.com)
- Download: [videofn.com/download](https://videofn.com/download)
- Pricing: [videofn.com/pricing](https://videofn.com/pricing)
- Privacy: [videofn.com/privacy](https://videofn.com/privacy)
- Support: [support@videofn.com](mailto:support@videofn.com)

## Licence

The files in this repository, including the launcher in `videoFn.mcpb`, are
under the MIT licence. The videoFn app is proprietary software.
