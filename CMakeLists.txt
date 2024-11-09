cmake_minimum_required(VERSION 3.10.0)

project(xease-lib VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(INC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/inc)

add_library(
    ${PROJECT_NAME}
    ${SRC_DIR}/xease.cpp
)

target_include_directories(${PROJECT_NAME} PUBLIC ${INC_DIR})