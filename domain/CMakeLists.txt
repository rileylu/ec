cmake_minimum_required(VERSION 3.10)
project(domain)

set(CMAKE_CXX_STANDARD 11)
set(SRC_LIST model/expressconfig.cpp model/expressconfig.h)

add_library(domain ${SRC_LIST})
target_link_libraries(domain PocoFoundation PocoData PocoDataMySQL)
