# Com AI Desktop — Downloads

Desktop application built with [Tauri](https://tauri.app/) + React/Vite.

**Latest version: `0.2.0`**

## Download

### Windows

| File | Description |
|------|-------------|
| [com-ai_0.2.0_x64-setup.exe](com-ai_0.2.0_x64-setup.exe) | Windows Installer (NSIS) — Recommended |
| [com-ai_0.2.0_x64_en-US.msi](com-ai_0.2.0_x64_en-US.msi) | Windows Installer (MSI) |

### Linux

| File | Description |
|------|-------------|
| [com-ai_0.2.0_amd64.deb](com-ai_0.2.0_amd64.deb) | Debian / Ubuntu package — Recommended |
| [com-ai-0.2.0-1.x86_64.rpm](com-ai-0.2.0-1.x86_64.rpm) | Fedora / RHEL / openSUSE package |
| [com-ai_0.2.0_amd64.AppImage](com-ai_0.2.0_amd64.AppImage) | Portable AppImage (any distro) |

Install on Debian/Ubuntu:

```bash
sudo apt install ./com-ai_0.2.0_amd64.deb
```

Or run the AppImage directly:

```bash
chmod +x com-ai_0.2.0_amd64.AppImage
./com-ai_0.2.0_amd64.AppImage
```

### macOS

| File | Description |
|------|-------------|
| [com-ai_0.2.0_universal.dmg](com-ai_0.2.0_universal.dmg) | Universal (Apple Silicon + Intel) |

## Building from source

You can also run the app directly on any platform:

```bash
git clone https://github.com/jyotiradityajmj1810/com_ai.git
cd com_ai
npm install
npm run tauri:dev      # dev, or: npm run tauri:build for local installers
```

Linux build prerequisites (Debian/Ubuntu):

```bash
sudo apt install libwebkit2gtk-4.1-dev libgtk-3-dev libappindicator3-dev librsvg2-dev patchelf
```

## Source Code

Source code is available at [jyotiradityajmj1810/com_ai](https://github.com/jyotiradityajmj1810/com_ai).
