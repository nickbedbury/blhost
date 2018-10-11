cmake_minimum_required (VERSION 2.6)
project (blhost)

file(GLOB_RECURSE blhost_SOURCES "blfwk/*.cpp" "blfwk/*.c" "crc/*.c" "blhost/*.cpp" "blhost/*.c" "blhost.cpp")

add_executable(blhost ${blhost_SOURCES})
#target_link_libraries (blhost)
target_include_directories(blhost PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
add_definitions(-DBOOTLOADER_HOST)
add_definitions(-DLINUX)
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
