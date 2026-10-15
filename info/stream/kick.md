# Kick Stream Management

## Overview

LiveLens provides direct integration with **Kick**, allowing creators to manage their stream details and connection settings without leaving the app. The integration is designed for high-performance streaming with support for Kick's native chat and metadata systems.

---

## 🛠️ Kick Setup Interface

When you select Kick in the Stream Setup dashboard, you can configure your broadcast using the dedicated Kick management form.

### 1. Stream Information (Metadata)
Update your channel details in real-time before going live:
- **Title**: Set your stream title (up to 128 characters).
- **Category Search**: 
    - Use the **Search** field to find specific games or categories on Kick.
    - Selecting a game from the results updates your channel's category instantly.
- **Language**: Choose your primary stream language (English, Hindi, Spanish, etc.) from the dropdown menu.
- **Mature Content Toggle**: Enable the **"18+ Mature Audience Only"** switch if your content is intended for adult audiences. This updates your stream's safety classification on Kick.

### 2. Stream Connection
- **Stream Key**: 
    - **Auto-Fetching**: LiveLens automatically pulls your stream key once you are logged in.
    - **Refresh**: Use the **Refresh icon** to re-sync your key if the connection fails or the key was reset on the Kick dashboard.
    - **Security**: The key is masked by default. Tap the **Eye Icon** to reveal it.
- **Server URL**: The app uses Kick's optimized global ingest points automatically.

---

## 💬 Native Chat Integration

Connecting your Kick account enables high-performance chat features:
- **Auth-Based Connection**: Uses your login token for a stable and fast chat connection.
- **Chat Box Support**: If you have a **Chat Box Source** in your scene, it will automatically connect to your Kick chat the moment your stream starts.

---

## 🔐 Login Benefits

By logging in with Kick via the official authentication flow:
- **No Manual Keys**: Forget about copying and pasting stream keys manually.
- **Instant Updates**: Change your game category and title on the fly for every stream.
- **Unified Dashboard**: Manage your Twitch and Kick metadata from the same interface in Multi-Stream mode.

---

## Kick Stream Summary

| Feature | Description |
|---|---|
| Metadata Management | In-app Title, Category, and Language updates |
| Category Search | Integrated database of all Kick gaming categories |
| Mature Toggle | One-tap 18+ content classification |
| Auto-Key Sync | Seamless stream key retrieval and refreshing |
| Native Chat | Reliable auth-based chat overlay support |

---

## Related Documentation

- [Stream Setup Guide](../home/stream_setup.md)
- [Account Settings](../settings/account.md)
- [Live Chat Overlay](../sources/chatbox.md)
