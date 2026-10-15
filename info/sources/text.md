# Text Source

## Overview

The Text Source allows users to add custom text overlays to a LiveLens scene. 

It features a powerful **Text Editor Pro** that supports standard typography settings and advanced **CSS-based styling**, allowing creators to design professional-looking overlays directly on their mobile device.

---

## Opening Text Settings

To open the Text Editor:

1. Add a **Text Source** to the scene.
2. Select the Text Source on the canvas.
3. Tap the **Settings** icon.

The Text Editor popup opens, featuring a live preview area on the left and styling controls on the right.

---

## Text Editor Interface

### Preview Area
The left side shows how your text looks with the current styles applied.
- **Dark/Light Toggle**: Switch the preview background between dark and light modes to check visibility.
- **Edit Text**: Tap anywhere on the preview box to open the text input dialog.
- **Multi-line Input**: You can enter multiple lines of text (up to 5 lines). The renderer will automatically center and layout the text.

### Apply Button
Tap the **Apply** button at the top right to save your changes and update the text on the main canvas.

---

## Typography & Fonts

LiveLens provides flexible font support:

### System Fonts
Choose from built-in styles:
- **Default**: Standard system font.
- **Serif**: Traditional font with small decorative lines.
- **Sans**: Clean, modern font without decorative lines.
- **Mono**: Fixed-width font, great for technical looks.
- **Bold**: Thickened version of the default font.

### Custom Fonts
You can use your own branded fonts:
1. Tap the **+ (Plus)** icon in the Typography section.
2. Select a **.ttf** font file from your device storage.
3. The font will be added to your custom list.
4. **Deleting Fonts**: Long-press a custom font chip to remove it from your library.

---

## Appearance Settings

### Colors
- **Color Wheel**: Use the visual picker to find the exact hue.
- **HEX Input**: Enter a specific color code (e.g., `#FF0000` for red).
- **Presets**: Quickly select from a list of common colors.

### Opacity
Adjust the **Opacity slider** from 0% to 100% to make your text transparent or fully solid.

---

## Advanced CSS Styling

For power users, LiveLens supports a subset of CSS properties to create unique styles. You can either select from **CSS Presets** or type your own code in the Advanced section.

### Supported Properties

| Property | Description | Example |
|---|---|---|
| `font-size` | Change the size of the text | `font-size: 100px;` |
| `font-weight` | Make text bold | `font-weight: bold;` |
| `font-style` | Make text italic | `font-style: italic;` |
| `letter-spacing` | Adjust space between letters | `letter-spacing: 5px;` |
| `text-shadow` | Add a drop shadow (x, y, radius, color) | `text-shadow: 2px 2px 5px #000;` |
| `text-stroke` | Add an outline (width, color) | `text-stroke: 2px #FFF;` |
| `background-color` | Add a background behind the text | `background-color: #000;` |
| `border-radius` | Round the background corners | `border-radius: 10px;` |
| `padding` | Add space around the text | `padding: 20px 40px;` |
| `color` | Support for linear gradients | `color: linear-gradient(#F00, #00F);` |

**CSS Reset**: If you want to start over, tap the red **RESET** button next to the Advanced (CSS) header to clear all custom CSS.

### Text Animations
You can animate your text using the `animation` property:
`animation: [type] [duration]s;`

**Available Types:**
- `blink`: Text flashes on and off.
- `rainbow`: Colors cycle through the spectrum.
- `scroll`: Text moves horizontally (Infinite loop).
- `glow`: Text pulses with a bright light.
- `pulse`: Text fades in and out slightly.
- `fade`: Text fades in and out fully.
- `wave`: Text moves in a wave-like motion.
- `shake`: Text jitters rapidly.

*Example: `animation: rainbow 3s;`*

---

## Canvas Controls

The Text Source supports all standard LiveLens canvas interactions:
- **Move**: Drag to position.
- **Resize**: Pinch to scale.
- **Rotate**: Use the rotation handle (bottom-right) to spin the text.
- **Rotation Degree**: While rotating, a degree indicator appears at the **top-center** of the text box.
- **Reset Rotation**: Tap the reset handle at the **top-right** corner to instantly return the rotation to 0 degrees.
- **Double Tap**: Fit the text to the canvas width (or height depending on aspect ratio).
- **Z-Order**: Move above or below other sources.

---

## Text Source Settings Summary

| Setting | Description |
|---|---|
| Edit Text | Change the actual message |
| Font | Select from System or Custom (.ttf) fonts |
| Opacity | Control transparency (0-100%) |
| Color | Choose solid colors or gradients |
| CSS | Apply advanced styles and animations |

---

## Related Documentation

- [Sources](./README.md)
- [Scenes](../scenes/README.md)
- [Fonts Management](../settings/fonts.md)
