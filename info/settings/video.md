# Video & Stream Settings

## Overview

The **Video & Stream Settings** in LiveLens are designed to provide a high-performance broadcast experience while maintaining connection stability and local recording quality. 

These settings are divided into three main sections: **Recording & Storage**, **Stream Quality**, and **Advanced Encoder Settings**.

---

## 🚀 Performance & Status Badges

At the top of the settings panel, you will see status indicators that inform you about your current configuration and device limits:

- **Settings Locked**: Appears when you are actively streaming or recording. You must stop the activity to change video configurations.
- **Device Optimization**: LiveLens automatically detects your **CPU Tier** (e.g., HIGH END, MID RANGE, ENTRY) and restricts resolutions and FPS to ensure stability.
- **Force Unlocked Mode**: If enabled in advanced settings, this bypasses hardware checks, allowing higher settings which may cause lag or crashes on weaker devices.

---

## 1. Recording & Storage

Manage how your videos are saved and monitor your device's capacity.

### 📊 Storage Estimation
LiveLens features a built-in estimator that calculates:
- **Estimated Recording Time**: How many hours/minutes of footage you can fit. This is calculated based on your **Video Bitrate**, which is directly influenced by your selected **Resolution** and **FPS** (higher quality settings require higher bitrates, thus reducing available recording time).
- **Available Storage**: Shows the free space in your selected location.

### ⏺️ Local Recording
Enable this to automatically save a high-quality video copy of your stream to your device. 
> **Note**: Enabling local recording on lower-tier devices may restrict your **FPS to 30** to prevent the processor from overloading.

### 📂 Save Location
- **Change Location**: Select any folder on internal storage or an external **SD Card**.
- **Reset to Default**: Quickly switch back to the standard `Internal/Movies/LiveLens` folder.

---

## 2. Stream Quality

Configure the visual clarity and smoothness of your broadcast.

### 📺 Resolution
Choose from **480p, 720p, 1080p, 1440p (2K), and 4K**.
- Available options are filtered based on your device's hardware capabilities.
- Higher resolutions require more upload bandwidth and CPU power.

### ⏱️ Frame Rate (FPS)
- **30 FPS**: Recommended for stability and most gameplay.
- **60 FPS**: Provides ultra-smooth motion for high-action content but requires a high-performance device and stable internet.

### 📉 Video Bitrate
- **Bitrate (kbps)**: Controls the visual data density. Higher bitrate equals better quality but requires faster upload speed.
- **Recommended Values**: The app shows recommendations for your selected resolution (e.g., 3250 kbps for 720p).
- **Manual Input**: You can use the slider or type a precise value in the text field.

### 📉 Adaptive Bitrate (ABR)
Automatically lowers your stream quality during network fluctuations to prevent the stream from lagging or disconnecting. **Recommendation: Keep this ON.**

---

## 3. Advanced Encoder Settings

Fine-tune how the video signal is processed by the hardware.

### 🎞️ Video Encoder (Codec)
- **H.264**: The universal standard for streaming. Highly compatible with all platforms.
- **H.265 (HEVC)**: Higher efficiency and better quality. 
- **Important**: H.265 is supported for **Local Recording ONLY**. Live broadcasts will always use H.264 to ensure they can be played back by streaming platforms.

### 🗝️ I-Frame Interval
Controls how often a full "keyframe" is generated (1s, 2s, or 5s). A **2s interval** is standard for YouTube and Twitch.

### 🗡️ Sharpness
Adjust from **0.0 to 1.0** to enhance the clarity of edges in your video. High sharpness makes the image look "crisper" but may introduce visual noise.

---

## 🔄 Reset to Defaults

If you experience performance issues or lag, use the **"Reset to Performance Defaults"** button. This instantly restores a stable configuration:
- **Resolution**: 720p
- **FPS**: 30
- **Bitrate**: 3250 kbps
- **Recording**: Disabled

---

## Video Settings Summary

| Feature | Description |
|---|---|
| ABR | Prevents stream crashes by adjusting quality to network speed |
| H.265 | Advanced codec for local recordings (high quality, small size) |
| Device Optimization | Automatically locks settings based on CPU power |
| Storage Estimator | Shows remaining footage time based on bitrate |
| Sharpness | Enhances video edge clarity (0.0 to 1.0 range) |

---

## Related Documentation

- [Canvas Settings](./canvas.md)
- [Advanced Settings](./advanced.md)
- [Performance Tiers](../performance_limits.md)
- [Account Linking](./account.md)
