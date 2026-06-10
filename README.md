# KBCPS Virtual Tour

An interactive **360-degree virtual campus tour** for **KB CBSE School**, built using the [TheDarkValley (TDV) Virtual Tour Player](https://www.thedarkvalley.com/) platform.

## Overview

This project provides an immersive web-based experience that allows students, parents, and visitors to explore the school campus remotely from any device — including VR headsets.

## Campus Locations

| # | Location | Type |
|---|----------|------|
| 00 | KB CBSE Drone 01 | Aerial View |
| 00 | KB CBSE Drone 02 | Aerial View |
| 01 | KB CBSE | Main Building |
| 02 | KB CBSE | Main Building |
| 04 | KB CBSE Reception | Reception Area |
| 05 | KB CBSE Principal Office | Admin |
| 06 | KB CBSE Computer Lab 01 | Lab |
| 07 | KB CBSE Computer Lab 02 | Lab |
| 08 | KB CBSE Lab 01 | Science Lab |
| 09 | KB CBSE Lab 02 | Science Lab |
| -- | Class 02 - Class 07 | Classrooms |

## Features

- **360° Panoramic Views** — Cube-map rendered panoramas for seamless exploration
- **Multi-Device Support** — Desktop, Mobile, iPad, and VR headsets
- **VR Ready** — Compatible with Oculus Quest 2/3, Pico 4, HTC Vive Focus, and Google Cardboard
- **Quiz System** — Built-in interactive quiz and trivia functionality
- **Text-to-Speech** — Audio narration support for accessibility
- **Multi-Language** — Localization system with English as default
- **Responsive Design** — Adapts to all screen sizes and orientations

## Tech Stack

- **TDV Player** — Core virtual tour rendering engine
- **HTML5 / CSS3 / JavaScript** — Frontend technologies
- **WebVR / WebXR Polyfill** — VR headset compatibility
- **HLS.js** — HTTP Live Streaming support

## Project Structure

```
KBCPS/
├── index.htm              # Entry point
├── script.js              # Tour initialization & core logic
├── script_general.js      # Quiz, TTS, localization, components
├── thumbnail.png          # Tour thumbnail
├── lib/                   # TDV Player libraries
│   ├── tdvplayer.js       # Main player engine
│   ├── WebVRPolyfill.js   # VR compatibility
│   ├── Hls.js             # Video streaming
│   └── ...
├── locale/                # Language files
│   └── en.txt             # English translations
└── media/                 # 360° panoramic images
    ├── panorama_*/        # Cube-map panoramas (r/l/f/b/u/d)
    └── ...
```

## Deployment

This is a static site with no build step required. Deploy to any static hosting platform:

### Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy from project root
vercel --prod
```

### Netlify / GitHub Pages
Simply drag-and-drop the `KBCPS/` folder or configure your repo's root directory to point here.

## License

This project uses the **TDV Virtual Tour Player** platform. Please refer to [TheDarkValley](https://www.thedarkvalley.com/) for licensing terms.
