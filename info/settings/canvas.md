# Canvas Setup & Tools

## Overview

The **Canvas Settings** allow you to define the foundation of your stream or recording. Here, you can choose your layout's orientation, customize the editor's look, and enable precision tools for scene building.

---

## 📐 Aspect Ratio & Orientation

LiveLens supports two primary orientations:

- **16:9 Landscape (1920x1080)**: Ideal for traditional gaming, YouTube streaming, and horizontal content.
- **9:16 Portrait (1080x1920)**: Best for mobile-first platforms like TikTok, YouTube Shorts, or Instagram Live.

### Auto-Rotate to Portrait
When the **9:16 Portrait** ratio is selected, you can enable **Auto-Rotate**. This feature automatically switches your phone's UI to portrait mode whenever the bottom settings panels are hidden, giving you a full-screen vertical editing experience.

---

## 🎨 Canvas Appearance

Customize the workspace to suit your needs. These settings affect the **Editor only** and do not change your final stream output.

### Background Color (Hex)
- Change the color of the empty canvas in the editor.
- **Important**: This is for preview purposes only. The background of your actual stream or recording remains **transparent**, allowing your gameplay or camera to be the base layer.

### Border Color (Hex)
- Customize the color of:
    - Source selection outlines.
    - Canvas boundaries.
    - Alignment and snapping guides.
- High-contrast colors (like Cyan or Neon Green) are recommended for precise alignment.

---

## 🧲 Editor Tools (Magnet Snapping)

Build your scenes with pixel-perfect precision using **Magnet Snapping**.

- **Toggle Snapping**: When enabled, sources will "snap" or stick to invisible grid lines and canvas edges as you drag them.
- **Snap Sensitivity**: Adjust how strongly objects stick to the grid:
    - **Weak**: For minor guidance.
    - **Medium**: Balanced snapping.
    - **Strong**: Objects aggressively jump to the nearest grid line.

---

## 🔒 Settings Lock

For stability, **Canvas Settings are locked** while you are actively **Streaming** or **Recording**. You must stop the encoder before changing the aspect ratio or orientation to prevent crashes.

---

## Canvas Settings Summary

| Setting | Description |
|---|---|
| Aspect Ratio | Choose between Landscape (16:9) or Portrait (9:16) |
| Auto-Rotate | Automatically flips the phone UI for vertical layouts |
| Background Color | Sets the editor's preview canvas color (Output is transparent) |
| Border Color | Changes the color of outlines and guides |
| Magnet Snapping | Helps align sources to a grid automatically |
| Snap Sensitivity | Controls the "stickiness" of the snapping tool |

---

## Related Documentation

- [Sources](../sources/sources.md)
- [Performance Tiers](../performance_limits.md)
- [Video & Stream Settings](./video.md)
