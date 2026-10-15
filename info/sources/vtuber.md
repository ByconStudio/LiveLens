# VTuber Source (Live2D)

## Overview

The **VTuber Source** brings your Live2D models to life directly on your Android device. It uses an industry-standard rendering engine to support high-quality `.moc3` models with real-time physics, camera-based face tracking, audio-based lip-syncing, and expression overlays.

LiveLens is designed to give mobile VTubers a professional production environment without needing a PC.

---

## 🛠️ Step 1: Configuring Your Model (Required)

Before you can add a VTuber source to your scene, you must select a model folder in the app settings.

1. Go to **Global Settings** → **VTuber**.
2. Tap **Select & Configure VTuber Model**.
3. **Disclaimer**: Read and agree to the Live2D disclaimer if prompted.
4. **Selection Guide**: Tap "How to select?" for a visual guide.
5. **Folder Selection**: A file picker will open. Navigate to the **folder** that contains your `.model3.json` file.
6. **Crucial**: Do **NOT** select individual files. Simply enter the model's folder and tap **"USE THIS FOLDER"** at the bottom.
7. Grant the app permission to access the folder.

### Compatibility Note
- **Supported**: Cubism models up to version **6.0**.
- **Higher Versions**: For models exported from newer Live2D Editors, please ensure the export target version is set to **SDK 5.0 / SDK 4.2 compatibility mode** in the Live2D Editor.

---

## 🎭 Step 2: Adding the VTuber Source

### Method A: Regular Addition
1. Open your streaming scene.
2. Tap the **+ (plus)** icon and select **VTuber**.
3. If you have already selected a model in settings, your avatar will appear on the canvas.

### Method B: Shortcut (If No Model Selected)
If you try to add a VTuber source without setting up a model first:
1. A popup titled **"VTuber Model Required"** will appear.
2. Tap **"Go to Global Settings"** in the popup.
3. This will take you directly to the VTuber configuration tab, where you can follow the folder selection steps.

> **Update Note**: If you update to a new model in Settings while a VTuber source is already active, you should remove and re-add the source to ensure the new rig loads correctly.

---

## 🔍 VTuber Inspector (Settings)

To fine-tune your avatar, select it on the canvas and tap the **Settings** icon to open the **VTuber Inspector**.

The Inspector opens as a left-docked sidebar drawer with no background dimming, allowing you to clearly view your avatar on the canvas in real time while adjusting settings.

### 1. Input Mode Selection
The top dropdown menu allows you to switch between tracking input sources:
- **Face Tracking (Camera)**: Uses your phone's camera to track facial movements and expressions in real time.
- **Lip Sync (Voice)**: Uses your microphone volume and audio amplitude to drive mouth movement and physics.

### 2. Face Tracking Camera Options
When **Face Tracking** is selected:
- **Camera Facing**: Toggle between **FRONT** and **BACK** cameras for face tracking input.
- **Auto Permission Fallback**: If camera permission is denied, LiveLens automatically falls back to Voice Lip Sync mode.

### 3. Model Controls
- **Opacity Slider**: Adjust transparency from 0% to 100%.
- **Physics Strength Slider**: Adjust hair, clothing, and accessory physics reactivity (0.0x to 2.0x).

### 4. Voice & Lip Sync Settings
When **Lip Sync (Voice)** is active:
- **Enable/Disable Switch**: Toggle voice tracking on or off.
- **Lip Sync Threshold**: Set the minimum audio level required to trigger mouth movement (helps suppress background noise).
- **Physics Boost Threshold**: Increases physics intensity dynamically when speaking louder.

---

## ⚙️ Advanced Parameter Mode

For professional riggers, **Advanced Mode** enables direct manipulation of individual Live2D parameters:
- **Double Warning Dialog**: For safety, a two-step confirmation dialog appears before unlocking Advanced Mode for the first time.
- **Search Bar**: Real-time parameter search field (`Search parameters...`) to find specific parameters quickly (e.g., `ParamEyeBallX`).
- **Live Parameter Sliders**: Adjust parameter values directly within their rigged `min` to `max` bounds.
- **Reset Button**: Tap **Reset Only** / **Reset All** (red refresh icon) to instantly restore all manual parameters to default.

---

## 🎭 Expressions & Overlays
- **Toggle Expressions**: If your model has built-in expressions (Happy, Blush, etc.), you can toggle them in the Inspector.
- **Floating Overlay**: In **Global Settings** → **VTuber**, enable **"Show Expressions"** to place quick-toggle buttons on your screen during streams.

---

## Canvas Controls

- **Move & Resize**: Place your avatar anywhere on the screen.
- **Rotate**: Full 360-degree rotation support with degree feedback.
- **Reset Rotation**: Tap the top-right handle to instantly reset to 0°.
- **Double Tap**: Scale the avatar to fill the canvas.

---

## VTuber Source Settings Summary

| Setting | Description |
|---|---|
| Input Mode Selection | Switch between Face Tracking (Camera) and Lip Sync (Voice) |
| Camera Facing | Toggle FRONT or BACK camera for face tracking |
| Model Opacity | Set avatar transparency level |
| Physics Strength | Adjust reactivity of hair, clothing, and physics chains |
| Lip Sync Threshold | Minimum microphone volume needed to trigger mouth movement |
| Physics Boost Threshold | Boost physics strength dynamically when speaking loudly |
| Advanced Parameter Mode | Direct slider control of Live2D parameter IDs (with Double Warning unlock) |
| Parameter Search & Reset | Search parameters in real time and reset values to rigging defaults |

---

## Related Documentation

- [Sources](./README.md)
- [Audio Configuration](../audio/README.md)
- [Live2D Export Guide](../vtuber/export.md)
