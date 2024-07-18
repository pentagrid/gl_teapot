cmake_minimum_required(VERSION 3.10)

# Set the project name
project(gl_teapot VERSION 1.0)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

#find_package(OpenGl REQUIRED)
find_package(GLUT REQUIRED)

# Add the executable
add_executable(teapot src/main.cpp)

# Link Libraries
target_link_libraries(teapot ${GLUT_LIBRARIES} -lGL -lGLU)

