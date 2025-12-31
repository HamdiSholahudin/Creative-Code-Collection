<div align="center">

🪐 AETHER: Gesture-Based Particle System

Control 3D Particles with Your Hand


</div>

🔮 About The Project

Aether bukan sekadar partikel biasa. Ini adalah eksperimen Creative Coding yang menggabungkan keindahan matematika, visi komputer (Computer Vision), dan kecerdasan buatan (Generative AI).

Bayangkan mengendalikan ribuan bintang di layar hanya dengan mengepalkan tangan atau menjentikkan jari. Aether mewujudkannya langsung di browser Anda.

✨ Key Features

Gesture

Visual Effect

Description

✊ Fist

Saturn Planet

Membentuk planet biru dengan cincin yang berputar.

✌️ V-Sign

"I LOVE YOU"

Partikel menyusun teks 3D emas yang padat & berkilau.

🤌 Pinch

Heart Shape

Membentuk hati berwarna pink (Finger Heart style).

🖐 Open

Rainbow Boom

Ledakan partikel warna-warni (Dispersion).

✨ AI Magic

Gemini Powered

Ketik imajinasimu (misal: "Spiral DNA"), AI yang akan koding visualnya!

🛠️ Installation

Project ini butuh Local Server karena menggunakan ES Modules modern.

Cara Cepat (VS Code)

Clone repo ini ke komputer.

Buka folder di Visual Studio Code.

Install Ekstensi Live Server.

Klik kanan index.html > pilih Open with Live Server.

Cara Manual (Terminal)

# Clone repository
git clone [https://github.com/HamdiSholahudin/Creative-Code-Collection.git](https://github.com/HamdiSholahudin/Creative-Code-Collection.git)

# Masuk ke folder
cd Creative-Code-Collection/Aether-Gesture-Particles

# Jalankan server (Python)
python -m http.server 8000


⚡ The "Magic" Prompt

Ini adalah prompt rahasia yang digunakan untuk men-generate kode inti proyek ini menggunakan Gemini 3 Pro. Copy prompt ini jika kamu ingin mencoba membuatnya sendiri!

Act as a Senior Creative Developer expert in Three.js, WebGL, and Computer Vision.

Create a robust, single-file HTML application: "Gesture-Based Interactive Particle System" integrated with the Google Gemini API.

**Tech Stack:**
1. Three.js (BufferGeometry, ~20k particles).
2. MediaPipe Hands (Real-time tracking).
3. Google Gemini API (Generative logic for shapes/colors).
4. Tailwind CSS (Glassmorphism UI).

**✨ Core Visuals:**
- Use UnrealBloomPass for a neon/glowing effect.
- Use MeshSurfaceSampler for dense, clear 3D Text.
- Smooth Lerp interpolation for all movements (no jitter).

**✋ Gesture Logic:**
1. Fist ✊       -> Form a Saturn Planet (Blue sphere, Beige rings).
2. Open Hand 🖐  -> Rainbow Sphere explosion.
3. V-Sign ✌️     -> Form 3D Text "I LOVE YOU" (Gold).
4. Pinch 🤌      -> Form a Pink Heart shape.

**🤖 AI Features:**
- "AI Magic" button to open a prompt modal.
- User types: "Spiral DNA" -> Gemini writes JS loop code -> Particles reshape.
- User types: "Cyberpunk" -> Gemini writes JS loop code -> Particles recolor.

**UI Requirements:**
- Minimalist Glassmorphism panel.
- Large, mirrored webcam preview.
- Fullscreen & Color Picker support.


🔑 Configuration

Agar fitur AI Magic berjalan, kamu butuh API Key gratis dari Google:

Dapatkan key di Google AI Studio.

Buka index.html.

Paste key kamu di baris ~260:

const apiKey = "PASTE_YOUR_API_KEY_HERE";


<div align="center">

Built with ❤️ using Gemini 3 Pro
Follow for more creative coding contents!

</div>
