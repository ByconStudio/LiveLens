# VTuber Settings

## Overview

The **VTuber Settings** tab allows you to configure your animated avatar for streaming. LiveLens supports industry-standard Live2D Cubism models, providing a high-quality projected experience directly on your device.

---

## 🏗️ Model Configuration

This is the primary setup required to use a VTuber avatar in your scenes.

### 1. Selection & Setup
- **Select & Configure VTuber Model**: Use this button to load your model into the app.
- **Disclaimer**: Before selecting a model for the first time, you must read and agree to the VTuber disclaimer.
- **Selection Guide**: A built-in guide ("How to select?") explains the folder selection process:
    - You must select the **entire folder** containing your `.model3.json` file.
    - Do **NOT** select individual files inside the folder.
    - Navigate into the model folder and tap **"USE THIS FOLDER"** to grant permission.

### 2. Compatibility Details
- **Cubism Versions**: Supports models up to version **6.0**.
- **Newer Editors**: For models exported from newer Live2D Editors, please set the export target version to **SDK 5.0 / SDK 4.2 compatibility mode** in the Live2D Editor.

### 3. Model Updates
- **Update Note**: If you are updating an existing model and already have a VTuber source added to your scene, you must **remove and re-add the source** to ensure the new rig loads correctly.

---

## 🎭 Overlay Settings

Control how you interact with your avatar during a live stream.

### Show Expressions
- **Toggle**: Enable this switch to show expression buttons in the **Floating Overlay Dashboard**.
- **Function**: This allows you to trigger your model's expressions (e.g., Happy, Sad, Blush) with one tap while you are in another app or game.

---

## VTuber Settings Summary

| Feature | Description |
|---|---|
| Folder Selection | Grant access to the entire model directory |
| SDK Compatibility | Supports Cubism 6.0 (newer editors require SDK 5.0/4.2 export target mode) |
| Expressions Overlay | Control avatar emotions from the floating bubble |
| Model Refresh | Required removal/re-addition of source for updates |

---

## Related Documentation

- [VTuber Source](../sources/vtuber.md)
- [Floating Control](./floating.md)
- [Video Settings](./video.md)
