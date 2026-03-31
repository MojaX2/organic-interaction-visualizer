# Organic Interaction Visualizer

A lightweight, high-performance web-based visualizer designed to provide "living" feedback for human-AI interactions using the Web Audio API.

## Overview

This project provides a fluid, biomorphic visual representation for voice-based AI agents. Unlike traditional waveform displays, it uses a 12-to-60 point spline-based geometry that pulses and morphs based on real-time audio amplitude, creating a sense of "presence" and "physicality" for the digital agent.

## Key Features

- **Dual-Source Analysis**: Simultaneously monitors local microphone (User) and system audio (AI) via separate analysers.
- **Priority Logic**: AI audio is prioritized. When the agent speaks, the visualizer locks into "AI mode" to maintain the agent's presence.
- **State-Hold Mechanism**: Implements a 500ms state-locking logic to prevent flickering between user and AI modes during brief pauses.
- **Advanced Control Panel**: Real-time tuning of thresholds, sensitivity, colors, vertex counts, and state-hold duration directly in the browser.
- **Biomorphic Animation**: Features an "idling pulse" that simulates breathing or a heartbeat even when no audio is detected.

## Setup & Usage

1. **Prerequisites**: Requires a secure context (**HTTPS** or **localhost**) to access Web Audio and MediaDevices.
2. **Connection**:
   - **Step 1**: Click "1. Connect Microphone" to bind your local voice.
   - **Step 2**: Click "2. Connect AI Voice" and select the browser tab playing the AI's audio. **Ensure "Share system audio" is checked.**
3. **Tuning**: Open "Advanced Settings" in the top-left to adjust sensitivity and thresholds based on your environment.

## To-Do / Roadmap

- [ ] **Virtual Audio Device Support**: Add a guide for integrating tools like BlackHole to eliminate the browser's "Sharing" bar.
- [ ] **Frequency-Linked Morphing**: Implement logic to change the blob's complexity based on pitch/frequency characteristics.
- [ ] **PWA Implementation**: Add a manifest to allow the visualizer to be installed as a standalone app for cleaner demos.
- [ ] **WebSocket Triggering**: Support external events (e.g., from an LLM server) to force state changes or "thinking" animations.

## License

MIT License
