cmake_minimum_required(VERSION 3.10)
project(ec)

add_subdirectory(googletest)
add_subdirectory(domain)

set(CMAKE_CXX_STANDARD 11)

set(SRC_LIST main.cpp)

add_executable(ec ${SRC_LIST} )
target_link_libraries(ec gtest)