# 🌌 PROJECT: SATURN  
**A hand-tracked, interactive particle simulation of Saturn built with Three.js + MediaPipe Hands**

Project Saturn is an experimental WebGL experience that lets you **assemble, scatter, rotate, and compress a particle-based Saturn** using nothing but **your hand in front of your webcam**.  
The entire planet, including thousands of particles forming the globe and ring, reacts to your gestures in real time.

---
## 🖼️ Demo Screenshots

### ✨ Saturn Fully Assembled
![Saturn Assembled](<img width="1525" height="801" alt="image" src="https://github.com/user-attachments/assets/d74b6b12-7c17-41d4-8621-24f62b8c69a0" />
)

### 💥 Scatter Mode (No Hand Detected)
![Scatter Mode](<img width="1499" height="840" alt="image" src="https://github.com/user-attachments/assets/37ec64fa-d882-4f88-a6f3-672e6a5e5173" />
)

### 👌 Pinch → Shrink Mode
![Shrink Mode](<img width="1514" height="814" alt="image" src="https://github.com/user-attachments/assets/499f73c6-3864-4520-90a3-a482eccdd29b" />
)


## 🚀 Features

### ✋ Real-time Hand Tracking  
Powered by **MediaPipe Hands**, the system detects:
- **No Hand → SCATTER**  
  Particles explode outward into deep space.  
- **Open Hand → ASSEMBLE**  
  Saturn reforms smoothly into its spherical body and rings.  
- **Pinch Gesture → SHRINK**  
  Compress the planet into a dense, glowing core.  
- **Move Hand → ROTATE**  
  Tilt and spin Saturn by moving your hand horizontally or vertically.

### 🪐 10,000 Particle Saturn  
- **4,000 planet particles**  
- **6,000 pure-white ring particles**  
- Smooth transitions between scatter/assemble/shrink  
- Additive blending & glowing particle sprite  
- Slight natural tilt applied to the rings

### 🎥 Debug Camera View  
A small mirrored camera feed helps you see exactly what MediaPipe is tracking.

---

## 🧩 Tech Stack
- **Three.js** (particle rendering & scene animation)  
- **MediaPipe Hands** (gesture recognition)  
- **HTML + JavaScript modules**  
- **WebGL2** via Three.js renderer  

---

## 📁 How It Works (Overview)

### Particle Systems  
- Each particle has:
  - `currentPositions`  
  - `targetPositions` (planet shape)  
  - `scatterPositions` (deep-space scatter)  
- Smooth interpolation blends between states at different speeds.

### Gestures  
- **Pinch distance** (thumb–index) toggles SHRINK mode.  
- **Hand presence** controls SCATTER vs ASSEMBLE.  
- **Index finger coordinates** map to rotation smoothing.

---

## ▶️ Run It  
Just open the HTML file in any browser that supports WebGL & webcam access (Chrome recommended).

> ⚠️ Requires webcam permissions.

---

## 🖼️ Demo (What You’ll See)
- Saturn assembles from a cloud of particles  
- Rings align beautifully  
- Moving your hand rotates the entire system  
- Pinch compresses the planet inward  
- Removing your hand sends it exploding outward again  

---

## 📜 License
MIT License — free to use, remix, and experiment with.

---

## ⭐ Contribute
Feel free to:
- Add new gestures  
- Improve ring physics  
- Add moons  
- Add UI buttons / VR support  
- Port it to React Three Fiber  

Pull requests welcome!

---

## 💬 Author Notes
This project blends **creative coding**, **gesture interaction**, and **GPU-accelerated particle animation** into a single cinematic experiment.  
Have fun bending a tiny universe with your hands!  
