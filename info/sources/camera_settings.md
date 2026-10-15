# Camera Source

## Overview

The Camera Source allows users to add a device camera to a LiveLens scene.

After adding a Camera Source, users can configure the camera through its dedicated settings panel.

---

## Opening Camera Settings

To open the Camera Source settings:

1. Add a Camera Source to the scene.
2. Select the Camera Source.
3. Tap the **Settings** icon.

The Camera Settings popup opens.

The settings interface contains a camera preview on the left side and camera controls on the right side.

---

## Camera Preview

The left side of the Camera Settings popup displays a preview of the selected camera.

The preview allows users to see the camera feed while configuring the camera.

When selecting a chroma-key color, the preview is also used to choose the color that should be removed.

> The chroma-key background is not removed from this settings preview. The chroma-key effect is applied to the Camera Source displayed on the main canvas.

---

## Front and Back Camera

The Camera Source provides controls for switching between the device's available front and back cameras.

Users can tap the **Front/Back** camera option to switch between:

- Front camera
- Back camera

The selected camera is then used by the Camera Source.

---

# Chroma Key

The Camera Source includes a **Chroma Key** option for removing a selected background color from the camera feed.

This can be useful when the subject is recorded in front of a consistent-color background, such as a green screen.

### Enabling Chroma Key

To enable Chroma Key:

1. Open Camera Source Settings.
2. Enable the **Chroma Key** switch.
3. Additional chroma-key controls become available.

These controls include:

- Color picker
- Similarity
- Smoothness

---

## Chroma Key Color

When Chroma Key is enabled, a color picker control appears.

The selected color is displayed next to the color picker, allowing users to see which color is currently configured for removal.

### Selecting a Different Color

To select a different background color:

1. Tap the color-picker/dropper icon.
2. The camera preview becomes the color-selection area.
3. Tap the color in the preview that should be removed.
4. The selected color becomes the new chroma-key color.

The selected color is reflected in the color indicator next to the picker.

> The camera preview inside the settings popup does not display the background-removal effect. The chroma-key effect is visible on the Camera Source placed on the main canvas.

---

## Similarity

The **Similarity** slider controls how closely a color must match the selected chroma-key color before it is considered part of the background to remove.

A lower similarity value generally makes the color selection more restrictive, removing colors that are very close to the selected color.

A higher similarity value expands the range of colors considered similar to the selected color, allowing more variations of the background color to be removed.

This can be useful when the background contains slight color variations caused by lighting, shadows, or camera conditions.

---

## Smoothness

The **Smoothness** slider controls how gradually the edges of the chroma-keyed area transition between the visible subject and the removed background.

Lower smoothness generally produces a harder edge.

Higher smoothness creates a softer transition around the detected background boundary, which can help reduce harsh or jagged edges around the subject.

Similarity and Smoothness can be adjusted together to achieve a cleaner chroma-key result depending on the background and lighting conditions.

---

## Camera Transformations

The Camera Source can be positioned and resized on the canvas using the common source controls.

However, the Camera Source **cannot be rotated on the canvas**.

Other common source controls, such as moving, resizing, hiding, locking, and source ordering, are documented in the [Sources](./README.md) documentation.

---

## Android 14+ System Limitations

Starting with **Android 14 (API 34)**, the Android system imposes stricter privacy and resource restrictions on camera usage.

### ⚠ Camera Limitation Warning
When you use the Camera Source on a device running Android 14 or above, LiveLens may display a warning dialog with the following information:

- **Minimized App Restriction**: The system restricts camera access when the app is minimized or sent to the background.
- **Freeze/Stop Behavior**: If you leave the LiveLens app (e.g., to check another app) while streaming or recording, the camera feed may **stop or freeze**.
- **Unaffected Sources**: Other sources such as **Screen Capture, Images, Text, and Overlays** will continue to function normally even when the app is in the background.

**Pro-Tip**: For the most stable streaming experience with a camera, it is highly recommended to keep the LiveLens app open and in the foreground.

---

## Camera Source Settings Summary

| Setting | Description |
|---|---|
| Camera | Switch between front and back camera |
| Chroma Key | Remove a selected background color |
| Color Picker | Select the color to remove |
| Similarity | Controls the range of colors considered similar to the selected key color |
| Smoothness | Controls the softness of the transition around the keyed area |

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Chroma Key](../settings/chroma-key.md)