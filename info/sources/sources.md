# Sources

## Overview

Sources are the individual content elements that users add to a LiveLens scene.

A scene can contain multiple sources, allowing users to build their own custom streaming layout.

LiveLens currently provides the following source types:

- Screen Capture
- Camera
- Image
- Text
- GIF
- Video
- Web
- Chat Box
- Sound
- VTuber
- UVC (Beta)

Each source type has its own settings and behavior. Detailed settings for each source are documented on their respective pages.

---

## Adding a Source

To add a source to a scene:

1. Open the scene where the source should be added.
2. Tap the **+ (plus)** icon next to **Add Sources**.
3. The source selection popup appears.
4. Select the source type you want to add.
5. The selected source is added to the current scene.

The source selection popup currently provides:

- Screen Capture
- Camera
- Image
- Text
- GIF
- Video
- Web
- Chat Box 
- Sound
- VTuber
- UVC (Beta)

To add a source, simply tap the source type you want to use.

---

# Source Controls

After a source has been added to a scene, LiveLens provides common controls for managing that source.

These controls are available across the source system, while individual source types may provide additional settings through their own settings panel.

---

## Move and Position a Source

Users can drag a source on the canvas to change its position.

This allows sources to be placed anywhere within the scene according to the user's layout.

---

## Zoom In and Zoom Out

Users can zoom a source in or out to change its size.

This allows the size of individual sources to be adjusted independently within the scene.

---

## Double Tap to Fit the Canvas

Double-tapping a source makes it **cover the entire canvas**.

This provides a quick way to make a source fill the scene without manually resizing it.

### Double Tap Again

Double-tapping the same source again returns it to its previous size and position.

This allows users to quickly switch between the source's normal layout and a full-canvas view.

---

## Z-Order

LiveLens allows users to change the **Z-order** of sources.

Z-order determines which source appears in front of or behind another source when multiple sources overlap.

Users can change the Z-order using the **up and down arrow controls**.

This allows a source to be:

- Moved above another source.
- Moved below another source.
- Reordered within the scene.

---

## Hide and Show a Source

The **eye icon** can be used to hide or show a source.

### Visible

When the eye control is enabled, the source is visible on the canvas.

### Hidden

When the source is hidden, it is not displayed on the canvas.

The source remains part of the scene and can be shown again using the same control.

---

## Locking a Source

The **lock icon** can be used to lock a source.

When a source is locked, its touch interaction is disabled.

This prevents accidental changes such as:

- Dragging the source.
- Zooming the source.
- Accidentally repositioning it.

Locking is useful when a source has already been positioned correctly and should not be changed accidentally while working on the rest of the scene.

Unlocking the source restores its normal touch interaction.

---

## Source Settings

Each source type has its own settings panel.

Users can open the settings for a selected source by tapping the **settings icon**.

The settings popup is specific to the selected source.

For example, a Video source and a Web source do not necessarily have the same settings because each source type has different functionality.

Detailed settings are documented separately for each source type.

---

## Removing a Source

A source can be removed from the current scene using the **delete/trash icon**.

Removing a source deletes that source from the scene.

This does not delete the scene itself.

---

# Common Source Workflow

A typical source workflow is:

1. Tap **+** next to **Add Sources**.
2. Select a source type.
3. Position the source by dragging it.
4. Adjust its size using zoom controls.
5. Use double-tap to quickly make it cover the canvas if needed.
6. Adjust its Z-order when sources overlap.
7. Hide or show the source using the eye icon.
8. Lock the source when its position should no longer be changed.
9. Open the source's settings to configure source-specific options.
10. Delete the source when it is no longer needed.

---

## Source-Specific Documentation

Each source has its own dedicated documentation page containing its available settings and source-specific behavior.

### Sources

- [Screen Capture](./screen-capture.md)
- [Camera](./camera.md)
- [Image](image.md)
- [Text](text.md)
- [GIF](gif.md)
- [Video](video.md)
- [Web](web.md)
- [Chat Box](chatbox.md)
- [Sound](sound.md)
- [VTuber](vtuber.md)
- [UVC (Beta)](uvc.md)

These pages will document the individual settings and behavior of each source.

---

## Related Documentation

- [Home Screen (Broadcast Center)](../home/home.md)
- [Scenes](../scenes/README.md)
- [Scene Import & Export](../import-export/README.md)
- [Canvas](../settings/canvas.md)
- [Video & Stream Settings](../settings/video.md)
- [Account Linking](../settings/account.md)
- [VTuber Settings](../settings/vtuber.md)
