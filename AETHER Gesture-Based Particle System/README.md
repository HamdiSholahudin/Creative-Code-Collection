<div align="center">

🪐 AETHER: Gesture-Based Particle System

Interactive 3D Visuals Powered by Hand Gestures & Gemini AI

Created by HamdiSholahudin

</div>

📖 Overview

Aether is a cutting-edge web experiment that combines Computer Vision and Generative AI. It allows users to control 20,000+ 3D particles using hand gestures in real-time.

Additionally, it features an "AI Magic" mode where you can type any description (e.g., "Spiral DNA made of fire"), and Google's Gemini 3 Pro model will generate the mathematical code to render that shape instantly.

✨ Features & Gestures

Gesture

Visual Effect

Fist (✊)

Forms a Blue Saturn Planet with rings.

V-Sign (✌️)

Forms clear 3D Text: "I LOVE YOU" (Gold).

Pinch (🤌)

Forms a Pink Heart shape (Finger Heart).

Open Hand (🖐)

Rainbow Dispersion (Particles explode).

AI Magic (✨)

Generates custom shapes/colors via Gemini API.

🛠️ Technology Stack

Three.js: WebGL rendering engine for high-performance graphics.

MediaPipe Hands: Machine learning pipeline for hand tracking.

Google Gemini API: LLM for generating creative coding logic on the fly.

Tailwind CSS: For the Glassmorphism UI overlay.

🚀 How to Run (Installation)

Since this project uses ES Modules (import syntax), you cannot simply double-click the index.html file. You must run it through a local server.

Option A: Using VS Code (Recommended)

Clone or Download this repository.

Open the folder in Visual Studio Code.

Install the "Live Server" extension by Ritwick Dey.

Right-click on index.html and select "Open with Live Server".

Allow camera access when prompted in the browser.

Option B: Using Python (Terminal)

If you have Python installed, you can create a simple server via terminal:

Open terminal/command prompt in the project folder.

Run:

python -m http.server 8000


Open your browser and go to http://localhost:8000.

🔑 Configuration (Important!)

To use the AI Magic feature, you need a Google Gemini API Key.

Get your key from Google AI Studio.

Open index.html in your code editor.

Find line ~260:

const apiKey = ""; // PUT YOUR API KEY HERE


Paste your key inside the quotes.

🤖 The "Magic" Prompt

Want to recreate this from scratch? Click below to see the prompt used to generate this code.

<details>
<summary><b>Click to reveal the Full Prompt 🪄</b></summary>

Act as a Senior Creative Developer expert in Three.js, WebGL, and Computer Vision.

Create a robust, single-file HTML application: "Gesture-Based Interactive Particle System" integrated with the Google Gemini API.

**1. Technology Stack**
* **Three.js:** Use `BufferGeometry` to handle ~20,000 particles efficiently.
* **MediaPipe Hands:** For real-time hand tracking and gesture recognition.
* **Google Gemini API:** To generate JavaScript code for particle shapes/colors dynamically.
* **Tailwind CSS:** For a modern "Glassmorphism" UI overlay.

**2. Visual & Graphics Requirements**
* **Post-Processing:** Implement `UnrealBloomPass` to give particles a glowing, neon aesthetic.
* **Particle Material:** Use `THREE.PointsMaterial` with vertex colors.
* **Surface Sampling:** For the text "I LOVE YOU", use `MeshSurfaceSampler` (from Three.js examples) to distribute particles evenly on the text surface, ensuring it looks solid and readable (not just vertices).
* **Smooth Animation:** Use Linear Interpolation (Lerp) for all particle movements to ensure smooth transitions between shapes.

**3. Gesture Recognition Logic**
* **Fist (✊):** Particles morph into **Saturn**.
    * *Visuals:* A Blue central sphere with Beige/Gold flat rings.
    * *Animation:* The rings should be tilted and rotate slowly.
* **V-Sign (✌️):** Particles form 3D Text **"I LOVE YOU"**.
    * *Visuals:* Gold color, thick 3D geometry, facing the camera.
* **Finger Heart (🤌):** Particles form a **Heart Shape**.
    * *Logic:* Detect when Thumb and Index tips are close while other fingers are folded. Add tolerance to detection so it's easy to perform.
    * *Visuals:* Pink color.
* **Open Hand (🖐):** Particles disperse into a **Rainbow Sphere**.
    * *Visuals:* Random rainbow colors, particles float with noise.

**4. AI "Magic" Feature (Gemini Integration)**
* Create an "AI Magic" button that opens a modal.
* Allow the user to type a text prompt (e.g., "Spiral DNA" or "Matrix Rain").
* **API Call:** Send this prompt to the Gemini API.
* **Instruction to AI:** Ask Gemini to generate *only* the raw JavaScript loop code to calculate `targetPositions` and `targetColors` arrays based on the math of the described shape.
* **Execution:** Use `new Function()` to safely execute the returned code and update the particle system in real-time.

**5. UI & UX**
* **Camera:** Display a large, mirrored webcam preview (flipped horizontally).
* **Controls:** Include a Color Picker and a Fullscreen button.
* **Feedback:** Show the current detected gesture name on screen.
* **Loading:** Add a loading overlay while fonts and MediaPipe models initialize.

**6. Camera Setup**
* Set the Three.js camera position (z=35) so objects appear large and fill the screen nicely.

Produce the complete `index.html` code with all scripts and styles included.


</details>

<div align="center">

Star this repo if you find it cool! ⭐
Visit my GitHub Profile

</div>
