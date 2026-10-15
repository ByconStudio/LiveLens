# Performance Tiers & Source Limits

## Overview

LiveLens is designed to run on a wide range of Android devices, from entry-level phones to high-end flagships. To ensure a smooth streaming experience, the app automatically categorizes your device into a **Performance Tier** based on its processor (SoC).

Each tier comes with recommended limits for sources and resolution/FPS.

---

## Understanding Device Tiers

LiveLens detects your phone's CPU and assigns it to one of the following tiers:

| Tier | Typical Limits (Text / Image / Web / Video / Sound) |
|---|---|
| **Entry** | 3 / 2 / 1 / 0 / 1 |
| **Low-Mid** | 4 / 2 / 1 / 0 / 1 |
| **Mid** | 5 / 3 / 2 / 1 / 1 |
| **Upper-Mid** | 6 / 4 / 2 / 1 / 1 |
| **Flagship** | 8 / 5 / 3 / 2 / 2 |
| **Ultra Flagship** | 10 / 6 / 4 / 3 / 2 |

---

## 🚫 Fixed Source Limits

Some sources have **fixed limits** due to extreme resource requirements or technical constraints. These **cannot** be increased, even in Advanced Settings:

- **VTuber Source**: Limit is fixed at **1**. Live2D rendering is highly CPU/GPU intensive, and the engine is optimized for a single high-quality avatar.
- **UVC (Capture Card)**: Limit is fixed at **1**. Most Android devices support only one active high-bandwidth USB video class device at a time.
- **Screen Capture**: Limit is fixed at **1** (System restriction).
- **Camera**: Limit is fixed at **1** active camera feed on most device tiers.

---

## How to Increase Limits (Boost Mode)

For other sources (Text, Image, Web, GIF, Video), you can manually override the recommended limits.

### 1. Custom Source Limits
1. Go to **Global Settings** → **Advanced**.
2. Toggle **Custom Source Limits** to ON.
3. Use the sliders to boost the maximum allowed count.

**Maximum "Boost" Limits:**
- **Text**: Up to 20
- **Image**: Up to 15
- **Web**: Up to 10
- **GIF**: Up to 10
- **Video**: Up to 5 (Only on devices that support video sources)
- **Sound**: Up to 5

> **Warning**: Increasing these limits beyond recommendations will use significantly more CPU and RAM. This may cause stream lag, device overheating, or app crashes.

### 2. Unlock All Settings (Pro Mode)
1. In **Global Settings** → **Advanced**, toggle **Unlock All Settings**.
2. This allows you to force-enable resolutions (like 4K) or FPS (60fps) that are normally hidden for your device tier.

---

## Important Safety Checks

- **Cannot Disable Limits**: If you have already added more sources than your device's default tier supports, you cannot turn off "Custom Source Limits" until you remove the extra items from your scene.
- **Scene Optimizer**: When importing a scene from a more powerful device, LiveLens will alert you if the source count exceeds your hardware's capabilities and help you optimize it.

---

## Related Documentation

- [Sources](./sources.md)
- [Scene Management](./scene/scene.md)
- [Troubleshooting Lag](../troubleshooting/performance.md)
