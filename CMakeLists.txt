cmake_minimum_required(VERSION 3.14)
project(Registry)

set(CMAKE_CXX_STANDARD 17)

add_library(${PROJECT_NAME} STATIC
        Registry/include/Registry.hpp
        Registry/src/Registry.cpp)
target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/Registry/include)