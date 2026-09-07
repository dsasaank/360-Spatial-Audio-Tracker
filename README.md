# 360 Spatial Audio Tracker
**Step inside the sound.**

A browser-based spatial audio engine that uses your webcam to track your head movements and map music around you in real-time 3D space. 

## Features
* **360° Head Tracking:** Turn your head to pan the audio dynamically using MediaPipe Face Mesh.
* **Blink Detection:** Close your eyes to trigger a "Dream State" (activates a custom 10-band EQ and massive inverse binaural reverb).
* **Audiophile DSP:** Custom crossover networks keep bass grounded while mids and highs pan seamlessly.
* **Zero Installation:** Runs entirely client-side. No server required.

## Upcoming Features
* **Audio-Only Mode:** Ability to disable head tracking so you can sit back, work, and just listen to the custom DSP and EQ routing without needing to stay centered on camera.

## How to Use
1. Clone or download this repository.
2. Open `index.html` in any modern web browser.
3. Allow webcam access (vision processing is 100% local, no video is recorded).
4. Upload an audio file (MP3/FLAC), hit play, and initiate tracking.

## Tech Stack
* **Audio:** Web Audio API 
* **Vision:** MediaPipe Face Mesh
* **UI/UX:** HTML, JavaScript, Tailwind CSS

---
*Built by [Sasaank Dake](https://github.com/dsasaank)*
