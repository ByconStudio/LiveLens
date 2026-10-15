# Streaming Quality & Destinations

## Overview

The **Streaming Settings** in LiveLens are designed to provide a high-performance broadcast experience while maintaining connection stability. You can configure your resolution, bitrate, and stream to multiple platforms simultaneously.

---

## 🚀 Quality Configuration

Adjust these settings based on your internet speed and device performance.

### 1. Resolution & FPS
- **Resolutions**: Choose from 480p up to 4K (Depending on your [Performance Tier](../performance_limits.md)).
- **Frame Rate (FPS)**: Select **30 FPS** for stability or **60 FPS** for smooth gameplay.
- **Note**: Using 60 FPS or high resolutions increases heat and battery usage.

### 2. Video Bitrate
- **Bitrate (kbps)**: Controls the visual quality of your stream.
- **Recommendations**:
    - **720p 30fps**: 3250 kbps
    - **1080p 30fps**: 6500 kbps
    - **1080p 60fps**: 10,000 kbps
- **Manual Input**: You can type a specific bitrate in the text box for professional fine-tuning.

### 3. Adaptive Bitrate (ABR)
- **What it does**: Automatically lowers your stream quality when your internet connection becomes unstable, instead of letting the stream crash.
- **Recommendation**: Keep this **ON** to prevent "Buffer" or "Disconnect" issues for your viewers.

---

## 🛠️ Advanced Encoder Settings

These settings are for power users who want to fine-tune the video encoding process.

### 1. Video Encoder (Codec)
- **H.264**: The universal standard for streaming. Works on all platforms.
- **H.265 (HEVC)**: Higher efficiency but requires more CPU power. 
- **Note**: H.265 is currently supported for **Local Recording** only. Live broadcasts will always use H.264 for maximum compatibility.

### 2. I-Frame Interval
- Controls how often a full "keyframe" is generated. 
- **Recommendation**: Set to **2s** for most streaming platforms (YouTube/Twitch).

### 3. Sharpness
- **Strength**: Adjust from 0.0 to 1.0.
- **What it does**: Enhances the edges in your video to make the stream look "crisper". 
- **Warning**: High sharpness can sometimes introduce "noise" in low-light conditions.

---

## 📺 Streaming Destinations

LiveLens supports two ways to go live:

### 1. Account-Based (YouTube, Twitch, Facebook)
- Log in once in **Global Settings** → **Account**.
- One-tap "Go Live" with automatic stream title and chat integration.

### 2. Custom RTMP
- Stream to any platform (Kick, Trovo, Private Servers) by entering the **Server URL** and **Stream Key**.
- **Multi-Stream Support**: Enable **"Multi-Stream Mode"** in **Global Settings** → **Streaming** to add multiple RTMP destinations and go live on all of them at once.

---

## 📅 Stream Scheduling (YouTube)

If you are logged into YouTube, you can use the **"Create Schedule"** button on the home screen to:
- Set a future stream time.
- Update your stream Title and Description.
- Select your privacy setting (Public, Unlisted, or Private).

---

## 🔒 Settings Lock

All video and stream quality settings are **locked** while you are live. You must stop your stream to change resolutions or bitrates.

---

## Streaming Settings Summary

| Feature | Description |
|---|---|
| ABR | Prevents crashes by adjusting quality to network speed |
| Sharpness | Enhances video edge clarity (0.0 to 1.0 range) |
| Multi-Streaming | Stream to YouTube, Twitch, and RTMP at the same time |
| Scheduling | Manage YouTube stream metadata from the app |
| H.264 | Standard codec used for all live broadcasts |

---

## Related Documentation

- [Account Linking](./accounts.md)
- [Performance Tiers](../performance_limits.md)
- [Recording Settings](./recording.md)
