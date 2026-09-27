# ⚡ Neon Rider Extreme 🏍️💨

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Matter.js](https://img.shields.io/badge/Physics-Matter.js-00e5ff)](https://brm.io/matter-js/)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-brightgreen)](https://pages.github.com/)
[![Mobile Friendly](https://img.shields.io/badge/Mobile-Ready%20%F0%9F%93%B1-ff007f)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)

**Neon Rider Extreme** is a high-octane, retro-futuristic 2D physics motorcycle stunt racing game built with vanilla JavaScript, HTML5 Canvas, and Matter.js. Features full-screen Cyberpunk aesthetics, an interactive Garage with 3 customizable bikes and upgrade tiers, a persistent coin economy, Color-Phasing track mechanics, Bullet-Time Slow-Mo, zero-asset Web Audio synthesis, and the Prompt Overdrive meta system. Plays instantly on **any phone, tablet, laptop, or desktop**.

---

## 🚀 How to Play / Host on GitHub Pages (Instant Setup)

Anyone can open and play this game directly from your GitHub repository! Follow these simple steps:

1. **Push this repository to your GitHub account**.
2. On your GitHub repository page, click **Settings** (top navigation tab).
3. In the left sidebar, click **Pages** (under "Code and automation").
4. Under **Build and deployment > Source**, select **Deploy from a branch**.
5. Set Branch to **`main`** (or `master`) and Folder to **`/(root)`**, then click **Save**.
6. Wait 30 seconds! GitHub will generate your live public game link:
   ```text
   https://<your-username>.github.io/<your-repository-name>/
   ```
👉 *Anyone in the world can now open that link on their phone, iPad, or computer and play immediately!*

---

## 🎮 Game Controls

The game automatically adapts to whichever device you are playing on:

### 💻 Desktop / Laptop (Keyboard)
| Key | Action |
|:---:|:---|
| **`W`** / **`▶`** / **`▲`** | **Gas / Accelerate Forward** |
| **`S`** / **`◀`** / **`▼`** | **Brake / Reverse** |
| **`A`** | **Lean Back / Wheelie / Backflip** |
| **`D`** | **Lean Forward / Stoppie / Frontflip** |
| **`Shift`** | **Color-Phase Toggle (Cyan ⇄ Magenta)** |
| **`Space`** | **Prompt Overdrive Terminal** *(Requires Overdrive $\ge 50\%$)* |
| **`R`** | **Quick Restart / Respawn** |
| **`F`** | **Toggle Fullscreen Mode** |

### 📱 Mobile & Tablet (Touch Controls)
- **Left Thumb Dock**: Tilt Back (`↺`), Tilt Forward (`↻`), and Color-Phase Toggle (`PHASE`).
- **Right Thumb Dock**: Gas (`▶`), Brake (`◀`), and Quick Restart (`🔄`).
- **HUD Overdrive (`⚡ PROMPT`)**: Appears when Overdrive Bar is $\ge 50\%$. Tap to suspend physics and open the Command Terminal.
- **Fullscreen Button (`⛶`)**: Tap to enter immersive borderless arcade mode.
- **Share Button (`🔗`)**: Tap to open your device's native share sheet (WhatsApp, Discord, Instagram, Messages, Twitter) or copy the game link with one tap!

---

## 🌟 Key Features & Mechanics

### 1. 🌈 The Color-Phasing Mechanic (Prompt 5)
- The track procedurally alternates between **Neon Cyan (`#00FFFF`)** and **Neon Magenta (`#FF00FF`)**.
- Press **`Shift`** (or tap **`PHASE`**) to instantly toggle your bike's color and neon glow.
- **Matching Rule**: Your bike's color must match the segment you land on! Touching a mismatched track color triggers an immediate crash.

### 2. ⏳ "Bullet-Time" Slow-Mo on Big Air (Prompt 6)
- Launching off high ramps with vertical velocity triggers cinematic slow-motion at **25% physics speed** (`timeScale = 0.25`).
- The camera zooms in smoothly (`1.16x`) and applies a dark radial vignette around the canvas.
- Landing resets physics to normal speed and triggers an impact camera shake.

### 3. 🔊 Zero-Asset Synthesized Web Audio API (Prompt 7)
- Zero external MP3 downloads! All sounds are generated in real-time using native Web Audio:
  - **Engine Hum**: Sawtooth wave continuously pitch-modulated by rear-wheel angular velocity.
  - **Coin Chime**: High-pitched sine wave sweep ($800\text{Hz} \to 1200\text{Hz}$).
  - **Crash Explosion**: Synthesized white-noise buffer passed through a swept lowpass filter.

### 4. ⚡ The "Prompt Overdrive" Meta Mechanic (Prompt 8)
- Collecting coins fills the HUD Overdrive Bar (+20% per coin).
- At $\ge 50\%$, hit **`Spacebar`** to pause physics and open the Command Input modal:
  - **`MOON`**: Reduces gravity to $0.2\times$ for 5 seconds of soaring moon jumps.
  - **`ROCKET`**: Delivers an explosive forward rocket boost with flame particles.
  - **`MAGNET`**: Magnetically pulls all coins within an 800-pixel radius toward your bike for 5 seconds.

### 5. 🏎️ Cyber Garage & Upgrade Matrix
- 3 distinct bikes: **Starter Bike**, **Sport Bike** (150 coins), and **Heavy Cruiser** (300 coins).
- Upgrade **Speed**, **Torque**, and **Suspension** up to 5 tiers each using coins saved in `localStorage`.

---

## 🛠️ Technology Stack & Architecture

- **Core**: Vanilla HTML5, CSS3, and JavaScript (ES6+).
- **Physics**: [Matter.js](https://brm.io/matter-js/) (Imported via CDN).
- **Renderer**: High-performance custom canvas render loop via `requestAnimationFrame` with camera lerp tracking and zoom scaling.
- **Audio**: Web Audio API (Zero external MP3/WAV files required).
- **Storage**: `localStorage` (Preserves coins, unlocked bikes, and upgrades across browser sessions).
- **Deployability**: **Zero build step required**. Pure static files that run directly from any web server or GitHub Pages!

---

## 📱 Progressive Web App (PWA)
- **Add to Home Screen**: Installable as a standalone offline-ready web app on iOS Safari and Android Chrome.
- **Open Graph & Twitter Cards**: High-impact social media link previews.

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).
