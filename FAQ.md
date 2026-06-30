# Frequently Asked Questions (FAQ)

## General Questions

### What is LiveLens?
LiveLens is a professional live streaming, recording, scene control, and VTuber tool for Android. It brings OBS-style production capabilities directly to your mobile device.

### Is LiveLens free?
Yes! LiveLens is completely free to use. There are no forced accounts, ads, watermarks, or hidden paywalls.

### What are the system requirements?
- **Android:** Android 8.0 or higher
- **RAM:** Minimum 4GB (6GB+ recommended for better performance)
- **Storage:** At least 500MB free space
- **Internet:** Stable connection for streaming

### Where can I download LiveLens?
Download from the official website: [livelens.live](https://www.livelens.live/)

---

## Streaming & Recording

### How do I stream to Twitch?
1. Get your RTMP URL and stream key from Twitch
2. In LiveLens, go to Settings → Streaming
3. Enter your RTMP URL and stream key
4. Tap "Start Stream"

### Can I stream to multiple platforms at once?
Yes! LiveLens supports multi-streaming. Set up multiple streaming destinations in the settings.

### What are the recommended streaming settings?
- **Resolution:** 720p (1080p if device supports)
- **FPS:** 30 or 60 (based on preference)
- **Bitrate:** 2500-6000 kbps (adjust based on internet speed)
- **Encoder:** H.264 for compatibility, H.265 for better quality

### Can I record locally while streaming?
Yes! You can record high-quality video locally even while streaming.

### What video formats are supported?
LiveLens supports H.264 and H.265 video codecs (device dependent).

---

## Scenes & Sources

### How do I create a new scene?
1. Tap the "Scenes" button
2. Tap "+" to create a new scene
3. Add sources (camera, screen, images, text, etc.)

### What sources can I add?
- Screen capture
- Camera
- Images
- Text
- Video files
- Web sources
- GIFs
- VTuber models

### Can I import and export scenes?
Yes! You can save and load scenes from JSON files.

### How do I switch scenes?
Tap on the scene name to switch. Note: Scene switching is unavailable during active streaming or recording.

---

## Audio

### How do I capture microphone and internal audio?
1. Go to Settings → Audio
2. Enable both microphone and internal audio
3. Adjust levels as needed

Note: This feature depends on Android version and device support.

### What audio tools are available?
- Noise suppression
- Echo cancellation
- Gain boost
- Noise gate
- High-pass filtering
- Automatic gain control

### Can I monitor audio in real-time?
Yes! Use the audio monitor to listen to your microphone levels.

---

## VTuber Tools

### How do I import a Live2D model?
1. Prepare your Live2D model in Cubism format (up to v5.1)
2. In LiveLens, add a VTuber source
3. Select your model file
4. Customize settings (breathing, idle motion, etc.)

### What Live2D versions are supported?
LiveLens supports Cubism 5.1 and earlier versions.

### Can I use lip sync with my VTuber model?
Yes! LiveLens includes real-time microphone lip sync.

### How do I adjust VTuber expressions?
Use the VTuber inspector to:
- Control expressions
- Adjust opacity
- Enable/disable breathing
- Adjust physics and motion

---

## Voice Chat

### How do I use the voice chat feature?
1. Go to Voice Chat section
2. Create or join a voice room
3. Share the deep link with others
4. Start chatting!

### Do I need an account for voice chat?
No! LiveLens voice chat works without creating an account.

### Can I use voice chat between LiveLens and LiveLens Lite?
Yes! Both versions support voice chat together.

---

## Settings & Customization

### How do I customize overlays?
LiveLens supports custom JSON themes for floating controls. Import themes from the settings.

### Can I use custom countdown timers?
Yes! Add and customize countdown timers in your scenes.

### How do I change canvas layout?
LiveLens supports 16:9 and 9:16 layouts. Choose from Settings → Canvas.

### What are snap guides?
Snap guides help you align and position sources precisely on your canvas.

---

## Troubleshooting

### LiveLens keeps crashing
- **Solution:** Update to the latest version
- Clear app cache: Settings → Apps → LiveLens → Storage → Clear Cache
- Restart your device
- Check available storage (at least 500MB free)

### My stream quality is poor
- Check internet connection speed
- Lower bitrate or resolution
- Close other apps consuming bandwidth
- Use 2.4GHz or 5GHz WiFi (check which is more stable)

### Audio is not syncing with video
- Restart the app
- Check audio/video encoder settings
- Try using H.264 encoder
- Reduce resolution or FPS

### VTuber model is not showing
- Verify model is in correct Cubism format
- Check file permissions
- Try re-importing the model
- Update to the latest LiveLens version

### Scene switching doesn't work during streaming
- This is by design! Scene switching is disabled during active streaming
- Plan your scenes before going live
- Use different cameras/sources to switch between layouts

### Device is getting too hot
- Reduce FPS (30 instead of 60)
- Lower resolution
- Take breaks during long streams
- Ensure device has good ventilation

---

## Performance & Limits

### What's the maximum resolution?
Up to 4K (depending on device capabilities).

### How many sources can I add?
Maximum source count depends on device performance. Start with 5-10 sources and adjust based on performance.

### Can I use multiple scenes simultaneously?
No, but you can quickly switch between scenes (when not streaming).

### Why is my device slow during streaming?
- Check available RAM
- Close background apps
- Reduce number of sources
- Lower quality settings (resolution/FPS)
- Enable hardware acceleration

---

## Privacy & Security

### Does LiveLens collect my data?
No! LiveLens is privacy-first and doesn't require creating an account.

### Is my stream key safe?
Yes, your stream credentials are stored locally on your device.

### Can I delete my settings/data?
Yes! Go to Settings → Clear All Data to reset LiveLens.

For more details, see our [Privacy Policy](https://www.livelens.live/pages/privacy.html)

---

## Support

### I still have questions
- Check our [Official Website](https://www.livelens.live/)
- Join our [Discord Community](https://discord.gg/kUqmbKhs6w)
- Visit our [Contact & Support](https://www.livelens.live/pages/contact.html) page
- Create a Discussion in this repository

### How do I report a bug?
Open an Issue or Discussion on GitHub with:
- Device model and Android version
- LiveLens version
- Steps to reproduce the bug
- Screenshots or videos (if applicable)

### How do I request a feature?
Create a Feature Request Discussion on GitHub with:
- Clear feature description
- Problem it solves
- Proposed solution
- Any mockups or examples

---

**Last Updated:** June 2026
**LiveLens - Created by Arpan**