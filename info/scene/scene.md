# Scene Management & Assets

## Overview

Scenes are the foundation of your streaming layout in LiveLens. They allow you to create and organize different setups (e.g., "Starting Soon", "Gameplay", "Just Chatting") and switch between them instantly.

LiveLens uses an advanced **Scene Engine** that handles not just the layout, but also cross-device hardware compatibility and asset tracking.

---

## Opening the Scene Manager

The Scene Manager can be opened by tapping the **scene/movie icon** located next to **Add Sources**.

### Core Actions
- **Create**: Tap **+** to start a new blank canvas. Your current layout is automatically saved before the switch.
- **Switch**: Tap any scene name to load it. A loading overlay will appear while the engine re-initializes sources.
- **Rename**: Tap the **Pencil/Edit icon** to give your scene a custom name.
- **Delete**: Tap the **Trash icon**. Note: The **Default Scene** cannot be deleted to ensure you always have a workspace.

---

## 📥 Importing & Exporting Scenes

LiveLens allows you to share your layouts or move them between devices using `.json` files.

### Exporting
1. Open the Scene Manager.
2. Tap the **Export (Download) icon**.
3. Choose a location on your phone to save the scene file.

### Importing & The "Scene Optimizer"
When you import a scene (especially one made on a more powerful phone), LiveLens runs a **Scene Optimizer** check:
- **Auto-Resolution**: If the imported scene is 4K but your phone only supports 1080p, the app will auto-adjust the resolution to prevent encoder crashes.
- **Source Limits**: If the scene has more sources (e.g., too many cameras) than your device's "Tier" supports, the Optimizer will ask you to select which "extra" sources to remove before importing.
- **Version Check**: If the scene was made in an older version of LiveLens, the app will handle legacy conversion to ensure stability.

---

## ⚠️ Asset Management (Missing Files)

Since scene files only store "links" (URIs) to your images, videos, and fonts, those files might go "missing" if you delete them from your gallery or move them to a different folder.

### The Missing Assets Dialog
If you switch to a scene with broken links, a warning dialog will appear listing all missing files (Images, Videos, Fonts, VTuber Models).

### Smart Relink (Pro Tip)
Instead of fixing every file one by one:
1. Tap **Relink** on one of the missing assets.
2. Locate the file in its new folder.
3. **Magic**: LiveLens will automatically search that same folder for **all other missing assets** in the scene and fix them instantly.

### Ignoring & Cleanup
- **Ignore**: If you don't need a missing asset right now, you can select "Ignore". LiveLens will stop showing warnings for that specific file.
- **Cleanup**: You can choose to permanently remove references to missing assets to keep your scene configuration clean.

For a deep dive into how to recover your scene, see [Missing Assets & Smart Relink](missing_assets.md).

---

## 🔄 Scene Switching During Stream

**Supported**: You can now switch scenes while an active stream or recording is running.

- **Smooth Transitions**: Switching scenes allows you to change your entire layout (e.g., from "Gameplay" to "Just Chatting") without stopping your broadcast.
- **How to Switch**:
    - **In-App**: Open the Scene Manager and tap the scene you want to load.
    - **Floating Panel**: Use **Pinned Scenes** in the floating dashboard to switch scenes without leaving your game.
- **Best Practice**: To ensure the best quality, make sure all your scenes use the same canvas resolution (e.g., all 1080p).

---

## Scene Settings Summary

| Feature | Description |
|---|---|
| Scene Optimizer | Auto-adjusts imported layouts to fit your hardware capabilities |
| Smart Relink | Fixes all missing images/videos in a single step |
| Import/Export | Share and backup layouts as `.json` files |
| Default Scene | A permanent safety scene that cannot be deleted |
| Scene Switching | Fully supported during active streaming and recording |

---

## Related Documentation

- [Sources](../sources/sources.md)
- [Overlay Settings](../settings/overlay.md)
- [Performance Tips](../troubleshooting/performance.md)
