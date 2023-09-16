cmake_minimum_required(VERSION 3.26)
project(VoltEngine)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(VoltEngine
        main.cpp
        main.h)

target_link_libraries(VoltEngine ${OPENGL_LIBRARIES})
target_link_libraries(VoltEngine ${GLUT_LIBRARIES})
target_link_libraries(VoltEngine -lopengl32 -g -lfreeglut)