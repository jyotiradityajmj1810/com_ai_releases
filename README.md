# Com AI Desktop — Downloads

Desktop app for **Elite English Coach**, built with [Tauri](https://tauri.app/) + React/Vite.

**Latest version: `0.4.3`** — [release notes](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/latest)

### What's new in 0.4

- **Reports even for long or dropped calls**, with Retry if a report fails.
- **Fewer voice breaks**, and the coach **stays in English**.
- **Full transcripts** for every session in History.
- **Accurate analytics** in your local time, and **much lower memory use**.
- **Backup & Restore** in Settings, plus automatic data upgrades.

> ⚠️ **0.4.3 was withdrawn.** Its update deleted the transcripts of older sessions. If you installed it, update to 0.4.4 now.

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
| [com-ai_0.4.4_amd64.deb](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.4/com-ai_0.4.4_amd64.deb) | Debian / Ubuntu package |
| [com-ai-0.4.4-1.x86_64.rpm](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.4/com-ai-0.4.4-1.x86_64.rpm) | Fedora / RHEL / openSUSE package |
| [com-ai_0.4.4_amd64.AppImage](https://github.com/jyotiradityajmj1810/com_ai_releases/releases/download/v0.4.4/com-ai_0.4.4_amd64.AppImage) | Portable AppImage (any distro) |

Install on Debian/Ubuntu:

```bash
sudo apt install ./com-ai_0.4.4_amd64.deb
```

Or run the AppImage directly:

```bash
chmod +x com-ai_0.4.4_amd64.AppImage
./com-ai_0.4.4_amd64.AppImage
```

### macOS

A macOS build of 0.4.3 is not available yet.

## Setup

AI features need a Google Gemini API key. Open **Settings** in the app and paste
in up to four keys — the app rotates through them to spread out free-tier rate
limits. Keys are stored only on your device.
