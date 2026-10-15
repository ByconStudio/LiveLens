# Platform Accounts & Multi-Streaming

## Overview

LiveLens allows you to connect directly to major streaming platforms for a seamless experience. Linking your accounts enables one-tap streaming and integrated chat features.

---

## 📺 Supported Platforms

You can securely log in to the following platforms within LiveLens:
- **YouTube**: Authorize via Google to manage stream titles and fetch live chat.
- **Twitch**: Authorize via Twitch to access your channel dashboard and chat alerts.
- **Facebook**: Connect your page or profile to go live directly on Facebook Gaming.
- **Kick**: Direct integration for the emerging gaming platform with support for native chat.

---

## 🌐 Multi-Stream Mode

One of the most powerful features of LiveLens is the ability to stream to **multiple platforms at once**.

- **Toggle Multi-Stream**: Enable this switch in **Global Settings** → **Streaming** to reveal multi-destination options on the Go-Live screen.
- **Layout Management**: Even when multi-streaming, LiveLens uses a single canvas layout to ensure your device performance remains stable.
- **Bandwidth Note**: Multi-streaming requires a significantly stronger upload connection, as the app sends data to multiple servers simultaneously.

---

## 🔒 Security & Privacy

- **No Passwords Stored**: LiveLens uses official OAuth methods (standard login popups) to connect to platforms. The app never sees or stores your passwords.
- **Revoking Access**: You can log out of any account at any time from the **Global Settings** → **Account** screen.

---

## Account Settings Summary

| Feature | Description |
|---|---|
| Native Login | Official integration for YouTube, Twitch, Facebook, and Kick |
| Multi-Stream | Go live on multiple platforms simultaneously |
| Auto-Refresh | Keeps your Twitch and YouTube sessions active automatically |
| One-Tap Chat | Chat overlays are automatically prepared for logged-in accounts |

---
## 🤖 Discord Bot Login Troubleshooting

The LiveLens Discord bot can help users diagnose login and OAuth-related problems for supported streaming platforms.

### Supported Platforms

The bot can assist with login issues for:

- YouTube
- Twitch
- Facebook
- Kick

LiveLens uses official authentication methods for each platform. The app does not request or store users' platform passwords.

---

## 🔐 Login Troubleshooting Information

When a user reports that they cannot log in, the bot should collect the following information before suggesting advanced troubleshooting:

### Required Information

- **Platform:** YouTube / Twitch / Facebook / Kick
- **LiveLens version**
- **Device / Android version**
- **Exact error message**
- **Where the login process fails**
- Whether the login works with another account
- Whether the login works on another device
- Whether the user reaches the OAuth consent screen
- Whether the user can select their account
- Whether the user can press **Allow**
- Whether the error appears after returning to LiveLens

### OAuth Login Stages

The bot should determine which stage of the authentication flow is failing:

1. LiveLens login button
2. OAuth login page opens
3. Platform account selection
4. OAuth consent screen
5. User grants requested permissions
6. OAuth redirects back to LiveLens
7. Authorization code/token is processed
8. Account appears as connected in LiveLens

Identifying the failed stage can significantly narrow down the cause.

---

## 🧪 YouTube Login Diagnostics

### Login fails before the Google account selection screen

Possible causes include:

- Network connectivity problems
- VPN interference
- Ad-blocker interference
- OAuth/browser popup problems
- Device-specific Google authentication issues

Recommended actions:

1. **Switch Networks**: Network restrictions or ISP blocks often cause login failures. 
    - If you are on **Wi-Fi**, turn it off and try using **Mobile Data**.
    - If you are already on **Mobile Data**, try switching to a stable **Wi-Fi** connection.
2. **Use a Hotspot**: If you don't have access to another network, try connecting to a **mobile hotspot** from a friend or family member. This is the best way to determine if your specific internet provider is blocking the login service.
3. Check the internet connection stability.
4. Disable any active VPN or Ad-blocker.
5. Update LiveLens to the latest version.
6. Retry the login.
7. Check your **Global Settings** to ensure platform modules are active.

---

### Login reaches Google but fails after account selection

Collect the exact Google error message.

If possible, also determine whether:

- Other Google accounts can log in successfully.
- The same account works on another device.
- The user previously denied the requested permission.
- The user previously connected LiveLens and later removed its Google account access.

If other accounts can successfully authenticate using the same LiveLens version, OAuth configuration problems are less likely and an account-specific or device-specific issue should be investigated.

---

### `access_denied`

If the OAuth authorization returns an `access_denied` error, the user may have cancelled or denied the authorization request.

Recommended actions:

1. Retry the LiveLens login.
2. Make sure the user selects **Allow** on the Google consent screen.
3. If the problem continues, check whether LiveLens still has an existing connection in the user's Google Account.
4. Retry authorization after removing the existing LiveLens connection if necessary.

Do not assume that every `access_denied` error has the same cause. The exact OAuth flow and error context should be collected.

---

### YouTube Brand Account Issues

If the user receives an authentication or access error while using a YouTube Brand Account:

- Try logging in with the primary Google account associated with the Brand Account.
- If native login continues to fail, use the **Custom RTMP** option as an alternative.

Android may restrict or behave differently with some Brand Account authentication flows.

---

## 🔎 Account-Specific Login Diagnosis

If multiple Google accounts can successfully log in to LiveLens but one specific account cannot, collect:

- Exact account-specific error
- OAuth stage where the failure occurs
- Whether the same account works on another device
- Whether the account previously denied LiveLens permissions
- Whether LiveLens access was previously revoked
- Whether the account is associated with a YouTube Brand Account

This helps distinguish between:

- Account-specific authorization problems
- Device-specific problems
- OAuth/browser problems
- LiveLens configuration problems

---

## 📱 Device-Specific Diagnosis

If the account works on another device but fails on the user's current device, investigate:

- Android version
- LiveLens version
- Network configuration
- VPN
- Ad-blocking software
- Browser/WebView configuration
- Google account configuration on the device

The issue should not automatically be treated as an OAuth configuration problem if the same account successfully authenticates elsewhere.

---

## 🧹 Cache and App Data

### Clear Cache

Clearing the LiveLens cache is a relatively safe first troubleshooting step.

It should not delete locally saved scenes or account logins.

**Recommended for:**

- Minor application glitches
- Slow UI
- Temporary cached data problems

### Clear App Data

Clearing application data resets LiveLens to its factory state.

**WARNING:** This deletes locally stored:

- Scenes
- Themes
- Settings
- Login information

Before clearing app data:

1. Open the Scene Manager.
2. Export important scenes.
3. Save the `.json` files to Downloads/Documents or another safe location.
4. Clear LiveLens app data.
5. Re-open LiveLens.
6. Retry the login.
7. Import the saved scene files again.

### Uninstall/Reinstall

Uninstalling LiveLens can also remove locally stored application data.

Users should export important scenes before uninstalling.

---

## 📝 Information to Send to Support

If the problem cannot be resolved, the user should provide:

```text
Platform:
LiveLens Version:
Android Version:
Device:

Login Account:
[Do NOT provide password, OAuth token, refresh token, stream key, or client secret]

Login Stage:
[Example: OAuth consent / after pressing Allow / returning to LiveLens]

Exact Error:
[Paste the exact error message]

Does another account work?
Yes / No

Does the same account work on another device?
Yes / No / Unknown

VPN Enabled:
Yes / No

Ad-blocker Enabled:
Yes / No

Brand Account:
Yes / No / Unknown

Previous LiveLens Authorization:
Yes / No / Unknown
---

## Related Documentation

- [Chat Overlay](./chat.md)
- [Privacy Policy](../privacy.md)
- [Video & Stream Settings](./video.md)
- [Import & Export](../scene/scene.md#importing--exporting-scenes)
