# 🖥️ SS3DV —Schartz's  Simple 3D Model Viewer 

A lightweight, cross-platform 3D model viewer built with modern OpenGL, GLFW, and GLAD. 

## 🧰 Features 
✅ OpenGL 3.3 Core Context
✅ GLFW for window & input handling
✅ GLAD for OpenGL function loading
✅ CMake-based build system (Linux tested)
✅ Planned: OBJ/GLTF model loading, camera controls, lighting


## 🛠️ Build Instructions (Linux) 
Prerequisites 
Make sure you have these installed: 
```bash
sudo apt update
sudo apt install build-essential cmake xorg-dev libgl1-mesa-dev
```

Build & Run 
```bash
git clone https://github.com/schartz/SS3DV.git 
cd SS3DV
mkdir build
cd build
cmake ..
make -j4
./bin/SS3DV
``` 
***A note on GLAD***
This progect uses glfw via [GLAD](https://glad.dav1d.de/).
The permalink for GLAD used in this project is following:
[GLAD permalink](https://glad.dav1d.de/#language=c&specification=gl&api=gl%3D4.6&api=gles1%3Dnone&api=gles2%3Dnone&api=glsc2%3Dnone&profile=core&loader=on)
Feel free to change it according your platform/needs.

## 📂 Project Structure 
```
SS3DV/
├── CMakeLists.txt          # Project configuration
├── README.md               # This file
├── .gitignore              # Keeps repo clean
├── Libs/                   # Third-party libraries (GLFW, GLAD)
├── src/                    # Source code
│   └── main.cpp            # Entry point
└── build/                  # Build output (ignored by git)
``` 

## 🎯 Roadmap 
Initialize OpenGL context + clear screen
Add vertex & fragment shaders
Render a colored triangle
Load and render OBJ models
Add camera (WASD + mouse look)
Add basic lighting (Phong)
Support for materials/textures
UI with ImGui (optional)

## 🤝 Contributing 
Contributions are welcome! Fork the repo, create a feature branch, and submit a PR. 
 
## 📜 License 
MIT — Do whatever you want with it 😊
(Will add LICENSE file later.) 

 
## 💬 Contact 
Made by Schart
Questions? Ideas? → [rehan.qt[AT]gmail[DOT][COM] ] or open an issue!

