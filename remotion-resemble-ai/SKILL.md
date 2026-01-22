---
name: remotion-resemble-ai
description: Create AI-generated voiceovers for Remotion videos using Resemble.ai Text-to-Speech
metadata:
  tags: remotion, video, react, resemble, tts, text-to-speech, voiceover, audio, ai-voice
---

## When to use

Use this skill when you need to:
- Generate AI voiceovers for Remotion video projects
- Create text-to-speech audio tracks using Resemble.ai
- Synchronize generated speech with video animations
- Add captions/subtitles using Resemble.ai's timestamp data (only when explicitly requested)

## Required Setup - IMPORTANT

Before proceeding with any Resemble.ai operations, you MUST verify the user has the required credentials configured.

### Step 1: Check for existing configuration

Check if `.env` file exists and contains the required variables:
- `RESEMBLE_API_KEY` - The Resemble.ai API token
- `RESEMBLE_VOICE_UUID` - The voice ID to use for synthesis

### Step 2: Prompt for missing credentials

If credentials are missing, ask the user for them using these prompts:

**If RESEMBLE_API_KEY is missing:**
Ask: "I need your Resemble.ai API key to generate voiceovers. You can get one from https://app.resemble.ai/account/api - please paste your API key:"

**If RESEMBLE_VOICE_UUID is missing:**
Ask: "I need a voice UUID to synthesize speech. You can find your available voices in the Resemble.ai dashboard under Voices. Please provide the voice UUID you'd like to use (or type 'list' if you want me to help you find available voices after setting up the API key):"

### Step 3: Save credentials

Once the user provides credentials:
1. Create or update the `.env` file with the provided values
2. Ensure `.env` is in `.gitignore` to prevent accidental commits
3. Confirm the setup is complete before proceeding

### Example interaction flow:

```
Agent: I'll help you create a voiceover for your Remotion video. First, let me check if you have Resemble.ai configured...

Agent: I don't see a Resemble.ai API key configured. I need your API key to generate voiceovers.

You can get one from: https://app.resemble.ai/account/api

Please paste your Resemble.ai API key:

User: rsm_xxxxxxxxxxxx

Agent: Got it! Now I need a voice UUID. You can find your voices in the Resemble.ai dashboard.

Please provide the voice UUID you'd like to use:

User: 55592656

Agent: I've saved your credentials to .env. You're all set! Now let's create your voiceover...
```

## How to use

Read individual rule files for detailed explanations and code examples:

- [rules/resemble-setup.md](rules/resemble-setup.md) - Setting up Resemble.ai API credentials and project configuration
- [rules/resemble-sync-tts.md](rules/resemble-sync-tts.md) - Synchronous text-to-speech generation for short content
- [rules/resemble-streaming-tts.md](rules/resemble-streaming-tts.md) - Streaming TTS for longer scripts with progressive playback
- [rules/resemble-voices.md](rules/resemble-voices.md) - Listing, selecting, and managing Resemble.ai voices
- [rules/resemble-remotion-integration.md](rules/resemble-remotion-integration.md) - Integrating Resemble.ai audio into Remotion compositions
- [rules/resemble-captions.md](rules/resemble-captions.md) - Using Resemble.ai timestamps to create synchronized captions

## Captions Behavior - IMPORTANT

**Captions are DISABLED by default.** Only generate word-level timestamps and caption components when the user explicitly requests captions/subtitles.

### Default behavior (no captions):
- Generate audio file only
- Save basic metadata (duration, fps, durationInFrames)
- Do NOT process timestamps into words
- Do NOT include caption components in the composition

### When user requests captions:
- User must explicitly ask for "captions", "subtitles", or "word highlighting"
- Only then process `audio_timestamps` into word-level data
- Include caption components in the composition
- Save words array to config file

### Example interactions:

**User says:** "Create a video with voiceover about our product"
→ Generate audio only, no captions

**User says:** "Create a video with voiceover and captions"
→ Generate audio AND process timestamps for captions

**User says:** "Add TikTok-style word highlighting to the video"
→ Generate audio AND process timestamps for captions

## Quick Start

1. Get an API key from [Resemble.ai Dashboard](https://app.resemble.ai/account/api)
2. Install dependencies: `npm install @remotion/media`
3. Use the synchronous endpoint to generate audio
4. Import the generated audio into your Remotion composition
5. **Only if user requests captions:** use timestamp data for word-level captions

## API Overview

Resemble.ai offers three synthesis modes:

| Mode | Best For | Latency |
|------|----------|---------|
| Synchronous | Short content, notifications, alerts | Request-based |
| Streaming HTTP | Longer scripts, progressive playback | Chunked response |
| Streaming WebSocket | Real-time, conversational agents | Lowest latency |

For video production workflows, **synchronous** mode is typically preferred as it delivers a complete audio file that can be easily imported into Remotion.

## Credential Security

- NEVER commit API keys to version control
- NEVER display the full API key back to the user after they provide it
- ALWAYS ensure `.env` is in `.gitignore`
- Store credentials only in `.env` file, never hardcoded in source files
