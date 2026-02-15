# 🐴 Neigh - CNY Trojan Horse Minigame

A Chinese New Year themed browser game with a Windows 2000 aesthetic. Battle through waves of popup windows in this single-file HTML game featuring glitchGL shader effects, zodiac animals, and plenty of horse puns.

## 🎮 Play

Open `index.html` in a modern web browser (Chrome/Firefox/Safari recommended).

**Controls:**
- Click to close windows
- Click the boss 8 times to defeat it
- The boss flees from your cursor!

## ✨ Features

- **3 Stages of Chaos**: Floating windows → Diagonal zodiac line → Boss battle with dummy distractions
- **Windows 2000 Aesthetic**: Authentic Win2000 window styling with chromatic aberration hover effects
- **glitchGL Shader Effects**: WebGL-powered visual glitches that intensify each stage
- **Mobile Friendly**: Responsive design with touch support
- **Single File**: Entire game in one HTML file (~3200 lines)
- **Audio**: Wind ambience, background music, victory fanfare, horse neighs
- **10 Horse Puns**: Non-interactive dummy windows with terrible horse jokes

## 🎯 Gameplay

1. **Stage 1**: 8 floating windows spawn. Close 6 to advance.
2. **Stage 2**: 12 zodiac windows appear in a diagonal line that pivots. Dummy distraction windows begin spawning (1/sec, max 12).
3. **Stage 3**: Click the Horse zodiac to activate boss mode. The boss flees from your cursor. Dummy spawning accelerates (2/sec, max 24). Click the boss 8 times to win!

## 🛠 Tech Stack

- **HTML5 Canvas/Video**
- **Vanilla JavaScript** (ES5 for compatibility)
- **CSS3** (animations, blend modes, responsive media queries)
- **[three.js r128](https://threejs.org/)** - WebGL rendering
- **glitchGL** - Custom shader effect library

## 📁 Project Structure

```
neigh/
├── index.html              # Main game file (single-file architecture)
├── scripts/
│   └── glitchGL.min.js    # WebGL shader effects library
└── 00_assets/
    ├── audio/             # 6 MP3 files (sfx, music, ambience)
    ├── fonts/             # MS Sans Serif TTF (regular + bold)
    ├── horsemp4/          # 4 MP4 videos (horse animations, starbursts)
    ├── intro/
    │   ├── *.mp4          # 4 intro sequence videos
    │   └── grain/         # 10-frame grain overlay PNG sequence
    ├── OUTRO/             # 38-frame victory animation PNG sequence
    ├── bg.mp4             # Background glitch video
    ├── main_bg.png        # Start screen background
    ├── warning.png        # Window icon
    └── horse_head.svg     # Custom glitchGL interaction shape
```

## 🎨 Development

The game uses a single-file architecture with embedded CSS and JavaScript for portability. All assets are referenced via relative paths.

**Key Systems:**
- **Stage Manager**: Three-stage progression system
- **Window Spawner**: Procedural popup generation with configurable types/behaviors
- **Movement System**: Float, diagonal pivot, boss flee mechanics
- **glitchGL Integration**: Dynamic pixelation, custom interaction shapes
- **Mobile Scaling**: Viewport-responsive window sizes and touch event handlers

## 📱 Mobile Support

- **Portrait Crop**: Intro videos show the left ~520px (important content area)
- **Scaled Windows**: Game windows auto-scale based on viewport width
- **Touch Events**: Boss flee and shader interaction work with finger tracking
- **Smaller Horse**: 75vh on mobile (vs 70vh on desktop) to leave room for windows
- **Reduced Dummy Count**: 8/16 max (vs 12/24 on desktop) for performance

## 🐛 Known Issues

None! Ship it! 🚢

## 📜 License

[Add your license here]

## 🙏 Credits

Built with love for Chinese New Year 2025 (Year of the Snake... wait, Horse? 🐴)
