# Troubleshooting & FAQ

## Overview

This guide helps you resolve common issues encountered while using LiveLens. Most issues can be solved by checking permissions, internet speed, or device performance limits.

---

## 📸 Visual & Camera Issues

### Why is my camera screen black?
1. **Permission**: Ensure LiveLens has "Camera" permission in your phone settings.
2. **Device Conflict**: Close other apps that might be using the camera in the background.
3. **Toggle**: Try switching from Front to Back camera and back again in the source settings.

### I added an image/video, but it shows an error icon.
- This happens when the file has been **moved or deleted** from your phone's gallery.
- **Fix**: Use the **Missing Assets** dialog (found in Scene Manager) to relink the file to its new location.

---

## 🎙️ Audio Issues

### Why can't my viewers hear my game audio?
- **Android Restriction**: Some games (like Call of Duty or PUBG) might block 3rd-party apps from recording internal audio.
- **Fix**: Ensure "Mute Internal Audio" is OFF in **Global Settings** → **Audio**. On some Android versions, you must use a high-quality headset for the system to allow internal capture.

### My voice sounds metallic or has an echo.
- **Echo**: This happens if your speakers are too loud and the mic picks up the output. **Always use headphones** when streaming.
- **Processing**: Try enabling **Hardware Noise Suppression** and **Echo Cancellation** in Advanced Audio filters.

---

## ⚡ Performance & Lag

### The app is lagging or dropping frames.
1. **Tier Check**: Your device might be overloaded. Refer to [CPU Compatibility](./cpu_info.md) and [Performance Tiers](./performance_limits.md).
2. **Fixes**:
    - Lower your **Bitrate** to 3500 kbps.
    - Change **Resolution** to 720p 30fps.
    - Reduce the number of active sources (especially Web and VTuber).
    - Enable **Adaptive Bitrate (ABR)** in **Global Settings** → **Streaming**.

### How do I switch scenes while streaming?
- **Seamless Switching**: You can switch scenes directly from the Scene Manager or use the **Pinned Scenes** feature in the **Floating Panel** for quick transitions during gameplay.
- **Note**: Ensure your scenes use the same canvas resolution for the best experience.

---

## 🌐 Connection Issues

### Stream disconnected unexpectedly.
- Check your **Upload Speed**. Multi-streaming requires at least 15-20 Mbps for stable 1080p output.
- If you are on Mobile Data, signal fluctuations can drop the connection. Try switching to a stable Wi-Fi.

### Custom RTMP not working.
- Ensure your **Stream Key** is correct.
- Some platforms require `rtmps://` (secure) instead of `rtmp://`. Check your platform's dashboard.

---

## 🛠️ Still having issues?

1. **Reset Settings**: Use **"Reset to Performance Defaults"** in **Global Settings** → **Streaming** (or Video).
2. **Report Issue**: Tap the **"Send Feedback"** button in Settings -> Privacy or use the **"Report Issue"** button inside the UVC source.
3. **Join Discord**: Get real-time help from Arpan and the community: [Join LiveLens Discord](https://discord.gg/kUqmbKhs6w).

---

## Related Documentation

- [Performance Tiers](./performance_limits.md)
- [Audio Filters](./settings/audio.md)
- [Canvas Setup](./settings/canvas.md)
