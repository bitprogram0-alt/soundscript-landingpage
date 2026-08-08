# SoundScript

Text-to-speech generation powered by ElevenLabs, with an integrated AI writing assistant powered by Google Gemini.

## Features

- 🎙️ High-quality voice generation via ElevenLabs
- 🤖 AI script assistant powered by Google Gemini
- 💾 Smart caching — never pay to regenerate the same audio twice
- 📦 Batch mode for processing multiple scripts at once
- 🎚️ Adjustable stability and speed controls
- 🗣️ 14 starter voices included
- And Much More...

## Requirements

- Windows, or Linux
- An [ElevenLabs](https://try.elevenlabs.io/14i8lk1yiu8u) account
- A [Google AI Studio](https://aistudio.google.com) account (for Gemini)

## Installation

1. Extract the Zip folder.
2. Run the 'SoundScript.exe' OR 'SoundScript.deb' for Linux.
3. And Start Using the SoundScript

## Setup

### 1. Get your ElevenLabs API key

1. Log into your [ElevenLabs](https://try.elevenlabs.io/14i8lk1yiu8u) account (or create a free one).
2. Click **Developers** below the left sidepanel.
3. In **Quick Links** Click **Create API Key**, name it (e.g. `SoundScript`).
4. Set **Text-Speech** from No Access to Access **AND** Voices from No Access to Read.
5. Or Disable **Restrict Key** for easy setup (Recommended).
6. Click on **Create Key**.
7. Copy the Key **(Note: This key appears only once.)**

> ⚠️ Treat this key like a password — don't share it.

### 2. Get your Google Gemini API key (free)

1. Go to [Google AI Studio](https://aistudio.google.com).
2. Sign in with your Google account and click **Get API Key** in the left sidebar.
3. Click **Create API Key**, select a project (default is fine), and copy the key.

The free tier is generous and sufficient for script assistance.

### 3. Enter your keys in SoundScript

1. Open SoundScript and click to open **Settings**.
2. Paste your ElevenLabs key into the **ElevenLabs API Key** field.
3. Paste your Gemini key into the **Gemini API Key** field.
4. Use the show button to reveal a key and confirm it was pasted correctly.

### 4. Test your connections

In the Settings window:

| Button | Purpose |
|---|---|
| **Validate ElevenLabs Connection** | Confirms your ElevenLabs key is valid |
| **Validate Gemini Connection** | Confirms the AI assistant is reachable |

A green checkmark confirms success. If a test fails, check for typos, verify your internet connection, and confirm your account is active.

## Usage

### Generate your first audio clip

1. Close Settings and return to the main workspace.
2. Type or paste a script into the text area.
3. Choose a voice from the dropdown (14 starter voices available).
4. Adjust the **Stability** and **Speed** sliders, or leave them at their defaults.
5. Click **Generate**. Your audio appears in the playback bar — press **Play** to listen.

### Use the AI assistant (optional)

1. Switch to the **Assistant** tab to chat with Gemini.
2. Ask things like:
   - *"Make this script more conversational"*
   - *"Suggest settings for a calm bedtime story"*
3. Apply the refined text and recommended voice parameters with one click.

### Caching

Generating the same script with the same settings a second time returns a **Cached** result instead of billing a new API call — saving you cost on repeat generations.

### Batch mode

To process multiple scripts at once:

1. Open **Batch Mode**.
2. Select a folder of `.txt` files.
3. Choose your voice.
4. Start the queue — SoundScript processes each file in order.

## Support

Stuck on something? Reply to your purchase receipt email or reach out to our [support address](bitprogram0@gmail.com). We typically respond within a few hours.

---

*Enjoy creating — without ever paying twice for the same audio.*
