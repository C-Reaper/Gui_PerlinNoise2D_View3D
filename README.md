# Project README

## Overview
- A 3D visualization tool using Perlin noise for mesh generation.
  
## Features
- Real-time rendering of 3D meshes based on Perlin noise.
- User interaction through keyboard and mouse.
- Cross-platform support: Linux, Windows, Wine, and WebAssembly.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC)
- Make utility

## Build & Run
### Linux
To build the project for Linux:
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.linux all
```
To run the project:
```bash
./build/Main
```

### Windows
To build the project for Windows:
```bash
cd C:\path\to\project
make -f Makefile.windows all
```
To run the project:
```cmd
build\Main.exe
```

### Wine (Linux Cross Compile for Windows)
To build the project using Wine on Linux:
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.wine all
```
To run the project:
```cmd
wine build\Main.exe
```

### WebAssembly (Emscripten)
To build the project for WebAssembly:
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.web all
```
To run the project:
```bash
emrun --no_browser --port 8080 build/index.html
```

# Project Organization
- `build/`: .exe files produced by Main.c
- `src/`: Source code, including Main.c and other *.h files
- `Makefile.linux`
- `Makefile.windows`
- `Makefile.wine`
- `Makefile.web`
- `README.md`

---

# Build Steps

### Linux
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.linux all
```

### Windows
```cmd
cd C:\path\to\project
make -f Makefile.windows all
```

### Wine (Linux Cross Compile for Windows)
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.wine all
```

### WebAssembly (Emscripten)
```bash
cd /home/codeleaded/Hecke/C/Gui_PerlinNoise2D_View3D
make -f Makefile.web all
```

### Build Options
- `all`: build output
- `do`: build + exe output
- `clean`: Remove build artifacts