
cmake_minimum_required(VERSION 3.5)

set(CMAKE_CXX_STANDARD 17)

# project
set(PRJ_NAME rawtoplt)
project(${PRJ_NAME})

# exe
add_executable(${PRJ_NAME})

# source
file(GLOB src ${CMAKE_SOURCE_DIR}/src/*.cpp)
target_sources(${PRJ_NAME} PRIVATE ${src})

# include
target_include_directories(${PRJ_NAME} PRIVATE ${CMAKE_SOURCE_DIR})
