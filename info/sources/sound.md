# Sound Source

## Overview

The Sound Source allows you to add high-quality audio playback to your LiveLens scene. 

Unlike simple background music, the LiveLens Sound Source is integrated directly into the **Native Audio Mixer**. This ensures your audio is perfectly synchronized with your stream, supports real-time monitoring, and provides professional-grade volume control.

---

## Opening Sound Settings

To configure your Sound Source:

1. Add a **Sound Source** to the scene.
2. Select the Sound Source on the canvas.
3. Tap the **Settings** icon.

The Sound Settings popup opens, featuring a **Live Audio Visualizer** on the left and a comprehensive **Control Panel** on the right.

---

## Settings Interface

### 📊 Live Audio Visualizer
The left side provides visual feedback for your audio playback:
- **Real-time Spectrum**: An animated bar visualizer that reacts to the current loudness of the audio.
- **Progress Bar**: Shows the current playback position.
- **Time Indicators**: Displays the elapsed time and total duration of the track.

### ⚙️ Control Panel
The right side contains all functional settings for the sound:

#### 1. Sound Selection
- **Select File**: Choose a single audio file from your device (supports MP3, WAV, M4A, OGG, FLAC).
- **Select Folder**: Select an entire directory. The app will automatically scan and create a playlist from all compatible audio files found in that folder.
- **File Info**: Shows the name of the currently loaded file or the number of files detected in Folder Mode.

#### 2. Volume & Monitoring
- **Volume Slider**: Adjust the output volume from 0% to 100%.
- **Hear It (Monitoring)**: Toggle this to hear the audio through your device's speakers or headphones while you are streaming.
- **Output to Stream**: Toggle this to include/exclude this specific sound source from the final stream or recording.

#### 3. Playback Behavior
- **Loop Audio**: When enabled, the current file will restart automatically once it ends.
- **Shuffle Folder (Folder Mode Only)**: Randomizes the playback order of files within the selected folder.

---

## Technical Features

### Multi-Format Support
The native decoder supports a wide range of professional audio formats:
- **MP3**: Standard compressed audio.
- **WAV**: High-quality uncompressed audio.
- **FLAC**: Lossless compression for audiophiles.
- **M4A / OGG**: Modern efficient audio formats.

### Performance
- **Asynchronous Decoding**: Audio is processed on a background thread to prevent UI lag.
- **Low Latency**: Optimized for real-time streaming environments.
- **Folder Mode Logic**: Automatically advances to the next track in the playlist once a file finishes playing.

---

## Canvas Controls

Since the Sound Source is a functional element, it has a minimal presence on the canvas:
- **Move**: Drag the sound icon to keep your workspace organized.
- **Visibility**: Use the eye icon in the source list to "Mute" the source (disables decoding and playback).
- **Locking**: Lock the source to prevent accidental movement.

---

## Related Documentation

- [Sources](./README.md)
- [Audio Mixer](../settings/audio.md)
- [Scenes](../scenes/README.md)
