# <img src="https://raw.githubusercontent.com/lavalink-devs/Lavalink/master/assets/logo.png" width="40" height="40" /> Master Lavalink Node (2025 Edition)

[![Lavalink Version](https://img.shields.io/badge/Lavalink-v4.0.8+-667fff?style=for-the-badge&logo=java)](https://github.com/lavalink-devs/Lavalink)
[![Java Version](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)](https://adoptium.net/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](https://opensource.org/licenses/MIT)

> **The ultimate Lavalink configuration for high-fidelity audio, featuring 11+ plugins, 40+ music sources, and anti-ban persistent sessions.**

---

## 💎 Features & Capabilities

### 🎧 Audio & Performance
* **High-Fidelity Streaming:** Optimized for **320kbps equivalent** audio using Opus 10 encoding.
* **Zero Stutter:** Deep-buffered (5000ms) frame management for smooth playback even on high-latency connections.
* **Pro Filters:** Bassboost, Nightcore, Karaoke, Timescale, Vibrato, and Tremolo pre-configured.

### 🌐 Supported Platforms (40+)
| Platform | Plugin | Status |
| :--- | :--- | :--- |
| **YouTube / YT Music** | `youtube-plugin` | ✅ Persistent OAuth + POT |
| **Spotify / Apple Music** | `LavaSrc` | ✅ ISRC Matching |
| **Deezer / Tidal** | `MediaPack` | ✅ High Quality |
| **TikTok / Mixcloud** | `SkyBot` | ✅ Native Support |
| **SoundCloud / Twitch** | `Standard` | ✅ 24/7 Live Support |

### 🛠️ Advanced Stability
* **Anti-Ban Rotation:** IPv6 RoutePlanner integrated to bypass "Waitlisted IP" and 403 errors.
* **Persistent Sessions:** Automated OAuth Refresh Token flow — **Never lose your web login.**
* **Ad-Blocking:** Integrated **SponsorBlock** to skip non-music segments automatically.
* **Timed Lyrics:** Synced lyrics support via **LrcLib** and **Spotify API**.

---

## 🚀 Quick Deployment

### 1. Requirements
* **Java 21** or higher.
* A VPS with an **IPv6 /64 range** (Recommended for scaling).
* Spotify Developer Credentials.

### 2. Installation
1.  Download the latest `Lavalink.jar` from [Lavalink Releases](https://github.com/lavalink-devs/Lavalink/releases).
2.  Create a folder named `plugins` in the root directory.
3.  Copy the `application.yml` provided in this repository.
4.  Run the server: lavalink.jar

### ⚙️ Configuration Highlight (application.yml)
This node uses a specialized Double-Auth system to ensure 100% uptime on YouTube:
``youtube:
  oauth:
    enabled: true
    refreshToken: "YOUR_PERSISTENT_TOKEN"
    skipInitialization: true
  pot:
    token: "YOUR_SESSION_TOKEN" ``
 ### 📊 Monitoring & Metrics
This node exports real-time metrics for Prometheus and Grafana.
Endpoint: http://your-ip:2000/metrics
Tracked Stats: Playing players, CPU/RAM usage, Uptime, and Voice Connection stability.
🤝 Contributing
Feel free to fork this repository, open issues, or submit pull requests to improve the plugin ecosystem or configuration tuning.
### 🛡️ Credits & Disclaimer
LavaLink application : ALLAY_XD_20
Core: Lavalink Devs
Plugins: Topi314, DuncteBot, Arbjerg
Disclaimer: This configuration is for educational purposes. Ensure you comply with the Terms of Service of all integrated music platforms.
<p align="center">Made with ❤️ for the Devine bot Community</p>


