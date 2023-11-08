cmake_minimum_required(VERSION 3.27.7)
project(HELLO CXX)

# 设置变量
set(SRC_LIST main.cpp)

# 打印信息
message(STATUS "This is BINARY dir " ${HELLO_BINARY_DIR})
message(STATUS "This is SOURCE dir " ${HELLO_SOURCE_DIR})
message(STATUS "This is CMAKE_INSTALL_PREFIX " ${CMAKE_INSTALL_PREFIX})

# add_executable(hello ${SRC_LIST})
# 添加子目录
add_subdirectory(src bin)
add_subdirectory(lib lib/bin)