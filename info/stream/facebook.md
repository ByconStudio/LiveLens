# Facebook Live Management

## Overview

LiveLens integrates with the Facebook Graph API to provide a seamless streaming experience for Facebook Gaming and personal profiles. You can manage your stream's privacy, metadata, and keys directly within the app.

---

## 🛠️ Facebook Setup Interface

Selecting Facebook in the Stream Setup dashboard opens a configuration panel tailored for Facebook Live.

### 1. Stream Information
- **Stream Title**: A brief title for your broadcast.
- **Description**: Detailed information about your stream that will appear in the Facebook post.

### 2. Privacy Controls
You can control who sees your broadcast directly from the setup screen:
- **Public**: Your stream is visible to everyone on Facebook.
- **Only Me**: A private stream useful for testing your setup before going live to an audience.

### 3. Gaming Tag (Optional)
If you are a gaming creator, tagging your game is essential for discovery in the Facebook Gaming tab.
- **Integrated Search**: Type the name of the game (e.g., "BGMI", "Free Fire") in the search field.
- **Real-time Results**: Select the correct game from the dropdown list to ensure your stream is properly categorized.

---

## 🔑 Stream Key Management

Facebook uses unique RTMP keys to identify your stream. LiveLens provides advanced management for these keys:

### 1. Generating Keys
- **Generate New Stream Key**: Tap this button to communicate with Facebook and create a new Live Video instance. This automatically fetches the correct **RTMP URL** and **Stream Key** for your session.

### 2. Key Persistence
- **Persistent Key**: Enable this toggle if you use a permanent stream key provided by Facebook.
- **Temporary Keys**: If not persistent, LiveLens includes safety logic that expires and clears the key after **5 minutes** of inactivity to ensure security.

### 3. Security
- **Masked Input**: Your stream key is hidden by default. Use the **Eye Icon** to reveal it if you need to verify the string.

---

## 🔐 Account Management

- **Official Login**: Securely authorize LiveLens using the official Facebook login flow.
- **Profile Display**: Your Facebook profile picture and name are displayed at the top of the setup panel to confirm the active account.
- **Logout**: You can quickly sign out of your Facebook account directly from the bottom of the setup interface.

---

## Facebook Stream Summary

| Feature | Description |
|---|---|
| Auto-Generation | Create Facebook Live instances with one tap |
| Privacy Toggle | Quickly switch between Public and Private tests |
| Gaming Search | Integrated database for tagging mobile and PC games |
| Persistent Key | Support for static keys from Facebook Producer |
| Key Expiration | Enhanced security for temporary session keys |

---

## Related Documentation

- [Stream Setup Guide](../home/stream_setup.md)
- [Account Settings](../settings/account.md)
- [Video Settings](../settings/video.md)
