# Chat Box Source

## Overview

The Chat Box Source allows you to display a real-time, high-performance native chat overlay in your LiveLens scene. 

Unlike traditional web-based overlays, LiveLens uses a **Native Rendering Engine** (OpenGL + Android Canvas) to ensure smooth animations, low memory usage, and perfect legibility even during high-intensity streaming.

---

## Opening Chat Box Settings

To configure your Chat Box:

1. Add a **Chat Box Source** to the scene.
2. Select the Chat Box on the canvas.
3. Tap the **Settings** icon.

The Chat Box Settings popup opens, featuring a **Live Simulation Preview** on the left and a list of **Available Presets** on the right.

---

## Settings Interface

The Settings Interface is split into two main sections: **Live Preview** (left) and **Control Panel** (right).

### 📺 Live Simulation Preview
The left side shows a live preview of the selected preset. 
- **Dummy Messages**: The preview automatically generates simulated messages from YouTube and Twitch to show you exactly how the chat will look and animate.
- **Real-time Feedback**: As you select different presets or change visibility settings, the preview updates instantly.

### ⚙️ Control Panel
The right side contains the settings for behavior, dimensions, and appearance:

**1. Dimensions & Resolution**
- **Width & Height**: Set custom pixel dimensions for the Chat Box canvas (default: 600x600).
- **Reset Size**: Tap the refresh icon next to the input fields to instantly reset dimensions back to 600x600.

**2. Timer Settings (Auto-Hide)**
- **AUTO-HIDE CHAT**: Toggle this to automatically hide messages after they have been visible for a certain duration. This is useful for keeping the stream clean when there is no active chat.
- **HIDE DELAY**: When Auto-Hide is enabled, use the slider to set the delay from **3 to 60 seconds**.

**3. Available Presets**
LiveLens includes all **24 professional presets** found in your library, categorized by their visual style. Selecting a preset dynamically moves it to the top of the grid for quick identification:

#### 🌟 Glow & Cyber Styles
- **Cyber Glow**: High-contrast green glow with a tech-inspired border.
- **Lava Glow**: Deep red and orange tones with intense glow effects.
- **Magma Neon**: Intense volcanic orange glow with a sharp border.
- **Toxic Neon**: Radioactive green glow with rounded bubble containers.
- **Electric Neon**: High-voltage blue glow for a high-energy look.
- **Ultraviolet**: Deep magenta/purple glow with large rounded bubbles.
- **Neon Drift**: Vibrant cyan aesthetics for fast-paced action.
- **Neon Pulse**: Intense magenta pulse with rounded bubble containers.
- **Vaporwave**: Retro-futuristic purple and teal aesthetics.
- **Ethereal White**: Pure white glow for a clean, heavenly appearance.

#### 🫧 Modern & Glass Styles
- **Modern Bubble**: Clean, semi-transparent bubbles with high corner radius.
- **Glass Morphism**: Trendy frosted-glass effect with subtle borders.
- **Rose Pop**: Soft pink aesthetics with elegant rounded containers.
- **Arctic Frost**: Cool blue tones with a crisp, frost-like glow.
- **Aurora Stream**: Shifting northern-light aesthetics with glass backgrounds.
- **Studio Glass Gold**: Professional studio-quality glass with gold accents.

#### ⚔️ Gaming & Esports
- **Esports Lime**: Sharp angles and bright lime accents for competitive play.
- **Shadow Pro**: Stealthy dark design with a focused name highlight.
- **Midnight Stealth**: Ultra-dark, low-distraction design for long streams.
- **Solaris Gold**: Premium gold accents for high-end production value.

#### 🕹️ Specialized & Retro
- **Retro Pixel**: 16-bit vibe using a custom pixel font and sharp borders.
- **Destroy Mode**: Aggressive red aesthetic with a custom "Destroy" font.
- **Horror Night**: Spooky red-on-black aesthetic with a custom horror font.
- **Classic**: The reliable, high-legibility standard chat style.

Tap a preset to see it in the preview, and tap **Apply** at the top-right corner to use it in your scene.

---

## Important Notice: Chat Visibility

If your Chat Box is not showing any messages, please note the following requirements:

- **Supported Platforms**: Currently, LiveLens only supports native chat integration for **YouTube** and **Twitch**.
- **Login Required**: You must be logged into your YouTube or Twitch account within the app and start the stream directly through the app's native streaming feature for the chat to be captured.
- **Custom RTMP Restriction**: If you are using a **Custom RTMP** server to stream, the Chat Box will **not** display any messages as the app cannot fetch the chat data from external RTMP servers.

---

## Technical Features

### Platform Integration
The Chat Box automatically aggregates messages from all connected platforms (YouTube, Twitch, etc.). Each message includes:
- **Platform Icon**: A small icon (e.g., YouTube logo) next to the sender's name.
- **Author Name**: Stylized according to the selected template.
- **Message Content**: Supports multi-line wrapping and emojis.

### Performance & Animation
- **Native GPU Rendering**: Chat messages are rendered using OpenGL textures, ensuring zero lag on the main UI thread.
- **Smooth Animations**: Supports entry animations like "Slide-Left" or "Fade-In" based on the template design.
- **Directional Flow**: Templates can be configured to flow from **Bottom-to-Top** (standard) or **Top-to-Bottom**.

---

## Canvas Controls

The Chat Box Source supports all standard LiveLens canvas interactions:
- **Move**: Drag to place the chat anywhere on your screen.
- **Resize**: Pinch to scale the entire chat box.
- **Rotate**: Use the rotation handle to tilt the chat box.
- **Reset Rotation**: Tap the reset handle at the top-right corner to return to 0 degrees.
- **Double Tap**: Quickly fit the chat box to the canvas.
- **Locking**: Use the lock icon to prevent accidental movement once positioned.

---

## Related Documentation

- [Sources](./README.md)
- [Chat Settings](../settings/chat.md)
- [Scenes](../scenes/README.md)
