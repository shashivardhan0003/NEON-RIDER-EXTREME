# 🚴‍♂️ NEON RIDER EXTREME

A high-octane 2D physics-based stunt bike browser game built with **Matter.js** and **HTML5 Canvas**.

🔗 **Live Demo:** [Play Neon Rider Extreme](https://shashivardhan0003.github.io/NEON-RIDER-EXTREME/)

---

## 🎮 Game Overview & Features
- **Realistic 2D Physics**: Built using Matter.js composite bodies for vehicle chassis, high-friction bouncy wheels, and dual-shock suspension constraints (`stiffness: 0.2`, `damping: 0.1`).
- **Dynamic Terrain**: Downhill acceleration slope, flat runway, high-launch mega jump ramp, deep valley gap, landing ramp, rolling hills, and boundary walls.
- **Full Control System**: Rear-wheel motor drive, braking system, and direct chassis torque for mid-air flips, landing balance, and wheelies.
- **Dynamic Viewport & HUD**: Real-time camera tracking following the vehicle via `Matter.Render.lookAt`, equipped with live Speed (km/h) and Distance (m) counters.

---

## 🕹️ Controls
| Input | Action |
|---|---|
| ➔ **Right Arrow** | Motor Drive / Accelerate Forward |
| ⬅️ **Left Arrow** | Brake / Reverse Motor |
| 🅰️ / 🇩 **A / D Keys** | Pitch / Tilt Chassis (Mid-Air Balance & Wheelies) |
| 🔄 **R Key** | Instant Bike Reset |

---

## 🛠️ Tech Stack
- **Game Engine**: [Matter.js v0.19.0](https://brm.io/matter-js/)
- **Graphics & UI**: HTML5 Canvas & CSS3
- **Language**: Vanilla JavaScript (ES6+)
