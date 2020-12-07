cmake_minimum_required (VERSION 2.6)
project (dynamixel-demos)

set(CMAKE_CXX_FLAGS "-D_REENTRANT -Wall -finline-functions -Wno-inline  -fPIC -O3 -std=c++11 -ftemplate-depth-128 -Wno-sign-compare")

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/tools)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/demos)
