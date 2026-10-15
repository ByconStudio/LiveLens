# Video Source

## Overview

The Video Source allows users to play video files as part of their LiveLens scene. 

It includes advanced features like **Chroma Key** for background removal, precise **Cropping**, and playback controls, making it ideal for streamers who want to use animated overlays, green-screen effects, or pre-recorded content.

---

## Opening Video Settings

To open the Video Editor:

1. Add a **Video Source** to the scene.
2. Select the Video Source on the canvas.
3. Tap the **Settings** icon.

The Video Editor popup opens with a preview player on the left and a detailed control panel on the right.

---

## Video Playback & Appearance

### Controls
- **Change Video**: Select a different video file from your device.
- **Loop Video**: When enabled, the video will restart automatically after finishing.
- **Mute Video**: Toggle audio playback for the video source.
- **Opacity**: Adjust the transparency of the video (0-100%).

### Performance Note
High-resolution videos (like 4K) significantly increase CPU and GPU usage. For the best streaming stability, **1080p or lower** is recommended.

---

## Visual Cropping

The Video Source features an interactive cropper in the preview area:
- **Blue Frame**: Drag the handles at the **Top-Left** and **Bottom-Right** to hide parts of the video frame.
- **Visual Feedback**: Areas outside the crop frame are dimmed to show exactly what will be removed on the canvas.

---

## Chroma Key (Background Removal)

The Video Source includes a powerful Chroma Key engine to remove specific colors (like a green screen).

### Enabling Chroma Key
Toggle the **Chroma Key** switch to reveal advanced controls.

### Selecting a Key Color
- **Color Presets**: Quickly toggle between common colors like Green and Blue.
- **Color Picker (Dropper)**: Tap the **dropper icon**, then tap anywhere on the video preview to pick a specific color for removal.

### Adjusting the Effect
- **Similarity**: Controls how close a color must be to the Key Color to be removed.
- **Smoothness**: Controls the softness of the edges around the subject after the background is removed.

---

## Canvas Controls

The Video Source supports standard LiveLens interactions:
- **Move**: Drag to reposition.
- **Resize**: Pinch to scale.
- **Rotate**: Use the rotation handle (bottom-right).
- **Rotation Degree**: A degree indicator appears at the **top-center** during rotation.
- **Reset Rotation**: Tap the reset handle at the **top-right** corner of the crop frame to return to 0°.
- **Double Tap**: Quickly scale the video to fill the canvas. Double-tap again to return to its previous size.

---

## Video Source Settings Summary

| Setting | Description |
|---|---|
| Change Video | Pick a new video file |
| Loop | Toggle infinite playback |
| Mute | Toggle audio |
| Opacity | Set transparency level |
| Chroma Key | Remove background color |
| Cropping | Frame specific parts of the video |

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Chroma Key Tips](../settings/chroma-key.md)
