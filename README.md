# 💎 PRISM Lossless Music Master Database

Official open-source database repository for **PRISM Vault Studio** and **PRISM Music Player**.

## 🌐 Public CDN Access

- **jsDelivr Edge CDN (Ultra-Fast):**
  ```
  https://cdn.jsdelivr.net/gh/mrahatcreations/Prism-music-database@main/vault.json
  ```
- **GitHub Raw:**
  ```
  https://raw.githubusercontent.com/mrahatcreations/Prism-music-database/main/vault.json
  ```

---

## 📋 JSON Schema (`vault.json`)

```json
[
  {
    "isrc": "USUMV2002770",
    "title": "Save Your Tears",
    "artist": "The Weeknd",
    "telegram_message_id": 4673,
    "file_id": "CQACAgUAAx0...",
    "quality": "FLAC",
    "format": "FLAC (24-bit / 96kHz Lossless)"
  }
]
```

---

## ⚡ Integration Architecture
- **Admin App (`PRISM_ADMIN`):** Directly commits and syncs new lossless studio tracks via GitHub REST API.
- **Player App (`Priam Player final`):** Caches `vault.json` in-memory for instant 0ms track lookup and playback.
- **Storage:** Telegram Supergroup Master Vault (Topic #4).