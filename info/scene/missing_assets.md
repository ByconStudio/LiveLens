# ⚠️ Missing Assets & Smart Relink

## Why do assets go missing?

LiveLens scenes don't store your images, videos, or fonts directly inside the `.json` file. Instead, they store **references** (URIs) to where those files are located on your device.

An asset becomes "missing" if:
- You delete the file from your Gallery or File Manager.
- You move the file to a different folder.
- You rename the file.
- You clear the app's storage permission for that specific file.
- You import a scene from another device that doesn't have the same files.

---

## 🚨 Automatic Detection

LiveLens includes an **Asset Integrity Monitor**. Every time you switch to a scene or start the app, the `AssetManager` automatically checks if all referenced files are reachable.

If even one file is missing, the **Missing Assets Popup** will appear automatically. You don't need to manually check your sources; the app does it for you to prevent black screens or default font fallbacks during your stream.

---

## 🛠️ The Missing Assets Dialog

When the dialog appears, it categorizes missing files by their type:
- **Images & GIFs**: Used in Image sources, Backgrounds, or Overlays.
- **Videos**: Used in Video sources.
- **Fonts**: Used in Text sources or the Global Timer.
- **VTuber Models**: `.vrm` or `.json` model files.
- **Audio**: Background music or sound effects.

For each asset, the dialog shows the **Reason** for failure (e.g., "File moved or deleted" or "Permission revoked").

---

## 🚀 Smart Relink (Bulk Resolution)

This is the most powerful feature of the LiveLens Asset Engine. If you have moved an entire folder of assets, you don't have to fix them one by one.

### How it works:
1. Tap **Relink** on any missing asset in the list.
2. Use the system file picker to locate the **correct version** of that file.
3. Once selected, LiveLens triggers **Smart Bulk Resolution**:
    - It analyzes the folder where you found the first file.
    - It scans for every other missing filename in that scene configuration.
    - If a filename match is found in that new folder, it **automatically relinks** it without asking you again.

> [!TIP]
> Keep your stream assets (overlays, alerts, models) in a single dedicated folder. If you ever move that folder, a single relink will fix your entire scene in seconds.

---

## 🧹 Ignore vs. Cleanup

If you cannot find a file or don't want to fix it right now, you have two options:

### 1. Ignore
- **Action**: Marks the URI as "Known Missing".
- **Result**: The asset will not appear in the scene, and the Missing Assets Popup will **stop bothering you** about this specific file for the current session.
- **Use Case**: When you temporarily don't have access to a drive or SD card.

### 2. Cleanup
- **Action**: Permanently removes the reference from the scene configuration.
- **Result**: The source using that asset will be reset to default or removed.
- **Use Case**: When you have deleted a file permanently and want to keep your scene data clean.

---

## Related Documentation

- [Scene Management](scene.md)
- [Source Settings](../sources/sources.md)
