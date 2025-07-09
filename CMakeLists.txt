cmake_minimum_required(VERSION 3.10)
project(OpenGLTemplate)

set(CMAKE_CXX_STANDARD 17)

# Find OpenGL
find_package(OpenGL REQUIRED)
# Find GLFW
find_package(glfw3 REQUIRED)
# Find GLEW
find_package(GLEW REQUIRED)

# Add source files
add_executable(${PROJECT_NAME} src/main.cpp)

# Include directories
include_directories(include)

# Link OpenGL
target_link_libraries(${PROJECT_NAME} OpenGL::GL glfw GLEW::GLEW)
