cmake_minimum_required(VERSION 3.5)
project(learn VERSION 0.0.1 LANGUAGES C CXX)

#include some modul
include(${CMAKE_CURRENT_LIST_DIR}/cmake/CPrint.cmake)
include(${CMAKE_CURRENT_LIST_DIR}/cmake/CFlowControl.cmake)

test_for()
print_me()
say_hallo("Iqbal Hadi Purnomo")

option(SERIAL_DEBUG "enable/disable debugging output" OFF)
option(MINIMAL "exclude optional source code to keep compile size compact" OFF)

#add sub directory
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/src/say)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/src/math)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/src)

set(TEST_VARIABLE "This is a variable")

message(${TEST_VARIABLE})