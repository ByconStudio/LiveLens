# Post Processing Effects & GPU Performance

## Overview

The **Post Processing** menu allows you to apply real-time OpenGL-based visual filters, color enhancements, and cinematic effects to your live canvas preview and broadcast output. 

You can access the Post Processing panel by tapping the **Tune (Slider) icon** in the header of the **Sources Panel** on the Home Screen.

---

## ⚡ Quick GPU Performance Summary

Post-processing effects are rendered in real-time on the device's GPU shaders. Depending on your System-on-Chip (SoC) tier, enabling multiple complex effects simultaneously may affect your stream's frame rate (FPS) or increase device battery consumption.

| Effect | GPU Impact Level | Recommended Device Tier |
| :--- | :---: | :--- |
| **✨ Sharpness** | 🟢 Low | All Tiers (Entry, Low-Mid, High) |
| **🎨 Color Grading** | 🟢 Low | All Tiers (Entry, Low-Mid, High) |
| **🎬 Vignette** | 🟢 Low | All Tiers (Entry, Low-Mid, High) |
| **🎞️ LUT Presets** | 🟡 Low - Moderate | Low-Mid & High-End Tiers |
| **🧹 Denoise** | 🟡 Moderate | Low-Mid & High-End Tiers |
| **💡 Bloom (Glow)** | 🔴 High | High-End Tiers Only |

---

## 🎛️ Post Processing Effects Breakdown

### 1. ✨ Sharpness
- **Toggle Switch**: Enable or disable edge sharpening.
- **Intensity Slider**: Range `0.00` to `1.00` (Default: `0.30`).
- **Description**: Enhances edge definition and fine details across your visual sources, making camera feeds and text look crisper.
- **Usage Tip**: Avoid setting intensity too high (`> 0.70`), as it can introduce visual noise or harsh edges.
- **GPU Load**: 🟢 **Low Impact** (Single-pass kernel calculation; safe for all devices).

---

### 2. 🎨 Color Grading
- **Toggle Switch**: Enable or disable global color adjustments.
- **Controls**:
  - **Brightness**: Range `-0.50` to `+0.50` (Default: `0.00`). Adjusts overall light exposure.
  - **Contrast**: Range `0.50` to `2.00` (Default: `1.00`). Controls the difference between light and dark regions.
  - **Saturation**: Range `0.00` to `2.00` (Default: `1.00`). Adjusts color intensity (set to `0.00` for monochrome).
  - **Temperature**: Range `-0.50` to `+0.50` (Default: `0.00`). Shifts color tone between cool (blue) and warm (orange).
- **GPU Load**: 🟢 **Low Impact** (Simple pixel arithmetic in fragment shader; highly optimized).

---

### 3. 🎬 Vignette
- **Toggle Switch**: Enable or disable edge darkening.
- **Intensity Slider**: Range `0.00` to `1.00` (Default: `0.30`).
- **Description**: Smoothly darkens the outer borders of the frame to draw viewer attention toward the center of your canvas.
- **GPU Load**: 🟢 **Low Impact** (Distance-based color attenuation; minimal GPU overhead).

---

### 4. 🧹 Denoise (Noise Reduction)
- **Toggle Switch**: Enable or disable noise reduction.
- **Strength Slider**: Range `0.00` to `1.00` (Default: `0.30`).
- **Description**: Smooths out grain and sensor noise, especially useful for webcams operating in low-light environments.
- **Usage Tip**: Setting strength too high may soften fine details or create a slight "smoothing" effect.
- **GPU Load**: 🟡 **Moderate Impact** (Requires multi-sample neighbor pixel sampling; best used on Low-Mid or High-End SoCs).

---

### 5. 🎞️ LUT Presets (Color Filter Styles)
- **Toggle Switch**: Enable or disable color filter presets.
- **Preset Styles**:
  - **Default / Cinematic**: Balanced movie-style color grading.
  - **Cyberpunk**: Vibrant neon blue and magenta color scheme.
  - **Vintage**: Warm retro look with desaturated shadows.
  - **Black & White**: Classic high-contrast monochrome filter.
- **Intensity Slider**: Range `0.00` to `1.00` (Default: `1.00`). Controls preset blend strength.
- **GPU Load**: 🟡 **Low to Moderate Impact** (Uses texture LUT lookup; fast and efficient on modern GPUs).

---

### 6. 💡 Bloom (Glow Effect)
- **Toggle Switch**: Enable or disable highlight glowing.
- **Controls**:
  - **Intensity**: Range `0.00` to `1.00` (Default: `0.50`). Controls glow brightness and spread.
  - **Threshold**: Range `0.00` to `1.00` (Default: `0.70`). Sets the minimum brightness required to create a glow.
- **Description**: Adds a soft, atmospheric glow around bright lights, game highlights, and neon elements.
- **GPU Load**: 🔴 **High Impact** (Requires multi-pass brightness extraction and blur operations; may cause frame drops on Entry-Level hardware or while streaming demanding games).

---

## 🛠️ SoC Tier Recommendations

- **Entry Tier Devices**:
  - Keep **Bloom** and **Denoise** turned **OFF**.
  - Use **Sharpness**, **Color Grading**, or **Vignette** for lightweight enhancements.
- **Low-Mid Tier Devices**:
  - **Color Grading**, **LUTs**, **Sharpness**, and **Vignette** run smoothly.
  - Use **Denoise** when camera noise is present.
  - Use **Bloom** sparingly.
- **High-End Tier Devices**:
  - All post-processing effects can be enabled simultaneously without performance issues.

---

## Related Documentation

- [Home Screen Overview](./home.md)
- [Controls Deep Dive](./controls.md)
- [Performance & CPU Limits](../performance_limits.md)
- [Video Settings](../settings/video.md)
