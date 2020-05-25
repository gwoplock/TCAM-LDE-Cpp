cmake_minimum_required(VERSION 3.10)

project(Tcam-Lde VERSION 1.0)

add_executable(Tcam-Lde src/main.cpp src/Tcam/test.cpp)

configure_file(src/config.h.in config.h)

target_include_directories(Tcam-Lde PUBLIC "${PROJECT_BINARY_DIR}")

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)