# 🌐 Textured 3D Sphere (HTML Canvas)

This project renders a textured 3D sphere onto an HTML5 `<canvas>` element using JavaScript. It simulates 3D geometry and rotates the sphere in real time by mapping an equirectangular image texture across thousands of computed points on the sphere’s surface.

---

## 🚀 Features

- Real-time rotation around the Y-axis
- Texture mapping from a flat world map
- Perspective projection and scale-based depth illusion
- Lightweight: no libraries, WebGL, or frameworks required

---

## 📁 How It Works

1. A canvas is created and sized to the browser window.
2. Randomized points are distributed over a virtual sphere using spherical coordinates.
3. Each point is rotated and projected to 2D space with perspective scaling.
4. UV coordinates are calculated dynamically for each rotated point.
5. Colors are sampled from a texture image (`imgData`) and used to draw the point.
6. This process repeats in an animation loop to simulate rotation.

---

## 🖼️ Texture

By default, the globe uses:
https://upload.wikimedia.org/wikipedia/commons/8/83/Equirectangular_projection_SW.jpg



> You can replace it with any **equirectangular map projection** by modifying the `img.src` value in the script.

---

## 🧪 Quick Start

1. Clone or download the HTML file.
2. Serve it using a local server (e.g. VS Code Live Server or `python -m http.server`).
3. Open in your browser and enjoy the animated sphere.

---

## 🔧 Customization

- `radius`: Controls the size of the sphere.
- `totalPoints`: Controls rendering resolution (7000–10000 gives a smooth result).
- `rotation`: Adjust for spin speed or direction.
- `img.src`: Swap for another texture or pattern.

---

## 🎯 Example Use Cases

- Creative coding demonstrations
- Planet simulation
- Data-driven globe visualizations (e.g. meteor impacts, satellite tracking)

---

## 📄 License

This is an open educational project for experimentation and learning. Feel free to adapt, remix, and share.
