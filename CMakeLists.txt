cmake_minimum_required(VERSION 3.26)
project(VoltEngine)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(VoltEngine
        main.cpp
        main.h)
