cmake_minimum_required(VERSION 3.10)
project(SS3DV LANGUAGES C CXX)

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# Include directories
include_directories(
    Libs/glad/include
    Libs/glfw/include
)

# Add executable
add_executable(${PROJECT_NAME}
    src/main.cpp
    Libs/glad/src/glad.c
)

# GLFW build as static library
add_subdirectory(Libs/glfw)

# Link libraries
target_link_libraries(${PROJECT_NAME}
    glfw
    GL
    GLU
    X11
    Xrandr
    Xi
    Xxf86vm
    pthread
    dl
)

# Set output directory
set_target_properties(${PROJECT_NAME} PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin
)
