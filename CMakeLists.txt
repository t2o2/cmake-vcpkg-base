cmake_minimum_required(VERSION 3.10)
project(HelloWorld)
find_package(fmt CONFIG REQUIRED)
set(CMAKE_BUILD_TYPE Debug)
add_executable(HelloWorld main.cpp)
target_link_libraries(HelloWorld PRIVATE fmt::fmt)