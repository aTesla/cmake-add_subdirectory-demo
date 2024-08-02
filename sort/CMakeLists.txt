cmake_minimum_required(VERSION 3.22.1)
project(SORTLIB)

# include_directories(${PROJECT_SOURCE_DIR}/include)
include_directories(${HEAD_PATH})
file(GLOB SRC_MAIN ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)

# set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
set(LIBRARY_OUTPUT_PATH ${LIB_PATH})

add_library(${SORT_LIB} SHARED ${SRC_MAIN})