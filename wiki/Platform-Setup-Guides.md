# 🌐 Platform Setup Guides

Complete guides for setting up LiveLens with your favorite streaming platforms. LiveLens supports **multi-stream** capability, so you can stream to multiple platforms simultaneously!

---

## 📋 Table of Contents

1. [Multi-Stream Setup](#multi-stream-setup)
2. [YouTube Live Setup](#youtube-live-setup)
3. [Twitch Setup](#twitch-setup)
4. [Facebook Live Setup](#facebook-live-setup)
5. [Custom RTMP Setup](#custom-rtmp-setup)
6. [Comparison Table](#platform-comparison)

---

## 🔄 Multi-Stream Setup

**Stream to multiple platforms at the same time!**

### Enable Multi-Stream

1. Open **LiveLens** app
2. Tap **⚙️ Settings**
3. Go to **Accounts** tab
4. Find **"Multi-Stream"** option
5. Toggle **ON** ✅

### Add Multiple Platforms

Once Multi-Stream is enabled:

1. Go to **Settings → Accounts**
2. Tap **"Add Account"** or **"Add Stream"**
3. Select the platform you want to add:
   - YouTube
   - Twitch
   - Facebook
   - Custom RTMP

4. Complete the login/setup for each platform
5. All platforms will now stream simultaneously

### Multi-Stream Advantages

✅ Reach more audiences at once
✅ One stream, multiple platforms
✅ Save time - no need to stream separately
✅ Cross-platform presence

### ⚠️ Bandwidth Consideration

When streaming to multiple platforms:
- **2 Platforms**: 8-10 Mbps upload needed
- **3 Platforms**: 12-15 Mbps upload needed
- **4+ Platforms**: 15+ Mbps upload needed

> **Tip**: If you don't have enough bandwidth, lower your bitrate or resolution

---

## 📺 YouTube Live Setup

### Option 1: Login with Google Account

#### Step 1: Login to YouTube

1. Open **LiveLens** app
2. Tap **⚙️ Settings**
3. Go to **Accounts** tab
4. Tap **"Add YouTube Account"** or **"YouTube"**
5. Tap **"Sign In with Google"**
6. Complete Google authentication

#### Step 2: Access Your Schedules

Once logged in:
1. Go to **Settings → Accounts → YouTube**
2. Tap **"Your Schedules"** or **"Scheduled Streams"**
3. **All your scheduled streams from YouTube Studio will appear** 📅

#### Step 3: Select a Scheduled Stream

1. Browse your scheduled streams
2. Tap the stream you want to go live with
3. LiveLens will auto-fill:
   - Stream title
   - Description
   - Thumbnail (if set)
   - RTMP URL
   - Stream key

#### Step 4: Customize Your Stream

- ✏️ Edit title if needed
- 📝 Add stream description
- 🎨 Add custom overlays
- 🎬 Select your scene

#### Step 5: Go Live

1. Tap **"Go Live"** button
2. Your stream will start immediately
3. YouTube viewers will see your live stream

#### Step 6: Monitor Your Stream

- 👥 View live viewer count
- 💬 Check live chat (if enabled)
- 📊 Watch bitrate and FPS metrics
- 🎚️ Adjust audio levels in real-time

---

### Option 2: Use Custom RTMP (Without Login)

Don't want to login? You can still stream to YouTube using manual RTMP:

#### Get Your YouTube RTMP Details

1. Go to **YouTube Studio** (on computer)
2. Click **"Create"** → **"Go Live"**
3. Select **"Stream"** (left menu)
4. Copy:
   - **Stream URL** (RTMP server)
   - **Stream Key**
5. Keep these handy

#### Setup in LiveLens

1. Open **LiveLens**
2. Go to **Settings → Accounts**
3. Select **"Custom RTMP"** or **"Add Custom Stream"**
4. Paste your:
   - **RTMP URL** from YouTube
   - **Stream Key** from YouTube
5. Set stream details:
   - Title
   - Resolution (1080p recommended)
   - FPS (60 or 30)
   - Bitrate (4-5 Mbps recommended)

#### Go Live

1. Tap **"Go Live"**
2. Your stream starts on YouTube
3. You won't see chat/analytics in-app, but stream works perfectly

---

## 🎮 Twitch Setup

### Step 1: Login to Twitch

1. Open **LiveLens** app
2. Go to **Settings → Accounts**
3. Tap **"Add Twitch Account"** or **"Twitch"**
4. Tap **"Sign In with Twitch"**
5. Complete Twitch authentication
6. Grant permissions when asked

### Step 2: Access Your Twitch Settings

Once logged in:
1. Go to **Settings → Accounts → Twitch**
2. You'll see your Twitch profile info:
   - Channel name
   - Follower count
   - Verified status (if applicable)

### Step 3: Customize Your Stream

Before going live, you can customize:

#### Stream Title
- Tap **"Edit Stream Title"**
- Enter your broadcast title
- Example: "Chill Gaming Session 🎮"

#### Stream Category
- Select your game/category
- Twitch will categorize your stream
- Helps viewers find your content

#### Stream Language
- Choose broadcast language
- Important for discoverability

#### Tags
- Add relevant tags
- Helps with search and recommendations

#### Mature Content
- Toggle if your stream has mature content
- Set viewer restrictions if needed

### Step 4: Configure Stream Quality

1. Go to **Settings → Streaming**
2. Set your preferred quality:
   - **Resolution**: 1080p (if 60 FPS supported) or 720p
   - **FPS**: 60 (recommended) or 30
   - **Bitrate**: 4-6 Mbps (higher = better quality)
   - **Encoder**: H.264 (recommended)

### Step 5: Go Live on Twitch

1. Select your scene
2. Tap **"Go Live"** button
3. Your stream starts on Twitch
4. You can monitor:
   - Live viewer count
   - Chat messages
   - Bitrate metrics

### Step 6: Monitor During Stream

- 👥 Check concurrent viewers
- 💬 Read and respond to chat
- 📊 Watch CPU/bandwidth usage
- 🎚️ Adjust settings in real-time

### Step 7: End Your Stream

1. Tap **"Stop"** button
2. Stream ends on Twitch
3. View stream summary:
   - Total viewers
   - Peak concurrent viewers
   - Stream duration

---

## 📱 Facebook Live Setup

### Step 1: Login to Facebook

1. Open **LiveLens** app
2. Go to **Settings → Accounts**
3. Tap **"Add Facebook Account"** or **"Facebook"**
4. Tap **"Sign In with Facebook"**
5. Complete Facebook authentication
6. Grant permissions

### Step 2: Access Your Facebook Pages

Once logged in:
1. Go to **Settings → Accounts → Facebook**
2. Select which page you want to stream from:
   - Your personal profile
   - Business page
   - Community page

### Step 3: Customize Your Stream

You can customize before going live:

#### Stream Title
- Add engaging title for your stream
- Example: "Live Q&A - Ask Me Anything!"

#### Stream Description
- Add context about your stream
- Mention guests or topic

#### Stream Thumbnail
- Choose or upload custom thumbnail
- Custom thumbnails stand out more

#### Privacy Settings
- **Public**: Anyone can view
- **Friends Only**: Only friends can view
- **Private**: Only selected people can view
- **Scheduled**: Schedule stream for later

#### Add Co-Hosts
- If you want multiple people to stream
- Facebook allows co-hosting

### Step 4: Configure Stream Quality

1. Go to **Settings → Streaming**
2. Set your streaming parameters:
   - **Resolution**: 1080p or 720p
   - **FPS**: 30 or 60
   - **Bitrate**: 3-4 Mbps (Facebook is flexible)

### Step 5: Go Live on Facebook

1. Prepare your scene
2. Tap **"Go Live"** button
3. Stream starts on Facebook
4. Monitor:
   - Viewer count
   - Comments and reactions
   - Engagement metrics

### Step 6: Customize During Stream

- 🎨 Switch scenes
- 🎤 Adjust audio
- 🔊 Control volume
- 💬 Interact with comments

### Step 7: End Your Stream

1. Tap **"Stop"** button
2. Stream ends
3. Video is automatically saved to your Facebook page
4. You can keep it up or delete it

---

## 🔧 Custom RTMP Setup

**For servers not listed above or self-hosted streaming.**

### When to Use Custom RTMP

✅ Self-hosted streaming server
✅ Smaller platforms (Kick, DLive, etc.)
✅ Testing/development streaming
✅ Private streaming networks
✅ No account needed - completely anonymous

### Step 1: Get Your RTMP Details

From your streaming platform/server, get:
- **RTMP Server URL** (e.g., `rtmp://live.example.com/app`)
- **Stream Key** (unique identifier for your stream)
- **Stream Name** (optional, for display)

### Step 2: Add Custom RTMP in LiveLens

1. Open **LiveLens** app
2. Go to **Settings → Accounts**
3. Tap **"Add Custom Stream"** or **"Custom RTMP"**
4. Enter the following:

| Field | Example | Notes |
|-------|---------|-------|
| **RTMP URL** | `rtmp://live.example.com/app` | Server address from your platform |
| **Stream Key** | `your_secret_key_12345` | Your unique stream identifier |
| **Stream Name** | "My Custom Stream" | For display in LiveLens (optional) |

### Step 3: Configure Stream Settings

1. Go to **Settings → Streaming**
2. Configure your stream:
   - **Resolution**: Choose based on server capability
   - **FPS**: 30 or 60
   - **Bitrate**: Depends on server, usually 2-6 Mbps
   - **Encoder**: H.264 (most compatible)

### Step 4: Test Connection

1. Go to **Settings → Streaming**
2. Tap **"Test Connection"**
3. LiveLens will verify:
   - Server is reachable
   - Stream key is valid
   - Bitrate is acceptable

### Step 5: Go Live

1. Select your scene
2. Tap **"Go Live"** button
3. Stream will start
4. Monitor connection status

### Step 6: Troubleshooting Custom RTMP

**Connection Failed?**
- Verify RTMP URL is correct
- Check stream key hasn't expired
- Ensure server is online
- Check firewall/network permissions

**Stream Drops Frequently?**
- Lower bitrate by 1-2 Mbps
- Reduce resolution
- Move closer to WiFi router
- Check server capacity

**No Video Showing?**
- Verify stream settings match server requirements
- Check encoder compatibility
- Try H.264 instead of H.265

---

## 🚀 No-Login Streaming (Anonymous)

**Want to stream without logging into any account?**

### Using Custom RTMP Anonymously

1. Get RTMP details from any streaming service
2. Go to **Settings → Accounts → Custom RTMP**
3. Add your RTMP URL and stream key
4. Start streaming immediately
5. No login required! 🎉

### Advantages

✅ Complete privacy - no account needed
✅ No personal data shared
✅ Faster setup
✅ Works with any RTMP server

### Limitations

❌ Can't access platform features (chat, analytics)
❌ Can't schedule streams
❌ Limited moderation tools
❌ No built-in monetization

---

## 📊 Platform Comparison

| Feature | YouTube | Twitch | Facebook | Custom RTMP |
|---------|---------|--------|----------|------------|
| **Login Required** | Optional | Optional | Optional | No |
| **Viewer Count** | ✅ | ✅ | ✅ | ❌ |
| **Chat Integration** | ✅ | ✅ | ✅ | ❌ |
| **Schedule Streams** | ✅ | ✅ | ✅ | ❌ |
| **Auto-Save VOD** | ✅ | ✅ | ✅ | Varies |
| **Monetization** | ✅ | ✅ | ✅ | Custom |
| **Multi-Stream** | ✅ | ✅ | ✅ | ✅ |
| **Customization** | ✅ | ✅ | ✅ | ⚠️ Limited |
| **Privacy** | ✅ | ✅ | ✅ | ✅✅ (Best) |
| **Setup Time** | 2 min | 2 min | 2 min | 1 min |

---

## 💡 Pro Tips for Multi-Streaming

### Best Practices

✅ **Start with one platform** - Master one, then add more
✅ **Use lower bitrate for 2+ platforms** - 5-6 Mbps total per platform
✅ **Monitor all chats** - If supported, split screen for chat
✅ **Have backup plan** - If one platform fails, others continue
✅ **Test before going live** - Always test connection first

### Network Optimization

- Close unnecessary apps
- Use 5GHz WiFi if available
- Stream from stable location
- Avoid WiFi congestion times
- Consider wired connection if possible

### Content Tips

- **Intro**: Let viewers know you're on multiple platforms
- **Cross-promotion**: Mention where else you're streaming
- **Engagement**: Respond to all chats (rotate if needed)
- **Consistency**: Use same settings across all platforms

---

## 🆘 Troubleshooting Platform Issues

### YouTube Issues

**Stream key not showing?**
- Go to YouTube Studio
- Click "Stream" in left menu
- Refresh LiveLens app

**Schedule not appearing?**
- Check if streams are actually scheduled in YouTube Studio
- Try logging out and back in
- Ensure you have permission to stream

### Twitch Issues

**Stream appears offline on Twitch?**
- Check internet connection
- Verify stream key is current
- Try lowering bitrate
- Restart the app

**Chat not updating?**
- This is normal lag - chat updates every few seconds
- If completely stuck, restart app

### Facebook Issues

**Privacy settings not working?**
- Ensure page permissions are correct
- Check Facebook app permissions
- Try updating app

**Stream quality degrading?**
- Facebook throttles based on server load
- Lower bitrate slightly
- Try streaming during off-peak hours

### Custom RTMP Issues

**"Connection refused" error**
- RTMP server might be down
- Check server address is correct
- Verify firewall allows RTMP (port 1935)

**No video on platform**
- Verify stream key is active
- Check resolution/bitrate compatibility
- Ensure platform accepts incoming streams

---

## 📚 Next Steps

- Learn about [Advanced Stream Customization](/wiki/Advanced-Configuration)
- Check [Troubleshooting Guide](/wiki/Troubleshooting)
- Explore [Features](/wiki/Features-Guide)
- Join [Community](/wiki/Community-Guidelines)

---

## ❓ Need More Help?

- 📖 Check [FAQ](/wiki/FAQ)
- 💬 Join [Discord](https://discord.gg/kUqmbKhs6w)
- 📧 Contact [Support](https://www.livelens.live/pages/contact.html)
- 🐛 [Report Issues](https://github.com/ByconStudio/LiveLens/issues)

---

**Happy Streaming! 🎉**

Made with ❤️ by **ByconStudio**