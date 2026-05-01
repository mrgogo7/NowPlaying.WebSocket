# NowPlaying.WebSocket

A lightweight Windows Now Playing app that lets you view and control your currently playing media, while also streaming real-time data over WebSocket.

Use it as a simple desktop music controller, or connect to it from a browser or custom tools to read live JSON data and audio visualization.

---

## 🖥️ What is this?

NowPlaying.WebSocket is both:

- A **simple Windows media controller**
- A **real-time data source for developers**

You can control playback directly from the app, or use its WebSocket output to build your own visualizers and tools.

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

The app streams live data via: ws://localhost:27871


Includes:

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

Perfect for simple visualizers or reactive UIs.

---

## 🖼️ Album Art

Available via local HTTP endpoint: http://localhost:27871/album-art


---

## 🌐 Example HTML Visualizers

This repository includes example HTML files that:

- Connect to the WebSocket
- Display now playing info
- Render audio visualizations

You can open them directly in your browser or modify them.

---

## 💡 Use Cases

- Desktop Now Playing widget
- Simple music controller
- Browser-based visualizers
- OBS browser source
- Custom tools & experiments

---

## ⚙️ Features

- Lightweight tray application
- WebSocket server (local)
- Media control shortcuts
- Dark theme
- Adjustable visualizer interval
- Optional anonymous analytics

---

## 🔐 Privacy

This app does **not collect personal data**.

If analytics is enabled:

- Only anonymous usage events are sent
- No track titles, artists, or media content are collected
- No usernames, IP addresses, or system identifiers are collected

You can disable analytics at any time.

---

## 📦 Installation

1. Download the latest release
2. Run the setup
3. Launch the app

---

## ☕ Support

If you like this project:

👉 Buy me a coffee

---

## ⚠️ Notes

- This repository contains only the compiled application
- Source code is not included

---

## 📄 License

This software is free for personal use.

Commercial use is not allowed without permission.  
If you are interested in using this software commercially, please contact the author.

See the LICENSE file for details.
