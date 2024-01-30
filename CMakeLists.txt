cmake_minimum_required(VERSION 3.27.2)
project(HELLO CXX)

# 设置变量
set(SRC_LIST main.cpp)

# 打印信息
message(STATUS "This is BINARY dir " ${PROJECT_BINARY_DIR})
message(STATUS "This is SOURCE dir " ${PROJECT_SOURCE_DIR})
message(STATUS "This is CMAKE_INSTALL_PREFIX " ${CMAKE_INSTALL_PREFIX})

# add_executable(hello ${SRC_LIST})
# 添加子目录
add_subdirectory(src)
add_subdirectory(lib)