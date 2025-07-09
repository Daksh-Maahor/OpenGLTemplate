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

> **Note:** If you want to rename your project, change the project name in the `project()` line at the top of `CMakeLists.txt`.

> **Note:** Whenever you create a new source file (e.g., a new `.cpp` file in `src/`), you must also add it to the `add_executable` line in `CMakeLists.txt`. Otherwise, you may get linker errors for missing function implementations. 