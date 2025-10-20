# Lab 4 – Upload Model
# Overview

This starter project is built on GLFW + GLAD + Assimp (Windows x64).
It provides a modern OpenGL setup for loading and rendering 3D models.

If you are using GLEW + FreeGLUT, please refer instead to the starter code Lab4_b, which is configured for the GLEW + FreeGLUT environment.

# 📦 Download Assimp

If you are using a system other than Windows x64, please download the correct Assimp version manually from the official site:
🔗 https://www.assimp.org/

# 📁 Project Structure

lab4/
├─ external/
│  ├─ assimp/
│  ├─ glad-3.3/
│  ├─ glfw-3.1.2/
│  ├─ glm-0.9.7.1/
│  └─ CMakeLists.txt
│
├─ source code/
│  ├─ main.cpp
│  ├─ maths_funcs.cpp
│  ├─ maths_funcs.h
│  ├─ monkeyhead_smooth.dae     # test model
│  ├─ simpleVertexShader.txt
│  └─ simpleFragmentShader.txt
│
└─ CMakeLists.txt

# ⚙️ Requirements

CMake ≥ 3.1, OpenGL 3.3+


# 🛠 Build Instructions

🪟 Windows (CLion – Recommended)

Open the folder lab4 in CLion.

Let CMake finish configuring.

Select the target lab4_main.

Build ▶ Run.

A window appears showing the rotating monkey head.

🍎 macOS

Install dependencies:

brew install cmake assimp glfw


Configure & build:

cd ~/path/to/lab4
cmake -S . -B build
cmake --build build --target lab4_main -j 8


Run:

./build/lab4_main

🐧 Linux

Install dependencies:

sudo apt update
sudo apt install build-essential cmake libglfw3-dev libassimp-dev


Configure, build, and run:

cd ~/path/to/lab4
cmake -S . -B build
cmake --build build --target lab4_main -j 8
./build/lab4_main

