cmake_minimum_required (VERSION 2.6)
project (dynamixel-demos)
find_package(Boost 1.54 REQUIRED COMPONENTS filesystem program_options system)

set(CMAKE_CXX_FLAGS "-D_REENTRANT -Wall -finline-functions -Wno-inline  -fPIC -O3 -std=c++11 -ftemplate-depth-128 -Wno-sign-compare")

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/tools)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/demos)

file(GLOB INSTALL_FILES_1 "./src/dynamixel/*/**")
file(GLOB INSTALL_FILES_2 "./src/dynamixel/*.hpp")

INSTALL(FILES
	${INSTALL_FILES_1}
	DESTINATION
	conf PERMISSIONS OWNER_READ GROUP_READ WORLD_READ)
INSTALL(FILES
	${INSTALL_FILES_2}
	DESTINATION
	conf PERMISSIONS OWNER_READ GROUP_READ WORLD_READ)