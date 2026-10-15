# YouTube Stream Management

## Overview

LiveLens provides deep integration with the YouTube Live API, allowing you to manage your broadcast events directly within the app. This eliminates the need to use the YouTube Studio website for basic stream configuration.

---

## 📅 Schedule Manager

When you select YouTube in the Stream Setup, you are presented with your **Scheduled Events List**.

- **Select Existing**: Choose any upcoming or ready event you created previously on YouTube or in LiveLens.
- **Refresh**: Tap the refresh icon to pull the latest events from your channel.
- **Create New**: Tap the **"+"** icon to open the **Schedule Live** dialog.

---

## 🛠️ Creating a New Event

The **Schedule Live** dialog allows you to configure every aspect of your YouTube broadcast:

### 1. Stream Info
- **Title**: The name of your stream as it will appear on YouTube.
- **Description**: Provide details about your broadcast.

### 2. Scheduled Time
- **Date & Time Pickers**: Set the exact moment you plan to go live. This helps YouTube notify your subscribers in advance.

### 3. Stream Settings
- **Privacy**: Choose between **Public**, **Unlisted**, or **Private**.
- **Category**: Select the type of content (e.g., Entertainment, Music, People & Blogs).
- **Game Search (Gaming Only)**: If you select the "Gaming" category, a **Search Game** field appears. You can search for specific game titles to ensure your stream is correctly indexed in YouTube's gaming section.
- **Latency**: 
    - **Normal**: Best for highest quality and 4K.
    - **Low**: Good for near real-time interaction.
    - **Ultra Low**: Best for highly interactive Q&A sessions.

### 4. Smart Automation
- **Auto Start**: When enabled, YouTube will automatically start the broadcast as soon as LiveLens begins sending data.
- **Auto Stop**: When enabled, the YouTube broadcast will automatically end when you stop the stream in LiveLens.

### 5. Mobile Optimization
- **Dual Stream (Shorts Feed)**: A unique LiveLens feature that optimizes your stream for **YouTube Shorts discovery**. It applies an auto-crop to help your content appear in the vertical Shorts feed while you stream.

### 6. Visual Branding
- **Custom Thumbnail**: Upload a **16:9 aspect ratio** cover image (Max 2MB) directly from your device to make your stream stand out in the feed.

---

## 🔐 Login Requirements

If you are not logged in, tapping "Create Schedule" or selecting YouTube will trigger a **Login Dialog**.
- **Official OAuth**: LiveLens uses YouTube's official secure login.
- **Permission**: The app requires permission to manage your YouTube Live events to function.

---

## YouTube Stream Summary

| Feature | Description |
|---|---|
| Schedule List | Manage and select existing YouTube events |
| Game Search | Dedicated indexing for gaming content |
| Auto Start/Stop | Hands-free stream state management |
| Shorts Optimization | Dual-stream feed for better discovery |
| Thumbnail Upload | Professional branding without leaving the app |

---

## Related Documentation

- [Stream Setup Guide](../home/stream_setup.md)
- [Account Settings](../settings/account.md)
- [Live Chat Overlay](../sources/chatbox.md)
