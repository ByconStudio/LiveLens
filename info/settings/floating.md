# Floating Control & Notifications

## Overview

The **Floating Control** system is designed for single-device streamers who need full control over their broadcast without switching back to the LiveLens app. It provides a real-time bridge between your game and the streaming engine.

The system consists of three main parts:
1. **In-App Settings**: Where you configure the behavior and appearance.
2. **The Control Bubble**: A movable entry point that stays on top of other apps.
3. **The Floating Panel**: A mini-dashboard for active stream management.

---

## ⚙️ In-App Settings (Setup)

Access these in **Settings → Floating Control**.

### 🛡️ Permissions Required
- **Overlay Permission**: Needed to draw the bubble and panel over other apps.
- **Notification Permission**: Required for the foreground service and notification bar controls (Android 13+).

### 🛠️ Configuration Options
- **Floating Control Bubble**: Toggle the main feature on/off.
- **Notification Bar Controls**: When enabled, adds stream actions directly to your phone's notification shade.
- **Hide from Stream**: When active, the floating panel and bubble will be **invisible to your viewers** (uses `FLAG_SECURE`).
- **Unmute on Exit**: Automatically restores your original audio settings when you close the floating dashboard.

---

## 🔘 The Control Bubble

The bubble is your interactive anchor on the screen.

### 🖐️ Interactions
- **Drag**: Move the bubble anywhere on the screen.
- **Tap**: Open the full **Floating Panel**.
- **Remove**: Drag the bubble to the **"X" area** at the bottom-center of your screen to instantly close the floating service.

### 🎨 Bubble Customization
- **Custom Icon**: Use any image from your gallery as the bubble icon.
- **Icon Size**: Scale the bubble from **32dp to 100dp**.
- **Reset**: Quickly restore the default icon and size.

---

## 📊 The Floating Panel (Dashboard)

Tapping the bubble expands the panel. It is divided into several functional areas:

### 1. Permanent Top Bar
- **Chat Toggle**: Switch between the dashboard and **Full Chat View**.
- **Live Monitoring**: 
    - **Stream Timer**: Active recording/streaming time.
    - **Bitrate**: Real-time upload speed.
    - **FPS**: Current capture engine performance.
- **Close Button**: Collapses the panel back into the bubble.

### 2. Action Controls
You can customize exactly which actions appear in your dashboard through the app settings:

- **Stream Management**: 
    - **Stop**: Ends the current stream or recording session.
    - **Mic Toggle**: Instantly mute or unmute your microphone.
- **Customizable Overlays (Toggleable)**: 
    - You can choose to **Show/Hide the BRB and Starting Soon buttons** from the Action Buttons settings if you don't use these specific overlays.
- **Dynamic Scene Switching (Pinned Scenes)**: 
    - This is a powerful feature that allows you to switch between your created scenes instantly.
    - **How it works**: Any scene you create in the app can be "Pinned" to the floating panel. 
    - In the **Action Buttons** settings, you will see a list of all your saved scenes. Toggle the switch next to a scene to pin it to the dashboard.
    - Pinned scenes appear as dynamic icons in the floating panel, allowing for seamless transitions during gameplay.

### 3. Audio & Expressions
- **Volume Management**: Adjust internal and mic audio levels.
- **Volume Styles**: Choose between **Default, Fluid, Glass, or Retro** bar aesthetics.
- **VTuber Expressions**: If using a VTuber source, trigger model expressions directly from the panel.

### 4. Personalization
- **Animated Wallpapers**: Supports static images or **GIFs (up to 5MB)** as panel backgrounds.
- **Glass Blur**: Adjust the blur intensity (0-25px) of the panel background for better text clarity.

---

## 🔔 Notification Bar Controls

When **Notification Bar Controls** are enabled, you can manage your stream from the Android notification shade:

- **Mic Mute/Unmute**: Toggle your microphone status.
- **BRB Toggle**: Switch to your BRB scene.
- **Soon Toggle**: Switch to your Starting Soon scene.
- **Stop Stream**: Gracefully end the broadcast.
- **Live Stats**: The notification title and text update in real-time to show streaming/recording duration.

---

## Floating Control Summary

| Feature | Description |
|---|---|
| Bubble Removal | Drag to the bottom "X" to stop the service |
| Secure Capture | Option to hide the UI from the final broadcast |
| Chat View | Integrated Twitch/YouTube chat reader |
| Pinned Scenes | One-tap scene switching during gameplay |
| GIF Support | Animated backgrounds for the control panel |

---

## Related Documentation

- [Scenes](../scenes/README.md)
- [Video Settings](./video.md)
- [Chat Settings](./chat.md)
