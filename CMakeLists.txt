cmake_minimum_required(VERSION 3.12)
project(_learnOpenGl)

set(CMAKE_CXX_STANDARD 14)

# uncomment for deployment
# set(CMAKE_EXE_LINKER_FLAGS -static)

add_executable(_learnOpenGl main.cpp glad.c Shader.h)

target_link_libraries(_learnOpenGl glfw3 gdi32 opengl32)