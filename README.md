# 🎧 NowPlaying.WebSocket

**Real-time Windows Now Playing data + Audio Visualizer JSON over WebSocket**

NowPlaying.WebSocket is a lightweight Windows application that:

✔ Streams **Now Playing media data**  
✔ Streams **real-time Audio Visualizer data**  
✔ Exposes everything via **local WebSocket (JSON)**  
✔ Works as a **standalone media controller app**

---

## 🔥 Why this project exists

Most tools can show "Now Playing".

Almost none provide:

- Real-time **Audio Visualizer data**
- Clean **JSON over WebSocket**
- Easy integration for **browser apps / overlays / OBS**

👉 This app does all of them.

---

## ⚡ Core Features

### 🎵 1. Real-Time Audio Visualizer (WebSocket JSON)

This is the **main feature**.

The app streams **live audio analysis data**:

- Volume level
- Bass / Mid / Treble
- Frequency spectrum array

Perfect for:

- Audio visualizers  
- Reactive UI  
- OBS browser sources  
- Web-based overlays  
- Stream tools  

📡 WebSocket endpoint: ```ws://localhost:27871```

---

### 🎧 2. Now Playing Data (Live JSON Stream)

Stream real-time media information:

- Title  
- Artist  
- Album  
- Playback state  
- Timeline (position / duration)  
- Album art URL  

---

### 🔊 Example Audio Visualizer JSON

```json
{
  "Type": "audioVisualizer",
  "Volume": 35,
  "Bass": 59,
  "Mid": 43,
  "Treble": 40,
  "Spectrum": [50,36,42,40,41,38,37,42,38,41],
  "UpdatedAt": "21:18:20"
}
```

🎵 Example Now Playing JSON
```
{
  "Type": "nowPlaying",
  "Title": "Come Together - Remastered 2009",
  "Artist": "The Beatles",
  "Album": "Abbey Road (Remastered)",
  "Playback": "Playing",
  "IsPlaying": true,
  "PositionSec": 74,
  "DurationSec": 259,
  "PositionText": "1:14",
  "DurationText": "4:19",
  "AlbumArtUrl": "http://localhost:27871/album-art"
}
```
---
###🖥️ Standalone Windows App (Not just WebSocket)

This is not only a WebSocket server.

It is also a full Now Playing desktop app:

###🎮 Media Controls
- Play / Pause
- Next / Previous
- Mute / Unmute
- Volume control (slider + mouse wheel)
----
###🧩 Tray & Flyout UI
- Tray icon with quick access
- Click → open control panel
- Lightweight, always accessible
----
###⚙️ App Features
- Always on top (optional)
- Run at startup
- Start minimized to tray
- Dark theme
- Hide tray icon
----
###🔊 Audio Capture & Devices
+  Automatic loopback capture
+ Manual device selection:
    + Speakers
    + Headphones
    + Microphones (WASAPI)
----
###🎚️ Visualizer Interval Control

Control update speed:
- Lower = smoother animation
- Higher = lower CPU usage
Perfect for fine-tuning real-time visualizers

###🖼️ Album Art Endpoint: 
```http://localhost:27871/album-art```

Use directly in:
- HTML <img>
- Canvas apps
- Overlays
----
###🌐 Built for Developers

This app is designed for:
- Frontend developers
- OBS users
- Stream tool creators
- Dashboard builders
----
###📂 Examples Included

Check /examples folder:

✔ Ready-to-use HTML files
✔ WebSocket client examples
✔ Audio visualizer demos

Just open in browser → works instantly.
----
###💡 Use Cases
- 🎛️ Audio Visualizer (Web)
- 🎥 OBS Browser Source
- 🖥️ Desktop widgets
- 📊 Music dashboards
- 🎮 Stream overlays
- 🌐 Web-based music UI

----
###📦 Download

👉 Latest version:

```https://raw.githubusercontent.com/mrgogo7/NowPlaying.WebSocket/main/releases/NowPlaying.WebSocket_Setup_v6.4.30.0.exe```

----

###🔐 Privacy
- No personal data collected
- No media content sent externally
- Everything runs locally

Optional: Anonymous usage analytics (can be disabled)
----
###☕ Support

If you find this useful: [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/mrgogo)
----
###⚠️ Important Notes
This repository contains compiled application only
Source code is not included
📄 License

Free for personal use.

Commercial use requires permission.
