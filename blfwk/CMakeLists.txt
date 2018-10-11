cmake_minimum_required (VERSION 2.6)
project (blhost)

file(GLOB_RECURSE blhost_SOURCES "*.cpp" "*.c")

add_executable(blhost ${blhost_SOURCES})
#target_link_libraries (blhost)
#target_include_directories(blhost)
