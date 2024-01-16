file(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)

include_directories("../lib/include")
link_libraries("")

add_executable(hello ${SRC})