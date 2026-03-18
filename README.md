# 📖 Chyoa Story Downloader (Android)

An Android application that allows you to download CHYOA stories directly to your device in multiple formats.

This app is inspired by the original CHYOA Story Downloader tool [1] and brings its core functionality into a native Android experience.

---

## ✨ Features

- ✅ Download CHYOA stories by pasting the **last chapter URL**
- ✅ Supported formats:
  - **HTML** (preserves structure and formatting) [1]
  - **TXT** (plain text version) [1]
  - **MP3** (Text-to-Speech audio) [1]
- ✅ Story preview before download [1]
- ✅ Optional **Table of Contents** [1]
- ✅ Automatic filename generation
- ✅ Live chapter fetching progress
- ✅ Proxy-based scraping logic (aligned with original tool) [1]
- ✅ Open file automatically after download
- ✅ Dark themed UI
- ✅ Adaptive book launcher icon

---

## 📥 How It Works

1. Paste the URL of the **last chapter** of a CHYOA story.
2. Tap **Load Story**.
3. The app fetches chapters backwards (like the original scraper logic).
4. Preview the Table of Contents.
5. Choose your preferred format.
6. Tap **Download**.
7. The file opens automatically after saving.

---

## 📂 Supported Formats

| Format | Description |
|--------|------------|
| HTML | Preserves chapter structure and formatting |
| TXT | Plain text version (no styling) |
| MP3 | Text-to-Speech audio version (experimental) |

---

## 📑 Table of Contents

You can choose whether to include a **Table of Contents**:

- ✅ Include — Adds clickable chapter navigation (HTML)
- ✅ Include — Adds numbered list (TXT)
- ✅ Include — Adds spoken chapter list (MP3)

---

## 📦 File Naming

If the filename field is left blank:
