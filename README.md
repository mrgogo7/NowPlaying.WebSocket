# 🎧 NowPlaying.WebSocket

A lightweight Windows Now Playing app with built-in media controls and a local WebSocket server for real-time JSON data and audio visualization.

Stream your current media data locally and use it in your own tools, browser apps, or visualizers.

---

## 🖥️ What is this?

NowPlaying.WebSocket is both:

- A simple Windows media controller  
- A local WebSocket server for real-time media data  

You can control playback directly from the app, or connect to it from a browser or custom tools to read live JSON data.

---

## 🎧 Media Controls (Built-in)

Control your music directly from the tray/taskbar:

- Play / Pause  
- Next / Previous track  
- Mute audio  
- Adjust volume (mouse wheel support)  

No need to switch apps.

---

## 📡 Real-Time Data (WebSocket)

The app runs a local WebSocket server: ws://localhost:27871


It streams real-time JSON data including:

- Now playing metadata  
- Playback state  
- Timeline (position & duration)  
- Audio visualization data  

---

## 🔊 Audio Visualization Data

Real-time values for:

- Volume  
- Bass / Mid / Treble  
- Frequency spectrum  

Perfect for building visualizers or reactive UI elements.

---

## 🖼️ Album Art

Available via local HTTP endpoint: http://localhost:27871/album-art


---

## 📦 Example JSON Output

```json
nowPlaying:
{
  "Type": "nowPlaying",
  "Title": "Thunderstruck",
  "Artist": "AC/DC",
  "Album": "The Razors Edge",
  "Playback": "Playing",
  "IsPlaying": true,
  "PositionSec": 7,
  "DurationSec": 292,
  "PositionText": "0:07",
  "DurationText": "4:52",
  "TimelineVisible": true,
  "TimelineState": "interpolating",
  "TimelineReason": "trusted.native.timelineEvent",
  "AlbumArtUrl": "http://localhost:27871/album-art",
  "UpdatedAt": "02:01:55"
}

audioVisualizer:
{
  "Type": "audioVisualizer",
  "Volume": 5,
  "Bass": 8,
  "Mid": 6,
  "Treble": 5,
  "Spectrum": [
    6,
    6,
    5,
    5,
    5,
    5,
    5,
    5,
    5,
    5
  ],
  "UpdatedAt": "02:01:55"
}
```

🌐 Example HTML (WebSocket Client)

This repository includes ready-to-use HTML examples that:

Connect to the WebSocket server
Display now playing data
Render audio visualizations

Open them directly in your browser while the app is running.

🖼️ Screenshots
<!-- Add your screenshots here --> <!-- Example: ![Main UI](screenshots/main-ui.png) ![Tray UI](screenshots/tray-ui.png) -->
💡 Use Cases
Desktop Now Playing widget
Simple music controller
Browser-based visualizers
OBS browser source
WebSocket API for music data
Real-time media data streaming
⚙️ Features
Lightweight tray application
Local WebSocket server
Media control shortcuts
Dark theme
Adjustable visualizer interval
Optional anonymous analytics
🔐 Privacy

This app does not collect personal data.

If analytics is enabled:

Only anonymous usage events are sent
No track titles, artists, or media content are collected
No usernames, IP addresses, or system identifiers are collected

All data stays on your machine unless analytics is enabled.

You can disable analytics at any time.

📦 Installation
Download the latest release
Run the setup
Launch the app
☕ Support

If you find this project useful:

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/mrgogo)

⚠️ Notes
This repository contains only the compiled application
Source code is not included
📄 License

Free for personal, non-commercial use.

Commercial use requires a separate license.
Please contact the author for commercial licensing.

See the LICENSE file for details.
