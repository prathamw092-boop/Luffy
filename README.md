<div align="center">

  <h1>🔥 GEAR SECOND — 二段</h1>
  <p><strong>A Scroll-Driven 3D Immersive Landing Experience for Monkey D. Luffy</strong></p>

  <p>
    <a href="https://react.dev/"><img src="https://img.shields.io/badge/React-19.0-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19"></a>
    <a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/Vite-8.1-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite 8"></a>
    <a href="https://threejs.org/"><img src="https://img.shields.io/badge/Three.js-r185-000000?style=for-the-badge&logo=three.js&logoColor=white" alt="Three.js"></a>
    <a href="https://gsap.com/"><img src="https://img.shields.io/badge/GSAP-3.15-88CE02?style=for-the-badge&logo=greensock&logoColor=black" alt="GSAP"></a>
    <a href="https://www.framer.com/motion/"><img src="https://img.shields.io/badge/Framer_Motion-12.4-0055FF?style=for-the-badge&logo=framer&logoColor=white" alt="Framer Motion"></a>
  </p>

</div>

---

## ⚡ Overview

**GEAR SECOND** is a scroll-driven web experience inspired by One Piece's iconic Monkey D. Luffy transformation. As the user scrolls down the page, Luffy's legendary Straw Hat descends through a dynamic 3D space, triggering dynamic Japanese kanji parallax, WebGL smoke and red lightning particle effects, backdrop atmospheric transformations, and camera shake upon landing.

Designed with cinematic depth, custom GLSL/Canvas FX, and zero scroll-jacking to maintain native scroll performance.

---

## ✨ Key Features

- **🎯 3D Scroll Synchronization:** Real-time synchronized Three.js canvas scrubbed directly by GSAP `ScrollTrigger` with zero lag or frame desynchronization.
- **⚡ Custom WebGL & Canvas Effects:**
  - Dynamic **Lightning & Smoke Particle FX** rendering in real-time on WebGL canvas.
  - Interactive **Fluid Red Splash Cursor** tracking mouse movement across the screen.
  - **Ambient Thunder System** generating organic red lightning strikes independently of scroll.
  - **Parallax Kanji Glyphs** falling at varied depth layers.
- **💥 Impact Transformation Sequence:**
  - Seamless background plate cross-fade to Gear Second aura (`bg.jpg` → `transition.jpg`).
  - Screen camera shake with 22 damped keyframe oscillations on landing.
  - Dramatic slam of the **二段 GEAR SECOND** impact stamp.
- **🎨 Modern Anime HUD & Manga Typography:**
  - Vertical Japanese *Tategaki* side margin rails (`海賊王に俺はなる` / `麦わらの一味`).
  - Animated HUD state indicators tracking scroll descent (`STATE: DESCENDING` → `GEAR SECOND`).

---

## 🛠️ Tech Stack & Architecture

| Category | Technology | Usage |
| :--- | :--- | :--- |
| **Core Framework** | React 19 + Vite 8 | Ultra-fast HMR & ESM module bundle |
| **3D Rendering** | Three.js + `@react-three/fiber` + `@react-three/drei` | 3D model loading (Straw Hat GLTF), camera control, lighting |
| **Animation Engine** | GSAP 3 + ScrollTrigger | Master timeline orchestrator driving WebGL & DOM elements |
| **UI Micro-Animations** | Framer Motion | Text blur-ins, smooth UI cues, HUD transitions |
| **Canvas & Shaders** | Native HTML5 Canvas / OGL | Particle engines, ambient lightning bolts, splash fluid |
| **Styling & Fonts** | Vanilla CSS + Google Fonts | Space Mono, Anton, Bebas Neue, Noto Sans JP |

---

## 📁 Project Structure

```
luffys_gear_2nd/
├── public/
│   ├── images/              # Background plates & Luffy cutouts
│   ├── models/              # 3D Straw Hat GLTF model & textures
│   ├── favicon.svg          # Custom SVG favicon
│   └── icons.svg            # UI vector icons
├── src/
│   ├── components/
│   │   ├── AmbientThunder.jsx   # Procedural red lightning strike generator
│   │   ├── FallingKanji.jsx     # Parallax floating Japanese glyphs
│   │   ├── LightningSmokeFX.jsx # WebGL smoke & lightning canvas overlay
│   │   ├── LuffyCutout.jsx      # Layered image transformation components
│   │   ├── Scene3D.jsx          # React Three Fiber canvas & 3D model handler
│   │   └── ScrollExperience.jsx # Master GSAP timeline orchestrator
│   ├── lib/
│   │   ├── math.js              # Vector & interpolation utilities
│   │   ├── rng.js               # Seeded random number generation
│   │   └── timeline.js          # Normalized scroll keyframes & timing constants
│   ├── reactbits/               # High-performance UI components
│   │   ├── BlurText/            # Staggered letter blur entrance
│   │   ├── Particles/           # WebGL starfield depth background
│   │   ├── ShinyText/           # Metallic text gradient animation
│   │   └── SplashCursor/        # Interactive fluid dissipation cursor
│   ├── App.jsx                  # Main entry component
│   ├── index.css                # Global styling & layout tokens
│   └── main.jsx                 # React DOM root setup
├── package.json
├── vite.config.js
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v18.0.0 or higher recommended)
- **npm** / **yarn** / **pnpm**

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Prathamwadiyar/luffys_gear_2nd.git
   cd luffys_gear_2nd
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Launch local development server:
   ```bash
   npm run dev
   ```
   Open `http://localhost:5173` in your browser to view the project.

4. Build for production:
   ```bash
   npm run build
   ```

---

## 👤 Author

Developed and Maintained by **Prathamwadiyar**

- **GitHub:** [@Prathamwadiyar](https://github.com/Prathamwadiyar)
- **Email:** [prathamwadiyar@gmail.com](mailto:prathamwadiyar@gmail.com)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
