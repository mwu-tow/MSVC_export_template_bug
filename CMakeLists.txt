cmake_minimum_required(VERSION 3.1)
project(Main)
set (CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
add_subdirectory(aa)
add_executable(Main main.cpp test.cpp)
target_link_libraries(Main PUBLIC AA)