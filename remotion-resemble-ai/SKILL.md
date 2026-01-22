---
name: remotion-resemble-ai
description: Create professional AI-narrated videos with Remotion and Resemble.ai - from educational tutorials to product launches
metadata:
  tags: remotion, video, react, resemble, tts, text-to-speech, voiceover, audio, ai-voice, motion-graphics, tutorial, demo
---

## When to use

Use this skill when the user wants to create:

1. **Educational Tutorial Videos** - Research a topic and create an animated explainer
   - Example: "Create a tutorial about the lifecycle of a butterfly for grade 3 students"

2. **SaaS Walkthrough Demos** - Showcase software features with animated UI
   - Example: "Create a demo video showing how to use Notion's database feature"

3. **Product Launch Announcements** - Marketing videos with motion graphics
   - Example: "Create a launch video announcing our new AI-powered search feature"

---

## Video Production Workflow

Follow this pipeline for all video types:

```
1. UNDERSTAND → 2. RESEARCH → 3. SCRIPT → 4. SCENES → 5. AUDIO → 6. ANIMATE
```

### Step 1: Understand the Request

Identify:
- **Video type:** Tutorial, demo, or announcement?
- **Target audience:** Age, expertise level, context
- **Tone:** Educational, professional, energetic, playful
- **Duration:** Short (30-60s), medium (1-3min), or long (3-5min)

### Step 2: Research (for tutorials and demos)

For educational content:
- Search for accurate, up-to-date information
- Use reliable sources (official docs, educational sites)
- Gather key facts, statistics, or steps to explain

For SaaS demos:
- Explore the product to understand features
- Capture screenshots or note UI patterns
- Identify the key workflow to demonstrate

### Step 3: Write the Script

Write a complete voiceover script BEFORE generating audio. Structure varies by video type (see below).

### Step 4: Plan Scenes

Break the script into visual segments:
- Each scene = one key idea or step
- Note what visuals accompany each line
- Plan transitions between scenes

### Step 5: Generate Audio

Use Resemble.ai to generate the voiceover (see setup below).

### Step 6: Create Animations

Build the Remotion composition with animations synchronized to the audio.

---

## Video Type: Educational Tutorial

**Goal:** Explain a concept clearly for a specific audience level.

### Script Structure

```
HOOK (5-10s)
"Have you ever wondered how a caterpillar becomes a butterfly?"

INTRODUCTION (10-15s)
Set context and preview what they'll learn.

BODY (main content, broken into 3-5 key points)
- Point 1: Explain with visual metaphor
- Point 2: Build on previous point
- Point 3: Add detail or example
- ...

RECAP (10-15s)
Summarize the key takeaways.

OUTRO (5s)
Call to action or closing thought.
```

### Audience Adaptation

| Audience | Language Style | Visuals |
|----------|---------------|---------|
| Grade K-2 | Very simple, playful, 5-word sentences | Bright colors, cute characters, big shapes |
| Grade 3-5 | Simple but informative, analogies | Clear diagrams, step-by-step, moderate pace |
| Grade 6-8 | More vocabulary, cause-effect | Charts, labeled diagrams, faster pace |
| High School+ | Technical terms OK, nuance | Data viz, detailed graphics |
| Adults | Professional, concise | Clean design, infographics |

### Animation Patterns for Tutorials

- **Reveals:** Fade in elements as narrator mentions them
- **Transformations:** Morph shapes to show change (caterpillar → butterfly)
- **Diagrams:** Animated labels, arrows pointing to parts
- **Timelines:** Progress bars, step indicators
- **Comparisons:** Side-by-side with highlighting

### Example Scene Plan

```
Script: "First, the butterfly lays tiny eggs on a leaf."

Scene 1:
- Visual: Leaf appears (slide in from bottom, spring animation)
- Visual: Small eggs fade in on leaf
- Timing: Sync "eggs" word with eggs appearing
- Duration: 4 seconds
```

---

## Video Type: SaaS Walkthrough Demo

**Goal:** Show users how to accomplish a task in software.

### Script Structure

```
HOOK (5-10s)
"Let me show you how to [accomplish goal] in [Product]."

CONTEXT (10s)
Why this feature matters, what problem it solves.

WALKTHROUGH (main content)
- Step 1: Navigate to X
- Step 2: Click on Y
- Step 3: Configure Z
- ...

RESULT (10s)
Show the outcome, the finished state.

OUTRO (5-10s)
Recap benefit, suggest next steps.
```

### Visual Elements

- **UI Mockups:** Stylized representations of the interface
- **Cursor animations:** Animated pointer moving to click targets
- **Highlights:** Glowing borders around buttons/fields being discussed
- **Zoom effects:** Focus on specific areas of the UI
- **Callouts:** Text labels pointing to UI elements

### Animation Patterns for Demos

- **Cursor movement:** Smooth bezier curves, slight pause before click
- **Click effect:** Ripple or pulse on click
- **Field focus:** Highlight border, slight scale up
- **Typing animation:** Characters appearing in input fields
- **Transition:** Slide or fade between screens
- **Callout arrows:** Animate in, point to element, fade out

### Example Scene Plan

```
Script: "Click the blue 'New Database' button in the sidebar."

Scene:
- Visual: UI mockup of sidebar
- Animation: Cursor moves to button (0.8s ease-out)
- Animation: Button highlights with glow
- Animation: Click ripple effect
- Animation: New panel slides in from right
- Duration: 3 seconds
```

---

## Video Type: Product Launch Announcement

**Goal:** Generate excitement about a new product or feature.

### Script Structure

```
HOOK (5-10s)
Bold statement or question that grabs attention.

PROBLEM (10-15s)
What pain point does this solve?

SOLUTION REVEAL (10-15s)
Introduce the product/feature dramatically.

KEY FEATURES (20-40s)
3-5 punchy feature highlights with visuals.

SOCIAL PROOF (optional, 10s)
Stats, testimonials, or credibility markers.

CALL TO ACTION (5-10s)
What should viewers do next?
```

### Visual Style

- **Bold typography:** Large text, kinetic type animations
- **Brand colors:** Use product's color palette consistently
- **Icons and graphics:** Abstract shapes, feature icons
- **High energy:** Faster cuts, dynamic movement
- **Logo reveal:** Animated logo at end

### Animation Patterns for Launches

- **Text slams:** Words slam in with impact
- **Kinetic typography:** Words that move, scale, rotate
- **Counter animations:** Numbers counting up (users, revenue, etc.)
- **Icon sequences:** Features appearing with bounce/spring
- **Gradient backgrounds:** Slowly shifting color gradients
- **Particle effects:** Subtle sparkles, floating shapes
- **Logo reveal:** Scale up, fade in, or assemble from pieces

### Example Scene Plan

```
Script: "Introducing Smart Search — find anything in milliseconds."

Scene:
- Visual: Dark background with gradient
- Animation: "Introducing" fades in (0.5s)
- Animation: "Smart Search" slams in large, bold (0.3s, with shake)
- Animation: Tagline types out below (typewriter, 1.5s)
- Animation: Search icon pulses
- Duration: 4 seconds
```

---

## Animation Vocabulary

Use these terms when describing animations:

| Term | Effect | Best For |
|------|--------|----------|
| **Fade** | Opacity 0→1 or 1→0 | Subtle entrances, transitions |
| **Slide** | Move from off-screen | UI elements, list items |
| **Scale** | Grow or shrink | Emphasis, entrances |
| **Spring** | Bouncy with overshoot | Playful, energetic feel |
| **Ease-out** | Starts fast, slows at end | Natural movement |
| **Ease-in-out** | Slow start and end | Smooth, polished |
| **Typewriter** | Characters appear one by one | Text reveals, code |
| **Stagger** | Sequential delay between items | Lists, multiple elements |
| **Morph** | Shape transforms into another | Transformations, transitions |
| **Pulse** | Scale up/down rhythmically | Drawing attention |
| **Shake** | Quick horizontal vibration | Impact, emphasis |
| **Wipe** | Reveal with moving edge | Scene transitions |

### Timing Guidelines

- **Fast:** 0.2-0.3s — Snappy, energetic
- **Medium:** 0.4-0.6s — Balanced, professional
- **Slow:** 0.8-1.2s — Dramatic, elegant
- **Stagger delay:** 0.1-0.2s between items

---

## Scene Planning Template

For each scene, document:

```
SCENE [number]: [title]
Script: "[exact voiceover text]"
Duration: [X seconds]
Visuals:
  - [element]: [description]
  - [element]: [description]
Animations:
  - [timing]: [element] [animation type] ([duration], [easing])
  - [timing]: [element] [animation type] ([duration], [easing])
Transition to next: [type]
```

---

## Required Setup - Resemble.ai

Before generating voiceovers, verify the user has credentials configured.

### Check for existing configuration

Check if `.env` file exists with:
- `RESEMBLE_API_KEY` - The Resemble.ai API token
- `RESEMBLE_VOICE_UUID` - Voice ID (optional, defaults to `7213a9ea`)

### Prompt for missing credentials

**If RESEMBLE_API_KEY is missing:**
Ask: "I need your Resemble.ai API key to generate voiceovers. You can get one from https://app.resemble.ai/account/api — please paste your API key:"

**If RESEMBLE_VOICE_UUID is missing:**
Use the default voice UUID `7213a9ea`. Only ask if they want a different voice.

### Save credentials

1. Create or update `.env` with the provided values
2. Ensure `.env` is in `.gitignore`
3. Confirm setup before proceeding

### Credential Security

- NEVER commit API keys to version control
- NEVER display the full API key back to the user
- ALWAYS ensure `.env` is in `.gitignore`
- Store credentials only in `.env`, never hardcoded

---

## Captions Behavior

**Captions are DISABLED by default.** Only generate word-level timestamps and caption components when explicitly requested.

### Default (no captions):
- Generate audio file only
- Save basic metadata (duration, fps, durationInFrames)
- Do NOT process timestamps into words

### When user requests captions:
- User must explicitly ask for "captions", "subtitles", or "word highlighting"
- Process `audio_timestamps` into word-level data
- Include caption components in composition

---

## Rule Files

Read these for detailed implementation:

- [rules/resemble-setup.md](rules/resemble-setup.md) - API credentials and configuration
- [rules/resemble-sync-tts.md](rules/resemble-sync-tts.md) - Synchronous TTS generation
- [rules/resemble-streaming-tts.md](rules/resemble-streaming-tts.md) - Streaming for longer scripts
- [rules/resemble-voices.md](rules/resemble-voices.md) - Voice selection and management
- [rules/resemble-remotion-integration.md](rules/resemble-remotion-integration.md) - Audio integration with Remotion
- [rules/resemble-captions.md](rules/resemble-captions.md) - Synchronized captions
- [rules/visual-animations.md](rules/visual-animations.md) - Animation patterns and Remotion primitives

---

## Quick Reference

### For Educational Tutorial:
1. Research the topic thoroughly
2. Adapt language to audience level
3. Use reveal animations synced to narration
4. Include visual metaphors and diagrams

### For SaaS Demo:
1. Understand the feature workflow
2. Create UI mockups or capture screenshots
3. Use cursor animations and highlights
4. Show the result/outcome clearly

### For Product Launch:
1. Focus on the problem → solution narrative
2. Use bold typography and brand colors
3. Keep it punchy — short sentences, fast cuts
4. End with clear call to action
