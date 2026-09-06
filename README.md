# 🎵 Spatial Audio Head Tracker

A real-time spatial audio experience controlled by your head movements and eye state. Turn your head left and right to pan audio in stereo, close your eyes to trigger a lush V-shaped EQ preset, and enjoy your music library with embedded cover art.

## ✨ Features

- **Head-Tracked Panning** — Your head rotation controls where you hear the audio. Bass stays centered for punch; mids pan naturally with your head movement.
- **Eye-State EQ** — Close your eyes → lush V-shaped EQ (bass and treble boost). Open your eyes → flat, neutral tone.
- **Song Library** — Add multiple MP3/FLAC files. Cover art, title, and artist are read automatically from ID3/FLAC tags.
- **3-Band Audio Processing** — Bass (< 300 Hz) universal. Mids (300–4700 Hz) pan with your head. Treble (> 4700 Hz) independently tunable.
- **Advanced Controls** — Tweak sensitivity, crossover frequencies, pan curves, and more via the DEV panel.

## 🚀 Quick Start

1. **Open the app:** Visit your deployed GitHub Pages link
2. **Allow camera:** Click "Start Camera" and permit webcam access
3. **Add songs:** Tap the "+" button to select MP3 or FLAC files
4. **Play:** Click any song to load it, then hit the native play button
5. **Experience:** Turn your head left/right to pan. Close your eyes for the EQ effect.

## 🎧 Best Experience

- **Headphones recommended** — spatial panning works best with stereo headphones
- **Good lighting** — helps your webcam track your head smoothly
- **Distance:** Sit 12–24 inches from your camera
- **MP3/FLAC with tags:** Songs with embedded cover art display nicely in the library

## 📋 Default Settings

| Setting | Value |
|---------|-------|
| Eyes Open Sensitivity | 0.7 |
| Eyes Closed Sensitivity | 1.3 |
| Pan Curve (Center Damping) | 1.8 |
| Bass/Mid Crossover | 300 Hz |
| Mid/Treble Crossover | 4700 Hz |
| Crossover Smoothness | 0.30 (smooth) |
| Treble Pan Behavior | −100% (opposite ear) |
| Mid Pan Attenuation | −0.5 dB |

## 🛠️ Technical Stack

- **Audio:** Web Audio API (10-band EQ, 4th-order Linkwitz-Riley crossover, safety limiter, real-time panning)
- **Head Tracking:** MediaPipe Face Mesh (runs 100% in-browser)
- **Metadata:** jsmediatags (reads ID3v2/FLAC tags from local files)
- **UI:** Tailwind CSS
- **Privacy:** Everything runs on your device — no server, no cloud upload

## 🌐 Browser Support

- ✅ Chrome, Edge, Firefox (Windows/Mac/Linux)
- ✅ Safari (iOS 14.5+)
- ✅ Chrome/Edge (Android)
- ⚠️ Requires HTTPS (GitHub Pages handles this automatically)
- ⚠️ Requires camera permission

## 🎯 Tips for Best Results

- If panning feels too sensitive, lower "Eyes Open Sensitivity" or raise "Pan Curve"
- If you don't see cover art, make sure your MP3/FLAC files have embedded ID3 tags
- Adjust "Crossover Smoothness" lower for a gentler blend between bass/mids/treble, higher for a tighter split
- Try "Treble Pan Behavior" at different values to find your sweet spot

## 📱 Mobile

Works on iOS and Android! Safari on iOS requires explicit camera permission each time.

## 🔧 Advanced Customization

All settings are sliders in the "[DEV]" panel. No code changes needed — just tweak and enjoy.

## 📄 License

MIT — free to use, modify, and share.

---

**Enjoy your spatial audio experience!** 🎶
