# Image Source

## Overview

The Image Source allows users to add static images (like logos, overlays, or backgrounds) to a LiveLens scene. 

It features an interactive **Image Editor** with precise cropping tools and opacity controls to help you fit the image perfectly into your layout.

---

## Opening Image Settings

To open the Image Editor:

1. Add an **Image Source** to the scene.
2. Select the Image Source on the canvas.
3. Tap the **Settings** icon.

The Image Editor popup opens, featuring a large preview area for cropping and setting adjustments.

---

## Image Editor Features

### Dynamic Preview & Cropper
The left side displays your image with a blue frame representing the current crop area.
- **Visual Cropping**: Drag the blue handles at the **Top-Left** and **Bottom-Right** corners of the frame to crop out unwanted parts of the image.
- **Aspect Ratio Awareness**: The preview area automatically adjusts to match the aspect ratio of the loaded image.
- **Dark Overlay**: Areas outside the blue crop frame are dimmed in the preview to show exactly what will be hidden on the canvas.

### Image Settings Controls
- **Change Image**: Tap the **Change Image** button to select a new file from your device.
- **Opacity**: Adjust the **Opacity slider** (0% to 100%) to make the image transparent. This is great for adding subtle watermarks or semi-transparent overlays.

### Apply Changes
Tap the **Apply** button at the top right to save your crop and opacity settings.

---

## Canvas Controls

The Image Source supports standard LiveLens interactions:
- **Move**: Drag to position the image.
- **Resize**: Pinch to scale.
- **Rotate**: Use the rotation handle (bottom-right) to spin the image.
- **Rotation Degree**: While rotating, a degree indicator appears at the **top-center** of the image box.
- **Reset Rotation**: Tap the reset handle at the **top-right** corner of the crop area to return the rotation to 0 degrees.
- **Double Tap (Fill)**: Double-tap to quickly scale the image to fill the entire canvas (Fit to height or width). Double-tap again to restore its original size and position.

---

## Image Source Settings Summary

| Setting | Description |
|---|---|
| Change Image | Select a different image file from storage |
| Cropping | Drag handles in the preview to crop the image |
| Opacity | Control transparency level (0-100%) |
| Reset Rotation | Instantly returns the image to 0Â° rotation |

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Canvas Layout](../settings/canvas.md)
