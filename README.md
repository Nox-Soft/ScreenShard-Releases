<div align="center">

# ScreenShard

**Screenshots, screen recording and image tools for Windows.**

**English** · [Українська](README.uk.md)

[Download the latest version](https://github.com/Nox-Soft/ScreenShard-Releases/releases/latest)

[screenshard.nox-soft.studio](https://screenshard.nox-soft.studio)

</div>

---

## What it is

ScreenShard is a free Windows app that lives in your system tray and helps you capture the
screen, record video, and annotate or process images quickly.

Beyond ordinary screenshots it can:

- **capture long scrolling pages** — the app scrolls and stitches one tall image for you;
- **record screen video** with system sound and microphone;
- **recognise text in an image (OCR)** and translate it right away;
- **search the web by image** — Google Lens, Bing or TinEye;
- **pick a colour from the screen** and extract a colour palette from a selection;
- **read QR codes** directly inside your selection;
- **find sensitive data** (email, phone, card number, IBAN, keys) and offer to mask it;
- **remove and replace photo backgrounds**;
- **enhance images** — upscale, sharpness, colour, noise;
- **build nice mockups** — browser, macOS, Windows, Linux, phone, tablet and laptop frames
  with shadow, background and tilt;
- **convert** images, video and audio between formats;
- **apply a watermark** automatically when saving or copying.

All screenshots, recordings and text are stored **on your computer only**.

## Installing

Open the [latest release page](https://github.com/Nox-Soft/ScreenShard-Releases/releases/latest)
and pick one file:

| File | Who it's for |
|---|---|
| **`ScreenShard-<version>-Installer.exe`** | **Recommended.** A normal setup wizard: choose folder, language, desktop shortcut and start-with-Windows. |
| `ScreenShard-Setup.exe` | Alternative installer, in case the first one won't start. |
| `ScreenShard-<version>-Portable.exe` | Portable build — nothing is installed, it runs from a single file (e.g. a USB stick). |

The other files on the release page (`app.asar`, `latest.yml`, `.sha512`, module archives)
are internal — they are only used by the automatic updater. You don't need to download them.

**Default install folder:** `%LOCALAPPDATA%\Programs\ScreenShard` (no administrator rights
needed).

**Windows or your antivirus may warn about an unknown publisher** — the files are not signed
with a developer certificate. That is expected for a free app without commercial signing.

## First run

1. After installing, ScreenShard **minimises to the system tray** — look for its icon near
   the clock. There is no separate main window.
2. Press **`PrintScreen`** to open the capture panel, or click the tray icon.
3. Choose a mode (Area / Window / Screen / Long / Polyline) and select what you need.
4. Then Save, Copy, Pin to screen, or send the capture to a tool or an AI assistant.

Right-clicking the tray icon opens a menu with galleries, tools and settings.

## Keyboard shortcuts

| Action | Keys |
|---|---|
| Open capture panel | `PrintScreen` |
| Capture area | `Alt+Shift+S` |
| Capture window | `Alt+Shift+W` |
| Capture whole screen | `Alt+Shift+F` |
| Long scrolling capture | `Alt+Shift+L` |
| Record video | `Alt+Shift+V` |
| Screenshot gallery | `Alt+Shift+G` |
| Video gallery | `Alt+Shift+M` |
| Recognised-text history | `Alt+Shift+H` |
| Photo-search history | `Alt+Shift+J` |
| Settings | `Alt+Shift+O` |
| Editor | `Alt+Shift+E` |
| Converter | `Alt+Shift+C` |
| Background tools | `Alt+Shift+B` |
| Audio | `Alt+Shift+A` |
| Image enhancer | `Alt+Shift+I` |
| Mockup frames | `Alt+Shift+K` |
| Colour picker | `Alt+Shift+P` |

Every shortcut can be changed in **Settings → Hotkeys**.

## Where your files go

By default the app creates its own folders inside your standard user folders:

| What | Where |
|---|---|
| Screenshots | `Pictures\ScreenShard` |
| Video | `Videos\ScreenShard` |
| Audio | `Music\ScreenShard` |
| Recognised text | `Documents\ScreenShard` |
| Photo-search history | `Pictures\ScreenShardSearch` |

Any of these can be changed in **Settings → Tools**.

## Formats

- **Screenshots:** PNG, JPG, WebP, PDF
- **Video:** MP4, WebM, GIF
- **Converter, images:** JPG, PNG, WebP, BMP, TIFF, ICO, TGA
- **Converter, video:** MP4, WebM, GIF, MOV, AVI, MKV
- **Audio:** MP3, WAV, AAC, OGG, FLAC

## Updates

ScreenShard checks for a new version by itself: shortly after start, then every half hour.
When an update is available you get a tray notification and a menu entry. The update is
downloaded and applied in the update window, and the app restarts on its own.

There is nothing to reinstall by hand. If you prefer, you can always just download the newer
installer from the releases page.

## Uninstalling

- **Start → Settings → Apps → ScreenShard → Uninstall**, or
- run **`Uninstall ScreenShard.exe`** in the install folder.

The uninstaller removes the app, its settings and the start-with-Windows entry. **Your saved
screenshots, videos and text stay where they are** — delete those separately if you want to.

The portable build needs no uninstalling — just delete the file.

## Language

The interface is available in **Ukrainian** and **English**. You pick a language during
installation and can change it any time in **Settings → General → Language**. A restart may
be needed for it to apply everywhere.

## Privacy

- Screenshots, recordings and recognised text are **kept on your computer only**. The app
  does not upload them anywhere on its own.
- No usage analytics or telemetry is collected or sent.
- The app uses the internet only for:
  - checking for and downloading updates from GitHub;
  - **image search** — here the selected image really is sent to Google Lens, Bing or
    TinEye. This only happens when you trigger a search;
  - **translation** of recognised text — the text is sent to a translation service;
  - **AI hand-off** (ChatGPT / Gemini / Claude) — opens the service in your browser and
    inserts your capture there; again, only on your action;
  - a one-time download of text-recognition language data and of the models for AI background
    removal and AI upscaling (afterwards they run from the local cache);
  - loading the interface icon font.

## Good to know

- **Windows only.** There are no macOS or Linux builds.
- **`PrintScreen` no longer opens Snipping Tool.** So the key can work for ScreenShard, the
  app turns off the Windows "PrtScn opens Snipping Tool" behaviour. You can restore it in
  Windows Settings (Accessibility → Keyboard), but then assign ScreenShard a different key.
- **Some things need internet:** interface icons may not appear, the first text recognition
  won't start, AI background removal and AI upscaling can't fetch their models, and image
  search, translation and the AI hand-off won't work. Screenshots, video recording, the
  editor, the converter and mockups all work offline.
- **The Integrations tab in Settings is currently disabled** — there is no cloud storage or
  publishing to services in this version.
- The software is provided "as is", without warranty. Licensed under MIT.

## Issues and suggestions

Open an issue at [ScreenShard-Releases/issues](https://github.com/Nox-Soft/ScreenShard-Releases/issues).
Please include your app version (shown in **About**) and, if you can, steps to reproduce.

The full list of changes for each version is in the `CHANGELOG-<version>.md` file on that
release's page (in both languages).
