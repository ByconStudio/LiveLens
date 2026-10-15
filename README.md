<div align="center">

# 🎬 LiveLens

### Professional Live Streaming, Recording & Production Suite for Android

**PC-style production control directly from your phone**

Stream • Record • Create • Control • Produce

---

### ⚡ Quick Links

[![Download](https://img.shields.io/badge/📲_Download-LiveLens-2563EB?style=for-the-badge&labelColor=1f2937)](https://www.livelens.live/)
[![Features](https://img.shields.io/badge/✨_Explore-All_Features-7C3AED?style=for-the-badge&labelColor=1f2937)](https://www.livelens.live/pages/feature.html)
[![Documentation](https://img.shields.io/badge/📖_Docs-Hub-059669?style=for-the-badge&labelColor=1f2937)](https://www.livelens.live/pages/docs.html)
[![Star us on GitHub](https://img.shields.io/github/stars/ByconStudio/LiveLens?style=for-the-badge&logo=github&labelColor=1f2937&color=FFD700)](https://github.com/ByconStudio/LiveLens/stargazers)
[![Discord](https://img.shields.io/badge/💬_Join-Discord-5865F2?style=for-the-badge&labelColor=1f2937)](https://discord.gg/kUqmbKhs6w)
[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-GitHub-pink?style=for-the-badge&logo=github&labelColor=1f2937)](https://github.com/sponsors/ByconStudio)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge&labelColor=1f2937)](info/LICENSE.md)

---

<a href="https://www.livelens.live/" target="_blank">
  <img src="https://img.shields.io/badge/🌐_Visit_Website-Get_APK_Now-FF6B6B?style=for-the-badge&logoColor=white" alt="Visit LiveLens Website">
</a>

### 📱 Android Only • Android 10+ Required

</div>

---

## 🎯 What is LiveLens?

**LiveLens** brings **OBS-style, empty-canvas production workflow** directly to mobile creators. Instead of forcing you into pre-defined layouts or rigid templates, LiveLens gives you an empty canvas where you can place, layer, transform, and arrange your own sources to build custom streaming setups.

Whether you are a **Gamer, IRL Streamer, Content Creator, VTuber, or Influencer**, LiveLens puts studio-grade production power right in your pocket.

> **"Freedom in your pocket, not a smaller version of a locked-down tool."**

---

## 👨‍💻 Built by a Creator, for Creators

LiveLens was born from real streaming experience. It is developed and led by **Arpan Das**, an independent creator and streamer based in Kolkata, India, under **Bycon Studio**. 

Tired of the limitations, mandatory watermarks, intrusive ads, and subscription paywalls of existing mobile streaming tools, Arpan spent years self-teaching OpenGL ES rendering, hardware video encoding pipelines, and audio mixing to build a zero-compromise tool for the community.

### 🌟 Core Principles
- 🚫 **Zero Watermarks & Zero Forced Ads** – Your broadcast belongs to you.
- 🔐 **Privacy First** – No mandatory account creation or data harvesting.
- 🎨 **Empty-Canvas Freedom** – Complete control over your scene layouts.
- 💡 **Community Funded** – Supported by sponsorships and optional user contributions.

---

## 📸 Visual Preview

<div align="center">

![LiveLens Preview Grid](https://pub-94c38fc644f94737b41d832ef8c28371.r2.dev/Screenshot/screenshot.gif)

**Desktop-Class Production on Mobile**

</div>

---

## 🚀 Key Features & Sources

### 🎨 Rendering Engine
- ⚡ **GPU-Accelerated OpenGL ES**: Ultra-low latency FBO-based composition.
- 🔄 **Real-Time Transforms**: Scale, rotate, crop, and layer sources dynamically.
- 🖼️ **Unified Scene Pipeline**: Single composition pass for live preview, streaming, and local recording.
- ⚡ **60 FPS Hardware Encoding**: Smooth high-framerate output on modern mobile GPUs.

### 📡 Streaming & Recording
- 🌐 **Multi-Platform RTMP / RTMPS**: Direct streaming to **Twitch**, **YouTube Live**, **Facebook Live**, **Kick**, **Instagram**, and custom servers.
- 📹 **4K & High Bitrate Recording**: Concurrent local recording up to 4K resolution at 30/60 FPS.
- ⚙️ **H.264 & H.265 (HEVC)**: Flexible hardware encoder selection.
- 📊 **Adaptive Bitrate (ABR)**: Dynamic quality scaling based on network conditions and device thermal load.

### 🧩 11 Modular Source Types
Combine any of the following sources into custom scenes:

| Source | Description | Documentation |
|---|---|---|
| 🖥️ **Screen Capture** | Low-latency game screen recording & live streaming | [Guide](info/sources/screen_capture.md) |
| 📹 **Camera** | Front & Back camera capture with exposure, focus & zoom control | [Guide](info/sources/camera_settings.md) |
| 📝 **Text** | Dynamic text overlays, titles, custom fonts, and colors | [Guide](info/sources/text.md) |
| 🖼️ **Image** | PNG/JPG overlay graphics, logos, and banners | [Guide](info/sources/image.md) |
| 🖼️ **GIF** | Animated stickers, alert animations, and badge overlays | [Guide](info/sources/gif.md) |
| 🎥 **Video** | Background video loops, intros, and media playback | [Guide](info/sources/video.md) |
| 🌐 **Web Source** | Real-time web pages, custom alert boxes, and browser overlays | [Guide](info/sources/web.md) |
| 💬 **Chat Box** | Embedded live stream chat overlay for viewer interaction | [Guide](info/sources/chatbox.md) |
| 👾 **VTuber Avatar** | Native Live2D Cubism v5.1 (5.3+ compat) with mic lip-sync & physics | [Guide](info/sources/vtuber.md) |
| 🔌 **UVC (Capture Card)** | Connect external HDMI capture cards via USB-C (Beta) | [Guide](info/sources/uvc.md) |
| 🔊 **Sound** | Background music tracks, sound effects, and audio clips | [Guide](info/sources/sound.md) |

### 🎙️ Studio-Grade Audio
- 🎚️ **Dual-Channel Capture**: Record internal system audio and microphone simultaneously.
- 🛡️ **Advanced Filters**: Hardware Noise Suppression, Echo Cancellation, and Automatic Gain Control (AGC).
- 📈 **Real-Time Level Meters**: Floating audio level adjusters and multi-channel audio mixing.

### 🎧 Voice Chat & Team Rooms
- 🚀 **Account-Free Voice Rooms**: Instant room creation with zero sign-up.
- 🔗 **Deep-Link Sharing**: Join team chat via a single shareable link.
- 💻 **Cross-App Communication**: Full interoperability between LiveLens & LiveLens Lite.

---

## ⚡ Performance Tiers & Hardware Optimization

LiveLens automatically categorizes your device into a **Performance Tier** based on its SoC (processor) to maintain stable framerates and prevent thermal throttling.

### 📊 Device Tiers & Default Source Limits

| Tier | Example Devices | Recommended Limits (Text / Image / Web / Video / Sound) | Max FPS / Res |
|---|---|---|---|
| **Entry** | Helio G80 / Snapdragon 680 | 3 / 2 / 1 / 0 / 1 | 720p 30 FPS |
| **Low-Mid** | Snapdragon 720G / Dimensity 700 | 4 / 2 / 1 / 0 / 1 | 720p 30 FPS |
| **Mid** | Snapdragon 778G / Dimensity 1080 | 5 / 3 / 2 / 1 / 1 | 1080p 30 FPS |
| **Upper-Mid** | Snapdragon 870 / Dimensity 8100 | 6 / 4 / 2 / 1 / 1 | 1080p 60 FPS |
| **Flagship** | Snapdragon 8 Gen 1 / Dimensity 9000 | 8 / 5 / 3 / 2 / 2 | 1080p 60 FPS / 4K |
| **Ultra Flagship** | Snapdragon 8 Gen 2/3 / Dimensity 9300+ | 10 / 6 / 4 / 3 / 2 | 4K 60 FPS |

### 🔒 Fixed Hardware Constraints
Due to extreme CPU/GPU rendering demands or Android system limits, the following sources have a **fixed limit of 1**:
- 👾 **VTuber Source**: Fixed at **1** (Live2D physics & lip-sync rendering pipeline).
- 🔌 **UVC Capture Card**: Fixed at **1** (USB video bandwidth restriction).
- 🖥️ **Screen Capture**: Fixed at **1** (Android OS media projection limit).
- 📹 **Camera**: Fixed at **1** active camera feed on most tiers.

### 🚀 Boost Mode & Custom Limits
Advanced users can manually override default tier limits:
1. Navigate to **Global Settings** → **Advanced**.
2. Enable **Custom Source Limits** to boost limits up to **20 Text**, **15 Images**, **10 Web**, and **5 Videos**.
3. Toggle **Unlock All Settings** to force-enable 4K resolution or 60 FPS modes on supported hardware.

*For full details, see [Performance Limits & Source Tiers](info/performance_limits.md).*

---

## 📋 Mobile Streaming Feature Comparison

| Feature | LiveLens | Most Mobile Streaming Apps |
|---------|----------|----------------------------|
| 🎨 Empty Canvas & Multi-Scene | ✅ Full OBS Freedom | ❌ Fixed Templates |
| 👾 Live2D / VTuber Support | ✅ Native Cubism v5.1/5.3+ | ❌ None / Restricted |
| 🌐 Web & Custom HTML Sources | ✅ Full Interactive Support | ⚠️ Very Limited |
| 🔌 USB Capture Card (UVC) | ✅ Supported (Beta) | ❌ Unsupported |
| 🎙️ Concurrent Mic + Game Audio | ✅ Supported | ⚠️ Device Dependent |
| 🎧 Integrated Team Voice Chat | ✅ Account-Free Rooms | ❌ None |
| 🧩 Scene Import / Export | ✅ JSON Config Sync | ❌ None |
| 🚫 Watermarks & Forced Ads | ❌ ZERO Watermarks / Ads | ⚠️ Forced Watermarks / Ads |
| 🔐 Account Required | ❌ No Mandatory Sign-in | ⚠️ Mandatory Account |

---

## 🗺️ Release Timeline & Roadmap

### 🗓️ Current Release Status
- **Android Version (Primary Focus)**: Actively developed and optimized first.
- **iOS Version (Phase 2)**: Planned following the official Android release and community funding/hardware setup (Mac & iPhone hardware).

### 🚀 Upcoming Roadmap Items
- ⚡ **Enhanced 4K Rendering Stability**: Optimized pipeline for long 4K broadcasts.
- 🎚️ **Professional Audio Mixer**: Multi-track gain sliders, noise gate controls, and compressor presets.
- 🎭 **Advanced VTuber Animations**: Smooth expression transitions and character motion blending.
- 🎨 **Custom Theme Engine**: Extended styling options for overlays and floating control bars.

*Check out the [Upcoming Features Guide](info/upcoming.md) for full details.*

---

## 🛠️ Quick Troubleshooting Guide

| Issue | Cause | Solution |
|---|---|---|
| 📷 **Black Camera Screen** | Permission or App Conflict | Grant Camera permissions; close background camera apps; toggle front/back camera in settings. |
| ⚠️ **Error Icon on Image/Video** | Missing or Moved File | Open **Scene Manager** → **Missing Assets** to relink the file to its new path. |
| 🔇 **Game Audio Not Streamed** | Game Security Restriction | Ensure "Mute Internal Audio" is OFF in Audio Settings. Use a headset on Android 10+. |
| 🔊 **Metallic Mic Audio or Echo** | Speaker Feed-through | **Always use headphones** while streaming with a microphone; enable Hardware Noise Suppression. |
| 📉 **Stream Lag or Frame Drops** | Bitrate or Hardware Overload | Lower bitrate to 3500 kbps, drop to 720p 30 FPS, or enable **Adaptive Bitrate (ABR)**. |

*For in-depth help, view the [Complete Troubleshooting Guide](info/troubleshooting.md) and [FAQ](info/FAQ.md).*

---

## 🤝 Monetization & Sponsorship Program

LiveLens is built on a **creator-first monetization model**. We believe creators should never be forced to display watermarks or pay recurring subscriptions for essential tools.

### 💖 How to Support Development
If you love LiveLens and want to keep it ad-free and free for everyone, consider supporting:
- 🌸 **GitHub Sponsors**: [github.com/sponsors/ByconStudio](https://github.com/sponsors/ByconStudio)
- 💳 **PayPal (International)**: [paypal.me/arpanstream](https://www.paypal.me/arpanstream)
- 📱 **UPI (India)**: Available directly inside **Global Settings** in the app.

### 🏢 Corporate & Brand Sponsorships
Brands and organizations can support LiveLens development while gaining high-visibility partner positioning:
- 🚀 **Splash Screen Branding**: Dedicated logo placement during startup.
- ⚙️ **Settings Screen Card**: Clickable promotional banner linking to official brand websites.
- 🤝 **Official Partner Title**: Co-branding and sponsor positioning opportunities.

*Learn more about brand benefits in [Sponsorship Benefits](info/sponsorship_benefits.md) and our [Monetization Philosophy](info/MONETIZATION.md).*

---

## 📚 Complete Documentation Directory

Explore the full documentation hosted directly in this repository:

### 🚀 Getting Started & Overview
- 📖 [What is LiveLens?](info/what_is_livelens.md) – App philosophy & core design
- 🎓 [Getting Started Guide](info/Getting-Started.md) – Step-by-step 5-minute setup
- 👨‍💻 [Developer & Studio Info](info/dev_info.md) – Story behind Bycon Studio
- ❓ [Frequently Asked Questions (FAQ)](info/FAQ.md) – Complete Q&A

### 📺 Platform Streaming Guides
- 🟣 [Twitch Setup Guide](info/stream/twitch.md)
- 🔴 [YouTube Live Setup Guide](info/stream/youtube.md)
- 🔵 [Facebook Live Setup Guide](info/stream/facebook.md)
- 🟢 [Kick Setup Guide](info/stream/kick.md)
- ⚙️ [General Stream Setup](info/home/stream_setup.md)

### ⚙️ Settings & Configuration
- 📹 [Video Settings](info/settings/video.md) | 📡 [Streaming Settings](info/settings/streaming.md) | 📹 [Recording Settings](info/settings/recording.md)
- 🎙️ [Audio Settings](info/settings/audio.md) | 📐 [Canvas & Resolution](info/settings/canvas.md) | 👾 [VTuber Settings](info/settings/vtuber.md)
- 💬 [Chat Settings](info/settings/chat.md) | 🎨 [Overlay Customization](info/settings/overlay.md) | 🎛️ [Floating Controls](info/settings/floating.md)
- 🔒 [Privacy Settings](info/settings/privacy.md) | 🛠️ [Advanced Settings](info/settings/advanced.md) | 🗣️ [Voice Chat Settings](info/settings/voice.md)

### ⚡ System & Hardware
- 📊 [Performance Tiers & Limits](info/performance_limits.md)
- 🛠️ [Troubleshooting Guide](info/troubleshooting.md)
- 💻 [CPU Compatibility Info](info/cpu_info.md)
- 💡 [Upcoming Features & Roadmap](info/upcoming.md)
- 🤝 [Support & Contribute](info/contribute.md)
- 💼 [Sponsorship Benefits](info/sponsorship_benefits.md)
- 📜 [Monetization Philosophy](info/MONETIZATION.md)

---

## 📱 System Requirements

### Minimum Requirements
- **Android OS**: Android 10 or higher (Required)
- **RAM**: 4GB RAM
- **Storage**: 100MB free space
- **Camera & Mic**: Standard phone camera & microphone

### Recommended Specifications
- **Android OS**: Android 12 or higher
- **RAM**: 8GB+ RAM
- **Processor**: Snapdragon 870 / Dimensity 8100 or higher
- **Storage**: 256GB+ for 4K local recording
- **Network**: 15+ Mbps upload speed for high-bitrate streaming

---

## 🐛 Bug Reports & Community Support

- 💬 **Discord Community**: [Join LiveLens Discord](https://discord.gg/kUqmbKhs6w)
- 💡 **Community Discussions**: [GitHub Discussions](https://github.com/ByconStudio/LiveLens/discussions)
- 🐛 **Issue Tracker**: [Report a Bug](https://github.com/ByconStudio/LiveLens/issues/new?template=bug_report.yml)
- 📧 **Support Email**: [support@livelens.live](mailto:support@livelens.live)

---

## 📜 License

```
All rights reserved © LiveLens / Bycon Studio

This project is proprietary software. 
Unauthorized copying, modification, or distribution is strictly prohibited.
For licensing inquiries, contact: support@livelens.live
```

---

<div align="center">

### Made with ❤️ for Content Creators Everywhere

**[🌐 Visit LiveLens Website](https://www.livelens.live/)** • **[💬 Join Discord](https://discord.gg/kUqmbKhs6w)** • **[💖 Sponsor Project](https://github.com/sponsors/ByconStudio)**

</div>
