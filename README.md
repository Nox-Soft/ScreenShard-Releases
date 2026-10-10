<div align="center">

# ScreenShard

**Screenshots, screen recording and image tools — for Windows, with beta builds for Linux and macOS.**

**English** · [Українська](README.uk.md)

[Download the latest Windows version](https://github.com/Nox-Soft/ScreenShard-Releases/releases/latest) · [Linux and macOS beta builds](https://github.com/Nox-Soft/ScreenShard-Releases/releases)

[screenshard.nox-soft.studio](https://screenshard.nox-soft.studio)

</div>

---

## What it is

ScreenShard is a free app that lives in your system tray and helps you capture the
screen, record video, and annotate or process images quickly. Windows is the main
platform; **Linux and macOS are available as beta builds** (see [Installing](#installing)).

Beyond ordinary screenshots it can:

- **capture long scrolling pages** — the app scrolls and stitches one tall image for you
  (Windows and Linux);
- **record screen video** with system sound (Windows) and microphone, with pause that keeps
  one file;
- **annotate right on the shot** — pen, marker, line, arrow, rectangle, circle, triangle,
  heart, text, blur, numbered steps; each tool has an adjustable line width, and closed
  shapes can be an outline or filled;
- **recognise text in an image (OCR)** — the text appears right on your selection, so you
  can pick out any fragment and copy just that; the language is detected automatically and
  it can be translated on the spot;
- **search the web by image** — Google Lens, Bing or TinEye;
- **pick a colour from the screen** — with a magnifier from 2× to 32×, a name for every shade
  ("dark muted turquoise"), and a palette of 8 dominant colours from a selection;
- **read QR codes** directly inside your selection;
- **find sensitive data** (email, phone, card number, IBAN, keys) and offer to mask it;
- **remove and replace photo backgrounds**;
- **enhance images** — upscale, sharpness, colour, noise;
- **build nice mockups** — browser, macOS, Windows, Linux, phone, tablet and laptop frames
  with shadow, background and tilt;
- **compare two screenshots** and see exactly what changed — highlight, heatmap or mask,
  with a before/after shutter and change-by-change navigation;
- **convert** images, video and audio between formats;
- **apply a watermark** automatically when saving or copying.

All screenshots, recordings and text are stored **on your computer only**.

## Installing

Every platform has its own releases. A tag without a suffix (`vX.Y.Z`) is the **Windows**
release and is marked *Latest*; `vX.Y.Z-linux` and `vX.Y.Z-mac` are **beta** pre-releases for
Linux and macOS. Open the [releases page](https://github.com/Nox-Soft/ScreenShard-Releases/releases)
and pick the release for your system.

### Windows

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

### Linux (beta, x64)

Pick the release tagged `-linux`. Tested on Fedora; other distributions are experimental.

| File | Who it's for |
|---|---|
| `ScreenShard-<version>-x86_64.AppImage` | Runs on most distributions with no installation: `chmod +x ScreenShard-*.AppImage`, then `./ScreenShard-*.AppImage`. Updates itself in place. |
| `ScreenShard-<version>-amd64.deb` | Debian, Ubuntu and derivatives. |
| `ScreenShard-<version>-x86_64.rpm` | Fedora, openSUSE and derivatives. |

The `.sha512` files next to them are checksums (base64) if you want to verify a download.

- On **GNOME** there is no native tray icon, so ScreenShard opens a small window with
  buttons for the capture panel, Settings and Quit (it also shows in Alt+Tab).
- On **Wayland**, global shortcuts go through the system's shortcuts portal, which asks for
  confirmation once. Some keys (arrows, Home/End, Insert/Delete, PageUp/PageDown, F13+,
  PrintScreen) work only through that portal. In **Settings → Hotkeys** every field has a
  list button, so any key can be picked even if the desktop has grabbed it.
- The **long scrolling screenshot** needs `ydotool` and `kdotool`. The `.deb` sets them up
  for you; for the AppImage and `.rpm` install them yourself.
- `.deb` and `.rpm` installs do not update themselves — install the newer package instead.

### macOS (beta, Intel x64)

Pick the release tagged `-mac`: `ScreenShard-<version>-mac-x64.dmg` or `.zip`. The build is
for Intel; on Apple Silicon it runs through Rosetta.

- The app is **not signed or notarized yet.** On first launch right-click `ScreenShard.app`
  → **Open** (or allow it in System Settings → Privacy & Security).
- Grant **Screen Recording** (screenshots) and **Accessibility** (global hotkeys) in System
  Settings → Privacy & Security, then restart ScreenShard.
- There is no `PrintScreen` key on a Mac: open the capture panel from the tray icon or give
  it your own shortcut in **Settings → Hotkeys**.
- The app updates itself: it downloads the new `.app`, checks its checksum, swaps it in after
  quitting and rolls back if anything goes wrong. The folder with the app must be writable.

## First run

1. After installing, ScreenShard **minimises to the system tray** — look for its icon near
   the clock (on a Mac, in the menu bar). There is no separate main window.
2. Press **`PrintScreen`** (Windows) to open the capture panel, or click the tray icon.
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
| Compare images | `Alt+Shift+D` |
| Colour picker | `Alt+Shift+P` |

Every shortcut can be changed in **Settings → Hotkeys**. One combination can belong to only
one action: Settings refuses a taken combination and names the action that holds it.

## Where your files go

By default the app creates its own folders inside your standard user folders (Windows
spelling shown; on Linux and macOS they are the same folders — `Pictures/ScreenShard` and so on):

| What | Where |
|---|---|
| Screenshots | `Pictures\ScreenShard` |
| Video | `Videos\ScreenShard` |
| Audio | `Music\ScreenShard` |
| Recognised text | `Documents\ScreenShard` |
| Photo-search history | `Pictures\ScreenShardSearch` |

Any of these can be changed in **Settings → Tools**. If the video folder cannot be written
to, the recording goes to `Videos/ScreenShard` and then `Documents/ScreenShard`, and you are
told where it ended up.

## Formats

- **Screenshots:** PNG, JPG, WebP, PDF
- **Video:** MP4, WebM, GIF
- **Converter, images:** JPG, PNG, WebP, BMP, TIFF, ICO, TGA
- **Converter, video:** MP4, WebM, GIF, MOV, AVI, MKV
- **Audio:** MP3, WAV, AAC, OGG, FLAC

## Recording

- Area, window or the whole screen; FPS 30, 60, 144, 240 or 360 (on Windows an area or the
  screen is never recorded above the monitor's refresh rate); cursor on or off.
- On **Windows** an area or the screen is captured through the GPU (DXGI) — about 50 frames
  per second instead of 16–22 in our tests; the older GDI capture steps in on a remote
  desktop or when the area spans several monitors.
- **Pause** keeps a single file. Start waits until the recorder is ready (grey indicator,
  then green).
- After Stop a "Processing video…" window appears while the file is saved. There is no
  save dialog — the file goes straight to the video folder named by date and time. MP4 is
  saved almost instantly; WebM and GIF are re-encoded, so they take longer.
- **System sound** is recorded on Windows only; on Linux and macOS the button is disabled.

## Annotating and colours

- Choosing the pen, marker or a shape opens a narrow **options panel**: a vertical slider and
  a number field, 1–64 px (defaults: pen 3, marker 16, shapes 3). Rectangle, circle, triangle
  and heart also get **Outline / Fill**.
- The **eyedropper** loupe starts at 4×; hold `Ctrl` and scroll to go from 2× to 32× (the pixel
  grid appears from 4×). It shows the shade name, and the palette and colour windows add hue,
  saturation, lightness and which text colour reads better on it, with the contrast ratio.

## Updates

ScreenShard checks for a new version by itself: shortly after start, then every half hour,
looking only at releases for your own platform. When an update is available there is a menu
entry in the tray (and, on Windows, also a tray notification). The update is downloaded and
applied in the update window, and the app restarts on its own. The update window does not
pop up by itself — it opens when you click the notification or the menu entry.

There is nothing to reinstall by hand on Windows, in the Linux AppImage or on macOS. If you
prefer, you can always just download the newer file from the releases page.

## Uninstalling

- **Windows:** **Start → Settings → Apps → ScreenShard → Uninstall**, or run
  **`Uninstall ScreenShard.exe`** in the install folder. The uninstaller removes the app, its
  settings and the start-with-Windows entry. The portable build needs no uninstalling — just
  delete the file.
- **Linux:** remove the `.deb`/`.rpm` package with your package manager, or delete the
  AppImage. Turn autostart off in **Settings → General** first if you had it on.
- **macOS:** move `ScreenShard.app` to the Trash.

**Your saved screenshots, videos and text stay where they are** — delete those separately if
you want to.

## Language

The interface is available in **Ukrainian** and **English**. You pick a language during
installation (Windows) and can change it any time in **Settings → General → Language**. A
restart may be needed for it to apply everywhere.

## Privacy

- Screenshots, recordings and recognised text are **kept on your computer only**. The app
  does not upload them anywhere on its own.
- **Anonymous usage statistics are on by default** and can be switched off in
  **Settings → General** ("Anonymous statistics"). Only de-identified actions (for example
  "saved a PNG") and the OS version are sent to Google Analytics, under a random identifier
  generated on your device. **Never sent:** your screenshots, videos, recognised text,
  clipboard, file names and paths, app names, keys and passwords. With the switch off, not a
  single request is made.
- The app uses the internet only for:
  - the statistics above, unless you turn them off;
  - checking for and downloading updates from GitHub;
  - **image search** — here the selected image really is sent to Google Lens, Bing or
    TinEye. This only happens when you trigger a search;
  - **translation** of recognised text — the text is sent to a translation service;
  - **AI hand-off** (ChatGPT / Gemini / Claude) — opens the service in your browser and
    inserts your capture there; again, only on your action;
  - a one-time download of text-recognition language data and of the models for AI background
    removal and AI upscaling (afterwards they run from the local cache);
  - loading the icon font used by a few windows (most icons are built in).

## Selecting an area

While you drag out a selection — or resize one by its corner handles:

- hold **Ctrl** or **Shift** for a perfect square;
- hold **Alt** to draw from the centre, so the point you pressed becomes the middle;
- click the **size badge** to type an exact width and height, pick a ready-made size, or
  lock an aspect ratio that then keeps itself;
- use the **arrow keys** to nudge by one pixel, **Shift+arrow** to resize, **Alt** for a
  step of ten;
- click the **padlock** on the size badge to freeze the area so you cannot move or resize
  it by accident.

You can press or release a key in the middle of dragging — the frame reshapes immediately.

## Good to know

- **Windows is the main platform.** Linux and macOS builds are **beta** — expect some bugs
  there; tell us if something breaks.
- **Linux and macOS limits:** system sound is not recorded; recording without the cursor or
  across several monitors is likely to fail; a long scrolling screenshot is not available on
  macOS; on Linux it needs `ydotool` and `kdotool`.
- **`PrintScreen` no longer opens Snipping Tool (Windows).** So the key can work for ScreenShard,
  the app turns off the Windows "PrtScn opens Snipping Tool" behaviour. You can restore it in
  Windows Settings (Accessibility → Keyboard), but then assign ScreenShard a different key.
- **Some things need internet:** a few interface icons may not appear (four windows load an icon font), the first text recognition
  won't start, AI background removal and AI upscaling can't fetch their models, and image
  search, translation and the AI hand-off won't work. Screenshots, video recording, the
  editor, the converter and mockups all work offline.
- **The Integrations tab in Settings is currently disabled** — there is no cloud storage or
  publishing to services in this version.
- The software is provided "as is", without warranty. Licensed under MIT.

## Issues and suggestions

Open an issue at [ScreenShard-Releases/issues](https://github.com/Nox-Soft/ScreenShard-Releases/issues).
Please include your app version (shown in **About**), your system (Windows / Linux with the
desktop you use / macOS) and, if you can, steps to reproduce.

The full list of changes for each version is in the `CHANGELOG-<version>.md` file on that
release's page (in both languages); the Linux and macOS releases each carry their own notes.
