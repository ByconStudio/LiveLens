# Controls Panel Deep Dive

## Overview

The **Controls Panel**, located at the bottom-right of the Home Screen, is where you execute your main broadcasting actions. It provides a streamlined interface to go live, record, schedule events, and access system settings.

---

## 🚦 Status Indicator

At the top-right corner of the Controls Panel, you will see a status badge that reflects the current state of the engine:

- **READY**: Everything is initialized and you are prepared to start.
- **CONNECTING**: The app is currently handshaking with the streaming servers.
- **LIVE**: Your broadcast is actively being transmitted to your selected platforms.
- **RECORDING**: A local copy is being saved to your storage.

---

## 🔘 Panel Buttons

### 1. Start Streaming
This is the primary action button to begin your broadcast.
- **Detailed Setup**: Tapping this opens the [Stream Setup Interface](./stream_setup.md).
- **Single Stream**: If Multi-Stream is OFF, you select one destination (YouTube, Twitch, Custom, etc.) and go live.
- **Multi-Stream**: If enabled, you can toggle multiple connected accounts and stream to all of them at once.

### 2. Start Recording
Tap this to save a high-quality local copy of your current scene.
- **Independent Operation**: You can record without streaming, or record and stream at the same time.
- **Validation**: If your device storage is low, a warning may appear before recording starts.

### 3. Create Schedule (YouTube)
Manage your YouTube events directly from LiveLens.
- **Function**: Allows you to set a title, description, and privacy level (Public, Private, Unlisted) for a future stream.
- **🔐 YouTube Account Required**: If you are not logged into YouTube, tapping this button will trigger a **"YouTube Account Required"** popup.
    - This popup informs you that a login is necessary for scheduling.
    - You can choose to jump directly to the **Account Settings** tab to log in or handle it later.

### 4. Global Settings
Tapping this opens the full configuration suite of LiveLens.
- **Direct Access**: Instantly navigate to Canvas, Video, Audio, Accounts, VTuber, and Advanced settings tabs.
- **Real-time Updates**: Any settings changed here are applied instantly to the active scene once you return to the home screen.

---

## Related Documentation

- [Home Screen Overview](./home.md)
- [Account Linking](../settings/account.md)
- [Video & Stream Settings](../settings/video.md)
- [Advanced Settings](../settings/advanced.md)
