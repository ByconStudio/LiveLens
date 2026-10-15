# Stream Setup & Destination Management

## Overview

The **Stream Setup** screen is the final step before you go live. It allows you to select where your broadcast will be sent. Depending on your settings, LiveLens provides two distinct setup workflows: **Single Stream** and **Multi-Stream**.

---

## ⚙️ Workflow Selection

The setup interface you see depends on the **Multi-Stream Mode** toggle found in **Settings → Account Settings**.

### 1. Single Stream Mode (Default)
Ideal for focused streaming to one primary platform.
- **Interface**: A streamlined popup with platform tabs (YouTube, Twitch, Facebook, Kick, Custom) at the top.
- **Operation**: You select one destination, configure its details, and tap **"Start Stream"**.

### 2. Multi-Stream Mode
Designed for creators who want to reach multiple audiences simultaneously.
- **Interface**: A dual-pane dashboard with a **Platform Menu** on the left and **Configuration Area** on the right.
- **Operation**: Use checkboxes to select multiple platforms, configure each one, and tap the bottom bar to **"Start Streaming on X Platforms"**.

---

## 📺 Destination Types

### 1. Integrated Platforms (YouTube, Twitch, Kick, Facebook)
If you have linked your accounts in settings, LiveLens simplifies the handshake process:
- **YouTube**: Displays your **Schedule List**. You can select a pre-created event or create a new one directly from the setup screen. See the [YouTube Detailed Guide](../stream/youtube.md) for more info.
- **Twitch**: Automatically fetches your **Stream Key** and allows you to update your **Stream Title**, **Category**, and **Tags** before going live. See the [Twitch Detailed Guide](../stream/twitch.md) for more info.
- **Kick**: Similar to Twitch, it fetches your stream details and supports updating channel metadata (Title/Category). See the [Kick Detailed Guide](../stream/kick.md) for more info.
- **Facebook**: Provides a direct link to your connected page or profile for easy configuration. See the [Facebook Detailed Guide](../stream/facebook.md) for more info.

### 2. Custom RTMP
For platforms not natively integrated (like Trovo, LinkedIn, or private servers).
- **RTMP URL**: Enter the server address provided by your platform (e.g., `rtmp://live.platform.com/app`).
- **Stream Key**: Paste your unique secret key. Use the **Eye Icon** to reveal or hide the key for security.
- **Auto-Save**: LiveLens remembers your last used custom RTMP details so you don't have to paste them every time.

---

## 🛠️ Key Features during Setup

### 🔄 Metadata Synchronization
For Twitch and Kick, LiveLens performs a "Metadata Sync" before the stream starts. This ensures that your stream title and game category are updated on the platform the moment you go live.

### 🔐 Secure Inputs
Stream keys are sensitive information. In Custom RTMP mode, the app uses **Password Masking** by default to protect your keys from being seen on camera or by others nearby.

### 📱 Immersive Configuration
When the Stream Setup screen is open, the app enters **Immersive Mode**, hiding system navigation bars to give you maximum space to review your settings.

---

## Stream Setup Summary

| Feature | Single Stream Mode | Multi-Stream Mode |
|---|---|---|
| **Max Platforms** | 1 | Unlimited (Internet permitting) |
| **Selection** | Top Tabs | Left Menu + Checkboxes |
| **Metadata Update** | Active platform only | All enabled platforms |
| **Setup Storage** | Remembers last selected | Persists all platform configs |

---

## Related Documentation

- [Controls Panel Deep Dive](./controls.md)
- [Account Linking](../settings/account.md)
- [Video & Bitrate Settings](../settings/video.md)
