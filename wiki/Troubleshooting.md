# 🆘 Troubleshooting Guide

Complete troubleshooting guide for common LiveLens issues. Find solutions for streaming problems, recording issues, audio problems, performance, and more.

---

## 📋 Table of Contents

1. [Installation Issues](#installation-issues)
2. [Permission Issues](#permission-issues)
3. [Streaming Issues](#streaming-issues)
4. [Recording Issues](#recording-issues)
5. [Audio Issues](#audio-issues)
6. [Performance Issues](#performance-issues)
7. [Scene & Source Issues](#scene--source-issues)
8. [Platform-Specific Issues](#platform-specific-issues)
9. [VTuber Issues](#vtuber-issues)
10. [Network Issues](#network-issues)

---

## 📥 Installation Issues

### ❌ "App not installed" Error

**Problem**: Installation fails with "App not installed" message

**Possible Causes**:
- Not enough storage space
- Corrupted APK file
- Incompatible Android version
- Installation folder permissions issue

**Solutions**:
1. **Check Storage Space**
   - Go to Settings → Storage
   - Ensure at least 500MB free space available
   - Delete unnecessary apps/files if needed

2. **Re-download APK**
   - Clear Downloads cache
   - Visit [livelens.live](https://www.livelens.live/)
   - Download fresh APK file

3. **Verify Android Version**
   - Go to Settings → About Phone
   - Check Android version is 10 or higher
   - Update if older version

4. **Try Alternative Installation**
   - Use File Manager instead of browser
   - Or use ADB (Android Debug Bridge) if technical

---

### ❌ "Unknown Sources" Permission Denied

**Problem**: Can't find or enable "Unknown Sources" permission

**Solutions**:
1. **On Android 10-11**:
   - Settings → Security → Unknown Sources
   - Toggle ON for your file manager

2. **On Android 12+**:
   - Settings → Apps and Notifications
   - Find your file manager or browser
   - Tap → Permissions → Install unknown apps
   - Toggle ON

3. **Alternative Method**:
   - Use built-in Files app (pre-enabled usually)
   - Download APK using Files app
   - Tap to install directly

---

### ❌ "Insufficient Storage" Error

**Problem**: Installation says not enough storage despite free space showing

**Solutions**:
1. **Clear Cache**
   - Settings → Apps → LiveLens (if installed)
   - Storage → Clear Cache
   - Restart device

2. **Free Up Space**
   - Delete old recordings
   - Clear browser cache
   - Uninstall unused apps
   - Move photos/videos to cloud storage

3. **Try SD Card** (if supported)
   - Some devices allow app installation on SD card
   - Settings → Storage → Preferred location

---

### ❌ App Crashes During Installation

**Problem**: Installation completes but app won't open

**Solutions**:
1. **Restart Device**
   - Power off phone completely
   - Wait 30 seconds
   - Turn back on

2. **Clear App Data**
   - Settings → Apps → LiveLens
   - Storage → Clear Cache & Clear Data
   - Reinstall app

3. **Update System**
   - Check for Android OS updates
   - Settings → About Phone → System Update
   - Install if available

4. **Reinstall**
   - Uninstall LiveLens
   - Restart device
   - Reinstall fresh APK

---

## 🔒 Permission Issues

### ❌ Camera Not Working

**Problem**: Camera source shows black screen or won't enable

**Solutions**:
1. **Grant Camera Permission**
   - Settings → Apps → LiveLens → Permissions
   - Tap Camera → Allow

2. **Check if Camera is Blocked**
   - Close other camera apps
   - Restart LiveLens
   - Try again

3. **Test Camera**
   - Open default Camera app
   - If default camera fails, hardware issue
   - Try different camera (front/back)

4. **Restart Services**
   - Go to Settings → Apps
   - Find Camera service
   - Force stop
   - Restart device

5. **Camera Permission Cache**
   - Settings → Apps → LiveLens
   - Uninstall
   - Reinstall
   - Grant permissions on first launch

---

### ❌ Microphone Not Capturing Audio

**Problem**: Microphone source shows 0 dB or no audio

**Solutions**:
1. **Grant Microphone Permission**
   - Settings → Apps → LiveLens → Permissions
   - Tap Microphone → Allow

2. **Check Microphone Hardware**
   - Try voice recording app
   - If voice recorder fails, microphone issue
   - Try external microphone

3. **Microphone Muted**
   - Check physical mute switch (if present)
   - Go to LiveLens audio settings
   - Ensure microphone is not muted

4. **Audio Input Source**
   - Go to Settings → Streaming → Audio
   - Verify microphone is selected as input
   - Check "Microphone" toggle is ON

5. **Restart Audio Service**
   - Restart device
   - Restart LiveLens
   - Test microphone again

---

### ❌ Can't Save/Record Files

**Problem**: "Permission denied" when trying to save recordings

**Solutions**:
1. **Grant Storage Permission**
   - Settings → Apps → LiveLens → Permissions
   - Tap Storage/Files → Allow

2. **Check Storage Location**
   - Settings → Apps → LiveLens → Storage
   - Verify correct storage location selected
   - Ensure it's writable

3. **On Android 11+**
   - Some apps need "All Files Access"
   - Settings → Apps → Special app access
   - All Files Access
   - Enable LiveLens

4. **Free Up Storage**
   - Ensure at least 1GB free space
   - Delete old recordings
   - Move files to cloud or PC

5. **SD Card Issues**
   - If using SD card, ensure it's:
     - Properly mounted
     - Not full
     - Not corrupted

---

### ❌ Overlay Permission Denied

**Problem**: "Draw over other apps" permission missing

**Solutions**:
1. **Enable Overlay Permission**
   - Settings → Apps → Special app access
   - Appear on top/Draw over other apps
   - Find LiveLens → Enable

2. **On Different Android Versions**
   - Android 9-10: Settings → Apps → Permissions
   - Android 11-12: Settings → Display Overlay
   - Android 13+: Settings → All apps → Permissions

---

## 📡 Streaming Issues

### ❌ "Connection Failed" Error

**Problem**: Can't connect to streaming platform

**Solutions**:
1. **Check Internet Connection**
   - Open browser, visit google.com
   - If no internet, connect to WiFi or mobile data
   - Restart modem/router

2. **Verify RTMP URL**
   - Double-check RTMP URL spelling
   - Copy-paste from official source
   - Ensure no extra spaces

3. **Test Upload Speed**
   - Use speedtest.net on browser
   - Need 10+ Mbps upload speed
   - If slower, wait for better connection

4. **Firewall/Port Issue**
   - RTMP uses port 1935
   - May be blocked by network/router
   - Try WiFi instead of mobile data (or vice versa)
   - Contact ISP if port is blocked

5. **Platform Server Down**
   - Check platform status page:
     - YouTube: [status.youtube.com](https://status.youtube.com/)
     - Twitch: [status.twitch.tv](https://status.twitch.tv/)
     - Facebook: [developers.facebook.com/status](https://developers.facebook.com/status)

6. **Stream Key Invalid/Expired**
   - Get fresh stream key from platform
   - Update in LiveLens settings
   - Try connecting again

---

### ❌ Stream Keeps Disconnecting

**Problem**: Stream starts but disconnects after a few seconds/minutes

**Solutions**:
1. **Reduce Bitrate**
   - Lower by 1-2 Mbps
   - Example: 5 Mbps → 3-4 Mbps
   - Go to Settings → Streaming → Bitrate

2. **Lower Resolution**
   - Change from 1080p to 720p
   - Or 720p to 480p
   - Reconnect and try again

3. **Reduce FPS**
   - Change from 60 FPS to 30 FPS
   - Settings → Streaming → FPS

4. **Network Stability**
   - Move closer to WiFi router
   - Reduce distance/obstacles
   - Use 5GHz WiFi if available
   - Or switch to mobile data

5. **Close Background Apps**
   - Pause sync services
   - Close video players
   - Close browsers
   - Free up bandwidth

6. **Restart Router**
   - Power off WiFi router
   - Wait 30 seconds
   - Power back on
   - Reconnect to LiveLens

7. **Check Network Failover**
   - If on WiFi + mobile data, one may interfere
   - Disable mobile data or WiFi (not both)
   - Choose one primary connection

---

### ❌ Low Bitrate Warning

**Problem**: "Bitrate low" or "Network unstable" warning appears

**Solutions**:
1. **Immediate Action**
   - Move closer to WiFi
   - Switch to different network
   - Lower your set bitrate proactively

2. **Optimize Network**
   - Close all other apps using internet
   - Turn off auto-sync apps
   - Disable background app refresh
   - Settings → Battery → App Battery Usage

3. **Check Current Speed**
   - Open speedtest.net
   - Run speed test
   - Note upload speed
   - Ensure it's above your set bitrate

4. **Upgrade Connection**
   - Ask ISP for higher bandwidth
   - Move to area with better signal
   - Use wired connection if possible

5. **Reduce Quality**
   - Lower bitrate automatically by app
   - Reduce FPS or resolution
   - Accept lower quality for stability

---

### ❌ Stream Quality is Pixelated/Blurry

**Problem**: Video appears blocky or very blurry on platform

**Solutions**:
1. **Increase Bitrate**
   - Go to Settings → Streaming
   - Increase bitrate by 1-2 Mbps
   - Example: 3 Mbps → 5 Mbps

2. **Increase Resolution**
   - Change from 720p to 1080p
   - If device supports it

3. **Improve Network**
   - Move to WiFi (better than mobile)
   - Check upload speed (speedtest)
   - Ensure 10+ Mbps available

4. **Reduce FPS if Necessary**
   - Sometimes 30 FPS at high bitrate > 60 FPS at low bitrate
   - Try: 1080p 30 FPS vs 1080p 60 FPS

5. **Encoder Settings**
   - Try H.264 (more compatible, better quality)
   - H.265 (smaller file, less compatible)

---

### ❌ Chat Not Appearing

**Problem**: Live chat not showing or updating

**Solutions**:
1. **Refresh Chat**
   - Swipe down on chat area
   - Wait a few seconds
   - Chat should update

2. **Restart App**
   - Close LiveLens completely
   - Reopen app
   - Chat should connect

3. **Check Platform Status**
   - Verify platform's chat is working
   - Try opening chat on web browser
   - If web chat down, platform issue

4. **Permission Issue**
   - Ensure you have chat reading permission
   - Verify account is verified (some platforms)
   - Check moderation status

5. **Chat May Be Disabled**
   - Platform might have disabled chat
   - Check stream settings on web
   - Re-enable if needed

---

### ❌ Viewers Can't See Me

**Problem**: Stream appears online but viewers see black screen

**Solutions**:
1. **Verify Scene is Active**
   - Ensure scene is selected (highlighted)
   - Go Live button should be available
   - Check if you actually tapped "Go Live"

2. **Camera Permission**
   - Verify camera permission is granted
   - Check camera isn't being used by another app
   - Try switching camera (front/back)

3. **Scene Has No Sources**
   - Your scene might be empty
   - Add camera or image source
   - Ensure source is visible (not hidden)

4. **Test Connection First**
   - Always test connection before going live
   - Settings → Streaming → Test Connection
   - If test fails, fix issue before streaming

5. **Preview Not Shown**
   - Make sure live preview works locally
   - If black locally, viewers see black
   - Fix scene/camera issues first

---

## 🎬 Recording Issues

### ❌ Recording Not Starting

**Problem**: "Record" button doesn't work or recording won't start

**Solutions**:
1. **Check Storage Permission**
   - Settings → Apps → LiveLens → Permissions
   - Grant Storage/Files permission
   - Restart app

2. **Sufficient Storage Space**
   - Go to Settings → Storage
   - Ensure at least 2GB free space
   - Delete old recordings if full

3. **Recording Format Issue**
   - Some devices have codec limitations
   - Go to Settings → Recording
   - Try different resolution/bitrate

4. **Microphone Permission**
   - Some devices need microphone permission for recording
   - Grant microphone permission
   - Retry recording

---

### ❌ Recording Stops Unexpectedly

**Problem**: Recording starts but stops after a few seconds/minutes

**Solutions**:
1. **Storage Full**
   - Recording stopped due to full storage
   - Delete old files
   - Free up space
   - Resume recording

2. **Overheating**
   - Device got too hot
   - Stop recording
   - Let device cool down
   - Try again in 10 minutes

3. **Memory Pressure**
   - RAM is full from other apps
   - Close unnecessary apps
   - Restart device
   - Retry recording

4. **File System Error**
   - Try recording to different location
   - Or use different storage (SD card)
   - Restart device

---

### ❌ Recording Quality is Poor

**Problem**: Recorded video is choppy, pixelated, or has audio sync issues

**Solutions**:
1. **Reduce Recording Bitrate**
   - Settings → Recording → Bitrate
   - Lower bitrate for older devices
   - Example: 10 Mbps → 5 Mbps

2. **Lower Resolution**
   - Change from 1080p to 720p
   - For better performance

3. **Close Background Apps**
   - Free up RAM and CPU
   - Close YouTube, browsers, etc.
   - Restart device if necessary

4. **Use External Storage**
   - If using phone storage, try SD card
   - SD card might be faster

5. **Reduce FPS**
   - Change from 60 to 30 FPS
   - 30 FPS at high quality > 60 FPS at low quality

---

### ❌ Can't Find Recorded File

**Problem**: Recording completed but can't find the file

**Solutions**:
1. **Check Default Recording Folder**
   - Settings → Storage/Files
   - Note recording location
   - Open file manager to that location

2. **Common Locations**
   - Internal Storage → DCIM → LiveLens
   - Internal Storage → Documents → LiveLens
   - Internal Storage → Movies → LiveLens
   - SD Card (if configured)

3. **Search for File**
   - Open file manager
   - Search for `.mp4` files
   - Sort by date (newest first)

4. **Check Permissions**
   - May be saved but permission blocked
   - Grant file access permission
   - Restart app

5. **Wrong Recording Setting**
   - Verify recording was actually enabled
   - Check Settings → Recording is ON

---

### ❌ Video File Corrupted

**Problem**: Recorded video won't play or is incomplete

**Solutions**:
1. **Restart Device**
   - Sometimes file system needs reset
   - Power off/on device
   - Try playing file again

2. **Use Different Player**
   - Try VLC Media Player
   - Try Google Play Movies
   - Some players handle corrupted files better

3. **Check File Size**
   - If file size is tiny (< 1MB for 10 min recording)
   - Recording probably failed
   - Re-record with more storage space

4. **Recording Was Interrupted**
   - If you force-closed app during recording
   - File may be incomplete
   - This cannot be recovered
   - Use stable recording settings next time

5. **Storage Corruption**
   - If multiple files corrupted
   - Try different storage location
   - Restart device
   - Check SD card health if using SD

---

## 🎤 Audio Issues

### ❌ No Audio in Stream

**Problem**: Audio completely missing from stream or recording

**Solutions**:
1. **Microphone Permission**
   - Settings → Apps → LiveLens → Permissions
   - Grant Microphone permission
   - Restart app

2. **Microphone Muted**
   - Check audio icon in scene editor
   - Ensure microphone toggle is ON
   - Try unmuting

3. **Wrong Audio Source**
   - Go to Settings → Audio Input
   - Select "Microphone" option
   - Or "Microphone + System Audio"

4. **Audio Hardware Issue**
   - Open Voice Recorder app
   - Try recording with default app
   - If no audio there, microphone issue
   - Try external microphone

5. **Test Audio**
   - Go to Settings → Audio Test
   - Speak into microphone
   - Check if meters move
   - If no movement, no audio detected

---

### ❌ Audio is Very Quiet

**Problem**: Audio level too low even at max volume

**Solutions**:
1. **Increase Microphone Gain**
   - Settings → Audio → Microphone Gain
   - Increase to 80-100%
   - Test and adjust

2. **Move Microphone Closer**
   - Speak closer to device mic
   - About 6-12 inches away
   - Avoid background noise

3. **Use External Microphone**
   - Built-in mic may be weak
   - Use 3.5mm headset mic
   - Or Bluetooth microphone

4. **Reduce Noise Suppression**
   - Settings → Audio → Noise Suppression
   - If too aggressive, reduces overall volume
   - Lower or disable

5. **Check Audio Meter**
   - Real-time audio meter should show levels
   - If always at bottom, mic is very quiet
   - Adjust gain or get better microphone

---

### ❌ Audio is Too Loud/Distorted

**Problem**: Audio clipping or distorting, even at low volume

**Solutions**:
1. **Reduce Microphone Gain**
   - Settings → Audio → Microphone Gain
   - Lower from 100% to 50-70%
   - Test

2. **Reduce System Audio Level**
   - Settings → Audio → System Audio Volume
   - Lower the slider
   - Balance with mic audio

3. **Move Microphone Away**
   - Speak further from device (12-24 inches)
   - Avoid yelling directly into mic

4. **Use Noise Gate**
   - Settings → Audio → Noise Gate
   - Prevents silent parts from boosting volume
   - Helps with distortion

5. **Check Platform Settings**
   - Some platforms auto-amplify audio
   - Lower stream audio in Settings
   - Reduce overall bitrate for audio

---

### ❌ Audio Delay/Sync Issues

**Problem**: Audio and video not synced, audio lags behind video

**Solutions**:
1. **Audio Sync Setting**
   - Settings → Audio → Audio Sync Delay
   - Adjust if option available
   - Usually 0ms default

2. **Lower Bitrate**
   - Sometimes sync issues at very high bitrate
   - Reduce bitrate by 1-2 Mbps
   - Retry

3. **Reduce FPS**
   - Change from 60 to 30 FPS
   - Sometimes helps with sync

4. **Network Issue**
   - Sync issues often = network lag
   - Ensure stable 10+ Mbps connection
   - Move to better WiFi

5. **Platform Buffering**
   - This might be platform buffering, not LiveLens issue
   - Check raw stream locally (preview works?)
   - If local preview synced, platform is buffering

---

### ❌ Background Noise/Echo

**Problem**: Lots of background noise or echo in audio

**Solutions**:
1. **Enable Noise Suppression**
   - Settings → Audio → Noise Suppression
   - Toggle ON
   - Test

2. **Enable Echo Cancellation**
   - Settings → Audio → Echo Cancellation
   - Toggle ON
   - Helps if speakers nearby

3. **Reduce Noise Gate Threshold**
   - Settings → Audio → Noise Gate
   - Lower threshold to filter more noise
   - Too aggressive might cut voice

4. **Move Away from Noise Sources**
   - Avoid fans, AC units, traffic noise
   - Soundproof your space if possible
   - Use directional microphone

5. **External Microphone**
   - USB/Bluetooth mics often better noise handling
   - Position away from noise sources
   - Better audio path = less noise

---

### ❌ System Audio Not Capturing

**Problem**: Can't hear game/music audio in stream

**Solutions**:
1. **Enable System Audio**
   - Settings → Audio → System Audio
   - Toggle ON
   - Choose "Microphone + System Audio"

2. **Check Android Version**
   - System audio capture requires Android 10+
   - On older versions, not available
   - Update Android if possible

3. **Audio Source Permission**
   - Some apps require special permission
   - Go to Settings → Apps
   - Find app using audio
   - Grant audio capture permission

4. **Volume Level Check**
   - Go to Settings → Audio → System Audio Level
   - Increase if too low
   - Balance with microphone

5. **Test System Audio**
   - Play music or YouTube video
   - Check audio meter
   - Should show levels when audio playing
   - If no level, system audio not working

---

## ⚡ Performance Issues

### ❌ App is Laggy/Slow

**Problem**: App feels slow, interface lags, menus are slow to respond

**Solutions**:
1. **Close Background Apps**
   - Open Recent Apps
   - Swipe to close all other apps
   - Leave only LiveLens open
   - Restart app

2. **Clear App Cache**
   - Settings → Apps → LiveLens
   - Storage → Clear Cache (not data)
   - Restart app

3. **Reduce Quality Settings**
   - Settings → Streaming → Resolution
   - Lower to 720p (from 1080p)
   - Reduce FPS to 30 (from 60)

4. **Check RAM Usage**
   - Settings → About Phone → Memory
   - If using 90%+ of RAM, phone is full
   - Close apps
   - Restart device

5. **Restart Device**
   - Power off completely
   - Wait 30 seconds
   - Power back on
   - Try again

---

### ❌ FPS Dropping During Stream

**Problem**: Stream shows 30-40 FPS instead of set 60 FPS

**Solutions**:
1. **Close Background Apps**
   - Every open app uses resources
   - Close all except LiveLens
   - Free up CPU/GPU

2. **Lower FPS Setting**
   - Accept 30 FPS instead of forcing 60 FPS
   - 30 FPS consistently > 60 FPS inconsistent
   - Go to Settings → Streaming → FPS

3. **Reduce Resolution**
   - 720p 60 FPS > 1080p 30 FPS
   - Lower resolution allows more FPS
   - Settings → Streaming → Resolution

4. **Reduce Scene Complexity**
   - Too many sources = more GPU load
   - Remove unnecessary sources
   - Simplify scene

5. **Check Device Temperature**
   - Device might be thermal throttling
   - Touch back of device
   - If very hot, let it cool
   - FPS recovers when cool

---

### ❌ CPU/GPU Overheating

**Problem**: Device gets very hot, performance drops

**Solutions**:
1. **Stop Streaming/Recording**
   - Pause stream immediately
   - Let device cool down (10-15 minutes)
   - Resume after cooling

2. **Reduce Quality**
   - Lower resolution (1080p → 720p)
   - Lower FPS (60 → 30)
   - Lower bitrate (5 → 3 Mbps)

3. **Improve Ventilation**
   - Remove phone case if ventilated
   - Use external fan if available
   - Avoid direct sunlight
   - Stream in cooler environment

4. **Close Other Apps**
   - Every app generates heat
   - Close browsers, YouTube, etc.
   - More resources for LiveLens = less heat

5. **Reduce Scene Complexity**
   - Complex scenes use more GPU
   - Remove filters/effects
   - Use simpler overlays

---

### ❌ Battery Draining Quickly

**Problem**: Battery depletes very fast during streaming/recording

**Solutions**:
1. **Use Lower Quality**
   - Lower FPS = less CPU = less battery drain
   - Reduce resolution
   - Reduce bitrate

2. **Enable Battery Saver Mode**
   - Settings → Battery → Battery Saver
   - Toggle ON
   - May reduce performance slightly

3. **Keep Device Plugged In**
   - Use USB-C charger while streaming
   - Prevents battery depletion
   - Better long streams

4. **Close Background Apps**
   - Reduce CPU usage
   - Stops background refresh
   - Saves battery

5. **Reduce Screen Brightness**
   - Automatic brightness if available
   - Lower manual brightness if needed
   - Screen is biggest battery drain

6. **Reduce Recording**
   - Recording + streaming = high drain
   - Choose one or lower quality
   - Record at 720p 30 FPS instead of 1080p 60 FPS

---

### ❌ App Crashes During Stream

**Problem**: App suddenly closes/crashes while streaming

**Solutions**:
1. **Update App**
   - May have crash bug in current version
   - Visit [livelens.live](https://www.livelens.live/)
   - Download latest version
   - Install over existing

2. **Clear App Data**
   - Settings → Apps → LiveLens
   - Storage → Clear Data
   - This removes all settings/scenes
   - Reinstall app fresh

3. **Reduce Quality**
   - Crash might be due to high resource usage
   - Lower FPS, resolution, bitrate
   - Try again

4. **Close Background Apps**
   - Low RAM causes crashes
   - Close everything
   - Keep only LiveLens open

5. **Check Logs** (if available)
   - Go to Settings → Debug/Logs
   - Note any error messages
   - Report to support with logs

---

## 🎬 Scene & Source Issues

### ❌ Source Not Appearing

**Problem**: Added source but doesn't show on canvas

**Solutions**:
1. **Source is Hidden**
   - Tap the eye icon next to source
   - Toggle to show (eye should be open)
   - Source should appear

2. **Source is Outside Canvas**
   - Drag source to visible area
   - Pinch to zoom if very small

3. **Source Layer Issue**
   - Layers stack on top of each other
   - If source behind another, won't see it
   - Tap source to bring to front
   - Or reorder layers

4. **Permission Missing**
   - Some sources need permissions
   - Camera needs camera permission
   - Gallery image needs storage permission

5. **Remove and Re-add**
   - Delete the source
   - Add it again fresh
   - Configure properly

---

### ❌ Can't Edit Source

**Problem**: Source won't let you edit or move it

**Solutions**:
1. **Source is Locked**
   - Tap lock icon next to source
   - Unlock it
   - Now you can edit

2. **Selected Wrong Source**
   - Make sure you tapped the correct source
   - It should be highlighted
   - Try again

3. **Tap the Source Directly**
   - Some sources need direct tap to select
   - Tap on canvas where source is
   - Then adjust

---

### ❌ Scene Won't Save

**Problem**: Created scene but when exit, scene is gone

**Solutions**:
1. **Tap Save Explicitly**
   - Tap "Save" button or back button
   - Should prompt to save
   - Confirm save

2. **Insufficient Storage**
   - Check if storage is full
   - Free up space
   - Try saving again

3. **Restart App**
   - Close and reopen LiveLens
   - Scene should be there

4. **Scene is Actually Saved**
   - Check Scenes list
   - Your scene might be there but not showing
   - Swipe left to see all scenes

---

### ❌ Duplicate Scene Won't Work

**Problem**: Can't duplicate or copy scene

**Solutions**:
1. **Try Manual Copy**
   - Create new scene
   - Add same sources manually
   - Manually position
   - Save

2. **Restart App**
   - Close and reopen LiveLens
   - Try duplicating again

3. **Free Up Storage**
   - Duplicating needs space
   - Free up 100MB+
   - Try again

---

## 🌐 Platform-Specific Issues

### YouTube Issues

**❌ "YouTube account not recognized"**
- Logout and login again
- Settings → Accounts → YouTube → Logout
- Then login fresh

**❌ "Schedule not showing"**
- Go to YouTube Studio (web browser)
- Verify streams are actually scheduled
- Refresh LiveLens app
- If still not showing, check you have creator account (not regular account)

**❌ "Stream goes offline immediately"**
- Check RTMP URL is current
- Get fresh stream key
- Verify internet connection

---

### Twitch Issues

**❌ "Couldn't verify Twitch account"**
- Logout: Settings → Accounts → Twitch → Logout
- Login again with correct credentials
- Ensure you have two-factor auth if required

**❌ "No games showing in category"**
- Try typing game name manually
- Or leave category blank
- Twitch will auto-categorize

**❌ "Stream says offline on Twitch"**
- Verify stream key hasn't changed
- Check connection test passes
- Restart app and try again

---

### Facebook Issues

**❌ "Can't select page"**
- Ensure you're admin of the page
- Logout and login fresh
- Try again

**❌ "Stream quality bad on Facebook"**
- Facebook may throttle based on load
- Lower bitrate slightly
- Try streaming during off-peak hours

**❌ "Can't save stream video"**
- Go to Facebook page (web browser)
- Find your livestream
- Manually save if needed
- Facebook auto-saves some streams

---

### Custom RTMP Issues

**❌ "Connection refused"**
- RTMP server might be offline
- Verify server address is correct
- Try different RTMP service
- Check port 1935 not blocked

**❌ "Authentication failed"**
- Verify stream key is correct
- No extra spaces
- Check key hasn't expired
- Get new key if needed

**❌ "No video showing on platform"**
- Test your RTMP setup on web browser first
- If web streaming works, issue is local
- Verify resolution/bitrate compatible
- Try lower bitrate

---

## 👾 VTuber Issues

### ❌ Live2D Model Not Loading

**Problem**: Model file won't load or appears blank

**Solutions**:
1. **Check Model Format**
   - LiveLens supports Cubism up to v5.1
   - Verify model is correct format
   - Try different model if available

2. **Verify File Path**
   - Ensure model file is in correct location
   - Path should be accessible
   - Try copying model to Documents

3. **Permissions Issue**
   - Grant storage permission
   - Verify access to model files
   - Try different storage location

4. **Restart App**
   - Close LiveLens
   - Reopen
   - Try loading model again

---

### ❌ Model Animations Not Working

**Problem**: VTuber model is static, no animations or expressions

**Solutions**:
1. **Check Animation Settings**
   - Settings → VTuber → Animations
   - Ensure "Auto Animate" is ON
   - Check if idle animation enabled

2. **Microphone Not Detected**
   - Lip-sync needs microphone
   - Verify microphone permission granted
   - Test microphone in audio settings

3. **Physics Simulation Off**
   - Settings → VTuber → Physics
   - Toggle ON
   - Animations should play

4. **Update Model**
   - Model might be outdated
   - Try newer version if available

---

### ❌ Model Tracking Not Working

**Problem**: Touch tracking or gesture detection not responding

**Solutions**:
1. **Check Tracking Permission**
   - Settings → VTuber → Tracking
   - Ensure permission is granted

2. **Screen Touch Not Detected**
   - Try tapping directly on model
   - Make sure hand tracking is enabled
   - Model should respond to touch

3. **Calibrate Model**
   - Some models need calibration
   - Settings → VTuber → Calibrate
   - Follow on-screen instructions

4. **Model Incompatibility**
   - Model might not support tracking
   - Check model documentation
   - Try different model

---

### ❌ Lip-Sync Not Synced

**Problem**: Model's mouth doesn't sync with microphone audio

**Solutions**:
1. **Microphone Input**
   - Check microphone is working
   - Speak clearly toward device
   - Audio meter should show levels

2. **Adjust Sensitivity**
   - Settings → VTuber → Lip-Sync Sensitivity
   - Increase if not detecting speech
   - Test

3. **Audio Delay**
   - Settings → VTuber → Audio Delay
   - Adjust sync delay
   - Small increments (10ms at a time)

4. **Model Configuration**
   - Some models need parameter tuning
   - Check model settings
   - Adjust mouth movement intensity

---

### ❌ Expression/Parameter Changes Not Working

**Problem**: Can't change facial expressions or model parameters

**Solutions**:
1. **Parameter Editor**
   - Settings → VTuber → Parameter Editor
   - Find your expression parameter
   - Adjust slider to test

2. **Model Support**
   - Not all models support all expressions
   - Check model documentation
   - Some only support basic expressions

3. **Expression Binding**
   - Verify expressions are bound to correct parameters
   - Settings → VTuber → Expressions
   - Rebind if needed

4. **Model Reload**
   - Restart app
   - Reload model
   - Try changing expression again

---

## 🌐 Network Issues

### ❌ WiFi Keeps Disconnecting

**Problem**: WiFi drops repeatedly during stream

**Solutions**:
1. **Move Closer to Router**
   - WiFi signal weaker far away
   - Move to same room as router
   - Reduce walls/obstacles between

2. **Use 5GHz WiFi**
   - Settings → WiFi
   - Select 5GHz network if available
   - Better for streaming than 2.4GHz

3. **Restart Router**
   - Power off WiFi router
   - Wait 30 seconds
   - Power back on
   - Reconnect

4. **Check WiFi Password**
   - Ensure you're on correct WiFi
   - Sometimes phone auto-switches networks
   - Forget and reconnect to preferred network

5. **Router Issue**
   - Try connecting other devices
   - If other devices also disconnect, router problem
   - Contact ISP or replace router

---

### ❌ Mobile Data Connection Unstable

**Problem**: Mobile data keeps cutting out or very slow

**Solutions**:
1. **Check Signal Strength**
   - Top of screen shows signal bars
   - If less than 2 bars, signal weak
   - Move to better reception area

2. **Switch to WiFi**
   - WiFi usually more stable than mobile data
   - Connect to nearby WiFi if available

3. **Restart Mobile Connection**
   - Toggle Airplane Mode on then off
   - Wait 10 seconds between toggles
   - Should reset connection

4. **Check Data Plan**
   - Verify you have active mobile data plan
   - Contact carrier if needed

5. **Contact Carrier**
   - If repeatedly unstable
   - May be network issue in your area
   - Carrier can help troubleshoot

---

### ❌ High Ping/Latency

**Problem**: Stream latency is very high (5+ seconds delay)

**Solutions**:
1. **Latency is Normal**
   - Up to 5 seconds delay is typical
   - This is RTMP protocol delay
   - YouTube/Twitch adds 3-5 seconds

2. **Reduce Bitrate**
   - High bitrate can increase latency
   - Lower bitrate by 1-2 Mbps
   - Try again

3. **Reduce Resolution**
   - 1080p encoding takes longer
   - Try 720p for lower latency
   - Trade quality for lower delay

4. **Switch Encoder**
   - H.264 generally faster than H.265
   - Settings → Streaming → Encoder
   - Try H.264

5. **Better Internet**
   - Very low speed internet increases latency
   - Ensure 10+ Mbps upload speed
   - Better connection = lower latency

---

## 🛠️ General Troubleshooting Steps

### Before Asking for Help:

1. **Restart App**
   - Close LiveLens completely
   - Reopen app
   - Try again

2. **Restart Device**
   - Power off device
   - Wait 30 seconds
   - Power back on

3. **Check Internet**
   - Open browser
   - Try visiting google.com
   - Ensure internet working

4. **Update App**
   - Go to [livelens.live](https://www.livelens.live/)
   - Download latest version
   - Install over existing app

5. **Clear Cache**
   - Settings → Apps → LiveLens
   - Storage → Clear Cache
   - Restart app

6. **Free Up Resources**
   - Close all other apps
   - Clear RAM if possible
   - Disable background processes

---

## 📞 Still Having Issues?

If you've tried everything above:

1. **Check FAQ** → [FAQ Guide](/wiki/FAQ)

2. **Community Help** → [GitHub Discussions](https://github.com/ByconStudio/LiveLens/discussions)

3. **Discord Support** → [Join Discord](https://discord.gg/kUqmbKhs6w)

4. **Report Bug** → [Report Issue](https://github.com/ByconStudio/LiveLens/issues/new)

5. **Email Support** → [support@livelens.live](mailto:support@livelens.live)

**When reporting:**
- Include device model and Android version
- Describe exactly what went wrong
- Steps to reproduce issue
- Any error messages seen
- What you've already tried

---

**Happy Troubleshooting! 🚀**

Made with ❤️ by **ByconStudio**