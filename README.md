# Chyoa Story Downloader (Android)

An Android 8.0 application that allows you to download CHYOA stories directly to your device in multiple formats. 
It now has a build in browser as well.
---

## Features

- Download CHYOA stories by pasting the **last chapter URL**
- Supported formats:
  - **HTML** (preserves structure and formatting)
  - **TXT** (plain text version) 
  - **MP3** (Text-to-Speech audio) 
- Story preview before download
- Optional **Table of Contents**
- Automatic filename generation
- Live chapter fetching progress
- Proxy-based scraping logic
- Open file automatically after download

### Built‑in CHYOA Browser

- Full interactive WebView browser for chyoa.com
- JavaScript enabled
- Login supported
- Proper back navigation
- Respects status bar, notification bar & camera cutouts
- Floating overlay button:
  - Sends current chapter URL directly to downloader
  - Auto-fills URL field
  - Switches back to download screen

---

## Screenshots

![Demo VID](vid.mp4)

---

## How It Works
**Option 1 — Direct Download**
1. Paste the URL of the **last chapter** of a CHYOA story.
2. Tap **Load Story**.
3. The app fetches chapters backwards.
4. Preview the Table of Contents.
5. Choose your preferred format.
6. Tap **Download**.
7. The file opens automatically after saving.

**Option 2 — Use Built‑in Browser**

1. Tap Open CHYOA Browser.
2. Navigate normally on chyoa.com.
3. Open the chapter you want.
4. Tap the floating send button (bottom-right).
5. The app switches to the downloader.
6. URL is auto-filled.
7. Load & download.
---

## Supported Formats

| Format | Description |
|--------|------------|
| HTML | Preserves chapter structure and formatting |
| TXT | Plain text version (no styling) |
| MP3 | Text-to-Speech audio version (experimental) |

---

## Table of Contents

You can choose whether to include a **Table of Contents**:

- Adds clickable chapter navigation (HTML)
- Adds numbered list (TXT)
- Adds spoken chapter list (MP3)

---

## File Naming

If the filename field is left blank:
FirstChapterTitle-LastChapterTitle

---

## Scraping Logic

The scraper:

- Fetches chapters in reverse order
- Uses proxy-based requests
- Validates chapter structure
- Avoids infinite loops
- Emits live progress updates

---

## Architecture Overview
**UI Layer**
- Jetpack Compose
- Material 3 Design

**Network & Parsing**
- OkHttp (HTTP client)
- Jsoup (HTML parsing)
- Proxy-based fetch logic

**Export**
- HTML builder with anchor navigation
- TXT generator with numbering
- Android TextToSpeech → MP3 synthesis
- FileProvider for secure file access

**Browser Integration**
- Android WebView
- Proper system inset handling
- Modern back navigation support
- Floating overlay communication with MainActivity

---

## ⚠️ Disclaimer

This tool is intended for personal use only.
Please respect CHYOA’s:
- Terms of Service
- Content Guidelines
- Copyright policies

---

## Requirements
- Android 8.0 (API 26) or higher
- Internet connection

---
