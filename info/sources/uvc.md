# UVC Source (Capture Card)

## Overview

The **UVC (USB Video Class) Source** allows users to connect external USB devices like **HDMI Capture Cards**, USB Webcams, or DSLR cameras directly to their LiveLens scene. 

This is a powerful feature for mobile gamers who want to stream console games (Nintendo Switch, PlayStation, Xbox) or use professional camera hardware with their phone as the main streaming hub.

> **Note**: This feature is currently in **Beta**. Performance and compatibility depend on your Android device's USB OTG support and the capture card hardware.

---

## Adding a UVC Source

To add a capture card:

1. Connect your capture card to your phone using a USB-C cable or OTG adapter.
2. Tap the **+ (plus)** icon in LiveLens and select **UVC (Beta)**.
3. The USB device manager scans and lists connected capture cards.
4. Tap your device in the list and grant system USB permissions when prompted.

---

## Opening UVC Settings

To open the Capture Card Editor:

1. Select the **UVC Source** on the canvas.
2. Tap the **Settings** icon.

The Editor features a **Dynamic Aspect Ratio Preview** on the left and a scrollable **Controls Section** on the right, topped by an **Apply** button and **Close** button.

---

## Capture Card Editor Features

### 1. Devices & USB Diagnostics
- **Device Refresh**: Tap the **Refresh** icon to rescan for newly plugged USB video devices.
- **Hardware Info**: Displays device product name, **VID (Vendor ID)**, and **PID (Product ID)**.
- **Capabilities Badge**: Shows if the hardware supports *Video + Audio*, *Video Only*, or *Audio Only*.
- **Connection Status**:
  - 🔵 **Active / Streaming**: Currently active device.
  - 🟢 **Permission Granted • Tap to Connect**: Device authorized, ready to connect.
  - 🟠 **Permission Needed • Tap to Request**: Requires system USB permission prompt.

### 2. Resolution & Format Selection
- **Resolution Dropdown**: Choose from supported hardware resolutions (e.g., 1920x1080, 1280x720).
- **Format Indicators**: Displays the capture format and frame rate for each option (e.g., `MJPEG | 60 FPS` or `YUYV | 30 FPS`).
- **Device Default (Auto)**: Lets LiveLens automatically choose the optimal resolution and FPS for your device.

### 3. Transform & Visual Adjustments
- **Opacity Slider**: Smoothly adjust transparency from 0% to 100%.
- **Interactive Cropping**: Drag the blue edge handles on the live preview to crop out unwanted borders or black bars.
- **Reset Visuals**: Tap "Reset Visuals" to quickly restore scale (1.0x), crop margins (0), and opacity (100%).

### 4. Chroma Key (Green Screen Removal)
LiveLens includes a full-featured real-time Chroma Key engine for UVC sources:
- **Enable Chroma Key**: Toggle green screen removal on or off.
- **Eyedropper Color Picker**: Tap the **Eyedropper** icon, then tap anywhere directly on the live preview frame to pick your key color precisely using pixel-level sampling.
- **Similarity Slider**: Adjust color matching tolerance from 1% to 100%.
- **Smoothness Slider**: Blend edges smoothly with background elements from 1% to 100%.

### 5. Audio Configuration (UAC Audio)
- **Hear It (Local Monitoring)**: Toggle this on to monitor USB Audio (UAC) locally through your phone's speakers or headphones.
- **Direct Mixer (48kHz)**: Toggle this on to route high-quality 48kHz capture card audio directly into your stream or local recording.

---

## Canvas Controls

The UVC Source supports standard interactive canvas controls:
- **Move & Resize**: Drag and pinch to position and scale on screen.
- **Rotate**: Use the rotation handle (bottom-right) with degree indicator.
- **Reset Rotation**: Tap the top-right handle to return to 0°.
- **Double Tap**: Instantly fit the capture feed to cover the entire canvas.

---

## UVC Source Settings Summary

| Setting | Description |
|---|---|
| Device Manager | Rescan and select USB devices (with VID/PID & capability badges) |
| Resolution & Format | Choose capture resolution, FPS, and format type (MJPEG/YUYV) |
| Opacity & Crop | Frame the video feed and set transparency |
| Reset Visuals | Restore default scale, cropping, and opacity |
| Chroma Key | Remove green screen backgrounds with interactive eyedropper color picker |
| Similarity & Smoothness | Fine-tune chroma key edge blending |
| Hear It | Monitor USB capture audio locally through headphones/speakers |
| Direct Mixer (48kHz) | Feed capture card audio directly to stream/recording |

---

## Related Documentation

- [Sources](./README.md)
- [Audio Settings](../audio/README.md)
- [Troubleshooting UVC](../troubleshooting/uvc-beta.md)
