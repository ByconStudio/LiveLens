# Recording & Storage Settings

## Overview

LiveLens allows you to not only stream your content but also save high-quality local copies directly to your device. The **Recording & Storage** settings help you manage where your videos are saved and how they utilize your device's resources.

---

## 📂 Storage Management

### Estimated Recording Time
LiveLens features a built-in **Storage Estimator** that calculates how much footage you can record based on:
- Your current **Video Bitrate**.
- The **Available Free Space** in your selected storage location.
> **Note**: If you increase your bitrate, your estimated recording time will decrease.

### Save Location
By default, recordings are saved in `Internal/Movies/LiveLens`.
- **Change Location**: You can select any folder on your internal storage or an external **SD Card**.
- **Reset to Default**: Quickly switch back to the standard app folder.

---

## ⏺️ Local Recording

### Automatically Save Streams
Enable **Local Recording** to save a video copy of your broadcast while you are live. This is perfect for editing highlights later or uploading to other platforms.

### Performance & FPS Restrictions
Recording while streaming is resource-intensive. 
- On some device tiers, enabling local recording may restrict your **Frame Rate (FPS) to 30** to prevent the encoder from overloading and causing stream lag.

---

## ⚙️ Advanced Encoder Settings

These settings fine-tune how your video is processed.

### Video Encoder (H.264 vs H.265)
- **H.264**: The standard, most compatible codec.
- **H.265 (HEVC)**: Provides better quality at lower bitrates but requires more processing power.
> **Important**: H.265 is currently supported for **Local Recording only**. Active live streams will always use H.264 for maximum platform compatibility.

### I-Frame Interval
- Controls the frequency of "Keyframes" in your video (1s, 2s, or 5s).
- A lower interval (e.g., 1s) is better for high-action content but uses slightly more data.

---

## 🔒 Settings Lock & Reset

- **Safety Lock**: Video and recording settings are **locked** while you are actively streaming or recording to ensure system stability.
- **Performance Reset**: Use the **"Reset to Performance Defaults"** button to instantly restore stable settings (720p, 30fps, balanced bitrate) if you experience issues.

---

## Recording Settings Summary

| Feature | Description |
|---|---|
| Local Recording | Saves a high-quality copy of your stream |
| Storage Estimator | Shows how many hours of footage you can fit |
| Custom Save Path | Support for SD Cards and custom folders |
| H.265 Support | Advanced codec for local saves |
| Performance Defaults | One-tap fix for stable settings |

---

## Related Documentation

- [Canvas Setup](./canvas.md)
- [Streaming Setup](./streaming.md)
- [Performance Tiers](../performance_limits.md)
