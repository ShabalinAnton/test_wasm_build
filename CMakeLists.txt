cmake_minimum_required(VERSION 3.10)

project(hello_world)

add_executable(hello_world hello_world.cpp)
set_target_properties(hello_world PROPERTIES LINK_FLAGS "-s EXPORTED_FUNCTIONS=['_main'] -s WASM=1")