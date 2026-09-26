# Com AI Desktop — Downloads

Desktop app for **Elite English Coach**, built with [Tauri](https://tauri.app/) + React/Vite.

**Latest version: `0.4.2`** — [release notes](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest)

### What's new in 0.4.2

- **Voice breaks eliminated**: Audio chunk odd-byte carryover prevents waveform distortion; AudioContext pre-warming and tuned VAD (800ms silence, balanced start sensitivity) eliminate false cutoffs and interruptions during pauses.
- **Live Analytics working**: Dashboard reflects active practice time and words learned immediately without requiring an app reload; streak and date tracking anchored to local system calendar.
- **Language Lock (Strict English)**: Prompts explicitly prevent the model from drifting into Hindi or other languages, keeping focus 100% on English practice.
- **Optimized Memory**: Virtualized PDF rendering drastically reduces active DOM nodes for multi-page documents; audio contexts are cleanly torn down.
- **Data Backup & Migration**: Settings now includes full export and restore for all notes, flashcards, activity, transcripts, and session reports across updates.
- **History Linked to Dialogue**: Session feedback reports now link directly to the full conversation transcript with a tabbed view.
- **Long Session Reports**: Increased report timeout to 90 seconds and added automatic multi-key rotation fallback to ensure comprehensive evaluation reports even after long sessions.

## Download

### Windows

| File | Description |
|------|-------------|
| [com-ai_0.4.2_x64-setup.exe](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest/download/com-ai_0.4.2_x64-setup.exe) | Windows installer (NSIS) — recommended |
| [com-ai_0.4.2_x64_en-US.msi](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest/download/com-ai_0.4.2_x64_en-US.msi) | Windows installer (MSI) |

> **"Windows protected your PC"?** The installer isn't code-signed yet, so
> Windows SmartScreen shows this for any new publisher. Click **More info**,
> then **Run anyway**.

### Linux

| File | Description |
|------|-------------|
| [com-ai_0.4.1_amd64.deb](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.1/com-ai_0.4.1_amd64.deb) | Debian / Ubuntu package |
| [com-ai-0.4.1-1.x86_64.rpm](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.1/com-ai-0.4.1-1.x86_64.rpm) | Fedora / RHEL / openSUSE package |
| [com-ai_0.4.1_amd64.AppImage](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.1/com-ai_0.4.1_amd64.AppImage) | Portable AppImage (any distro) |

Install on Debian/Ubuntu:

```bash
sudo apt install ./com-ai_0.4.1_amd64.deb
```

Or run the AppImage directly:

```bash
chmod +x com-ai_0.4.1_amd64.AppImage
./com-ai_0.4.1_amd64.AppImage
```

### macOS

A macOS build of 0.4.2 is not available yet.

## Setup

AI features need a Google Gemini API key. Open **Settings** in the app and paste
in up to four keys — the app rotates through them to spread out free-tier rate
limits. Keys are stored only on your device.
