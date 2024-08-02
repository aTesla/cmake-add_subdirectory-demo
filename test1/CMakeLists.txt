cmake_minimum_required(VERSION 3.22.1)
project(CALCTEST)

# include_directories(${PROJECT_SOURCE_DIR}/include)
include_directories(${HEAD_PATH})
file(GLOB SRC_MAIN ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)
# set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${EXEC_PATH})

link_directories(${PROJECT_SOURCE_DIR}/lib)
link_libraries(${CALC_LIB})
add_executable(${APP_NAME_1} ${SRC_MAIN})