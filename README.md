# Multi-Chat Overlay for OBS (YouTube + Twitch)

Realtime overlay that merges **YouTube Live Chat** and **Twitch IRC** into one feed
and shows it on‑screen via an OBS *Browser Source*.

![overlay preview](docs/screenshot.png)

## ✨ Features
* Merged feed with platform icons and coloured nicknames  
* Auto-detects the current YouTube live stream (no need to hard‑code video ID)  
* Quota‑safe defaults (8 s polling ⇒ 4‑hour stream fits free 10 000‑unit limit)  
* Self‑contained: one HTML file, no server, no build step

## 🚀 Quick start
```text
git clone https://github.com/yourname/multichat-overlay.git
open multichat-overlay/index.html
```
Then add it to OBS as a **Browser Source** (Width 400, Height 600).

Edit three constants at the top of *index.html*:
```js
const TWITCH_CHANNEL      = "your_twitch_login";
const YT_CHANNEL          = "your_yt_channel_nickname";
const YT_API_KEY          = "YOUR_YT_KEY_HERE";
```
See `docs/` for how to generate a key and understand quota.

## 📚 Documentation
* **docs/en_quota_calculation.md** – Quota & API setup (EN)  
* **docs/ru_quota_calculation.md** – Настройка API и квоты (RU)

Licensed under MIT.
