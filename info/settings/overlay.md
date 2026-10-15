# Stream Overlays & Assets

## Overview

The **Overlay Settings** allow you to add professional visual touch-points to your stream, such as intro screens, "Be Right Back" (BRB) scenes, and a highly customizable cooldown timer. These elements help maintain audience engagement during breaks or before your stream officially starts.

---

## 🎭 Stream Assets (BRB & Starting Soon)

While you can switch scenes at any time, LiveLens also provides dedicated **Asset Overlays** (like BRB and Starting Soon) for quick visual changes without switching your entire scene layout. These are accessible via the **Settings → Overlay Settings** or directly from the Floating Control panel.

### 1. BRB (Be Right Back)
Show a custom image or GIF when you need to take a quick break.
- **Mixer Toggles**:
    - **Mute Mic**: Automatically mutes your microphone when the BRB screen is active.
    - **Mute Internal**: Automatically mutes game/app audio when the BRB screen is active.
- **Visuals**: Supports static images and animated GIFs.

### 2. Starting Soon
A professional intro screen to warm up your audience.
- **Auto-Activate on Start**: If enabled, this screen automatically appears as soon as you press "Go Live," giving you a few moments to prepare.
    - *Note: This option is only available if the "Soon" button is enabled in Floating Control settings.*
- **Mixer Toggles**: Independent "Mute Mic" and "Mute Internal" options, similar to the BRB asset.

### 🛠️ Managing Assets
You can easily add, change, or remove your stream assets directly within the settings cards:

- **Add/Change Asset**: Tap on the **Preview Box** (showing an "Add" icon or the current image/GIF) to open your device's gallery. Selecting a new file will automatically replace the existing one.
- **Delete Asset**: Once an image or GIF is loaded, a **Red Trash Icon** will appear at the top-right corner of the asset card. Tapping this will instantly remove the asset and restore the default state.

### 📐 Asset Requirements & Validation
To ensure stream stability and performance, LiveLens enforces the following limits for GIFs:
- **Max Size**: 10 MB.
- **Max Resolution**: 1080p (maximum dimension of 1920px).
- **Format**: `.gif` and common image formats (PNG, JPG).

---

## ⏳ Cooldown Timer Overlay
The **Cooldown Timer** is a professional widget that can be layered over your BRB or Starting Soon screens. It is perfect for "Stream Starting in X minutes" or "Break ending in X:XX" scenarios.

### 1. Basic Configuration
- **Enable Timer**: Toggle the timer on or off.
- **Duration**: Set the countdown duration in **minutes**.
- **Visibility**: 
    - **Show in BRB**: Render the timer specifically over your BRB asset.
    - **Show in Starting Soon**: Render the timer specifically over your Starting Soon asset.

### 2. Interactive Positioning & Scale
LiveLens features a dedicated **Positioning Popup** that allows you to:
- **Visual Drag & Drop**: Interact with a simulated canvas to drag the timer to your desired position.
- **Interactive Scaling**: Use a slider to adjust the timer size from **0.5x to 4.0x**.
- **Preview Toggling**: Switch between BRB and Starting Soon previews to set independent positions for each screen.

### 3. Style & Customization
- **Custom Fonts**: Use `.ttf` or `.otf` files from your device to match your stream's branding.
- **Color Selection**: Input precise **Hex codes** (e.g., #00E5FF) with a real-time color preview circle.
- **Animation Effects**: Choose from professional transitions including:
    - **FADE, POP, SLIDE_UP, GLITCH, FLIP, and ROTATE**.
- **Animation Speed**: Customize the effect duration in milliseconds.

### 4. Smart Automation
- **Auto-Off Assets**: When enabled, LiveLens will **automatically hide** the active BRB or Starting Soon screen once the timer reaches zero. This allows for a seamless transition directly into your live gameplay or content.

---

## Overlay Settings Summary

| Feature | Description |
|---|---|
| BRB Asset | Image/GIF overlay with independent audio mixer toggles |
| Starting Soon | Intro screen with "Auto-activate on Start" capability |
| Cooldown Timer | Countdown widget with custom fonts, colors, and animations |
| Interactive Positioning | Drag-and-drop timer placement on a simulated canvas |
| Asset Validation | Enforces 10MB and 1080p limits for performance stability |
| Auto-Off Behavior | Automatically closes assets when the timer hits 0:00 |

---

## Related Documentation

- [Canvas Settings](./canvas.md)
- [Floating Control](./floating.md)
- [Video Settings](./video.md)
