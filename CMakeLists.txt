cmake_minimum_required(VERSION 3.22)

project(potion)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(3rd/SDL)

file(GLOB SRC_FILES src/*.cpp)

add_executable(potion ${SRC_FILES})

target_link_libraries(potion PUBLIC SDL3::SDL3)
