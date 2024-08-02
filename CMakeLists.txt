cmake_minimum_required(VERSION 3.22.1)
project(test)

# set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/build)
# set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/build)
# set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/build)

set(LIB_PATH ${CMAKE_CURRENT_SOURCE_DIR}/build/lib)
set(EXEC_PATH ${CMAKE_CURRENT_SOURCE_DIR}/build/bin)
# set(LIB_PATH ${CMAKE_CURRENT_SOURCE_DIR}/lib)
# set(EXEC_PATH ${CMAKE_CURRENT_SOURCE_DIR}/bin)
set(HEAD_PATH ${CMAKE_CURRENT_SOURCE_DIR}/include)

set(CALC_LIB calc)
set(SORT_LIB sort)
set(APP_NAME_1 test1)
set(APP_NAME_2 test2)

add_subdirectory(./calc ./calc/build)
add_subdirectory(./sort ./sort/build)
add_subdirectory(./test1 ./test1/build)
add_subdirectory(./test2 ./test2/build)