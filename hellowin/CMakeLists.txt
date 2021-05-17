cmake_minimum_required(VERSION 3.0)

project(hellowwin)

include(${CMAKE_BINARY_DIR}/conan_paths.cmake)

add_executable(hellowin main.cpp)

find_package(glfw3)
find_package(glad)

target_link_libraries(hellowin glfw::glfw glad::glad)
