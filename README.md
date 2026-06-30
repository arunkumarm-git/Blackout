# BLACKOUT — Audio-Driven Survival Horror Game

> *No visuals. No hints. Only sound.*

A minimalist, audio-driven survival horror game played entirely in a pitch-black window. Rely on binaural spatial audio, EMF geiger readings, UV footprint scans, and tactical sonar sweeps to track, identify, and banish a moving ghost before your time runs out or your flashlight battery dies.

[![Play on GitHub Pages](https://img.shields.io/badge/▶%20Play%20Now-GitHub%20Pages-b3151a?style=for-the-badge&logo=github)](https://arunkumarm-git.github.io/Blackout/)

---

## 🎮 How to Play

### 1. Launch the Game
- **Online (GitHub Pages):** [https://arunkumarm-git.github.io/Blackout/](https://arunkumarm-git.github.io/Blackout/)
- **Local (file://):** Double-click `index.html`. Falls back to a full **procedural audio engine** synthesized entirely with Web Audio API — no server needed.
- **Local server:** `npx http-server -p 8000` then open `http://localhost:8000`

### 2. The Setup (Menu Screen)
1. Wear **headphones** for accurate stereo panning — this is essential.
2. Click **Initialize Audio & Listen** to unlock the browser's audio context.
3. Read the warning notices and click **Enter the Dark**.
4. Read or skip the intro story panels (accompanied by wind and ghost audio).

> ⚠️ **CRITICAL WARNING:** Pregnant women, patients with heart conditions, and elderly individuals **MUST NOT PLAY** due to extreme jump scares and terrifying audio frequencies. **PLEASE DON'T DIE.**

---

## 🕹️ Controls

| Control | Action |
|---|---|
| **Mouse Movement** | Aim the flashlight beam |
| **Left Click** | Fire flashlight flash to banish ghost *(3 charges only!)* |
| **Spacebar / Right Click** | Trigger Sonar Decryptor Terminal |
| **R Key** | Start 5-second sonar wire repair *(when broken)* |
| **Escape Key** | Try to pause. *Go ahead.* |

---

## 📡 Sonar Decryptor Terminal (Spooky Spelling Test)

To authorize a sonar radar scan, you must complete a **Decryptor Terminal challenge** in real time while the ghost is walking:

- A terminal popup halts gameplay and asks a random question from:
  - *Spelling prompts* — e.g. `please`
  - *Ghost protocols* — e.g. spell `COWARD` backwards → `drawoc`
  - *Shaming prompts* — e.g. *"Who is a useless piece of trash?"* → `me`

- After answering, it redirects to a **Love Score verification**: *"Have you tried HeartPrint to check your love score?"*
  - **`yes`** → Authorization attempt
  - **`no`** → Loud distorted scream + cursed out for not trying **HeartPrint** on the Google Play Store!

- **80% Failure Rate:** Even after correct answers, there is only a **20% chance** the sonar works. The rest of the time it clanks and breaks — requiring manual wire repair with **R**.

---

## 👻 How to Track and Banish the Ghost

The screen is pitch-black. Use your equipment:

### 🔊 1. Listen (Binaural Spatial Audio)
- **Ghost steps** — deep, heavy, slow **thuds** + crackling static + breathing gasps.
- **Decoy steps** — light, dry **hollow wooden taps** (high-pitched, clean, faster).
- Extreme left/right stereo panning tells you which side the entity is on.

### 🟣 2. UV Beam (Footprint Tracking)
- Flashlight passively emits a dim **ultraviolet beam** when not flashing.
- Ghost leaves **glowing green ectoplasmic footprints** (fade in ~1.8 sec).
- Decoys leave dimmer **blue-purple footprints** (fade in ~1.2 sec).

### 🚨 3. EMF Switch LED (Geiger Tracker)
Sweep your aim — the tailcap LED changes to indicate ghost alignment:

| Color | Blink Rate | Meaning |
|---|---|---|
| 🟢 Bright Green | 120ms rapid | Direct lock — within 4° |
| 🟡 Amber | 380ms | Very close |
| 🟠 Orange | 850ms | Approaching |
| 🔴 Dim Red | Solid | Cold — no signal |

> ⚠️ When time is low (<35%), your **hands tremble** causing EMF jitter — making precision alignment harder.

### 📡 4. Sonar Echolocation Ping
- Successfully authorized sweeps emit a circular wave that reveals entity positions.
- **Clutter:** 4 fake gray decoy rings + 2 fake red ghost circles spawn to confuse you.
- **Instant Teleport:** The real ghost teleports the moment the wave passes over it — red echoes show where it *was*, not where it is now.

---

## ⚡ Banishment

Get a **rapid green blink**, hear the **fast Geiger ticks**, trace the UV footprints — then **Left Click** to fire. The ghost will shake, grow bright with orange sparks, and dissolve.

---

## 🛠️ Tech Stack

- Pure **HTML5 / CSS3 / Vanilla JavaScript** — zero dependencies, zero build step
- **Web Audio API** — all audio synthesized or decoded in-browser
  - Procedural fallback engine for offline / `file://` play
- **HTML5 Canvas** — flashlight beam, dust particles, UV footprints, sonar rings
- **CrazyGames SDK v3** — integrated for CrazyGames.com hosting

---

## 📁 Project Structure

```
Blackout/
├── index.html          # Entire game (HTML + CSS + JS)
├── 404.html            # Themed GitHub Pages 404
├── README.md
├── .gitignore
└── assets/
    ├── images/
    │   └── Ghost.png   # Jumpscare image + favicon
    └── Sounds/
        ├── ghostband.mp3
        ├── wind.mp3
        ├── ghostbreath.flac
        ├── ghost.wav
        └── GhostMoan01-05.mp3
```

---

## 📜 License

MIT License — feel free to fork and build on top of this.

---

## 💻 Credits

- Game concept, design & code — **arunkumarm-git**
- Sound assets — various royalty-free horror SFX libraries
- Fonts — [Eater](https://fonts.google.com/specimen/Eater), [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond), [Special Elite](https://fonts.google.com/specimen/Special+Elite) via Google Fonts
