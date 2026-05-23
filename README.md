# EchoWeave

**AI-generated memory reconstruction platform that transforms scattered voice notes, screenshots, chats, and photos into structured digital timelines and searchable life archives.**

---

## The Problem

You have thousands of screenshots. Hundreds of voice notes. Years of chat history. But they're all *scattered* — across devices, apps, and time. Finding a specific memory, decision, or conversation means digging through noise with no map.

EchoWeave gives your digital fragments a spine.

---

## How It Works

```
Upload (screenshots / voice notes / chats / photos)
  → Extract — vision + speech models pull events, people, dates, emotions
  → Reconstruct — context reasoning links fragments into narratives
  → Explore — search memory maps, summaries, and interactive timelines
```

---

## Quickstart

### Web Workspace
1. Go to [echoweave.app](https://echoweave.app)
2. Create a private, encrypted workspace
3. Upload your fragments — drag and drop any file type
4. EchoWeave begins reconstructing in the background

### Mobile App
Available on iOS and Android. Capture voice notes, screenshots, and photos directly into your memory archive.

### API (for developers)
```bash
curl -X POST https://api.echoweave.app/v1/ingest \
  -H "Authorization: Bearer YOUR_KEY" \
  -F "file=@screenshot.png" \
  -F "file=@voice_note.m4a" \
  -F "context=founder-journal"
```

---

## Input Formats Supported

| Type | Formats |
|---|---|
| **Screenshots** | PNG, JPG, WebP |
| **Voice Notes** | M4A, MP3, OGG, WAV |
| **Chat Exports** | Telegram JSON, WhatsApp TXT, Slack export |
| **Photos** | JPEG, HEIC, RAW |
| **Documents** | PDF, Markdown, TXT |

---

## Use Cases

| Use Case | Description |
|---|---|
| **Personal Knowledge Management** | Searchable second brain from years of scattered notes |
| **Founder Journaling** | Reconstruct company history from voice memos and Slack exports |
| **Relationship Memory** | Arc of friendships and collaborations from chat history |
| **Research Organization** | Synthesize notes, screenshots, and interviews into knowledge maps |
| **Digital Archiving** | Encrypted, permanent, AI-searchable personal archive |
| **Life Narrative** | Generate summaries of life chapters from raw digital noise |

---

## Architecture Overview

```
┌──────────────────────────────────────────────────────────┐
│                     EchoWeave Pipeline                    │
│                                                           │
│  Ingestion          Understanding       Reconstruction    │
│  ──────────         ─────────────       ───────────────   │
│  Screenshots  →     Vision Model    →   Event Linking     │
│  Voice Notes  →     Speech-to-Text  →   Timeline Fusion   │
│  Chat Exports →     Entity Extract  →   Narrative Build   │
│  Photos       →     Emotion Detect  →   Memory Map Gen    │
│                                                           │
│  Storage: Private encrypted vault (AES-256, zero-access)  │
└──────────────────────────────────────────────────────────┘
```

---

## Privacy & Security

- **End-to-end encrypted storage** — your memories are readable only by you
- **Zero-knowledge architecture** — EchoWeave servers never see plaintext content
- **Local processing option** — run the pipeline locally for maximum privacy
- **GDPR compliant** — full export and deletion at any time

---

## Token Usage & Scale

| Metric | Value |
|---|---|
| Current consumption | ~120M tokens/month |
| Pipeline | Gemini (vision/speech) + Claude (reasoning) |
| Target (6 months) | 800M+ tokens/month |
| Architecture target | Persistent memory reasoning with MiMo V2.5 |

EchoWeave is an active participant in the **Xiaomi MiMo Orbit 100T Token Creator Incentive Program**, migrating core long-context reasoning workloads to MiMo V2.5.

---

## Deployment Options

### Cloud (Default)
- Mobile app + web workspace
- Automatic sync and backup
- Encrypted at rest and in transit

### Self-Hosted
```bash
docker run -d \
  -e MIMO_API_KEY=your_key \
  -e ENCRYPTION_KEY=your_key \
  -p 3000:3000 \
  echoweave/server:latest
```

---

## Requirements

- Node.js 20+ (self-hosted server)
- API key: MiMo, Gemini, or Claude
- Storage: local filesystem or S3-compatible bucket

---

## Links

- 🌐 App: [echoweave.app](#)
- 📱 iOS: [App Store](#)
- 🤖 Android: [Play Store](#)
- 📖 Docs: [docs.echoweave.app](#)
- 🔐 Privacy Policy: [echoweave.app/privacy](#)
- 🤖 MiMo API: [platform.xiaomimimo.com](https://platform.xiaomimimo.com)

---

## License

MIT — open core, self-hostable, privacy-first.
