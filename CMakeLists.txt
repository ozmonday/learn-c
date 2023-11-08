cmake_minimum_required(VERSION 3.5)
project(learn VERSION 0.0.1)

add_subdirectory(./src/math)
add_subdirectory(./src)

set(TEST_VARIABLE "This is a variable")

message(${TEST_VARIABLE})