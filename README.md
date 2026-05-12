# 🖐️ Quantum Hands — Real-Time Hand Tracking with Neon Visual Effects

**Quantum Hands** is a browser-based, real-time hand tracking application that transforms your webcam feed into an interactive visual experience. Built as a single, self-contained HTML file with zero build steps or external frameworks, it leverages Google's **MediaPipe Hands** AI model to detect and track hand landmarks, then renders stunning **neon-glitch visual effects** on a canvas overlay.

## ✨ Features

- **Real-Time Hand Detection** — Tracks up to 2 hands simultaneously using MediaPipe's `HandLandmarker` with GPU acceleration, detecting all 21 hand landmarks per hand.
- **Neon Skeleton Rendering** — Draws a glowing, multi-layered skeletal structure over detected hands with outer glow, mid-tone, and core line passes for a depth-rich visual effect.
- **Fingertip Glow Orbs** — Radial gradient orbs rendered on each fingertip using an offscreen canvas for optimized performance.
- **Pinch Detection & Electric Arcs** — Detects thumb-to-index pinch gestures and renders dynamic, jittery electric arc effects between the fingertips.
- **Inter-Hand Glitch Ribbons** — When two hands are detected, glitchy neon ribbons with chromatic ghost effects connect corresponding fingertips, creating a visually striking interaction.
- **Particle Glitch Dots** — Randomized, per-frame glitch particles scatter around hand landmarks for added visual dynamism.
- **Smooth Trail Fading** — Uses canvas compositing (`destination-out` + `lighter` blend modes) for smooth, trailing afterglow effects.
- **Fully Responsive** — Adapts to any screen size; the canvas and video feed resize dynamically.
- **Graceful Error Handling** — Clear, user-friendly messages for camera permission denial, missing devices, or network failures when loading the AI model.

## 🛠️ Tech Stack

- **HTML5 Canvas** for all visual rendering
- **MediaPipe Tasks Vision SDK** (loaded via CDN) for hand landmark detection
- **Vanilla JavaScript (ES Modules)** — no frameworks, no build tools, no dependencies to install
- **CSS** with neon-themed styling, glowing buttons, and a dark radial-gradient UI

## 🚀 Getting Started

Simply open `quantum-hands.html` in any modern browser (Chrome/Edge recommended for best GPU support), click **"Start Camera"**, grant camera access, and move your hands in front of the webcam.

No installation, no `npm install`, no server required — just open and play.

---
