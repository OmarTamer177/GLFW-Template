# OpenGL Setup Template with MinGW 

This repository provides a template to quickly set up an OpenGL project with MinGW on Windows. It includes everything you need to start working with OpenGL, such as a basic project structure, build instructions, and links to relevant libraries.

---

## Features

- Minimal OpenGL setup for Windows.
- Support for modern OpenGL (GLFW and GLAD).
- Easy to build with MinGW (Makefile provided).
- Example code to render a simple OpenGL window.

---

## Libraries
   - **GLFW**: Library for creating windows, contexts, and handling input.
   - **GLAD**: OpenGL loading library.

---

## Prerequisites

**MinGW**: Ensure that [MinGW](https://sourceforge.net/projects/mingw/) is installed and added to your system's PATH.

**OpenGL Drivers**: Ensure your system has the necessary OpenGL drivers.

---

## Setup

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/OmarTamer177/GLFW-Template
   cd GLFW-Template
   ```

2. **Directory Structure**:

   The project should have the following structure:

   ```
   GLFW-Template/
   ├── bin/
   │   ├── glfw3.dll
   │   └── Makefile
   ├── include/
   │   ├── glad/
   │   │   └── glad.h
   │   ├── GLFW/
   │   │   ├── glfw3.h
   │   │   └── glfw3native.h
   │   └── KHR/
   │       └── khrplatform.h
   ├── lib/
   │   ├── libglfw3.a
   │   └── libglfw3dll.a
   ├── src/
   │   ├── glad.c
   │   └── main.cpp
   └── README.md
   ```

3. **Build and Run the Project**:

   Go to `/bin` directory:
   ```bash
   cd bin
   ```

   Use the provided `Makefile` to build the project:

   ```bash
   mingw32-make
   ```

   This will generate an executable in the `bin/` directory and run the Application.

5. **Run the Application**:

   ```bash
   ./main
   ```
   
---

## Example Code

The template includes a basic example in `src/main.cpp` that creates an OpenGL context, opens a window, and clears the screen with a solid color.

---

## Troubleshooting

1. **Missing Dependencies**:
   - Ensure all required libraries are downloaded and placed correctly in the `lib/` and `include/` folders.

2. **MinGW Not Found**:
   - Add MinGW's `bin/` directory to your PATH environment variable.

3. **Runtime Errors**:
   - Check your GPU drivers and ensure they support the OpenGL version required by the project.
