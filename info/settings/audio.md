# Audio Configuration & Filters

## Overview

LiveLens provides a professional-grade audio mixer and processing suite. You can manage multiple audio sources, apply real-time filters to your microphone, and monitor your own voice with low latency.

---

## 🎚️ Mixer Toggles

The Mixer section allows you to control the basic audio flow of your stream.

### Microphone Controls
- **Mute Microphone**: Instantly disable all audio input from your phone's mic.
- **Stereo Microphone Capture**: Enable this to capture high-quality spatial audio.
    - **Smart Fallback**: If your device hardware does not support stereo recording, LiveLens will automatically fall back to **Mono** to ensure your stream always has audio.
- **Microphone Monitoring**: Enable this to hear your own voice (with all filters applied) through your headphones. 
    - *Note: Using headphones is highly recommended when monitoring to prevent echo.*

### System & App Audio
- **Mute Internal Audio**: Toggle sounds coming from your games and other applications.
- **Sync with System Volume**: When enabled, you can control the app's internal mixer volume using your phone's physical volume buttons.
- **Capture Voice Chat**: Use this to include voice chat from other apps (like Discord or In-Game chat) directly into your stream mix via Direct Mixer Injection.

---

## 🛠️ Advanced Processing (Filters)

Clean up your audio and make your voice sound professional with real-time filters.

### 1. Gain & Threshold
- **Microphone Gain Boost**: Increase the raw volume of your microphone (up to 5x). Useful if your headset mic is naturally quiet.
- **Noise Gate Threshold**: Cuts off all audio below a certain volume level. This is perfect for removing "dead air" or slight background hum when you aren't speaking.

### 2. Frequency & Hardware Filters
- **High-Pass Filter (HPF)**: Removes low-frequency "rumble" noise caused by ceiling fans, wind, or air conditioners.
- **Hardware Noise Suppression**: Utilizes your phone's system-level noise cleaning algorithms to remove consistent background noise.
- **Hardware Echo Cancellation**: Prevents your speakers' output from being picked up by the microphone and creating a loop.
- **Auto Gain Control (AGC)**: Automatically adjusts your volume on the fly so your voice remains at a consistent level, even if you move closer to or further from the mic.

---

## Audio Settings Summary

| Setting | Description |
|---|---|
| Stereo Mic | Captures spatial audio (Auto-fallback to Mono if unsupported) |
| Monitoring | Hear your own voice in real-time |
| Voice Chat | Injects game/app chat into the stream mix |
| Volume Sync | Syncs mixer volume with physical phone buttons |
| Noise Gate | Removes background noise when you aren't talking |
| Gain Boost | Amplifies quiet microphones (up to 5x) |
| HPF | Removes deep humming or fan noises |

---

## Related Documentation

- [Sources](../sources/sources.md)
- [UVC Audio](../sources/uvc.md)
- [Video & Stream Settings](./video.md)
