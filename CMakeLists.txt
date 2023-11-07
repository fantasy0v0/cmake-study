cmake_minimum_required(VERSION 3.27.7)
project(HELLO CXX)

set(SRC_LIST main.cpp)

message(STATUS "This is BINARY dir " ${HELLO_BINARY_DIR})
message(STATUS "This is SOURCE dir " ${HELLO_SOURCE_DIR})

add_executable(hello ${SRC_LIST})