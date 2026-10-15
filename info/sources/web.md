# Web Source

## Overview

The **Web Source** allows users to add web-based content directly to their LiveLens scene. This is perfect for adding stream alerts (Streamlabs, Streamelements), live chats, widgets, or even full websites to your broadcast.

LiveLens features a highly optimized web engine designed to handle real-time updates and interactive overlays without draining your device's battery.

---

## Adding a Web Source

To add web content:

1. Tap the **+ (plus)** icon and select **Web Source**.
2. By default, it will be added to the canvas.
3. Tap the source and open **Settings** to configure the URL or local file.

---

## Web Source Editor Features

The Web Source Editor is divided into a **Preview Section** (left) and a **Settings Panel** (right). The top header includes a **Toggle Settings Visibility** button (Fullscreen toggle) to hide or show the settings panel for an unobstructed web preview, an **Apply** button to commit changes, and a **Close** button.

### 1. Dimensions & Resolution
- **Width & Height**: Set custom rendering resolution dimensions for the web viewport (default: 672x378).
- **Reset Size**: Tap the refresh icon next to the dimension fields to reset the viewport back to default (672x378).

### 2. Source Types & URL
- **URL (Online)**: Enter any standard web address. Includes an **HTTPS Security Indicator** (Green lock icon for secure `https://` URLs, language globe for standard HTTP) and a **Clear URL** button.
- **Local HTML**: Load offline HTML files from your phone's storage using the "Select HTML File" button. Ideal for custom widgets that don't need internet.
- **Presets**: Quick-action preset buttons for popular destinations: **Google**, **Streamlabs**, and **StreamElements**.

### 3. Browser Mode (Interactive)
By default, web sources are "static" (non-interactive) on the canvas to prevent accidental clicks.
- **Toggle Browser Mode**: Turn this on to interact with the website directly within the settings preview area. This allows you to log in to accounts, click buttons, or scroll the page.
- **Browser Toolbar**: When Browser Mode is active, an expanded navigation bar provides:
  - **Home**: Instantly navigate back to your home URL.
  - **Back & Forward**: Navigate browser history.
  - **Reload / Stop**: Refresh the page, or stop loading while a page request is in progress (icon toggles dynamically).
  - **Current URL Bar**: Displays the currently active web page address.
  - **Go Button**: Trigger navigation to the typed URL.
  - **Progress Bar**: A top progress indicator bar showing real-time page loading state (0–100%).
  - **Interaction Tip**: Helpful reminder to complete logins or scrolling before configuring crop handles.

### 4. Crop Mode
If you only want to show a specific part of a page (e.g., just the chat box or alert box):
1. Toggle **Enable Cropping** in the settings panel.
2. Blue handles will appear in the preview area. Drag them to frame your content.
3. **Note**: Direct touch interaction with the webpage is disabled during Crop Mode to enable precise 4-edge handle dragging.

### 5. Rendering Quality
Adjust the rendering load based on your device's performance:
- **Performance (0.5x)**: Renders at half resolution (Best for older devices).
- **Balanced (0.75x)**: A mix of quality and speed.
- **Native (1.0x)**: Full-quality rendering.

---

## Smart Features for Streamers

### Auto-Scroll (Chat Support)
LiveLens includes an intelligent script that detects scrollable chat containers (like YouTube or Twitch chat). It automatically keeps the chat scrolled to the bottom so your stream always sees the latest messages.

### OBS Compatibility
The web source simulates an OBS (Open Broadcaster Software) environment, triggering standard visibility events (`obsSourceVisibleChanged`) so that animations and alerts start correctly when you switch scenes.

### Performance Optimization
- **Idle Pacing**: When the web page isn't changing, LiveLens reduces the capture rate to save battery.
- **Warm-up Mode**: When a page first loads, the engine runs in high-performance mode to ensure animations finish loading before slowing down for power saving.

---

## Canvas Controls

- **Move & Resize**: Position the widget anywhere on your layout.
- **Rotate**: Full rotation support with a degree indicator.
- **Reset Rotation**: Tap the top-right handle to instantly reset to 0°.
- **Double Tap**: Scale the web source to fill the canvas.

---

## Web Source Settings Summary

| Setting | Description |
|---|---|
| Fullscreen View Toggle | Hides/shows the settings panel for an unobstructed preview |
| Dimensions & Resolution | Customize web viewport width and height (with Reset button) |
| Browser Mode | Enables touch interaction within the settings preview (with full toolbar & progress bar) |
| Crop Mode | Frame a specific section of the page with 4-edge handles (disables touch for precision) |
| HTTPS Security Indicator | Displays Green Lock icon for HTTPS or Globe icon for HTTP |
| Local HTML | Load `.html` files from your device |
| Quality Scale | Choose between Performance (0.5x), Balanced (0.75x), and Native (1.0x) quality |
| Presets | Quick links for popular destinations (Google, Streamlabs, StreamElements) |

---

## Related Documentation

- [Sources](./README.md)
- [Stream Alerts Setup](../overlays/alerts.md)
- [Troubleshooting Web](../troubleshooting/web-loading.md)
