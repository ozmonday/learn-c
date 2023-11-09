cmake_minimum_required(VERSION 3.5)
project(learn VERSION 0.0.1 LANGUAGES C CXX)

#include some modul
include(${CMAKE_CURRENT_LIST_DIR}/cmake/CPrint.cmake)

print_me()
say_hallo("Iqbal Hadi Purnomo")

#add sub directory
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/src/math)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/src)

set(TEST_VARIABLE "This is a variable")

message(${TEST_VARIABLE})