cmake_minimum_required(VERSION 3.10)

project(Forest)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(SFML COMPONENTS window graphics REQUIRED)

file(GLOB SOURCES "*.cpp")

add_executable(Forest ${SOURCES})

target_link_libraries(Forest PRIVATE sfml-window sfml-graphics)
