# Chyoa Story Downloader (Android)

An Android application that allows you to download CHYOA stories directly to your device in multiple formats.

---

## Features

- Download CHYOA stories by pasting the **last chapter URL**
- Supported formats:
  - **HTML** (preserves structure and formatting)
  - **TXT** (plain text version) 
  - **MP3** (Text-to-Speech audio) 
- Story preview before download
- Optional **Table of Contents** [1]
- Automatic filename generation
- Live chapter fetching progress
- Proxy-based scraping logic (aligned with original tool) [1]
- Open file automatically after download

---

---

## Screenshots

*(Add screenshots here)*

---

## How It Works

1. Paste the URL of the **last chapter** of a CHYOA story.
2. Tap **Load Story**.
3. The app fetches chapters backwards (like the original scraper logic).
4. Preview the Table of Contents.
5. Choose your preferred format.
6. Tap **Download**.
7. The file opens automatically after saving.

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

## 📦 File Naming

If the filename field is left blank:
FirstChapterTitle-LastChapterTitle

---

## 🔄 Scraping Logic

The scraper:

- Fetches chapters in reverse order
- Uses proxy-based requests (like original implementation) [1]
- Validates chapter structure
- Avoids infinite loops
- Emits live progress updates

---

## 📱 Tech Stack

- Kotlin
- Jetpack Compose
- Material 3 (Dark Theme)
- Jsoup (HTML parsing)
- OkHttp (HTTP client)
- Android TextToSpeech API
- FileProvider (secure file opening)


## ⚠️ Disclaimer

This tool is intended for personal use.  
Respect CHYOA's terms of service and content guidelines.

---
