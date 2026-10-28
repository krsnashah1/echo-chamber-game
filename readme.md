# ECHO CHAMBER // Sector-09 Enhanced Survival
*An award-winning acoustic survival-horror game built for Problem Statement 3.3 (Audio-Visual Survival).*

[![HTML5 Canvas](https://img.shields.io/badge/Engine-HTML5%20Canvas-00f3ff?style=flat-square&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
[![Web Audio API](https://img.shields.io/badge/Audio-Web%20Audio%20API-00ff88?style=flat-square)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Vanilla JS](https://img.shields.io/badge/Code-Vanilla%20ES6%20JS-ffb700?style=flat-square&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/UI-Tailwind%20CSS-38bdf8?style=flat-square&logo=tailwindcss)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

---

## 🎮 Play Live
👉 **Play the game directly in your browser:** [https://krsnashah1.github.io/echo-chamber-game/](https://krsnashah1.github.io/echo-chamber-game/)

---

## 🌌 Overview
Power has failed across Sub-Level 09. Total darkness prevails. You are **Dr. Mara Ellis**, an acoustic engineer trapped in an abandoned facility. Your only vision is your suit's **Acoustic Sonar Emitter**—every ping maps the architecture in glowing cyan wireframe, but sound is lethal. **Subject-89** and its Chorus are blind and hunt purely by sound.

Designed as a single, self-contained, high-performance HTML file with **zero external assets or dependencies**, *Echo Chamber* pushes web-based gaming to deliver a AAA atmospheric horror experience.

---

## ✨ Key Features & Mechanics

1. **360° Acoustic Sonar & 4-Second Phosphor Decay:**
   - Press `SPACE` or `Left-Click` to emit an expanding acoustic ring. Walls, hazard stripes, terminals, and items illuminate and slowly decay back into pitch darkness over **4.0 seconds**.
2. **Noise vs. Information Trade-off (AI Hunting Anomaly):**
   - Sonar pings and sprinting (`SHIFT`) alert biological entities. Use `C` to toggle silent crouch-walking and avoid triggering crimson monster counter-pulses.
3. **GTA/Among Us-Style Keycard Hacking Mini-Puzzles:**
   - Secure 3 Keycards (Alpha, Beta, Gamma) across sectors by completing high-stakes memory sequence mini-puzzles with a strict **2-attempt limit**.
   - **Temporary Vent Mechanic:** The first hacking attempt deploys a temporary emergency escape vent to hide from hunters; it permanently collapses once the keycard is collected.
4. **Interactive Map Hazards & Economy:**
   - Dodge dynamic sliding security doors, lethal floor spikes, and proximity mines.
   - Collect rare resonance gems to spend at the **Field Store (`[S]`)** on powerups like Sonar Boosters, Speed Stims, and Noise Dampeners.
   - Fire the **Sonic Lance (`Q` or Mid-Click)** to stun or eliminate threats at the cost of high noise output.
5. **Procedural Web Audio API Soundscape & Music:**
   - Zero `.mp3` or `.wav` files. Dynamic submarine sonar pings, accelerating heartbeat audio as monsters approach, radio static bursts, and an eerie procedural ambient music bus powered by low-pass filters and delay feedback loops.
6. **Adaptive Mercy System & Stuck Guidance:**
   - If a player dies 3+ times, a mercy protocol prompts to reduce active hostiles. If stuck in a sector for 25+ seconds, an interactive tactical advisory tip screen appears.

---

## 🕹️ Controls

| Key / Input | Action |
| :--- | :--- |
| **`W A S D` / `Arrow Keys`** | Move through the laboratory |
| **`SPACE` / `Left-Click`** | Emit 360° Acoustic Sonar Pulse |
| **`E` / `Right-Click`** | Throw Decoy Radio (5s green lure) |
| **`F`** | Enter / Exit Stasis Hiding Pod or Vent |
| **`SHIFT`** | Sprint (Loud acoustic signature) |
| **`C`** | Toggle Crouch-Walk (Silent) |
| **`Q` / `Middle-Click`** | Fire Sonic Lance (Stun / Combat) |
| **`B` / `S`** | Open Field Store (Redeem Gems) |
| **`R`** | Restart Mission (with Confirmation Modal) |

---

## 🛠️ Technical Architecture

* **Zero Build Steps:** Packaged entirely inside a single `index.html` file combining HTML5 Canvas, Tailwind CSS, and vanilla ES6 JavaScript.
* **Smart Flow-Field Pathfinding:** Discretized $40\text{px}$ navigation grid paired with Breadth-First Search (BFS) distance markers, allowing AI entities to smoothly round complex architectural corners without getting stuck.
* **Swept-Collision Physics:** Continuous ray-segment intersection checks (`segT`) ensure player movement, enemy sliding, and thrown decoy bounces stay strictly bounded within the facility.

---

## 🚀 Local Execution
Clone the repository and open `index.html` in any modern web browser:
```bash
git clone [https://github.com/krsnashah1/echo-chamber-game.git](https://github.com/krsnashah1/echo-chamber-game.git)
cd echo-chamber-game
# Open index.html directly in Chrome, Firefox, or Edge
