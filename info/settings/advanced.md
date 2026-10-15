# Advanced Settings & Resource Limits

## Overview

**Advanced Settings** are the most critical control point for LiveLens power users. These settings allow you to bypass the app's built-in safety mechanisms and manually control how the app utilizes your device's CPU, GPU, and RAM.

> [!DANGER]
> These settings are designed for experimental use. Bypassing hardware capability checks or forcing high resource limits on mid-range or entry-level devices can lead to system instability, overheating, and app crashes.

---

## 🔓 Unlock All Settings (Override Mode)

By default, LiveLens performs a real-time hardware audit to determine the safest **Resolution** and **FPS** for your specific device.

### What it Does
Enabling **Unlock All Settings** triggers a dangerous "Override Mode":
- **Ignore Capability Checks**: All hardware-based restrictions for Resolution (up to 4K) and Frame Rate (up to 60 FPS) are removed.
- **Encoder Bypass**: Allows forced selection of advanced codecs like **H.265 (HEVC)** even if the hardware reports partial or no support.
- **Badge Indicator**: Once enabled, a **"Force Unlocked Mode"** warning badge will appear at the top of your Video and Advanced settings to remind you that safety checks are off.

### ⚠️ Risks
- **Encoder Overload**: If your processor cannot encode 4K/60fps in real-time, your stream will suffer from extreme lag and frame drops.
- **Device Thermal Throttling**: Intensive encoding generates significant heat. The Android system may throttle your CPU speed to cool down, causing the app to slow down further.

---

## 📊 Custom Source Limits (Manual Resource Allocation)

LiveLens categorizes devices into **Performance Tiers** (Entry, Mid, High, Flagship) and assigns source limits accordingly. **Advanced Settings** allow you to override these tiers.

### 1. Master Toggle: Custom Source Limits
Enable this to take full manual control of your scene's complexity. 
- **Warning**: Enabling this will display a performance warning, as increasing limits beyond recommended values uses significantly more RAM and CPU.

### 2. Manual Limit Sliders
You can manually adjust the maximum number of active sources. The maximum "Advanced" limits allowed are:
- **Max Text Sources**: Up to **20** elements.
- **Max Image Sources**: Up to **15** elements.
- **Max Web Sources**: Up to **10** widgets (Extremely RAM intensive).
- **Max GIF Sources**: Up to **10** animated stickers.
- **Max Video Sources**: Up to **5** concurrent video loops.
- **Max Sound Sources**: Up to **5** independent audio mixer tracks.
- **Max VTuber Sources**: Restricted to **1** (GPU intensive).

### 🛡️ The "Over-Limit" Lock
LiveLens enforces a strict safety check when trying to disable Custom Limits:
- If your current scene contains **more sources** than your device's default tier allows, you **cannot** turn off Custom Limits.
- A **Warning Dialog** will appear listing exactly which source types are exceeding the limit (e.g., *"Text (2 extra)"*). You must delete these extra sources before the app will allow you to return to standard tier-based limits.

---

## 🛠️ Performance Optimization Indicators

### 📱 Tier-Based Display
When Custom Limits are **OFF**, the app displays a summary of your current **Tier-Based Limits** at the bottom of the screen. This allows you to see the exact values for Text, Image, Web, GIF, Video, VTuber, and Sound sources that LiveLens has optimized for your device.

### 📊 Source Counter
In the manual sliders, you can see a **"Used: X"** counter for each source type. If your current usage exceeds your set limit, the counter will turn **RED** as a warning.

---

## Advanced Settings Summary

| Setting | Effect | Risk Level |
|---|---|---|
| Unlock All Settings | Bypasses Resolution/FPS hardware checks | **CRITICAL** |
| Custom Source Limits | Overrides Tier-based RAM/CPU allocations | **HIGH** |
| Manual Sliders | Fine-tune maximum counts for each source type | **MEDIUM** |
| Secure Exit | Prevents returning to defaults if over-capacity | **SAFETY** |

---

## Related Documentation

- [Video Settings](./video.md)
- [Performance Tiers](../performance_limits.md)
- [Canvas Settings](./canvas.md)
