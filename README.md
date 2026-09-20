# SoundScript

A desktop text-to-speech studio with **four AI engines** — two in the cloud, two fully offline. Write, refine, and generate professional voice-overs without subscriptions, telemetry, or cloud storage.

**Version:** 1.0.0
**Platforms:** Windows 10/11 · Linux (Ubuntu, Fedora, Kali, and most modern distros)
**Publisher:** BitProgram

---

## What's Inside

SoundScript gives you a choice between cloud-powered quality and fully local, offline generation:

### Text-to-Speech Engines

| Engine | Where it runs | Cost | Requires |
|---|---|---|---|
| **ElevenLabs** | Cloud | Pay per character | ElevenLabs API key |
| **Anhad** | On your device | Free | ~340 MB model download |

### AI Writing Assistant Engines

| Engine | Where it runs | Cost | Requires |
|---|---|---|---|
| **Gemini** | Cloud | Free tier available | Google AI Studio API key |
| **Nuqta** | On your device | Free | 400 MB – 2.5 GB model download (varies by size) |

Cloud engines deliver top-tier voice quality. Local engines work without internet, without API keys, and without sending any data off your machine.

---

## Features

- 🎙️ **24 built-in voices** across ElevenLabs and Anhad
- 🤖 **AI script assistant** powered by Gemini (cloud) or Nuqta (offline)
- 🔌 **Works fully offline** with downloaded models
- 💾 **Smart caching** — never pay to regenerate the same audio twice
- 📦 **Batch mode** for processing multiple `.txt` scripts at once
- 🎚️ **Tone tuning** — stability, similarity, and speed controls
- 🎭 **v3 emotion tags** — expressive delivery for supported models
- 🛡️ **Local-first privacy** — no telemetry, no cloud storage, no tracking
- 🚫 **No subscription** — one-time purchase, lifetime access

---

## System Requirements

| | Minimum | Recommended |
|---|---|---|
| **OS** | Windows 10 / Ubuntu 20.04 | Windows 11 / Ubuntu 22.04+ |
| **RAM** | 4 GB | 8 GB or more |
| **Disk** | 500 MB (app) | 3 GB+ (with all AI models) |
| **Internet** | Required for cloud engines | Not required once local models are downloaded |

---

## Installation

1. Extract the downloaded `.zip` file to a folder of your choice.
2. Run the installer for your platform:
   - **Windows:** `SoundScript-Setup.exe`
   - **Linux:** `SoundScript.deb` (install via `sudo dpkg -i SoundScript.deb`)
3. Launch SoundScript from your Start Menu or application launcher.

---

## First-Time Setup

### 1. Activate Your License

When you launch SoundScript for the first time, an activation dialog appears.

1. Open the purchase confirmation email from Gumroad.
2. Copy your license key (format: `XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX`).
3. Paste it into the activation dialog and click **Activate Product**.
4. SoundScript will verify your key with Gumroad and unlock.

**One license activates up to 3 devices.** You can deactivate old devices by contacting support if you've reached the limit.

### 2. Choose Your Engines (Optional)

By default, SoundScript is set to use the **cloud engines**. If you'd rather work offline, switch to local engines in **Settings → TTS** and **Settings → LLM**.

#### Option A — Cloud Engines

You'll need two API keys:

**ElevenLabs API Key** ([sign up free](https://try.elevenlabs.io/14i8lk1yiu8u))

1. Log into your ElevenLabs account.
2. Click **Developers** in the left sidebar.
3. Under **Quick Links**, click **Create API Key** and name it (e.g., `SoundScript`).
4. Set **Text to Speech** to *Access* and **Voices** to *Read*.
5. Click **Create Key** and copy it immediately — it's shown only once.

**Gemini API Key** ([sign up free](https://aistudio.google.com))

1. Go to Google AI Studio.
2. Sign in with your Google account.
3. Click **Get API Key** in the left sidebar → **Create API Key** → copy it.

#### Option B — Local Engines (Offline)

No API keys required.

1. Open **Settings → TTS → Manage Model** and download the **Anhad** model (~340 MB).
2. Open **Settings → LLM → Manage Models** and download a **Nuqta** model (choose based on quality vs. speed).
3. Switch both engine dropdowns to their local options.

#### Enter Your Keys

1. Open **Settings**.
2. Paste each key into the corresponding field.
3. Click **Validate** next to each to confirm the connection works.

> ⚠️ **Never share your API keys.** Treat them like passwords.

### 3. Set Your Output Folder

By default, generated audio is saved to `~/Music/SoundScript`. Change this in **Settings → Output Folder** if you'd prefer somewhere else.

---

## Usage

### Generate Your First Audio

1. Open the **Studio** tab.
2. Type or paste your script into the editor.
3. Choose a voice from the dropdown.
4. Adjust **Tone**, **Stability**, and **Speed** if desired.
5. Click **Generate**. Your audio appears in the **Library** tab when ready.

### Use the AI Assistant

1. Switch to the **Assistant** tab.
2. Pick your engine (Nuqta or Gemini) from the dropdown.
3. Ask things like:
   - *"Make this script more conversational"*
   - *"Write a four-scene story about a lost key"*
   - *"Suggest settings for a calm bedtime story"*
4. Copy any response back into the Studio editor.

### Batch Mode

1. Open **Studio → Batch Generate**.
2. Add multiple `.txt` files.
3. Choose voice and settings.
4. Click **Generate All** — SoundScript processes each file in order.

### Caching

Every generation is hashed by text, voice, tone, and settings. Re-generating the same script with the same settings returns the **cached file instantly** — no API call, no cost, no waiting.

Cache size can be limited in **Settings → Cache**. Clearing the cache is one click.

---

## Legal

- **[Privacy Policy](https://bitprogram0-alt.github.io/soundscript-landingpage/privacy.html)** — Full details on what data SoundScript does and doesn't collect.
- **[Terms of Service](https://bitprogram0-alt.github.io/soundscript-landingpage/terms.html)** — License terms, refund policy, and acceptable use.

**Summary:** SoundScript is local-first. We operate no servers that store your data. The only things that leave your device are (1) text you explicitly submit to cloud AI services, (2) your license key and a hashed machine identifier sent to Gumroad for verification, and (3) model downloads when you install a local engine.

---

## Troubleshooting

**"Invalid API key"**
Double-check the key was pasted fully (no trailing spaces). Regenerate the key in the provider's dashboard if it doesn't validate.

**"Quota exceeded" on ElevenLabs**
You've used up your monthly character allowance. Either top up your ElevenLabs account or switch to the local Anhad engine in Settings.

**"Model not installed"**
Open **Settings → TTS → Manage Model** (for Anhad) or **Settings → LLM → Manage Models** (for Nuqta) and download a model.

**"Download failed" repeatedly**
Check your internet connection and firewall. Downloading from HuggingFace may require allowing that domain through your firewall.

**Audio generation is slow (local engines)**
Local generation speed depends on your CPU. Nuqta-4B and Anhad are noticeably slower than cloud engines but completely private. Try a smaller model if speed is a priority.

**License activation limit reached**
Your license covers 3 devices. Contact support to reset activations if you've replaced hardware.

---

## Support

Stuck? We usually respond within a few hours.

📧 **Email:** [bitprogram0@gmail.com](mailto:bitprogram0@gmail.com)

When reporting a bug, please include:
- Your OS and version
- The exact error message
- What you were doing when the issue occurred
- Whether you were using a cloud or local engine

---

## Changelog

### v1.0.0 — Initial Release
- Four AI engines: ElevenLabs, Anhad, Gemini, Nuqta
- Studio, Assistant, Library, Settings, and About tabs
- Smart audio caching with configurable limits
- Batch generation from `.txt` files
- v3 emotion tag browser for ElevenLabs
- Local-first privacy model — no telemetry, no cloud storage
- Windows and Linux builds
- Gumroad license activation with 3-device limit

---

## Credits

SoundScript is built on the shoulders of excellent open-source projects:

- **PySide6** (Qt for Python) — LGPL v3
- **llama.cpp / llama-cpp-python** — MIT
- **Kokoro-82M** (base for Anhad) — Apache 2.0
- **Qwen** models (base for Nuqta) — Apache 2.0
- **onnxruntime** — MIT
- **lameenc** — LGPL v3

Full third-party licenses are available in-app under **About → View Third-Party Licenses**.

---

*SoundScript is a proprietary product of BitProgram. All rights reserved.*
*ElevenLabs, Gemini, Qwen, and Kokoro are trademarks of their respective owners.*
