cmake_minimum_required(VERSION 3.17)
project(LearnOpenGL)
set(CMAKE_CXX_STANDARD 14)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)
add_executable(LearnOpenGL newVis.cpp src/glad.c Shader/shader_s.h stb_image.h Shader/shader_m.h Camera/Camera.h)
target_link_libraries(LearnOpenGL ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)
