# OpenGL CMake Template

This is a minimal OpenGL project template using CMake, GLFW, and GLEW.

## Folder Structure
- `src/` - Source files
- `include/` - Header files
- `build/` - Build directory

## Dependencies
- OpenGL
- GLFW
- GLEW

On Ubuntu, you can install dependencies with:
```sh
sudo apt-get install libglfw3-dev libglew-dev libgl1-mesa-dev
```

On Arch Linux:
```sh
sudo pacman -S glfw glew mesa
```

## Build Instructions
```sh
mkdir -p build
cd build
cmake ..
make
./OpenGLTemplate
``` 