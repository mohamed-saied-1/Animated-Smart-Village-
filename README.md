# 🏘️ Animated Smart Village & Aircraft (3D OpenGL Simulation)

## 📝 Project Overview
**Animated Smart Village** is a dynamic 3D graphics simulation developed using **C++** and **OpenGL (GLUT/GLU)**. The project showcases a detailed "Smart Village" environment featuring real-time rendering of buildings, solar panels, windmills, and a fully functional flying aircraft. 

The core focus of this project is to demonstrate advanced graphics concepts like **Day/Night cycles**, dynamic lighting, and interactive camera systems within a complex 3D scene.

---

## 🌟 Key Features

### 1. Dynamic Environment & Lighting
* **Day/Night Cycle:** Implementation of a smooth transition between day and night based on the sun's trajectory.
* **Atmospheric Effects:** Interpolated fog and sky color changes using trigonometric functions to simulate realistic lighting.
* **Smart Streetlights:** Night mode triggers emissive material properties and localized light sources to simulate glowing streetlamps.

### 2. Complex 3D Modeling & Animation
* **Kinematic Animations:** Rotating windmills and solar panels that track "light" sources.
* **Animated Aircraft:** A fly-through aircraft with altitude control and smooth flight mechanics.
* **Procedural Details:** Dashed road lines, detailed tree models, and structured buildings using primitives (Quads, Triangles, Fans).

### 3. Interactive Navigation System
* **Dual-Mode Camera:**
    * **Orbit Mode:** Automatic cinematic rotation around the village center.
    * **Manual Mode:** Full "First-Person" control using keyboard inputs (WASD + QE for altitude).
* **Collision-Free Floor:** Ground-level clamping to prevent the camera from clipping through the terrain.

---

## 📊 Technical Implementation

### **Core Graphics Pipeline**
* **Primitives & Geometry:** Extensive use of `glBegin(GL_QUADS)`, `GL_TRIANGLE_FAN`, and `GL_LINES` for architectural modeling.
* **Material Properties:** Defined Ambient, Diffuse, and Specular properties via `glMaterial` to handle realistic light reflections on different surfaces.
* **Transformation Mathematics:** Utilized Trigonometry (Sin/Cos) for orbit mechanics, aircraft flight paths, and sun positioning.



### **Keyboard Controls**
| Key | Action |
| :--- | :--- |
| **W / S** | Move Forward / Backward |
| **A / D** | Strafe Left / Right |
| **Q / E** | Fly Up / Down |
| **J / L** | Turn Left / Right |
| **N / M / R** | Toggle Night / Morning / Auto Mode |
| **+ / -** | Adjust Aircraft Altitude |

---

## 🛠 Tech Stack
* **Language:** C++
* **Graphics API:** OpenGL (v1.1 - v2.1 compatibility)
* **Libraries:** GLUT (OpenGL Utility Toolkit), GLU (OpenGL Utility Library)
* **IDE:** Visual Studio

---

## 🚀 Installation & Execution

1.  **Prerequisites:**
    * Install **FreeGLUT** or **GLUT** libraries.
    * Set up OpenGL path in your C++ IDE (Visual Studio recommended).
2.  **Compilation:**
    ```bash
    g++ Full_Project.cpp -lglut -lGLU -lGL -o smart_village
    ```
3.  **Run:**
    ```bash
    ./smart_village
    ```

---

## 📁 Project Structure
* `Anmited Samrt Code.cpp`: The complete source code including shaders, geometry, and input handling.
* `Animated_Smart_village[1].pptx`: Presentation covering challenges like lighting transitions and orbit mechanics.
* `Full Project.txt`: Full source code version with additional comments for documentation.

---
**Visual Computing Solutions © 2025.**
*Simulating the future through real-time 3D graphics.*
