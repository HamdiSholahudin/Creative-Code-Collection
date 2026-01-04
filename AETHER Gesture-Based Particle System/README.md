<div align="center">

🪐 **AETHER**  
*Gesture-Based Interactive Particle System*  

**Control thousands of 3D particles with your bare hands — in real time.**

<br/>

<!-- Badges -->
<img src="https://img.shields.io/badge/Three.js-WebGL-black?style=flat-square&logo=three.js">
<img src="https://img.shields.io/badge/MediaPipe-Computer%20Vision-blue?style=flat-square">
<img src="https://img.shields.io/badge/Gemini%203%20Pro-Generative%20AI-purple?style=flat-square">
<img src="https://img.shields.io/badge/Status-Experimental-orange?style=flat-square">

<br/><br/>

<!-- Project Preview -->
<img src="./assets/preview.gif" width="85%">

</div>

---

## 🔮 About The Project

AETHER is not just another particle demo.  
It is a creative coding experiment that blends:

- 🧮 Mathematical beauty  
- 👁️ Computer Vision (real-time hand tracking)  
- 🤖 Generative AI (Google Gemini)  

Imagine controlling thousands of glowing particles in 3D space using nothing but your hands — all running directly in the browser.

### ✨ Gesture System

| Gesture          | Visual Effect     | Description                            |
| ---------------- | ---------------- | -------------------------------------- |
| ✊ **Fist**       | 🪐 Saturn Planet  | Blue sphere with rotating cosmic rings |
| ✌️ **V-Sign**    | 💛 I LOVE YOU     | Dense glowing golden 3D text           |
| 🤌 **Pinch**     | 💗 Heart Shape    | Pink finger-heart formation            |
| 🖐 **Open Hand** | 🌈 Rainbow Boom   | Colorful particle dispersion           |

### 🧠 AI Magic (Generative Mode)

Click **AI Magic**, then type prompts like:

- Spiral DNA  
- Cyberpunk Vortex  
- Golden Flower of Life  

**Gemini will:**  
- Generate JavaScript logic  
- Modify particle shapes, motion, and colors  
- Apply everything live to the 3D scene  

Human imagination → AI code → real-time visuals

---

## 🛠️ Tech Stack

- **Three.js** — WebGL particle engine (~20,000 particles)  
- **MediaPipe Hands** — Real-time hand tracking  
- **Google Gemini API** — Generative logic  
- **Tailwind CSS** — Glassmorphism UI  
- **UnrealBloomPass** — Neon glow  
- **MeshSurfaceSampler** — Dense 3D text  
- **Smooth Lerp** — Jitter-free motion  

---

## 🚀 Installation

⚠️ This project requires a local server due to ES Modules.

### Quick Start (VS Code)
1. Clone the repository  
2. Open the folder in Visual Studio Code  
3. Install **Live Server** extension  
4. Right-click `index.html` → **Open with Live Server**

### Manual Setup (Terminal)
```bash
# Clone repository
git clone https://github.com/HamdiSholahudin/Creative-Code-Collection.git

# Navigate to project
cd Creative-Code-Collection/Aether-Gesture-Particles

# Run local server
python -m http.server 8000
