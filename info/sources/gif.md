# GIF Source

## Overview

The GIF Source allows users to add animated GIF images to their LiveLens scenes. 

It is optimized for high performance using GPU frame caching and includes a dedicated **GIF Editor** for cropping, looping, and opacity adjustments.

---

## Opening GIF Settings

To open the GIF Editor:

1. Add a **GIF Source** to the scene.
2. Select the GIF Source on the canvas.
3. Tap the **Settings** icon.

The GIF Editor popup opens, featuring a live preview with cropping tools and control panels.

---

## GIF Editor Features

### Performance & Limits
To maintain app stability and smooth streaming, LiveLens enforces the following limits:
- **Max File Size**: 15MB.
- **Max Resolution**: 1920x1920 pixels (1080p).
> GIFs exceeding these limits will trigger a warning and will not be loaded.

### Preview & Cropping
The preview area allows you to precisely frame your animation.
- **Interactive Cropper**: Drag the blue handles at the **Top-Left** and **Bottom-Right** to crop the GIF.
- **Dimmed Areas**: Parts of the GIF outside the crop frame are shown with a dark overlay, indicating they will be hidden on the main canvas.

### GIF Controls
- **Select GIF**: Pick a `.gif` file from your device storage.
- **Loop GIF**: Check this box to make the animation play infinitely. If unchecked, the GIF will play once and stop at the last frame.
- **Opacity**: Use the slider (0-100%) to adjust transparency.

---

## Canvas Controls

The GIF Source supports full interactive controls on the canvas:
- **Move**: Drag to reposition.
- **Resize**: Pinch to scale up or down.
- **Rotate**: Use the rotation handle (bottom-right).
- **Rotation Degree**: A degree indicator appears at the **top-center** during rotation.
- **Reset Rotation**: Tap the reset handle at the **top-right** corner of the crop frame to return to 0°.
- **Double Tap**: Quickly scale the GIF to fill the canvas. Double-tap again to return to the previous size.

---

## GIF Source Settings Summary

| Setting | Description |
|---|---|
| Select GIF | Browse and load a GIF file from your phone |
| Loop GIF | Toggle between infinite playback and single play |
| Opacity | Adjust transparency level |
| Cropping | Manually crop the animated area |
| Reset Rotation | Instantly aligns the GIF to the original orientation |

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Performance Tips](../troubleshooting/performance.md)
