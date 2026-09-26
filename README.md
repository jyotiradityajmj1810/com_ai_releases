# Com AI Desktop — Downloads

Desktop app for **Elite English Coach**, built with [Tauri](https://tauri.app/) + React/Vite.

**Latest version: `0.4.3`** — [release notes](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest)

### What's new in 0.4.3

- **Voice breaks eliminated**: PCM odd-byte carryover fixed; AudioContext pre-warmed; mid-turn swap deferred until the current sentence completes; VAD presets added (snappy / balanced / patient).
- **Language lock**: Read-aloud synthesis strictly respects the configured language code and retries gracefully if the model rejects it.
- **Live Analytics working**: Dashboard reflects active practice time and words learned immediately; streak and date tracking anchored to local system calendar.
- **Optimized Memory**: Documents stored as metadata + pages separately so listing never loads full text; PDF scroll uses a height-estimate cache instead of a full DOM; alarm beep reuses one AudioContext.
- **Data Backup & Migration**: Full export/import is atomic; onupgradeneeded v8 migration splits docs, normalises flashcards, backfills report transcriptIds, and cleans orphaned data.
- **History Linked to Dialogue**: Session reports link to the correct transcript; consecutive same-role turns are coalesced in the transcript view.
- **Session robustness**: Reconnect, cooldown, key-rotation, and pre-warm logic hardened against races (R1–R4).

All 26 audited defects are fixed and covered by automated tests.

## Download

### Windows

| File | Description |
|------|-------------|
| [com-ai_0.4.3_x64-setup.exe](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest/download/com-ai_0.4.3_x64-setup.exe) | Windows installer (NSIS) — recommended |
| [com-ai_0.4.3_x64_en-US.msi](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest/download/com-ai_0.4.3_x64_en-US.msi) | Windows installer (MSI) |

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

A macOS build of 0.4.3 is not available yet.

## Setup

AI features need a Google Gemini API key. Open **Settings** in the app and paste
in up to four keys — the app rotates through them to spread out free-tier rate
limits. Keys are stored only on your device.
