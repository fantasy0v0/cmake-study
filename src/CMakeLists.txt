file(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)

include_directories("../lib/include")
if(CMAKE_BUILD_TYPE STREQUAL "Release")
  link_libraries("../lib/Release/func")
else()
  link_libraries("../lib/Debug/func")
endif()


add_executable(hello ${SRC})