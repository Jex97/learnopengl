cmake_minimum_required(VERSION 3.21)
project(learnopengl)

set(CMAKE_CXX_STANDARD 14)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)
add_executable(learnopengl main.cpp src/glad.c)
target_link_libraries(learnopengl ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)
