# 🎯 ThreeJS Multiplayer LAN FPS Game

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=13,25,3&height=210&section=header&text=ThreeJS%20Multiplayer%20LAN%20FPS&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Real-Time%20First-Person%20Combat%20in%20Your%20Browser&descAlignY=56&descSize=18" width="100%"/>

<br/>

[![Version](https://img.shields.io/badge/version-2.3.0-0F5257?style=for-the-badge&logo=semanticrelease&logoColor=white)](https://github.com)
[![Stack](https://img.shields.io/badge/Three.js%20%7C%20WebSocket%20%7C%20Node-0B6E4F?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org)
[![License](https://img.shields.io/badge/license-MIT-0A8754?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Players](https://img.shields.io/badge/players-up%20to%2016-8DE4AF?style=for-the-badge&logo=gamepad&logoColor=black)](https://github.com)

<br/>

### 🔫 A fully playable multiplayer FPS that runs in your browser over local network

*🌐 LAN Multiplayer • 🎮 Pointer Lock Controls • ⚡ Low Latency • 🖥️ No Install*

<br/>

<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/🎮_PLAY_DEMO-0F5257?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=0A3B3F" alt="Play Demo" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/📥_GET_SOURCE-0B6E4F?style=for-the-badge&logo=github&logoColor=white&labelColor=074F39" alt="Get Source" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/📚_DOCS-0A8754?style=for-the-badge&logo=readthedocs&logoColor=white&labelColor=07623C" alt="Docs" height="45"/>
</a>

</div>

<img width="1920" height="1080" alt="e3u0q7tyii561" src="https://github.com/user-attachments/assets/2a66d57c-5e74-433d-b87f-cee224a1799b" />


<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 About

**ThreeJS Multiplayer LAN FPS** is a **complete, browser-based first-person shooter** that runs over your local network — no installs, no accounts, no cloud servers. Spin up the Node.js server on one machine, and up to 16 players can join from any device on the LAN with just a browser.

It's a **real FPS**: pointer-lock mouse look, WASD movement, hitscan shooting, hit registration, kill feed, and respawns — all powered by **Three.js** for rendering and **WebSockets** for networking.

> 💡 **Perfect for:** Game dev students, web devs curious about multiplayer, LAN parties, and anyone who wants to learn real-time networking without leaving JavaScript.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Key Features

<div align="center">

| 🌐 **LAN Multiplayer** | 🎮 **FPS Controls** | 🔫 **Hit Registration** |
|:---:|:---:|:---:|
| Up to 16 players<br/>on local network | Pointer lock, WASD,<br/>sprint & jump | Server-authoritative<br/>hit detection |

| ⚡ **Low Latency** | 🗺️ **Arena Map** | 🎨 **HUD & Kill Feed** |
|:---:|:---:|:---:|
| Client prediction +<br/>server reconciliation | Symmetrical map<br/>with cover & spawns | Crosshair, health,<br/>ammo & kill feed |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Project

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| 🎯 **Real Netcode** | Client prediction, server reconciliation, and interpolation — done properly |
| ⚡ **Instant to Join** | Anyone on the LAN opens a URL and is in the match within seconds |
| 🖥️ **No Install Needed** | Pure browser — works on desktop, laptop, and even tablet |
| 🧠 **Learn Real Skills** | Perfect reference for snapshot sync, lag compensation, and state replication |
| 🛡️ **Server Authority** | All hit detection and movement validation on the server — no client cheating |
| 🧩 **Extendable** | Clean modular structure for adding weapons, maps, or game modes |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Game Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  🎯  ThreeJS LAN FPS  v2.3.0                     ║
╠══════════════════════════════════════════════════╣
║                                                  ║
║      ╱╲        🎯 Crosshair                     ║
║     ╱  ╲        ┼                                ║
║    ╱    ╲                                        ║
║   ╱      ╲     👤 Enemy (Player 3)               ║
║  ╱   🔫   ╲                                      ║
║ ╱          ╲   [ ▮▮▮▮▮▮▮░░ ]  HP 74/100          ║
║                                                  ║
║  💥 Player 2 killed Player 5                     ║
║  💥 Player 3 hit you for 26 damage               ║
║                                                  ║
║  📊 Kills: 4   Deaths: 2   Ping: 8ms             ║
║  🌐 Players: 6/16   ⏱️ Match: 3:42                ║
║                                                  ║
║  WASD Move  Shift Sprint  Space Jump  LMB Fire   ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
🎯 threejs-multiplayer-lan-fps/
├── 🎯 client/
│   ├── src/
│   │   ├── renderer/          # Three.js scene & camera
│   │   ├── input/             # Pointer lock & controls
│   │   ├── netcode/           # Prediction & interpolation
│   │   ├── weapons/           # Firing & effects
│   │   └── ui/                # HUD & kill feed
│   └── index.html
├── ⚙️  server/
│   ├── src/
│   │   ├── game/              # Authoritative game state
│   │   ├── network/           # WebSocket handling
│   │   └── physics/           # Hit detection & collision
│   └── server.js
├── 🗺️  maps/                   # Arena definitions
├── 🧪 tests/                  # Netcode & logic tests
└── 📖 docs/                   # Setup & netcode explainer
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=websocket&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a netcode bug? Want to add weapons, maps or game modes?

<div align="center">

<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-0F5257?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>
<a href="https://share.google/Mj8HdSCp4Tnbr24lP">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-8DE4AF?style=for-the-badge&logo=github&logoColor=black" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

<br/>

<div align="center">

### 🎯 Made with 🔫 by the ThreeJS LAN FPS Team

*If this project taught you netcode — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=13,25,3&height=120&section=footer" width="100%"/>

</div>
