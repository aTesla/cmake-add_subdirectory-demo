cmake_minimum_required(VERSION 3.22.1)
project(CALCLIB)

# include_directories(${PROJECT_SOURCE_DIR}/include)
include_directories(${HEAD_PATH})
file(GLOB SRC_MAIN ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)

# set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
# set(LIBRARY_OUTPUT_PATH ${LIB_PATH})

add_library(${CALC_LIB} STATIC ${SRC_MAIN})


message(STATUS "csd ${CMAKE_SOURCE_DIR}")
message(STATUS "cbd ${CMAKE_BINARY_DIR}")

message(STATUS "ccsd ${CMAKE_CURRENT_SOURCE_DIR}")
message(STATUS "ccbd ${CMAKE_CURRENT_BINARY_DIR}")

message(STATUS " psd ${PROJECT_SOURCE_DIR}")
message(STATUS " pbd ${PROJECT_BINARY_DIR}")

message(STATUS "HEAD_PATH= ${HEAD_PATH}")