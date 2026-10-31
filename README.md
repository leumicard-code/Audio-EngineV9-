 Audio Engine (Elegance Edition) — V9
[![Language: Rust](https://img.shields.io/badge/Language-Rust_2024-orange.svg)](https://www.rust-lang.org/)
[![UI: egui / eframe](https://img.shields.io/badge/UI-egui_0.36-blue.svg)](https://github.com/emilk/egui)
[![Audio: GStreamer](https://img.shields.io/badge/Audio-GStreamer_0.22-red.svg)](https://gstreamer.freedesktop.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](#license)
**Audio Engine (Elegance Edition)** is a high-performance, studio-grade desktop audio player and DSP suite written in **Rust**.  
Combining a sleek, modern dark-mode GUI powered by `egui` with a zero-latency audio pipeline built on `GStreamer`, it delivers audiophile-grade playback, real-time 64-band spectrum visualization, an interactive 10-band equalizer, and intelligent anti-clipping headroom management.
![Audio Player Main Window](assets/player_screenshot.png)
---
## ✨ Features
- 🎧 **Audiophile DSP & Equalizer Studio**:
  - **10-Band Graphic Equalizer** with frequency points tuned to standard octaves: `29 Hz`, `59 Hz`, `119 Hz`, `237 Hz`, `474 Hz`, `947 Hz`, `1.9 kHz`, `3.8 kHz`, `7.5 kHz`, and `15 kHz`.
  - **Studio Presets**: Instant one-click presets including *Flat*, *Warm Vintage*, *Modern Clean*, *Bass Boosted*, *Vocal Enhancer*, and *Club Master*.
  - **Smart Anti-Clipping Pre-Gain (Auto Headroom)**: Dynamically calculates required headroom to prevent digital distortion and harmonic clipping when boosting EQ bands.
  - **Sub-Bass Enhancer & Stereo Balance**: Low-end punch booster up to +12 dB with smooth L/R pan control.
- 〰️ **Real-Time Spectrum Visualizer**:
  - Live frequency spectrum analysis running at 60 FPS directly within the main player view.
  - Dynamic smooth gradient rendering transitions from cyan/turquoise to neon magenta.
- 📜 **Seamless Playlist & Media Library**:
  - Drag-and-drop audio files or entire directories on the fly.
  - Real-time search and filter with instant results.
  - Automatic metadata tag reading (Title, Artist, Album, Duration).
  - Context menu actions, quick track removal, and persistent playback state across launches.
- 🎛️ **Universal Audio Codec Support**:
  - Plays MP3, FLAC, WAV, OGG, M4A, AAC, Opus, and more through GStreamer's native `decodebin`.
---
## 🎚️ Equalizer & DSP Studio
The DSP Equalizer runs in a dedicated studio window for precision sound tweaking:
![Equalizer Studio](assets/eq_screenshot.png)
