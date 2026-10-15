# Screen Capture Source

## Overview

The **Screen Capture Source** allows users to stream or record their entire mobile screen. This is the primary source for mobile gaming and app demonstrations.

It leverages the Android **MediaProjection API** to capture everything displayed on the device in real-time.

---

## Adding Screen Capture

To start capturing your screen:

1. Tap the **+ (plus)** icon in LiveLens and select **Screen Capture**.
2. A system prompt will appear asking for permission to record or cast your screen.
3. Tap **Start now** to grant permission.
4. The screen feed will be added to your current scene.

> **Privacy Note**: While Screen Capture is active, everything on your screen—including notifications, messages, and passwords—will be visible to your stream or recording. It is recommended to enable **Do Not Disturb** mode on your device.

---

## Source Characteristics & Limits

Unlike other sources in LiveLens, the Screen Capture source has specific restrictions to ensure stability and performance:

- **No Settings Panel**: There is no dedicated settings popup for this source.
- **No Rotation**: The screen source cannot be rotated on the canvas. It always stays aligned with the device's physical orientation.
- **No Cropping**: The entire screen is always captured; manual cropping is not available for this source type.

---

## Canvas Controls

Despite the lack of a settings panel, you can still manage how the screen capture appears in your layout using standard canvas gestures:

- **Move**: Drag the screen capture to position it anywhere on the canvas.
- **Resize**: Pinch to scale the screen capture up or down.
- **Double Tap (Fill)**: Double-tap the source to quickly make it cover the entire canvas. Double-tap again to return to its previous size.
- **Z-Order**: Use the up/down arrows to move the screen capture above or below other overlays (like cameras or alerts).
- **Lock/Unlock**: Use the lock icon to prevent accidental moving or resizing once you've positioned it.

---

## Orientation & Resizing

LiveLens automatically detects when you rotate your device or when an app changes the screen resolution. The capture feed will dynamically resize to match your device's current display output.

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Privacy Policy](../privacy/README.md)
