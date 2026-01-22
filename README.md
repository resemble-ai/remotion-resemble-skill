# Remotion + Resemble.ai Skill

An AI agent skill for creating voiceovers in Remotion videos using [Resemble.ai](https://resemble.ai) text-to-speech.

## Installation

Install with a single command:

```bash
npx skills add yourusername/remotion-resemble-skill
```

## What This Skill Does

This skill teaches AI agents (Claude Code, Cursor, Copilot, etc.) how to:

- **Generate AI voiceovers** for Remotion video projects using Resemble.ai
- **Synchronize audio** with video compositions
- **Handle credentials** by prompting for API keys when needed
- **Create captions** (opt-in) with word-level synchronization

## Features

### Voice Generation
- Synchronous TTS for short content (up to 2,000 characters)
- Streaming TTS for longer scripts with progress feedback
- Support for custom cloned voices and pre-built library voices

### Remotion Integration
- Automatic audio duration detection
- Multi-segment composition support
- Volume control and audio fading
- Background music mixing

### Captions (Opt-in)
- Character-level timestamp extraction
- Word-synchronized captions
- TikTok-style word highlighting
- SRT export support

## Usage

Once installed, simply ask your AI agent to create a video with voiceover:

```
"Create a 30-second promotional video with voiceover about our product"
```

The agent will:
1. Check for Resemble.ai credentials (prompt if missing)
2. Generate the voiceover audio
3. Create a Remotion composition with the audio
4. Render the final video

### With Captions

To include captions, explicitly request them:

```
"Create a video with voiceover and TikTok-style captions"
```

## Requirements

- [Resemble.ai](https://resemble.ai) account and API key
- Node.js 18+
- Remotion project setup

## Skill Structure

```
remotion-resemble-ai/
├── SKILL.md                           # Main skill definition
└── rules/
    ├── resemble-setup.md              # API setup & credentials
    ├── resemble-sync-tts.md           # Synchronous TTS
    ├── resemble-streaming-tts.md      # Streaming TTS
    ├── resemble-voices.md             # Voice management
    ├── resemble-remotion-integration.md  # Remotion integration
    └── resemble-captions.md           # Caption generation (opt-in)
```

## Links

- [Resemble.ai](https://resemble.ai) - AI Voice Generator
- [Remotion](https://remotion.dev) - Make videos programmatically
- [skills.sh](https://skills.sh) - The Agent Skills Directory

## License

MIT
