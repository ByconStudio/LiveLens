# Twitch Stream Management

## Overview

LiveLens offers a powerful integration with the Twitch API, enabling you to manage your channel's metadata and stream keys directly from the app. This allows for a smooth, "PC-like" experience for mobile gaming and variety streaming.

---

## 🛠️ Twitch Setup Interface

When you select Twitch in the Stream Setup dashboard, the app provides a comprehensive form to configure your broadcast before you go live.

### 1. Stream Information (Metadata)
LiveLens allows you to update your Twitch channel info in real-time:
- **Title**: Set your stream's catchy title (up to 140 characters).
- **Go Live Notification**: Customize the message sent to your followers' mobile devices (up to 140 characters).
- **Category Selection**: 
    - Use the **Search** field to find games or categories (e.g., "Just Chatting", "Minecraft").
    - Select from search results to update your stream's category instantly.
- **Tags**: 
    - Add up to **10 tags** to help viewers discover your stream.
    - Each tag can be up to 25 characters long.
- **Language**: Select your primary stream language from a comprehensive list (English, Hindi, Spanish, Japanese, etc.).
- **Content Classification**: Toggle safety labels required by Twitch (e.g., Profanity or Vulgarity, Violent & Graphic Content, Drugs or Intoxication).

### 2. Stream Key Management
- **Automatic Fetching**: If you are logged in, LiveLens automatically fetches your unique Twitch Stream Key.
- **Refresh Control**: If your key has changed or failed to load, use the **Refresh icon** to pull the latest key from your Twitch dashboard.
- **Secure Input**: The stream key is masked by default. Use the **Eye Icon** to view or hide it.

---

## 💬 Native Chat Integration

Connecting your Twitch account automatically enables the following:
- **High-Performance Chat**: The app authenticates your chat connection using your login token, ensuring reliable message delivery.
- **Auto-Connect**: Once you start your stream, the **Chat Box Source** (if added to your scene) will automatically begin fetching and displaying your Twitch chat.

---

## 🔐 Login Benefits

Logging in with Twitch via Official OAuth provides:
- **Zero-Manual-Paste**: No need to hunt for your stream key in the Twitch Dashboard website.
- **One-Tap Updates**: Change your game category and title for every new stream without leaving LiveLens.
- **Enhanced Security**: Official login methods ensure your password is never seen by the app.

---

## Twitch Stream Summary

| Feature | Description |
|---|---|
| Metadata Form | Update Title, Category, and Tags in-app |
| Category Search | Integrated search for all Twitch games/categories |
| Auto-Key Fetch | No manual stream key entry required |
| Classification Labels | Direct support for Twitch's content safety system |
| Language Support | Multi-language stream indexing |

---

## Related Documentation

- [Stream Setup Guide](../home/stream_setup.md)
- [Account Settings](../settings/account.md)
- [Live Chat Overlay](../sources/chatbox.md)
